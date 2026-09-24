# Repository instructions

These instructions apply to every file in this repository.

## Before making changes

- Read `README.md` to understand the repository layout and routing model.
- Put company-wide skills in `company-wide/` and team-specific skills in the matching team directory.
- Keep each skill focused on one repeatable task.
- Use lowercase, hyphenated directory names. The directory name must match the skill's frontmatter `name`.
- Limit `SKILL.md` frontmatter to `name` and `description`.

## Required before every commit

Always review `README.md` before creating a commit and make sure it is up to date with the proposed changes.

Update `README.md` in the same commit whenever a skill is added, removed, renamed, moved, reassigned to another team, or materially changes purpose. Check that:

- every skill appears under the correct team;
- every skill link resolves to the correct `SKILL.md`;
- each one-line description still reflects the skill;
- the two explicitly installed entry-point skills remain clearly identified; and
- the routing explanation still matches the repository structure.

Do not create the commit until this README review is complete, even when no README edit is ultimately necessary.

## Pull requests

- Make skill changes on a dedicated branch.
- Use a short, descriptive commit and pull-request title.
- Explain which skill changed, why it changed, and whether `README.md` needed an update.
- Do not merge the pull request unless the user explicitly asks you to merge it.
