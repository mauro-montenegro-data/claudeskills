# Prompt Audit Template

## Context
- Task domain: [DOMAIN]
- Original prompt:
[PASTE_PROMPT]

## Objective
Audit and compress this prompt before sending it to Claude Code/Codex.

## Scope
- Keep intent and acceptance criteria.
- Remove ambiguity, duplication, and unnecessary context.
- Preserve required constraints and output format.

## Constraints
- Keep the revised prompt concise and copy/paste ready.
- Keep placeholders where inputs are missing.
- Do not invent requirements not present in the original.

## Expected output
1. Issues found (ambiguity, missing constraints, token waste).
2. Revised prompt (final version).
3. Optional clarifying questions (max 3) only if required.

## Audit checklist
- [ ] Clear objective and scope.
- [ ] Explicit constraints.
- [ ] Defined output format.
- [ ] No conflicting instructions.
