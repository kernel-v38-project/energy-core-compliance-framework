# Evidence Index Template

## Purpose

This template is used to catalog documentary evidence for energy_core Enterprise in a consistent and auditable way.

## How to use this template

For each evidence item:
- assign a unique evidence ID;
- link it to a control, claim, or review topic;
- record the owner and collection date;
- store the file in a stable location;
- keep the entry current when the artifact changes.

## Recommended columns

- Evidence ID.
- Title.
- Category.
- Related document or control.
- Owner.
- Source.
- Date collected.
- Last updated.
- Status.
- Access level.
- File path or URL.
- Version or hash.
- Retention date.
- Notes.

## Evidence index table

| Evidence ID | Title | Category | Related document or control | Owner | Source | Date collected | Last updated | Status | Access level | File path or URL | Version or hash | Retention date | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| EVD-001 | Security Policy | Security | SECURITY.md | Security Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./SECURITY.md | v1.0 | YYYY-MM-DD | Replace with the latest published version. |
| EVD-002 | Privacy Overview | Privacy | docs/privacy.md | Privacy Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./docs/privacy.md | v1.0 | YYYY-MM-DD | Keep aligned with data handling posture. |
| EVD-003 | DPA Summary | Compliance | docs/dpa.md | Compliance Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./docs/dpa.md | v1.0 | YYYY-MM-DD | Update when contract terms change. |
| EVD-004 | Subprocessor Inventory | Compliance | docs/subprocessors.md | Subprocessor Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./docs/subprocessors.md | v1.0 | YYYY-MM-DD | Record region and transfer implications. |
| EVD-005 | Architecture Overview | Architecture | docs/architecture.md | Architecture Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./docs/architecture.md | v1.0 | YYYY-MM-DD | Reflect the current platform shape. |
| EVD-006 | Incident Response Overview | Security | docs/incident-response.md | Security Owner | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./docs/incident-response.md | v1.0 | YYYY-MM-DD | Refresh after incident process changes. |
| EVD-007 | Release Notes | Release | RELEASE_NOTES.md | Release Maintainer | Repository | YYYY-MM-DD | YYYY-MM-DD | Current | Public | ./RELEASE_NOTES.md | v1.0 | YYYY-MM-DD | Keep aligned with public releases. |
| EVD-008 | GitHub Release Metadata | Release | GitHub release entry | Release Maintainer | GitHub | YYYY-MM-DD | YYYY-MM-DD | Current | Public | Release tag link | v1.0.0 | YYYY-MM-DD | Link to the published release. |

## Evidence item details

For each item, keep the following notes if needed:
- purpose of the artifact;
- why it is relevant;
- what control or claim it supports;
- whether it supersedes older evidence;
- where the previous version is stored.

## Status values

Use one of the following:
- Current.
- Superseded.
- Draft.
- Pending review.
- Archived.

## Access levels

Use one of the following:
- Public.
- Internal.
- NDA-gated.
- Restricted.

## Review rules

- Update the entry whenever the artifact changes.
- Keep the file path stable where possible.
- Retain historical versions when required for audit traceability.
- Remove stale entries only when the evidence is no longer relevant and the retention policy allows it.

## Notes

This template is intended to be copied into a spreadsheet or evidence tracker.
Adapt the columns only if the team can keep the same level of traceability.
