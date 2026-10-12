---
id: data-table
name: Data table
version: 0.1.0
status: active
source_id: null
source_version: null
---

# Data table

## Problem
Compare records and act on rows.

## Use/avoid
Comparable tabular data, not layout. Sorting/filtering only as needed.

## Behavior
Stable columns/row identity/actions; specify sort/pagination/selection when relevant, preserve context.

## States
Loading/empty/no matches/populated/error-retry; applicable sort/selection.

## Responsive
Intentional horizontal scroll or defined alternative preserving header meaning.

## Accessibility
Prefer native table/headers; aria-sort and operable sort controls. Interactive grid needs a separate keyboard model; avoid grid role for ordinary tables.

## Dependencies
Table/header/row/action/feedback; type/border/spacing/focus tokens.

## Exceptions
Pinned columns/large data/grid require explicit decisions.

## Example
Customers, Orders and Reports reuse table rules.

## References
https://www.w3.org/WAI/ARIA/apg/patterns/table/

Source guidance summarized; consulted 2026-10-12. Not a conformance certification.
