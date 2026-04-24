# Review Prompt Template

Project: [PROJECT]
Review target: [PR_OR_BRANCH_OR_FILES]
Objective: [OBJECTIVE]

Review the existing implementation and provide actionable findings.

## Scope
- In scope: [IN_SCOPE]
- Source material: [FILES_OR_DIFF]
- Out of scope: [OUT_OF_SCOPE]

## Constraints
- Prioritize correctness, security, maintainability, and scope adherence.
- Do not propose rewrites when a minimal fix is enough.
- Separate blocking issues from improvements.

## Expected output
1. Verdict: approve / changes requested.
2. Blocking issues (if any) with file references.
3. Non-blocking improvements.
4. Risk summary.
5. Focused retest checklist.

## Review checklist
- [ ] Requirements implemented as requested.
- [ ] No hidden scope creep.
- [ ] Error handling and edge cases covered.
- [ ] Tests/checks are sufficient for the change.
