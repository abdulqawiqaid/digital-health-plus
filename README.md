# Digital Health Plus

**Official blog:** https://digitalhealthplus.blogspot.com

Digital Health Plus is an educational publication focused on digital health, healthcare innovation, medical informatics, health information systems, and the responsible use of artificial intelligence in healthcare.

## Purpose of this repository

This repository maintains project documentation, editorial and security governance, issue templates, and approved website-related assets or source files.

The live publication remains hosted on **Blogger**. This repository does not automatically deploy changes to the blog or synchronize Blogger posts.

## Editorial and technical scope

- Digital health and digital transformation in healthcare
- Electronic health information systems (EHIS) and health informatics
- Artificial intelligence and data-informed healthcare
- Healthcare quality, patient safety, and clinical governance
- Interoperability, privacy, security, and responsible health-data use
- Technical documentation and continuous website improvement

## Repository structure

```text
digital-health-plus/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── workflows/
│       └── docs-quality.yml
├── docs/
│   ├── CHANGELOG.md
│   ├── CONTENT_GOVERNANCE.md
│   ├── INITIAL_STATIC_AUDIT.md
│   ├── MAIN_BRANCH_PROTECTION_PROPOSAL.md
│   ├── PROJECT_OVERVIEW.md
│   ├── REPOSITORY_AUDIT_2026-11-03.md
│   ├── SCIENTIFIC_CONTENT_REVIEW_CHECKLIST.md
│   ├── SECRET_AND_HEALTH_DATA_CHECKLIST.md
│   ├── SOURCE_EVIDENCE_MANIFEST.md
│   └── STATIC_SECURITY_AND_TECHNICAL_AUDIT.md
├── .lychee.toml
├── .markdownlint-cli2.jsonc
├── CONTRIBUTING.md
├── README.md
└── SECURITY.md
```

## Working principles

1. Verify medical, scientific, regulatory, and technical claims against reliable primary sources.
2. Include references and publication or review dates for substantive educational content.
3. Distinguish evidence-based information from opinion, interpretation, and emerging research.
4. Protect patient privacy: never commit identifiable patient information, medical records, credentials, or confidential organizational data.
5. Review changes before publishing them to the live Blogger site.
6. Keep a clear record of material documentation and website changes.
7. Use pull requests and automated documentation checks for changes proposed to `main`.

## Current status

The repository has an established documentation and governance baseline. A documentation-quality workflow has been added on the review branch for Markdown linting and link checking. The main-branch protection document is a proposal only; repository settings have not been changed.

The live Blogger site and its runtime behavior have not been certified by the repository documentation workflow. Outstanding live-site checks remain tracked separately and require direct evidence.

## Documentation checks

GitHub Actions runs Markdown linting and link checking for pushes to `main` and `audit/**`, pull requests targeting `main`, and manual dispatches. External websites may rate-limit automated requests; investigate failures before treating them as confirmed broken links.

These checks do not validate medical claims, inspect the live Blogger runtime, scan for secrets, or deploy content to Blogger.

## License

No license is granted unless a license file is added. Blog content, branding, and other materials remain subject to their applicable ownership and rights.
