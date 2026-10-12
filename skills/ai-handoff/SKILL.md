---
name: ai-handoff
description: Use when adapting a UI UX or frontend prompt for Codex, Claude, Devin, Kimi or another AI, preparing copyable handoff packets, explaining how to run prompts or transferring a design task between chat and coding environments.
---

# AI Handoff

Adapt delivery and execution instructions while retaining the task contract.

1. Obtain a core packet via [Prompt Builder](../prompt-builder/SKILL.md). Read its objective, scope, stack, pinned patterns, outputs/criteria and actual sources. If missing, build or request the consequential parts first.
2. Identify provider and surface; read [profile contract](references/profile-contract.md). Ask when ambiguous surface changes execution. Use only the selected profile: [Codex](profiles/codex.md), [Claude](profiles/claude.md), [Devin](profiles/devin.md), [Kimi](profiles/kimi.md), [generic](profiles/generic.md). Other providers use generic with unverified-specific guidance disclosed.
3. Confirm target capabilities independently of documentation/brand. An export producer having file tools does not prove the recipient has them. Mark unestablished capabilities unknown; adapt to attachment/inline/manual delivery when needed.
4. Produce a copyable variant and [execution guide](templates/execution-guide.md), plus context map/checklist/repair packet. Preserve objective, constraints, required flags and pattern versions. Explain prerequisites, context placement, prompt order, expected output, checks, recovery and resume. Do not execute the target task merely because you exported it.
5. For direct work use Vibe Coding Workflow when available, at the current host. External provider names produce packets unless an actual authorized integration exists. Do not create sessions/playbooks, log in, send data externally or override instruction files/settings by default.

| Surface | Handoff |
|---|---|
| Repo-capable coding environment | Accessible root/files, project instructions, actual scripts/checks |
| Chat without repo/browser | Attachments/inline sources, artifact export, manual checks |
| Unknown/other | Clarify consequential surface or generic fallback |

Example: one Reports contract exported to four providers retains ReactJS/plain CSS and data-table@0.1.0; only context delivery and execution guide differ.

Common mistakes: treating profiles as permissions, claiming live provider execution from local trials, adapting away stack/criteria, overwriting AGENTS.md/CLAUDE.md, or shipping unusable local paths as attachments.
