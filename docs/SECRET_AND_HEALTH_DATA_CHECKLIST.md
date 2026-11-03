# Secrets and Health Data Safety Checklist

Use this checklist before committing, uploading, sharing, or publishing any repository file, issue, pull-request comment, screenshot, log, or exported dataset.

## 1. Credentials and access material

- [ ] No passwords, API keys, access tokens, OAuth codes, session cookies, private keys, certificates with private key material, or database connection strings.
- [ ] No credential-bearing URLs, signed URLs, webhook secrets, or authorization headers.
- [ ] No production configuration containing secrets; use clearly named placeholders such as `REPLACE_WITH_SECRET`.
- [ ] No browser profiles, local environment files, backup archives, or debug dumps that may contain credentials.
- [ ] Any suspected exposed credential has been revoked/rotated through its provider; deleting the file alone is not sufficient.

## 2. Patient and health information

- [ ] No patient name, national or medical record number, phone number, address, exact date of birth, face, voice, or other direct identifier.
- [ ] No combination of dates, location, rare diagnosis, procedure, occupation, or family details that could re-identify a person.
- [ ] No screenshots or documents showing patient lists, EHR screens, labels, prescriptions, laboratory reports, imaging identifiers, or appointment schedules.
- [ ] No free-text clinical notes, discharge summaries, referral letters, or insurance claims containing identifiable details.
- [ ] Any dataset is demonstrably synthetic or appropriately de-identified under the applicable legal and institutional requirements; pseudonymization alone is not anonymization.
- [ ] Small cells and rare conditions are assessed for re-identification risk before aggregate statistics are shared.

## 3. Institutional and third-party confidentiality

- [ ] No confidential hospital, insurer, vendor, employee, or partner information without documented authorization.
- [ ] No internal contracts, pricing, credentials, security diagrams, incident reports, or non-public correspondence.
- [ ] Third-party code, images, fonts, datasets, and documents have a documented right to use and redistribute where applicable.

## 4. Repository and workflow hygiene

- [ ] Review the complete diff, including hidden files and generated artifacts.
- [ ] Search for likely secret patterns and inspect matches manually; automated scanners can produce false positives and miss secrets.
- [ ] Confirm GitHub secret scanning and push protection availability/status in repository settings; this checklist does not prove those controls are enabled.
- [ ] Use least-privilege workflow permissions and avoid printing secrets in logs.
- [ ] Use synthetic examples in issues and documentation.
- [ ] If sensitive information is discovered in Git history, restrict access as appropriate and follow the relevant credential revocation and incident-response process; a new commit does not erase historical exposure.

## 5. If a possible disclosure is found

1. Stop further publication or sharing.
2. Do not copy the sensitive value into an issue or chat.
3. Notify the repository owner through a private channel.
4. Revoke or rotate exposed credentials promptly.
5. Assess whether the information was accessed or redistributed and follow applicable organizational/legal incident procedures.
6. Remove exposed material from active files and, where necessary, coordinate careful history remediation.
7. Record the incident without reproducing the sensitive content.

**Rule:** When uncertain whether health information is safe to publish, do not commit it. Seek the appropriate privacy, security, or institutional review first.
