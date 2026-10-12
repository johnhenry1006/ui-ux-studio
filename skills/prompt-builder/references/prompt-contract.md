# Prompt and context contract

## Core sections
Objective and primary user task; actual sources/status; edit scope and excluded work; technology/design constraints; actions/dependencies and consequential questions; artifact/file/screen output; observable acceptance criteria; completion evidence and limitations. Avoid inflated role claims or generic “professional design” without a concrete outcome.

Use existing UX/UI/pattern skills for domain choices rather than inventing a second design process. New-project default is ReactJS/JavaScript/plain CSS or HTML/CSS/JavaScript; existing stacks stay unchanged. Preserve pinned project patterns and local edits. Current task instructions do not override host/system/repo permission policies.

Clarify consequential artifact ambiguity: “newsletter” can mean a signup webpage or an email message. Do not silently replace a requested HTML/CSS/JavaScript webpage with an email-client template; identify the intended artifact or label a provisional interpretation.

## Context map
schema_version 1; task_id/provider/surface; context_items with role/reference/access_status (read/provided/unknown/missing), revision string/null and required boolean. Read means actually read in the producing environment; it is not proof a receiving AI can access it. Guide explains how the recipient obtains each required item. Capabilities/evidence describe the identified target environment; recheck on arrival.

Every item reference is a nonempty string: a real project-relative path, attachment label or inline section ID. When a source has no known location, use a logical request label such as `requested:project-brief`, with access_status missing or unknown and revision null. This label names an unresolved input; it is not a file path, attachment delivered, or readable content. Keep required true when execution depends on that input. Do not use null for item references; capability evidence and unknown revisions may remain null.

Seven capability keys: read_files, edit_files, run_commands, inspect_images, browser, persist_files, external_actions. Value available/unavailable/unknown. capability_evidence uses the same keys and source-reference/null. Available requires tool/access actually established; provider docs alone are insufficient. Templates start unknown with null evidence. Surface unknown requires clarification when it affects execution or generic/manual fallback.

## Acceptance and repairs
Checklist rows: criterion ID, required boolean, observable criterion/check, pass/fail/not_run, evidence reference and provenance observed/user_provided/none. Required criteria are agreed before execution; do not lower required to hide failures. Not-run is not pass. Source checks do not prove runtime, accessibility or usability.

Repair references actual bad artifact/diff and expected behavior. Retain objective, stack, pattern pins, correct parts and user edits. Correct only stated drift, then rerun checks that can actually run. Missing evidence triggers a request for it or a provisional repair explicitly labeled, not an invented diagnosis. One repair does not authorize a migration or whole-project rewrite.

## Output and storage
Packet: prompt.md, context-map.json, acceptance-checklist.md, repair-prompt.md; AI Handoff supplies execution-guide.md. Small tasks may use one document with equivalent sections. Save in design/ai/ or equivalent only through available persistence tools; otherwise export content with accurate unsaved status. Do not store project progress in packaged skills. Refer to the project root/attachment label, not private absolute paths that another environment cannot resolve.
