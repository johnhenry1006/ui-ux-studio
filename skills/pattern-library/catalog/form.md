---
id: form
name: Form
version: 0.1.0
status: active
source_id: null
source_version: null
---

# Form

## Problem
Submit accurate information with recovery.

## Use/avoid
Data entry; only task-essential fields.

## Behavior
Persistent labels/help/autocomplete; validate at useful times, retain values, associate errors. Prevent duplicate pending submit; real backend validates input.

## States
Default/editing/invalid/submitting/success/error-retry; explain omissions.

## Responsive
Readable single-column groups when narrow.

## Accessibility
Native labels/inputs; aria-describedby help/errors, aria-invalid where applicable. Logical focus and accessible outcome notification.

## Dependencies
Input/button/help/feedback; semantic field/error/focus/spacing tokens.

## Exceptions
Privacy/destructive actions/project submit rules.

## Example
Email-only newsletter with confirmation/retry.

## References
https://www.w3.org/WAI/tutorials/forms/labels/

Source guidance summarized; consulted 2026-10-12. Not a conformance certification.
