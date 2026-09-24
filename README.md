# Rubber Duck Industries Skills

This repository is a small example of how a company can keep agent skills in one place without asking every employee to install every team skill.

Repository: <https://github.com/bart6114/rubber-duck-industries-skills>

## Install only these two skills

| Skill | Purpose | Path |
| --- | --- | --- |
| `rubber-duck-skills` | Finds and loads the right company or team skill for a task. | [`rubber-duck-skills/SKILL.md`](rubber-duck-skills/SKILL.md) |
| `rubber-duck-skills-updater` | Turns requested skill changes into pull requests. | [`rubber-duck-skills-updater/SKILL.md`](rubber-duck-skills-updater/SKILL.md) |

The remaining skills are not installed individually. The router reads this README, selects the narrowest relevant skill, and then reads that skill's `SKILL.md` from this repository.

## How routing works

1. A user asks for company-specific help.
2. `rubber-duck-skills` reads this README from the repository's default branch.
3. It chooses the most relevant company-wide or team skill from the directory below.
4. It reads only that skill's `SKILL.md` and follows its instructions.
5. If no listed skill applies, it answers normally and does not invent company policy.

Team-specific guidance takes precedence over company-wide guidance when both apply. Direct user instructions still take precedence over repository guidance.

## Skill directory

### Company-wide

| Skill | Use it for | Path |
| --- | --- | --- |
| `summarize-meeting` | Turn notes or a transcript into decisions, actions, and open questions. | [`company-wide/summarize-meeting/SKILL.md`](company-wide/summarize-meeting/SKILL.md) |
| `draft-company-announcement` | Draft a clear internal announcement. | [`company-wide/draft-company-announcement/SKILL.md`](company-wide/draft-company-announcement/SKILL.md) |

### HR

| Skill | Use it for | Path |
| --- | --- | --- |
| `write-job-description` | Draft a structured job description. | [`hr/write-job-description/SKILL.md`](hr/write-job-description/SKILL.md) |
| `prepare-onboarding-plan` | Create a practical first-30-days onboarding plan. | [`hr/prepare-onboarding-plan/SKILL.md`](hr/prepare-onboarding-plan/SKILL.md) |

### Operations

| Skill | Use it for | Path |
| --- | --- | --- |
| `write-runbook` | Document a repeatable operational procedure. | [`operations/write-runbook/SKILL.md`](operations/write-runbook/SKILL.md) |
| `draft-incident-update` | Write a factual internal incident update. | [`operations/draft-incident-update/SKILL.md`](operations/draft-incident-update/SKILL.md) |

### Backend engineering

| Skill | Use it for | Path |
| --- | --- | --- |
| `review-api-change` | Review an API change for compatibility and operational risk. | [`engineering-backend/review-api-change/SKILL.md`](engineering-backend/review-api-change/SKILL.md) |
| `plan-database-migration` | Plan a safe database schema or data migration. | [`engineering-backend/plan-database-migration/SKILL.md`](engineering-backend/plan-database-migration/SKILL.md) |

### Frontend engineering

| Skill | Use it for | Path |
| --- | --- | --- |
| `review-ui-change` | Review a UI change across states, devices, and accessibility. | [`engineering-frontend/review-ui-change/SKILL.md`](engineering-frontend/review-ui-change/SKILL.md) |
| `write-component-brief` | Specify a reusable UI component before implementation. | [`engineering-frontend/write-component-brief/SKILL.md`](engineering-frontend/write-component-brief/SKILL.md) |

### Data engineering

| Skill | Use it for | Path |
| --- | --- | --- |
| `document-data-pipeline` | Document the inputs, transformations, outputs, and ownership of a pipeline. | [`engineering-data/document-data-pipeline/SKILL.md`](engineering-data/document-data-pipeline/SKILL.md) |
| `review-data-quality-check` | Review whether a proposed data-quality check is useful and actionable. | [`engineering-data/review-data-quality-check/SKILL.md`](engineering-data/review-data-quality-check/SKILL.md) |

## Updating the repository

Use `rubber-duck-skills-updater` when adding, changing, moving, or removing a skill. It requires the agent to read [`AGENTS.md`](AGENTS.md), keep this directory current, work on a branch, and open a pull request rather than changing the default branch directly.

Every skill lives in a directory whose name matches the `name` in its `SKILL.md`. Keep skills concise and put detailed supporting material in a skill's `references/`, `scripts/`, or `assets/` directory only when it is genuinely needed.
