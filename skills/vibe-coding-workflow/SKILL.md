---
name: vibe-coding-workflow
description: Use when planning or executing a standard AI-assisted UI UX and frontend workflow, coordinating prompts across steps, tracking acceptance evidence, repairing drift or resuming a design project across sessions or AI environments.
---

# Vibe Coding Workflow

Progress by verified artifacts and task scope, not optimistic completion labels.

1. Read [context](../design-studio/references/context-contract.md), actual project sources and [state/evidence rules](references/state-and-evidence.md). Choose export or direct. Missing consequential sources/authorization block dependent work; a small task enters at its relevant step.
2. Build packets with [Prompt Builder](../prompt-builder/SKILL.md) and recipient guides with [AI Handoff](../ai-handoff/SKILL.md). Keep objective/stack/pins/required criteria fixed across surfaces.
3. Use applicable stages only: context → UX/UI → shared components → screens → verify/repair → synchronize/deliver. Use existing domain skills for the actual design, audit, frontend and pattern work. Preserve user edits; new visual choices stay proposed until agreed when consequential.
4. Record steps in [workflow](templates/workflow.json). Export prepares packets and manual guides; it does not execute the app or start external agents. Direct uses current tools within authorization. Produce actual artifacts/diffs/check evidence before completion.
5. Fail/not_run/missing evidence on a required criterion blocks the step. Optional unrun checks remain disclosed. Use scoped repair, then rerun relevant checks; do not lower required to hide failure.
6. Update project system/pins/inventory/decisions for actual changes. Shared edits require code search plus inventory, including missed/indirect consumers; report remaining source/runtime gaps. Save [resume packet](templates/resume-packet.md) and read current sources again next session.

| Situation | State |
|---|---|
| Packet exported, no execution | Ready if inputs/dependencies sufficient; otherwise pending/blocked |
| Required check fails or lacks evidence | Blocked, with unresolved items |
| Artifacts + required scope criteria evidenced | Complete at declared fidelity; optional gaps still listed |
| Old log but sources missing/stale | Revalidate, block affected work; no reused pass |

Example: source-only table caption task → locate four consumers including an omitted screen → change component/callers → inspect source/records → source criteria pass; browser optional not_run, no render claim.

Common mistakes: complete-by-log, export-as-execution, blanket rewrite/migration, reflexive approvals, invented checks or pretending a provider profile is an integration.
