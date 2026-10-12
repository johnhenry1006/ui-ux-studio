---
name: ux-design
description: Use when designing user flows, information architecture, navigation, screen states, forms, onboarding, task recovery or interaction behavior for a website or app.
---

# UX Design

Start from the user task and define behavior before visual polish.

1. Read [context](../design-studio/references/context-contract.md), current brief/system and relevant pinned patterns. Recover missing context; label hypotheses, not fabricated research.
2. Identify entry, desired outcome, minimum information, actions and completion. Choose only screens and steps needed; eliminate avoidable decisions.
3. Define default, loading, empty/no-results, validation, success, error/retry and permission states where applicable. Specify back/cancel, preservation and destructive-action recovery. Explain irrelevant states rather than adding them mechanically.
4. Use [flow checklist](references/flow-checklist.md). Include keyboard/focus/announcements and responsive navigation behavior. For native apps give platform-aware UX specifications; do not promise native code.
5. Update relevant screen inventory/decisions via [Pattern Library](../pattern-library/SKILL.md). Deliver flow, screen/state contract, open questions and evidence limits; feed agreed behavior to UI/frontend work.

| Artifact | Content |
|---|---|
| Flow | Entry → actions/decisions → outcome/recovery |
| Screen contract | User goal, content hierarchy, actions, applicable states |
| Validation plan | What can be tested now and what needs real users/data |

Example: email newsletter → input email → validate → submit/pending → confirmation or retry; avoid name/password/account onboarding.

Common mistakes: invented persona/research, happy-path-only flows, optional work made mandatory, and pretending mock data proves usability.
