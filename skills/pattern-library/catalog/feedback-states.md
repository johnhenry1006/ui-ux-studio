---
id: feedback-states
name: Feedback states
version: 0.1.0
status: active
source_id: null
source_version: null
---

# Feedback states

## Problem
Understand progress, absent content and recovery.

## Use/avoid
State affects a task; omit irrelevant states with reason.

## Behavior
Distinguish empty data/no matches; loading retains context, error offers recovery, success means actual completion. Prefer inline local status.

## States
Loading/empty/no matches/success/warning/error-retry; offline if applicable.

## Responsive
Keep message/action visible, limit layout shifts.

## Accessibility
Appropriate status/alert semantics, concise/non-color cues, no repeated announcements or focus stealing.

## Dependencies
Status/empty/error/retry; semantic feedback/type/spacing tokens.

## Exceptions
Record safe retry/product risk.

## Example
Invoice load error offers retry rather than claiming zero invoices.

## References
https://www.w3.org/WAI/tutorials/forms/notifications/

Source guidance summarized; consulted 2026-10-12. Not a conformance certification.
