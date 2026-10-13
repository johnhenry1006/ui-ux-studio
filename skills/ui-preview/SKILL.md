---
name: ui-preview
description: Use when a designer or developer wants to view a UI preview, select or highlight a region for focused editing, refresh an interface after changes or work from screenshots when a live preview is unavailable.
---

# UI Preview

Make the interface and selected target observable at the fidelity the host actually supports.

1. Read [context](../design-studio/references/context-contract.md) and [preview contract](references/preview-contract.md). Identify project/page, current sources/local changes, direct/export task and actual render/browser capabilities. Choose live/prototype/screenshot/unavailable; a reconstruction is prototype, not the real running app. Native apps without native tooling use specifications/screenshots.
2. Use existing repo/Sites preview workflow when present. If supported, open the actual page/state/viewport; otherwise export honest preview instructions or a clearly labeled standalone prototype. No silent publish/deployment/login or external site injection. Missing browser means visual/interaction checks not_run, not pass.
3. Create [manifest](templates/preview-manifest.json) from observed sources. Map regions using stable unique IDs and instance/data keys. Verified requires actual source correspondence and current relevant revision including dirty edits; DOM text/class or screen position alone is unresolved. Identify screenshot/attachment explicitly without inventing measurements or code mappings.
4. For controlled development preview, read [integration](references/selector-integration.md) and use the opt-in selector. Selection mode highlights one target, supports keyboard/parent/clear/exit and exports explicit metadata/instruction. Without selector use [selection](templates/selection.json) by description or annotated screenshot. Do not export form values/secrets/whole DOM. Copy fallback must remain available; no automatic chat delivery assumed.
5. Before export/edit revalidate current source/instance. Old index after sort/filter, changed revision, duplicate marker, missing/replaced node or unknown mapping requires resolve/reselect. Refresh manifest after edits and clear old highlight; old checks aren't evidence for changed source. Follow UI Refinement for scoped edit and existing workflow for evidence.

| Preview | Report |
|---|---|
| Actual running app | Observed page/state/revision, untested states |
| Standalone example | Prototype, explicit demonstration data |
| Screenshot | Visible evidence only, no runtime claim |
| No renderer/source | Unavailable/unresolved packet, next input |

Deliver selected target, preview kind/revision, copyable packet and checks/gaps. Store project records outside package, normally design/ai/refinements/. Example: same-label card uses key a; sorted/replaced DOM invalidates positional selection rather than editing card b. Common mistakes: screenshot-as-runtime, mock-as-live, fake source mapping, export-as-execution and stale highlight reused after refresh.
