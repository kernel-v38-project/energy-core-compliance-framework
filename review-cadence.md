# Review Cadence

## Purpose

This document defines the recurring review schedule for the public trust center, compliance documentation, and release-related assets for energy_core Enterprise.

## Review principles

- Keep public documents current.
- Review high-risk documents more often than general documentation.
- Update immediately when a material change occurs.
- Keep ownership and timing explicit.
- Record the result of each review.

## Monthly reviews

### Trust Center review
- Check README.md and index.html for wording drift.
- Confirm that all public links still resolve.
- Verify that the public story still matches the current posture.
- Review whether any buyer questions should be added to the FAQ.
- Check for stale claims, placeholder text, or outdated references.

### Release review
- Review RELEASE_NOTES.md.
- Confirm the latest tagged release matches the public documentation.
- Check whether .github/release.yml still reflects the current label taxonomy.
- Verify that any new public changes are captured in the release notes.

### Security review
- Confirm SECURITY.md still reflects the current security posture.
- Check incident response wording for accuracy.
- Review whether any security-related public statements need adjustment.

## Quarterly reviews

### Compliance review
- Review docs/compliance.md for legal and governance alignment.
- Check docs/dpa.md for contract consistency.
- Confirm docs/privacy.md still reflects current data handling.
- Review whether any compliance-related buyer-facing wording needs refinement.

### Subprocessor review
- Review docs/subprocessors.md for additions, removals, or region changes.
- Confirm that the list is versioned and dated.
- Check whether any transfer or residency language needs updating.

### Architecture review
- Review docs/architecture.md for accuracy.
- Confirm that system layers, deployment notes, and public architecture statements still match reality.
- Update the architecture overview if the platform shape changes materially.

### Process review
- Review docs/change-log-policy.md.
- Review docs/public-release-process.md.
- Review docs/roles-and-owners.md.
- Confirm that ownership and approval paths are still valid.

## As-needed reviews

Update immediately when any of the following happens:
- a subprocessor changes;
- the DPA changes;
- privacy handling changes;
- security controls change materially;
- the incident response process changes;
- the architecture changes;
- a new release is published;
- public wording changes materially;
- a file name or link path changes;
- NDA access procedures change.

## Suggested annual rhythm

### January
- Full trust center audit.
- Review ownership and approvals.
- Reset the review calendar for the year.

### April
- Review public posture and release language.
- Check documentation freshness.
- Reassess subprocessors and DPA consistency.

### July
- Mid-year compliance and architecture review.
- Validate release notes and changelog hygiene.

### October
- Review trust center wording.
- Check whether any docs need restructuring before year-end.

## Review record

For each completed review, record:
- date;
- reviewer;
- files reviewed;
- issues found;
- fixes applied;
- follow-up date.

## Notes

This cadence is intended to keep the public trust center accurate, auditable, and easy to maintain without creating unnecessary overhead.
