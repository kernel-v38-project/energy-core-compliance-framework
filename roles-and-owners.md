# Roles and Owners

## Purpose

This document defines the responsibilities for maintaining the public trust center, compliance documents, release process, and related repository assets for energy_core Enterprise.

## Ownership model

The repository uses a simple ownership model:
- one primary owner per domain;
- one backup owner where needed;
- a maintainer responsible for publication and repository hygiene;
- cross-functional review for compliance-impacting changes.

## Roles

### Trust Center Owner
Owns the overall public trust center posture.
Responsibilities:
- ensure public documentation is current;
- coordinate updates across README, index, and trust center documents;
- review buyer-facing wording for consistency;
- confirm that public claims match the evidence available.

### Security Owner
Owns security-related content and controls.
Responsibilities:
- maintain SECURITY.md;
- review incident response wording;
- confirm security claims are accurate;
- validate public security posture statements.

### Privacy Owner
Owns privacy and data handling content.
Responsibilities:
- maintain docs/privacy.md;
- review data categories, retention, and rights language;
- confirm privacy statements align with the actual processing model;
- coordinate updates when data handling changes.

### Compliance Owner
Owns compliance-facing content and governance alignment.
Responsibilities:
- maintain docs/compliance.md;
- review DPA alignment;
- confirm public compliance language is accurate;
- coordinate changes affecting legal or regulatory review.

### Subprocessor Owner
Owns vendor and subprocessors documentation.
Responsibilities:
- maintain docs/subprocessors.md;
- update the list when vendors change;
- record region, purpose, and transfer implications;
- ensure subprocessor changes are reflected in release notes.

### Architecture Owner
Owns architecture and platform overview content.
Responsibilities:
- maintain docs/architecture.md;
- review the public architecture narrative;
- confirm system layers and deployment notes are current;
- update content when the platform shape changes materially.

### Release Maintainer
Owns publication and repository release hygiene.
Responsibilities:
- maintain RELEASE_NOTES.md;
- update .github/release.yml when needed;
- publish releases after required approvals;
- ensure tags, notes, and public pages are aligned.

### Documentation Maintainer
Owns formatting, link integrity, and repository content hygiene.
Responsibilities:
- keep file names and links correct;
- ensure all public docs are readable and consistent;
- remove stale or duplicated content;
- verify that relative links resolve properly.

## Backup owners

Each critical domain should have a backup owner when possible.
Backup owners step in when the primary owner is unavailable and help with periodic review.

## Review and approval matrix

### README.md and index.html
Primary owner:
- Trust Center Owner

Required reviewers:
- Documentation Maintainer
- Release Maintainer if part of a release

### SECURITY.md
Primary owner:
- Security Owner

Required reviewers:
- Trust Center Owner
- Release Maintainer if public release is involved

### docs/privacy.md
Primary owner:
- Privacy Owner

Required reviewers:
- Compliance Owner
- Trust Center Owner

### docs/dpa.md
Primary owner:
- Compliance Owner

Required reviewers:
- Privacy Owner
- Trust Center Owner

### docs/subprocessors.md
Primary owner:
- Subprocessor Owner

Required reviewers:
- Compliance Owner
- Trust Center Owner

### docs/architecture.md
Primary owner:
- Architecture Owner

Required reviewers:
- Trust Center Owner
- Documentation Maintainer

### RELEASE_NOTES.md
Primary owner:
- Release Maintainer

Required reviewers:
- Trust Center Owner
- Compliance Owner when the change is compliance-impacting

### .github/release.yml
Primary owner:
- Release Maintainer

Required reviewers:
- Documentation Maintainer
- Trust Center Owner

## Escalation rules

Escalate to the relevant owner when:
- a document contains conflicting statements;
- a public claim cannot be supported by evidence;
- a legal, privacy, or security statement changes;
- a subprocessor changes;
- a release affects public trust center wording;
- a file name or link breaks public navigation.

## Review cadence

- Trust center owner: monthly.
- Security owner: monthly and after incidents.
- Privacy owner: quarterly, and when data handling changes.
- Compliance owner: quarterly, and when contract posture changes.
- Subprocessor owner: whenever a vendor changes.
- Architecture owner: whenever deployment or system structure changes.
- Release maintainer: every release.

## Notes

Ownership should always be explicit.
If a role is vacant, the trust center owner must assign a temporary backup before publication.
