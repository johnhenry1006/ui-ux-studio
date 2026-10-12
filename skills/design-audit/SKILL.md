---
name: design-audit
description: Use when evaluating an existing website, app interface, screenshot, prototype or frontend code for usability, visual consistency, responsive behavior, accessibility risks or conversion friction.
---

# Design Audit

Prioritize findings by user-task impact and evidence, not personal taste.

1. Read [context](../design-studio/references/context-contract.md); establish goal, scope and actual artifacts. Inspect provided image/code/page only through available tools. A written description supports conditional findings, not claims about a real image inspected.
2. Compare task flow, hierarchy, controls/states, responsive/accessibility basics and project patterns. Track observed defect separately from risk/hypothesis or aesthetic preference. Do not assert interaction defects from static evidence.
3. Use [audit report](templates/audit-report.md). Every finding has location, observation, impact, severity, recommendation and confidence. Priority: blocker prevents primary task; high causes substantial failure/confusion; medium creates recoverable friction; low is limited polish. Explain the evidence behind severity.
4. Provide actionable fixes using existing project rules. Implement only when requested; then use [Frontend Implementation](../frontend-implementation/SKILL.md) and update relevant records through [Pattern Library](../pattern-library/SKILL.md).
5. Report verified/unknown scope and retest actual fixes. Do not present a basic audit as full accessibility certification or validated conversion research.

Example: placeholders instead of labels in a description → conditional accessibility/usability risk; grey button alone does not prove disabled state or submit failure; dropdown behavior remains unknown without observation.

Common mistakes: fabricated screenshot/URL findings, subjective style as blocker, unexplained severity, and claiming fixed without rechecking.
