---
name: rubber-duck-skills
description: Routes Rubber Duck Industries work to the authoritative company-wide or team skill in the central skills repository. Use when a request concerns Rubber Duck Industries processes, internal communication, HR, operations, backend engineering, frontend engineering, data engineering, or when an agent needs to discover the company's current instructions for a task.
---

# Rubber Duck Industries skill router

Use <https://github.com/bart6114/rubber-duck-industries-skills> as the source of truth.

## Workflow

1. Read the repository's current `README.md` from the default branch.
2. Find the narrowest skill whose stated purpose matches the request.
3. Read that skill's `SKILL.md` from the repository and follow it.
4. Load linked references, scripts, or assets only when the selected skill requires them.
5. If several skills apply, use the smallest set that fully covers the task and state the order.

Prefer team-specific guidance over company-wide guidance when both cover the same subject. Follow direct user instructions over repository guidance.

If the repository cannot be accessed, say so and ask the user how to proceed. Do not reconstruct or guess company-specific instructions from memory.

If no listed skill applies, handle the request normally and make clear that no company-specific skill was used.
