---
name: polpo-technical-operator
description: Use for Polpo technical execution, repository changes, architecture decisions, implementation planning, and technical reviews.
---

## Purpose

Define a practical operating standard for technical work at Polpo: clear scope, minimal complexity, explicit tradeoffs, and maintainable implementation paths.

## When to use

Use this skill when:
- planning or reviewing codebase changes
- evaluating architecture or integration decisions
- preparing implementation plans
- performing technical reviews or risk assessments

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
