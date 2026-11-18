# boxinnovate/.github

Organisation-wide **issue forms** and **pull request template** for every boxinnovate repository that has no
templates of its own. GitHub reads these only from a public repo named `.github`, which is why this one exists.
It contains templates only — no code, no data.

## What's here

| File | Used for |
|---|---|
| `.github/ISSUE_TEMPLATE/1-feature.yml` | Feature / Epic — goal, work per repo, tenant flag, done-when |
| `.github/ISSUE_TEMPLATE/2-bug.yml` | Bug found before production |
| `.github/ISSUE_TEMPLATE/3-prod-bug.yml` | Production bug — server, tenant ids, Problem → How it happened → Where → Expected → Notes for the fix |
| `.github/ISSUE_TEMPLATE/4-tech-debt.yml` | Tech debt / Ops / Chore |
| `.github/ISSUE_TEMPLATE/config.yml` | Blank issues off; link to the delivery board |
| `pull_request_template.md` | `Fixes` / `Refs` line, tenant-flag checklist, how it was tested |

Every issue form adds the new issue to the **AcadWin Delivery** project board automatically.

## Rules the templates carry

- **No customer names, emails or personal data** in any issue or PR — tenant and exam ids only.
- **Feature = tenant flag**, OFF by default (one sub-flag per new capability inside a feature).
- **`Fixes` closes an issue only when the change reaches `release`** (the default branch, via the release PR).
  Sibling repos use `Refs`; a bug seen on the single-tenant server uses `Refs` everywhere.

## Do not edit here

This repo is a **published copy**. The source lives in the team's private tooling repo
(`dot-claude/pmo/github-templates/`) and is pushed with `dot-claude/pmo/scripts/publish-templates.sh`.
Edits made directly here are overwritten on the next publish — change the source, then re-publish.
