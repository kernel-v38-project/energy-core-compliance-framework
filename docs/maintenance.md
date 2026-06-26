# Maintenance Checklist

## Purpose

This document defines the recurring maintenance tasks required to keep the public trust center, compliance documentation, and release information current for energy_core Enterprise.

## Ownership

The repository maintainer or trust owner is responsible for:
- document accuracy;
- release note updates;
- subprocessor list updates;
- DPA and privacy consistency;
- link validation;
- public trust center alignment.

## Cadence

### Monthly
- Review whether any public-facing claims have changed.
- Check that README.md, index.html, and release notes still match the current public posture.
- Verify that all links in the trust center resolve correctly.
- Confirm that DPA, privacy, and subprocessors pages reflect the current state.
- Review whether any new customer questions should be added to the FAQ.
- Check that any new deployment or product changes are reflected in the architecture overview.
- Confirm that no placeholder text remains in public documents.

### Quarterly
- Audit all trust center documents for accuracy and relevance.
- Review the subprocessor inventory for additions, removals, or region changes.
- Review the DPA summary for contract alignment and legal updates.
- Check whether new releases require changelog or release note updates.
- Review access paths for NDA-based source code review.
- Validate that the public index still reflects the current repository structure.
- Refresh wording to keep the trust center evidence-led and precise.

### As needed
- Update documents immediately when a subprocessor changes.
- Update documents immediately when the DPA changes.
- Update release notes whenever a public release changes scope or posture.
- Update README.md and index.html when the public story changes.
- Add or remove links when documents are created, renamed, or retired.
- Adjust architecture notes when deployment behavior changes.
- Update the FAQ when repeated buyer questions appear.

## Verification checklist

Before publishing any change, verify:
- README.md is in English and matches index.html.
- All linked files exist and use the correct names.
- Security, compliance, privacy, DPA, subprocessors, incident response, architecture, and FAQ pages are present.
- Release notes reflect the latest public change.
- Subprocessor list is current and dated.
- DPA and privacy documents are consistent with the public trust center.
- No claim is stronger than the evidence provided.

## Change triggers

Trigger an update when any of the following changes:
- a new vendor is introduced;
- a vendor is removed;
- data residency or transfer behavior changes;
- privacy handling changes;
- the public architecture changes;
- a new release is published;
- NDA access terms change;
- security controls or incident response behavior changes.

## Release coordination

When preparing a release:
- update RELEASE_NOTES.md;
- confirm `.github/release.yml` still matches the current label taxonomy;
- verify that public documentation reflects the same wording as the release notes;
- confirm the GitHub release title and tag are consistent;
- review whether the release should be draft or published.

## Document hygiene

Keep all public documents:
- concise;
- factual;
- evidence-led;
- consistent in terminology;
- free from outdated or duplicated statements.

## Final review

After any significant update:
- read the README end to end;
- click every linked document;
- confirm that the trust center still presents a coherent public story;
- ensure the private and public access models remain clearly separated.
