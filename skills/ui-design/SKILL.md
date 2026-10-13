---
name: ui-design
description: Use when designing screen layouts, visual directions, typography, color, spacing, responsive UI, components and design tokens for websites or apps, including consistency across multiple pages.
---

# UI Design

Create a visual system that supports agreed UX and project identity.

1. Read [context](../design-studio/references/context-contract.md), brief, UX contract, project tokens/components and relevant [patterns](../pattern-library/SKILL.md).
2. For new projects without a direction offer two or three meaningfully different visual approaches with reasons; select through user feedback. Existing projects extend the established system. Project rules override personal taste unless an explicit scoped override is requested.
3. Define hierarchy, layout, typography, semantic colors, spacing, components/variants and applicable states. Do not invent exact values for an unresolved token. Use project tokens/CSS variables; record any new choice and impact.
4. Apply [UI checklist](references/ui-checklist.md). Design content-driven responsive layouts; include realistic content, long labels and relevant interaction states. Keep prototype fidelity and simulated data explicit.
5. Update system/tokens/screens/decisions via Pattern Library; align a visual change with actual component code when implementation is requested. Deliver the screen specification or supported visual/prototype artifact plus rationale and checks.

| Context | Choice |
|---|---|
| Existing UI | Reuse components/tokens/conventions |
| New simple page | HTML/CSS/JavaScript prototype |
| New stateful UI | ReactJS/JavaScript/plain CSS |

Example: project billing uses purple action token and 4px spacing despite personal blue/6px preference; mobile one-column hierarchy preserves plan/payment/invoice actions and states.

Common mistakes: generic decoration unrelated to product, silently changing shared tokens, arbitrary color values replacing named tokens, desktop-only screens and implementation details in user-facing flows.

For selected header/item/component edits use [UI Refinement](../ui-refinement/SKILL.md); for preview/selection/fidelity and refresh use [UI Preview](../ui-preview/SKILL.md). Retain current task scope and existing contracts.
