---
id: search-filter
name: Search and filter
version: 0.1.0
status: active
source_id: null
source_version: null
---

# Search and filter

## Problem
Narrow results while preserving context.

## Use/avoid
Meaningful result sets; avoid elaborate controls for trivial lists.

## Behavior
Separate query/filters; choose apply-on-change or explicit apply. Preserve values, clear/reset; async code handles stale responses.

## States
Initial/searching/results/no matches/error-retry.

## Responsive
Prioritize key filters; disclose secondary ones.

## Accessibility
Persistent labels/keyboard; meaningful result-count announcements, no focus movement each update.

## Dependencies
Search/filter/disclosure/results/feedback and semantic tokens.

## Exceptions
Record URL persistence/sensitive query rules.

## Example
Orders filtered by customer/status with reset.

## References
https://www.w3.org/WAI/tutorials/forms/notifications/

Source guidance summarized; consulted 2026-10-12. Not a conformance certification.
