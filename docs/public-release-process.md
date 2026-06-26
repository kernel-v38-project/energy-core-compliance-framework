# Public Release Process

## Purpose

This document defines the approval and publication process for public releases of the energy_core Enterprise trust center and documentation.

## Scope

This process applies to:
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
- any public-facing trust center or showcase content.

## Goals

The release process is designed to:
- keep public documentation accurate;
- prevent conflicting statements;
- ensure sensitive material remains gated;
- confirm that changes are reviewed before publication;
- maintain a clear audit trail for public-facing updates.

## Roles

### Author
Prepares the change, updates the content, and opens the release request.

### Reviewer
Checks accuracy, clarity, and consistency across files.

### Approver
Gives final approval for publication. Approval should come from the owner responsible for the impacted area.

### Maintainer
Publishes the release after approvals are complete.

## Approval rules

### General rule
No public release should be published until the required reviewers have approved it.

### Required approvals by change type

#### Documentation-only changes
Requires:
- author review;
- one maintainer or reviewer approval.

Examples:
- wording corrections;
- link updates;
- formatting changes;
- non-material clarifications.

#### Operational changes
Requires:
- author review;
- one reviewer approval;
- maintainer approval.

Examples:
- maintenance cadence updates;
- process changes;
- access flow changes;
- FAQ updates.

#### Compliance-impacting changes
Requires:
- author review;
- reviewer approval;
- approval from the relevant policy owner;
- maintainer approval.

Examples:
- DPA changes;
- privacy changes;
- subprocessor updates;
- incident response updates;
- security posture changes.

#### Public release changes
Requires:
- author review;
- reviewer approval;
- approver approval;
- maintainer approval.

Examples:
- tagged release publication;
- new trust center version;
- major README or index updates;
- changes to the public story or access model.

## Release criteria

A release may be published only when all of the following are true:
- the files are internally consistent;
- all links resolve correctly;
- the public wording matches the current policy posture;
- sensitive implementation details remain gated;
- RELEASE_NOTES.md reflects the change;
- the public-facing page and README use the same terminology;
- the release has the necessary approvals.

## Review checklist

Before approval, verify:
- English wording is consistent across public documents;
- file names and relative links are correct;
- DPA and subprocessors documents are current;
- release notes match the actual changes;
- no placeholder text remains;
- the public trust center reflects the intended buyer-facing position.

## Publication workflow

1. The author prepares the update.
2. The author opens a release request or pull request.
3. The reviewer checks the content for accuracy and consistency.
4. The approver reviews changes in the affected area.
5. The maintainer confirms the release criteria are met.
6. The release is tagged or published.
7. RELEASE_NOTES.md and any GitHub release entry are updated.
8. The final published pages are verified after deployment.

## Exceptions

If a change is urgent due to a material compliance or security update:
- the approver may fast-track review;
- the maintainer must still confirm release criteria before publication;
- the change must be documented after publication if pre-approval was not possible.

## Record keeping

Keep a record of:
- date of request;
- files changed;
- reviewers;
- approver;
- publication date;
- release tag or version;
- summary of the change.

## Maintenance

Review this process:
- monthly, for clarity and relevance;
- after any major release;
- after any change to the trust center structure;
- after any material change to DPA, privacy, or subprocessor handling.

## Notes

This process exists to keep public releases accurate, approved, and aligned with the current trust center posture.
