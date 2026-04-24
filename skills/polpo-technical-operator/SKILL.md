---
name: polpo-technical-operator
description: Use when deciding how to execute technical work (architecture tradeoffs, repo change sequencing, risk checks) before or around implementation.
---

## Purpose

Define a practical operating standard for technical work at Polpo: clear scope, minimal complexity, explicit tradeoffs, and maintainable implementation paths.

## When to use

Use this skill when:
- choosing between implementation options with different cost/risk profiles
- sequencing a repo change into minimal safe steps
- reviewing a proposal for assumptions, dependency risks, and rollback needs
- defining validation criteria before coding starts

Do not use this skill for domain-deep execution details (use the specialized skill first, then apply this one for final decision framing).

## Working principles

- Start from business and operational impact, then move to implementation.
- Prefer the simplest viable design that satisfies requirements.
- Make assumptions explicit; mark unknowns and validation steps.
- Separate must-have changes from optional improvements.
- Optimize for maintainability, handoff clarity, and predictable operations.
- Avoid introducing tools, abstractions, or layers without clear necessity.

## Output format

Return sections in this order:
1. Context snapshot
2. Recommended approach
3. Tradeoffs and risks
4. Execution plan (minimal ordered steps)
5. Validation checklist

## Anti-patterns / what to avoid

- Vague architecture advice without actionable steps
- Overengineered solutions for early-stage requirements
- Hidden assumptions or unclear dependencies
- Recommendations that ignore implementation cost
- Generic AI wording without technical specificity
- Rewriting domain-specific guidance that already exists in n8n/frontend/client-delivery skills
