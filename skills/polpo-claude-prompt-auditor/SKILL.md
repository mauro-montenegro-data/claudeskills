---
name: polpo-claude-prompt-auditor
description: Use for creating, auditing, and refining Claude Code prompts with strong context, clear acceptance criteria, safety controls, and efficient token usage.
---

## Purpose

Improve prompt quality for Claude Code while reducing token cost and preserving result quality, constraints, and safety.

## When to use

Use this skill when:
- writing new operational prompts for engineering tasks
- reviewing prompts before repeated team usage
- simplifying long prompts without losing requirements
- adding clearer acceptance criteria and guardrails

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
