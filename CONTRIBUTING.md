# Contributing

Thank you for helping improve Digital Health Plus.

## Before proposing a change

- Check existing documentation and open issues to avoid duplicate work.
- Keep proposals focused and explain the problem they solve.
- Do not include private data, credentials, patient records, or confidential material.
- Work on a feature or review branch; do not make unreviewed changes directly on `main`.

## Documentation and content proposals

Include, where applicable:

- Purpose and intended audience
- Reliable supporting references
- Relevant publication or review dates
- Known limitations or uncertainty
- Privacy, safety, accessibility, and copyright considerations
- Evidence of subject-matter or clinical review for high-impact claims

Use `docs/SCIENTIFIC_CONTENT_REVIEW_CHECKLIST.md` for substantive scientific or clinical material and `docs/SECRET_AND_HEALTH_DATA_CHECKLIST.md` before sharing files or examples.

## Technical changes

- Keep changes small and reviewable.
- Explain the files changed and expected effect.
- Do not commit secrets, generated personal data, or unapproved third-party assets.
- Test changes in a safe environment before proposing publication to the live Blogger site.
- Documentation changes are checked by GitHub Actions for Markdown style and links. Review workflow results and address failures before requesting merge.
- Link checks can be affected by external-site rate limits or temporary outages; explain any justified exception rather than silently suppressing failures.
- Do not assume that a GitHub change automatically updates Blogger.

## Pull requests

A pull request should describe:

1. What changed
2. Why the change is needed
3. How it was checked, including CI results
4. Any follow-up work or known risks

Maintainers review changes before they are merged or published. A passing documentation workflow does not establish the accuracy of medical content or the security of the live website.
