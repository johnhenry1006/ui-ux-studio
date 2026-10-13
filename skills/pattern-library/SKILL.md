---
name: pattern-library
description: Use when creating reusable UI UX patterns, maintaining a shared library or project design system, adding multiple screens, tracking component dependencies, detecting design drift, or selecting, adapting and upgrading pattern versions.
---

# Pattern Library

Keep screens consistent through durable files and versioned records.

1. Read [context](../design-studio/references/context-contract.md) and [lifecycle](references/pattern-lifecycle.md). Locate equivalent files; keep one authoritative copy per item.
2. Select only relevant seeds: [navigation](catalog/navigation.md), [form](catalog/form.md), [data table](catalog/data-table.md), [search/filter](catalog/search-filter.md), [onboarding](catalog/onboarding.md), [feedback](catalog/feedback-states.md). Adapt needed behaviors to the brief.
3. Use [system](templates/design-system.md), [tokens](templates/tokens.json), [pattern](templates/pattern.md), [screens](templates/screens.md), [decisions](templates/decisions.md), [lock](templates/pattern-lock.json).
4. Before a screen inspect components and pinned patterns. After changes update mapping/decisions. For shared changes search code as well as inventory; mark affected screens current/pending/unverified individually.
5. Keep versions pinned. Upgrade/promote only on request; remove private project details before promotion. Report actual checks and unsynchronized dependencies.

| Operation | Required record |
|---|---|
| Add screen | Reused IDs/versions, source paths, sync status |
| Add/adapt pattern | Metadata, behavior/states, rationale, lock |
| Shared change | Actual consumers, affected screens, migration status |
| Upgrade | Version diff, scope, per-screen checks, lock |

Example: Reports reuses data-table@0.1.0; keep lock despite library 0.2.0; find Archived import missing from inventory.

Common mistakes: duplicate root/design locks, treating a seed as installed code, automatic upgrades, docs-only synchronization.

For selected header/item/component edits use [UI Refinement](../ui-refinement/SKILL.md); for preview/selection/fidelity and refresh use [UI Preview](../ui-preview/SKILL.md). Retain current task scope and existing contracts.
