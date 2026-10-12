# Verification

Inspect available package scripts/test setup and repo instructions. Do not invent commands as executed. Choose checks appropriate to change; don't install new tooling just to claim coverage.

- Run relevant existing build/lint/test/typecheck when available. A repo using TS may require typecheck; this does not introduce TS into a new JS project.
- Exercise changed state transitions with actual data/fixtures; test pending/error/success where applicable.
- With browser: inspect relevant narrow/wide views, clipping/overflow, labels, keyboard/focus, and affected screens. Record what was observed. With no browser: mark these not run.
- Compare actual tokens/pattern/component usage with project records. Search imports and CSS variable references for shared changes, including indirect consumers where possible.
- Rerun a failed check after repair. Report unresolved and unrelated failures by name. Don't transform a failed build into a passing claim by excluding it silently.
- State checks absent due to missing scripts/dependencies/tools. A source-only fixture with no runnable app cannot prove render/build success.

For new React state decisions use official docs: https://react.dev/learn/sharing-state-between-components . For form semantics see https://www.w3.org/WAI/tutorials/forms/labels/ and https://www.w3.org/WAI/tutorials/forms/notifications/ (consulted 2026-10-12). Adapt current documentation to the installed version; retain JavaScript/plain CSS defaults.
