# Audit Evidence

## Purpose

This document defines how energy_core Enterprise stores, indexes, and maintains documentary evidence for internal governance, compliance review, and buyer diligence.

## Principles

- Keep evidence centralized and access-controlled.
- Store evidence with timestamps and source references.
- Link each artifact to a specific control, claim, or review item.
- Keep the evidence set current and versioned.
- Remove ambiguity by documenting what the evidence shows and who owns it.

## What counts as evidence

Acceptable evidence may include:
- policy documents;
- screenshots of system settings;
- configuration exports;
- signed approvals;
- access review records;
- release tags and changelogs;
- subprocessor change logs;
- incident summaries;
- architecture diagrams;
- deployment notes;
- test results;
- audit trail exports;
- date-stamped logs;
- NDA-based review records.

## Evidence structure

Recommended structure:
- `evidence/`
- `evidence/security/`
- `evidence/privacy/`
- `evidence/compliance/`
- `evidence/subprocessors/`
- `evidence/releases/`
- `evidence/architecture/`
- `evidence/incident-response/`

Each evidence item should include:
- title;
- date;
- owner;
- source;
- related document or control;
- short description;
- file name or path;
- version or hash, if available.

## Evidence quality standards

Each artifact should be:
- relevant;
- readable;
- dated;
- attributable to a source or owner;
- tied to a control or claim;
- stored in a stable format;
- easy to retrieve.

Avoid:
- duplicate copies without purpose;
- undocumented screenshots;
- undated exports;
- orphaned files;
- evidence with no control mapping;
- stale artifacts that no longer reflect current posture.

## Evidence log

Maintain a simple evidence log with:
- evidence ID;
- document name;
- category;
- date collected;
- collected by;
- related control or claim;
- retention date;
- access classification.

## Control mapping

Every material public claim should map to one or more evidence items.

Examples:
- Security claims map to SECURITY.md and supporting security evidence.
- Privacy claims map to docs/privacy.md and related processing evidence.
- DPA claims map to docs/dpa.md and signed contract references.
- Subprocessor claims map to docs/subprocessors.md and vendor records.
- Release claims map to RELEASE_NOTES.md and GitHub release metadata.
- Architecture claims map to docs/architecture.md and deployment notes.

## Retention

Retain evidence for as long as required by:
- internal governance policy;
- contractual obligations;
- legal obligations;
- audit or review needs.

If evidence is superseded, keep the prior version if it is needed for historical traceability.

## Access control

Evidence should be stored with appropriate restrictions:
- public evidence may be shared in the trust center;
- internal evidence should remain restricted;
- NDA-gated evidence should only be shared under the approved access process.

## Review cadence

Review evidence:
- monthly for current trust center claims;
- quarterly for broader governance posture;
- immediately when a material control or process changes;
- before any public release that changes buyer-facing language.

## Change handling

When evidence changes:
1. Update the evidence item.
2. Update the evidence log.
3. Review the related public document.
4. Update release notes if the change affects public posture.
5. Confirm that all references remain correct.

## Notes

The goal of evidence management is not to store everything.
The goal is to keep a clean, traceable, and supportable record of what the public trust center claims.
