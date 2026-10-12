# Lifecycle and contracts

## Storage
Use existing repo location; default design/. Shared preferences/library live outside repos in a user-selected accessible folder. Packaged catalog is immutable seed. Read user files again on new sessions. Without persistence/read tools provide exportable content and disclose limitation.

## Contracts
Pattern YAML: id, name, version, status (active/deprecated), source_id and source_version (both null for originals). Versions X.Y.Z. Body: Problem, Use/avoid, Behavior, States, Responsive, Accessibility, Dependencies, Exceptions, Example. Citation URLs belong under References; upstream identity stays in source metadata.

Tokens: schema_version 1, tokens object maps semantic names to {value, css_variable, description}. Values come from project decisions; empty template is intentional. Example mapping color.action.primary to agreed value and --color-action-primary; never impose sample colors.

Lock: schema_version 1, patterns array of {id, version, project_path}. Paths relative to design-data root must resolve and match ID/version. Adapted project records have their own version; source metadata pins upstream. Untouched seeds keep seed version. Do not hide upstream/project differences by overwriting metadata.

Screens: ID, route/name, status (planned/designed/implemented), component IDs/source paths, pattern IDs/versions, sync status (current/pending/unverified with evidence). A route without router implementation stays planned. Decisions: date, choice, reason, evidence/assumptions, affected screens, exceptions. Do not create duplicate authoritative locks/inventories.

## Select/adapt
Inspect existing UI/code first. Copy a selected seed only if no equivalent exists; pin it. Behavior changes create a project version and decision with upstream source. New records 0.1.0; corrections patch, compatible additions minor, incompatible behavior major. Explain impact; semver is not proof of compatibility.

## Shared change
Find imports, CSS token references and indirect/composed consumers using available search. Compare source/inventory; add discovered screens. Static search does not prove exhaustive runtime coverage. Update requested scope, mark remaining consumers pending/unverified and align docs/code.

## Upgrade
New library releases change nothing automatically. On explicit request compare behavior/dependencies/states, identify screens, migrate within scope, rerun checks, update record/source/lock for completed migration. Document pending screens and prior versions.

## Promote/deprecate
Promote only on request. Remove brands/private data/project URLs and assumptions; retain transferable behavior. Record source without sensitive detail. Do not silently update other projects. Deprecation explains replacement/migration; do not delete pinned records.
