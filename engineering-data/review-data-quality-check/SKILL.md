---
name: review-data-quality-check
description: Reviews a proposed Rubber Duck Industries data-quality check for usefulness, reliability, and clear ownership. Use when data engineers are adding or changing checks for validity, completeness, uniqueness, consistency, or timeliness.
---

# Review a data-quality check

Evaluate:

- the failure the check is meant to catch;
- the metric, query, threshold, and evaluation window;
- expected false positives and false negatives;
- behavior for late or missing data;
- alert destination and accountable owner; and
- the action someone should take when it fails.

Reject checks that cannot lead to a clear response. Prefer a small number of actionable checks over noisy coverage.
