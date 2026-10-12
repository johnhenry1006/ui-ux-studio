---
name: prompt-builder
description: Use when a designer or developer asks for prompts for AI UI UX design, frontend coding, auditing, multiple screens or correction of an AI output that drifted from project requirements.
---

# Prompt Builder

Create an executable task contract from actual project context. Prompt quality reduces ambiguity; it does not guarantee AI correctness.

1. Read [context](../design-studio/references/context-contract.md) and [prompt contract](references/prompt-contract.md). Determine whether the user wants a prompt only or also execution. Prompt-only requests authorize creating the requested packet, not implementing its target app.
2. Identify the target artifact type from explicit evidence before adapting technology: webpage/component/email message/specification, or unknown. If “newsletter email-only” is ambiguous, ask whether it means a signup webpage with an email field or an HTML email message; keep the type unknown until clarified. Read supplied/reachable brief, system/tokens, pins, inventory, decisions and repo instructions. Mark source status accurately, label minor assumptions, and preserve repo stack/local edits/project rules.
3. Use [prompt](templates/prompt.md), [context map](templates/context-map.json), [acceptance checklist](templates/acceptance-checklist.md) and [repair prompt](templates/repair-prompt.md). Include objective, source status, scope, actions, output contract and observable criteria. For a small task combine these sections into one document.
4. Record observed capabilities, not capabilities inferred from an AI brand or documentation. Use paths relative to an identified project root, or attachment/inline-section references for chat. For an input with no known location, use a nonempty logical label such as `requested:project-brief`, mark missing/unknown and revision null; this is an unresolved request, not an existing path or delivered attachment. A path without readable content is not context delivery. Exclude credentials and unrelated private data.
5. For provider adaptation use AI Handoff when available; for execution/state/resume use Vibe Coding Workflow. Deliver copyable prompt plus prerequisites/checklist and unresolved inputs. Report packet creation separately from target-task execution.

| Need | Contract |
|---|---|
| New task | Objective, authoritative sources, scope, output, evidence |
| Multi-page | Pinned pattern IDs, component reuse, actual dependency updates |
| Repair | Observed difference, preserved parts, scoped correction, rerun |

Example: Reports prompt references data-table@0.1.0 and ReactJS/plain CSS, identifies an absent brief, and requests source reuse/inventory update; it does not claim Reports was implemented.

Common mistakes: promising zero errors, vague “make it beautiful”, fabricated paths/approvals/research, secret credentials in packets, or requesting private chain-of-thought. Request concise rationale and checkable evidence instead.
