# Energy Core - System Architecture

Questo documento illustra il flusso dei dati e il disaccoppiamento tra il controllo in tempo reale e il livello di notarizzazione e conformità.

```mermaid
graph TD
    %% Stili Generali
    classDef asset fill:#f1f5f9,stroke:#475569,stroke-width:1px;
    classDef gateway fill:#e2e8f0,stroke:#475569,stroke-width:1.5px,stroke-dasharray: 5 5;
    classDef core fill:#f0fdf4,stroke:#16a34a,stroke-width:2px;
    classDef app fill:#eff6ff,stroke:#2563eb,stroke-width:1.5px;

    %% Livello 1: Assets sul campo
    subgraph FIELD_ASSETS [FIELD ASSETS]
        PV[PV Inverters<br/><i>SunSpec / Modbus</i>]:::asset
        BESS[BESS / BMS<br/><i>CAN / Modbus</i>]:::asset
        GEN[Backup Gen<br/><i>Modbus RTU</i>]:::asset
        METER[Grid Meter<br/><i>Modbus TCP</i>]:::asset
    end

    %% Livello 2: Gateway di Ingestione
    subgraph INGESTION_LAYER [INGESTION LAYER]
        GW[Edge Gateway / RTU]:::gateway
    end

    %% Livello 3: Energy Core
    subgraph ENERGY_CORE [ENERGY CORE - DECOUPLED INTEGRITY LAYER]
        QUEUE[Ingestion Queue<br/><i>MQTT / JSON Buffer</i>]:::core
        CRYPTO[Crypto Engine<br/><i>SHA-256 Validation</i>]:::core
        LEDGER[(Immutable Ledger<br/><i>Secure Telemetry Cache</i>)]:::core
    end

    %% Livello 4: Applicazioni & UI
    subgraph PRESENTATION [PRESENTATION & CONTROL]
        EMS[Third-Party EMS<br/><i>Control & Optimization</i>]:::app
        DASH[Compliance Dashboard<br/><i>GitHub Repo Frontend</i>]:::app
    end

    %% Connessioni
    PV --> GW
    BESS --> GW
    GEN --> GW
    METER --> GW

    %% Flussi Decoupled
    GW -->|1. Fast-Loop Control| EMS
    GW -->|2. Decoupled Compliance Stream| QUEUE

    %% Flusso interno
    QUEUE --> CRYPTO
    CRYPTO --> LEDGER

    %% Consumo dati
    LEDGER -->|Trusted Audit Trail| EMS
    LEDGER -->|REST API / Secure Query| DASH
