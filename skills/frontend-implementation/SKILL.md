---
name: frontend-implementation
description: Use when implementing or modifying website or web app screens, components and interactions in a codebase, turning UI UX designs into frontend code or building a ReactJS or HTML prototype.
---

# Frontend Implementation

Implement agreed behavior with existing conventions and truthful verification.

1. Read [context](../design-studio/references/context-contract.md), repo instructions/Git changes, project brief/system/lock/screens and relevant components. Preserve user changes; do not reset or overwrite them. Find real routing/build/data conventions before adding a page.
2. Existing repo: keep its framework, language and styling. A personal preference is not a migration request; clarify scope of any explicit migration. New project: HTML/CSS/JavaScript for simple pages/prototypes or ReactJS/JavaScript/plain CSS for reusable stateful UI; do not add Next.js/TypeScript/Tailwind/UI kit without request.
3. Reuse components/tokens and implement applicable UX states, labels, keyboard/focus and responsive behavior. Mark mock data/simulated persistence; do not invent working API integration. If repo capabilities are missing, implement only verifiable scope and report it.
4. Use [verification](references/verification.md). Run available relevant checks, fix in-scope failures and rerun. No browser means no visual/browser-pass claim. Check changed interactions meaningfully rather than tests that mirror code.
5. Update records through [Pattern Library](../pattern-library/SKILL.md), search shared consumers and flag pending drift. Deliver code/files, rationale, commands/results and unverified scope via [delivery](../design-studio/references/delivery-checklist.md).

| Target | Boundary |
|---|---|
| Existing repo | Compatible minimal change, preserve edits |
| New prototype | Explicit simulated vs real behavior |
| Native app | UX/UI specification; native build not promised |

Example: Vue/TS/Tailwind Settings → preserve stack and local notification edit → use existing route/components → report actual tests; personal React preference does not rewrite repo.

Common mistakes: unsolicited migrations, adding dependencies reflexively, route claims without router, declaring success after a failed build and ignoring affected screens.

For selected header/item/component edits use [UI Refinement](../ui-refinement/SKILL.md); for preview/selection/fidelity and refresh use [UI Preview](../ui-preview/SKILL.md). Retain current task scope and existing contracts.
