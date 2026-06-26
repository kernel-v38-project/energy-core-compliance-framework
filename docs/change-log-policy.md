# Change Log Policy

## Purpose

This policy defines when and how changes must be recorded for energy_core Enterprise documentation, trust center content, and public release information.

## Scope

This policy applies to:
- README.md;
- index.html;
- RELEASE_NOTES.md;
- docs/compliance.md;
- docs/privacy.md;
- docs/dpa.md;
- docs/subprocessors.md;
- docs/incident-response.md;
- docs/architecture.md;
- docs/security-questions.md;
- .github/release.yml;
- any public trust center page or related documentation.

## Principles

- Keep public documentation accurate and current.
- Record changes in a way that is easy to review and audit.
- Use clear, factual language.
- Avoid duplicate or conflicting statements across files.
- Update the public trust center when a material change affects buyer review, legal review, or technical due diligence.

## What must be logged

Record a change when any of the following occurs:
- a subprocessor is added, removed, or modified;
- the DPA changes;
- privacy handling changes;
- security controls change materially;
- incident response behavior changes;
- architecture, deployment, or access model changes;
- a public release is published;
- README.md or index.html wording changes materially;
- any link path or file name changes;
- the NDA access process changes;
- buyer-facing claims change.

## Change categories

### Documentation-only
Use for wording changes, clarification, formatting, or link fixes that do not alter the public posture.

### Operational
Use for updates that affect maintenance, update cadence, review workflow, or access procedures.

### Compliance-impacting
Use for changes involving privacy, DPA, subprocessors, security controls, retention, or incident handling.

### Public release
Use for any release that should appear in RELEASE_NOTES.md or GitHub release notes.

## Required fields for a change entry

Each logged change should include:
- date;
- file or page affected;
- change category;
- summary of what changed;
- reason for the change;
- owner or maintainer;
- whether public text, private text, or both were updated.

## Update workflow

1. Identify the change.
2. Determine whether it is documentation-only, operational, compliance-impacting, or a public release.
3. Update the relevant file(s).
4. Check cross-file consistency.
5. Update RELEASE_NOTES.md if the change should be visible to external readers.
6. Update GitHub release notes if the change is part of a tagged release.
7. Review the final text for tone, correctness, and link validity.

## Cross-file consistency rules

If one of the following changes, review all related files:
- README.md;
- index.html;
- RELEASE_NOTES.md;
- docs/dpa.md;
- docs/subprocessors.md;
- docs/privacy.md;
- docs/compliance.md.

Examples:
- If subprocessors change, update docs/subprocessors.md, RELEASE_NOTES.md, and any related trust center references.
- If the DPA changes, update docs/dpa.md, docs/privacy.md if needed, and the release notes.
- If the public positioning changes, update README.md and index.html together.
- If the release taxonomy changes, update .github/release.yml and the release notes workflow.

## Review cadence

- Review the change log policy monthly.
- Review compliance-impacting updates as soon as they are identified.
- Review public release entries before tagging a release.
- Review trust center wording whenever a significant buyer-facing change is made.

## Approval rule

Changes affecting DPA, privacy, subprocessors, or security posture should be reviewed by the relevant owner before publication.

## Record retention

Keep change log records for as long as the repository remains public or as required by internal governance policy.

## Notes

This policy is intended to keep the public trust center accurate, consistent, and easy to audit.
