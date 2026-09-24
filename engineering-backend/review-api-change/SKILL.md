---
name: review-api-change
description: Reviews a proposed Rubber Duck Industries API change for compatibility, correctness, security, and operability. Use when backend engineers want a focused review of an endpoint, request or response contract, or API version change.
---

# Review an API change

Check:

- backward compatibility and versioning;
- authentication and authorization;
- input validation and error behavior;
- idempotency, pagination, and rate limits where relevant;
- logging, metrics, and failure modes; and
- documentation and tests.

Report concrete risks first, then questions and optional improvements. Do not block the change for preferences that have no user or operational impact.
