# n8n Workflow Review Template

## Context
- Project: [PROJECT]
- Workflow source: [WORKFLOW_JSON_OR_REPO_PATH]

## Objective
[OBJECTIVE]

Review this n8n workflow for reliability and production readiness.

## Scope
- In scope: trigger logic, branching, node config, retries, idempotency, error paths.
- Input files: [FILES]
- Out of scope: [OUT_OF_SCOPE]

## Constraints
- Focus on practical fixes with lowest operational risk.
- Flag security/data exposure concerns explicitly.
- Do not redesign entire workflow unless required by a critical issue.

## Expected output
1. Executive verdict (ready / needs changes).
2. Critical issues and impact.
3. Recommended fixes in priority order.
4. Operational risks (failure modes, observability gaps).
5. Manual validation checklist with sample test scenarios.

## Manual validation checklist
- [ ] Trigger receives expected payload shape.
- [ ] Success path handles required fields.
- [ ] Failure path logs and alerts correctly.
- [ ] Retries/timeouts are configured safely.
- [ ] Duplicate event handling is controlled.
