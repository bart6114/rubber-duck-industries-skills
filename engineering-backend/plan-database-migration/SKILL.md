---
name: plan-database-migration
description: Plans a safe Rubber Duck Industries database schema or data migration. Use when backend engineers need deployment ordering, compatibility steps, backfill, verification, rollback, and monitoring guidance.
---

# Plan a database migration

Describe:

1. the current and target state;
2. compatibility between old and new application versions;
3. schema-change and deployment order;
4. backfill method and load controls;
5. verification and monitoring; and
6. rollback or forward-fix strategy.

Prefer expand-and-contract changes for live systems. Explicitly flag locking, long transactions, irreversible transformations, and assumptions about data volume.
