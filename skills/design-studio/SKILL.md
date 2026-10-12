---
name: design-studio
description: Use when a designer or developer requests website or app UI UX work, design prompts for an AI, prompt handoff, a vibe coding workflow, an interface audit, frontend implementation, multiple pages or continuation of a design project needing context coordination.
---

# Design Studio

Coordinate only the work required by the user's task. Match the user's language; use professional design terminology with concrete explanations.

1. Read [context contract](references/context-contract.md). Establish task mode, project sources and actual tool capabilities. Reuse an existing brief; ask only consequential missing questions.
2. For “continue / same as before”, obtain and read the prior project files before extending its design system. If unavailable, ask for brief/design system/inventory or an accessible location. If the user instead requests a standalone provisional draft, label it and record assumptions; do not represent it as the previous project.
3. Route by need, loading the linked skill body rather than treating its name as instructions:

| Need | Skill |
|---|---|
| Purpose/scope unclear | [Project Brief](../project-brief/SKILL.md) |
| Flow, navigation, task/state behavior | [UX Design](../ux-design/SKILL.md) |
| Layout, visual direction, components | [UI Design](../ui-design/SKILL.md) |
| Existing interface problems | [Design Audit](../design-audit/SKILL.md) |
| Frontend code | [Frontend Implementation](../frontend-implementation/SKILL.md) |
| Reuse, consistency, version updates | [Pattern Library](../pattern-library/SKILL.md) |
| Write or repair a task prompt | [Prompt Builder](../prompt-builder/SKILL.md) |
| Adapt a packet for an AI / explain execution | [AI Handoff](../ai-handoff/SKILL.md) |
| Export/direct workflow, evidence or resume | [Vibe Coding Workflow](../vibe-coding-workflow/SKILL.md) |

4. Keep a single source of truth per data item. Read relevant project tokens/patterns before a screen; update inventory/decisions after changes. Use Pattern Library for shared changes.
5. Deliver according to [delivery checklist](references/delivery-checklist.md). Stop at the requested artifact; do not force research, code or publication into a small task.

Prompt-only tasks create packets, not the described app. Target provider/surface/capabilities must be identified separately from the producing host. Exported workflow progress is separate from actual execution evidence.

Example: “Add Reports using our table” → read brief/system/lock and current table code → choose UX/UI/frontend work needed → reuse pinned table pattern → update screen mapping → report checks and remaining issues.

Common mistakes: assuming cross-session memory, loading every reference, treating a design suggestion as an approved project rule, or claiming tools the host does not expose.
