---
name: rubber-duck-skills-updater
description: Maintains the Rubber Duck Industries skills repository by turning requested additions, edits, moves, or removals into reviewed pull requests. Use whenever a Rubber Duck Industries skill or the repository's skill index needs to change.
---

# Rubber Duck Industries skills updater

Maintain <https://github.com/bart6114/rubber-duck-industries-skills> through pull requests.

## Workflow

1. Read the current `README.md` and `AGENTS.md` from the default branch.
2. Inspect the affected skill and any directly related skills before editing.
3. Create a dedicated branch named `skill/<short-change-name>`.
4. Make the smallest complete change. Keep each skill concise and focused on one repeatable task.
5. Validate every changed `SKILL.md`: its directory and frontmatter `name` must match, its frontmatter must contain only `name` and `description`, and its instructions must be actionable.
6. Follow the mandatory README review in `AGENTS.md`. Update the skill directory in `README.md` whenever the inventory, ownership, path, or purpose changes.
7. Commit the change, push the branch, and open a pull request.

In the pull request, explain what changed, why it changed, which team owns it, and whether `README.md` changed. Never commit directly to the default branch, and do not merge unless the user explicitly asks.

If repository write access is unavailable, prepare the exact patch and clearly identify the access problem instead of claiming that a pull request was created.
