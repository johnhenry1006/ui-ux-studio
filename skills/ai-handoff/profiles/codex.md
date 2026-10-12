# Codex profile
Provider: Codex. Surfaces: coding app/CLI/cloud environment when identified; generic/manual export when access is unknown.
Checked: 2026-10-12. Provider-specific execution tested: not established by this profile.

## Context and run
1. Identify repository/root, existing AGENTS.md guidance, brief/system/pins and relevant sources. Verify access in the target environment.
2. Open the selected coding workspace. For an already installed authorized CLI, launch `codex` at the repo root; otherwise use the actual host interface.
3. Provide core prompt plus accessible references. Ask it to read project guidance and report consequential missing inputs. Keep edits in scope and preserve local changes.
4. Ask for commands/results from available repo scripts and observed artifacts. If browser missing, report visual checks not run.
5. Transfer actual results back with source revision and evidence; do not infer completed execution from exported instructions.

## Durable guidance and fallback
AGENTS.md supports project instructions. Do not overwrite it or global guidance by default. Unknown tools/permissions use generic copyable packet/manual checks; no model or API integration is assumed.

## Official sources
https://learn.chatgpt.com/docs/agent-configuration/agents-md
https://learn.chatgpt.com/docs/prompting
