---
name: polpo-claude-prompt-auditor
description: Use when writing or auditing Claude Code prompts for repeated team use, especially to tighten scope, acceptance criteria, and token efficiency.
---

## Purpose

Improve prompt quality for Claude Code while reducing token cost and preserving result quality, constraints, and safety.

## When to use

Use this skill when:
- turning rough task notes into an operator-ready Claude Code prompt
- auditing an existing prompt that produces inconsistent results
- compressing long prompts while preserving non-negotiable constraints
- adding explicit acceptance criteria, safety boundaries, and output structure

Do not use this skill to execute the task itself; use it to improve the prompt that will drive execution.

## Working principles

- Keep prompts short, explicit, and task-oriented.
- Separate hard constraints from preferences.
- Define clear acceptance criteria with verifiable outcomes.
- Remove duplicate context and low-value prose.
- Preserve safety, privacy, and data handling boundaries.
- Favor stable templates for recurring tasks.

## Output format

Return sections in this order:
1. Prompt diagnosis (issues found)
2. Compressed prompt (improved version)
3. Change rationale (what was removed/kept)
4. Token-risk notes (possible ambiguity after compression)
5. Optional strict variant (for high-control runs)

## Anti-patterns / what to avoid

- Aggressive shortening that removes critical constraints
- Mixing unrelated objectives in one prompt
- Missing acceptance criteria
- Safety rules implied but not written
- Verbose style instructions with no operational impact
- Editing prompts without stating what behavior change is expected
