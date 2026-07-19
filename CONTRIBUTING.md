# Contributing to Energy Core

Thank you for your interest in improving Energy Core! To maintain the framework's stability, compliance standards, and hardware performance, please follow these guidelines.

## Development Principles
1. **Asynchronous Architecture:** The blockchain, compliance, and ROI layers MUST run asynchronously. Any pull request that introduces blocking loops or latency to the real-time telemetry core will be rejected.
2. **Deterministic Smart Contracts:** Ensure all automated ROI calculations are fully deterministic and thoroughly tested against edge cases (e.g., negative energy pricing).

## How to Contribute
1. Fork the repository and create your branch from `main`.
2. Ensure your code complies with the project's architecture guidelines.
3. Open a Pull Request with a clear description of the changes and the problem they solve.
4. 
