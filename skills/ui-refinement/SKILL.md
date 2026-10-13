---
name: ui-refinement
description: Use when a designer or developer wants to change only a header, button, card, text item, spacing or another selected UI detail, preserve the rest of an interface or reverse a specific previous UI change.
---

# UI Refinement

Edit the identified target and requested properties while preserving everything outside the agreed scope.

1. Read [context](../design-studio/references/context-contract.md), current source/local diff and [refinement contract](references/refinement-contract.md). Reuse supplied brief/system/pins/screens. Identify direct edit or export only, target page/region/item and expected result. Use UI Preview for live/prototype/screenshot/description selection.
2. Revalidate target and source revision immediately before editing. Repeated items need stable data/instance key; “second item” after sorting plus old revision is consequential ambiguity, not permission to guess. Missing screenshot/source/mapping stays unresolved; request focused input or label a provisional specification. Unknown revision does not establish current mapping.
3. Fill [change request](templates/change-request.json) and [prompt](templates/refinement-prompt.md). Default instance, one target, preserve list and observable criteria. Change item content at its actual record/prop/key, not the shared template. For appearance reuse an existing variant/prop/scoped style; no whole-page rewrite, global override, cloned component for text, migration or unsolicited pattern upgrade.
4. Search code imports/usages/CSS/token references plus inventory before any shared component/token edit. Include omitted consumers. Local request uses safe local variant or asks only consequential local/shared scope clarification if it cannot preserve others. Explicit user shared scope authorizes its routine steps; don't repeat approval. Use Frontend Implementation/UI Design for actual changes and Pattern Library for affected mappings/decisions.
5. Direct: make scoped patch with current tools, preserve all user edits and source contracts. Export: create packet/AI Handoff instructions, not code execution. Keep original patch/relevant before-after revision when reversal matters. Reverse only attributable hunks that still match your after-state; overlapping subsequent user edits/missing patch block stale undo pending resolution. Never reset repository or discard user edits.
6. Inspect actual diff and run applicable checks. Refresh actual preview when supported and record new revision/state. Required failed/unrun/missing evidence blocks existing workflow; source-only optional browser remains disclosed. Update project records and deliver target/scope/changed files/checks/gaps/resume. Code changed with unavailable preview is not a visual pass.

| Request | Boundary |
|---|---|
| Header smaller | Requested height/spacing only; preserve sidebar/content |
| One card text | Resolve stable item key, edit its source data |
| Shared token | Find real consumers; retain authorized scope |
| Undo my change | Original patch + current matching hunks, retain later edits |

Example: Home Header local height change discovers Hidden.jsx sharing global token; use Home-only variant and preserve shared token/Hidden/local gold badge. Common mistakes: guessed positional target, changing all cards, stale inverse patch, silently widening scope and copy/export called executed.
