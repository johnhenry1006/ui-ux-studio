# State, evidence and resume

## Storage and schema
Use design/ai/ or a project equivalent through actual file tools. Packaged skills are immutable project-independent instructions. No persistence tools means export content and accurate unsaved status.

workflow.json: schema_version 1, workflow_id, project_reference, mode export/direct, steps array. Each step: id, depends_on array, status pending/ready/in_progress/blocked/complete, packet_reference, artifact_references, evidence_references, unresolved_items and acceptance_results. References resolve relative to a declared root or identified attachments. IDs unique; dependencies exist and must not cycle.

Acceptance row: criterion_id, required boolean, status pass/fail/not_run, evidence_reference string/null, evidence_provenance observed/user_provided/none, note. Actual source/check records may be evidence; user-supplied evidence is not a check executed by the current plugin.

## Transitions
Pending awaits inputs/dependencies; ready has packet/required inputs and satisfied prerequisites; in_progress means actual execution begun; blocked means a consequential missing input, permission or required failed/unrun criterion prevents progress; complete means the requested artifact exists and required criteria pass with appropriate evidence. Do not claim verified beyond scope/fidelity. Optional unrun checks stay disclosed.

Export may prepare packets for all stages while downstream remains pending until prerequisites. Generated packets do not mark external design/code complete. The prompt-writing task itself can finish with packet-creation evidence, independently from the exported implementation workflow. Imported actual outputs may advance export workflow after source/criteria checks; tag provenance.

A missing browser can be optional in a clearly source-only task, but cannot make a required rendered-UI criterion pass. If scope must change, obtain/record the revised scope before changing required flags. Do not silently exclude a failed build.

## Direct execution and dependencies
Perform only already requested/authorized actions with tools actually present. Creating a plan or selecting a provider does not start external sessions, send messages, merge or publish. Don't default to agent dispatch. Small changes skip irrelevant stages. Do not ask again for routine steps within clear authorization; ask for consequential design/scope ambiguity.

Use source/repo instructions and existing conventions. Shared component/token edits search imports/usages/CSS variables and inventory; actual changed consumers, pending consumers and runtime gaps are separate. Use UX/UI/frontend/pattern skills rather than duplicate their procedures.

## Repair
Record expected vs observed and artifact evidence, preserve correct parts/local edits, fix within scope and rerun applicable checks. Required failures remain blocked. Missing diagnostic evidence requests focused input or a labeled provisional correction.

## Resume and stale evidence
Read brief/system/pins/screens/decisions and relevant source again. Verify referenced files and revisions, inspect actual artifacts and logs, identify changes since checkpoint. Old complete/pass labels do not survive missing/changed required sources without revalidation. Mark affected criteria/steps blocked or pending; also assess dependent steps. Retain useful historical evidence with its old revision, not as proof of the current code. Resume includes objective, constraints, current sources, evidenced progress, next action, unresolved items and checks not run.
