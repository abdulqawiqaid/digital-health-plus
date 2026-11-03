# Main Branch Protection Proposal

**Status:** Proposal only — no GitHub repository settings have been changed.  
**Target:** `main`  
**Purpose:** Reduce accidental or unreviewed changes while preserving a practical maintenance workflow.

## Recommended rules

| Control | Proposed setting | Rationale |
|---|---|---|
| Pull requests | Require a pull request before merging | Keep changes reviewable and traceable |
| Approvals | Require at least 1 approval when another qualified reviewer is available | Independent review |
| Stale approvals | Dismiss approvals when the reviewed commit changes | Ensure approval applies to the final diff |
| Conversation resolution | Require all review conversations to be resolved | Close review feedback loops |
| Status checks | Require the Markdown lint and link-check jobs after they have run successfully | Prevent known documentation-quality failures |
| Branch updates | Require branches to be up to date before merging, if operationally practical | Reduce integration surprises |
| Force pushes | Block force pushes | Preserve history |
| Deletion | Block deletion of `main` | Protect the default branch |
| Bypass | Keep bypass access limited to repository owner/administrators and document exceptions | Least privilege |

## Safe rollout sequence

1. Confirm who can review and approve changes; do not require an approval that no available collaborator can provide.
2. Add and run the documentation CI workflow on the review branch.
3. Confirm the exact status-check names reported by GitHub; select those names rather than guessing.
4. Configure a repository ruleset or branch protection rule targeting only `main`.
5. Test the rule with a small pull request before relying on it.
6. Record the enabled settings and review them periodically.

## Important limitations

- This document is a recommendation, not an applied configuration.
- GitHub plan, repository visibility, and account permissions can affect available controls.
- If the owner is the only contributor, a one-approval requirement may block legitimate work. Consider an owner-controlled exception or no approval requirement until another reviewer is available.
- Do not enable required status checks until the workflow has completed successfully and its check names are visible in GitHub.
- Do not enable rules that unintentionally prevent emergency recovery or repository administration.

## Approval record

- [ ] Repository owner reviewed this proposal.
- [ ] Reviewer availability and exception process confirmed.
- [ ] CI checks observed on a pull request.
- [ ] Ruleset applied by an authorized owner.
- [ ] Effective settings independently verified.
