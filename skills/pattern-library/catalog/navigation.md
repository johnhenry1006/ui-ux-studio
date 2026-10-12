---
id: navigation
name: Navigation
version: 0.1.0
status: active
source_id: null
source_version: null
---

# Navigation

## Problem
Locate destinations and current location.

## Use/avoid
Multiple destinations; avoid app navigation for a single landing page.

## Behavior
Stable names/order/current indicator; distinguish links/actions, preserve back/deep links.

## States
Current, expanded/collapsed, unavailable when relevant.

## Responsive
Compact disclosure or alternate layout, essential paths reachable.

## Accessibility
Nav landmark, links, aria-current; disclosure button conveys expanded state. Visible focus/keyboard. Ordinary site nav is not automatically an ARIA menu.

## Dependencies
Navigation/link/disclosure; semantic text/action/focus/spacing tokens.

## Exceptions
Record hierarchy/permissions.

## Example
Dashboard sidebar becomes labeled disclosure.

## References
https://www.w3.org/WAI/ARIA/apg/patterns/disclosure/

Source guidance summarized; consulted 2026-10-12. Not a conformance certification.
