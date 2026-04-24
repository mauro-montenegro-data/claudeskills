---
name: polpo-n8n-architect
description: Use for n8n workflow design/review work: node architecture, data contracts, failure paths, test payloads, and rollback-safe operations.
---

## Purpose

Provide practical standards for n8n workflow engineering with emphasis on reliability, traceability, and maintainable operations.

## When to use

Use this skill when:
- reviewing workflow JSON before deploy or migration
- designing webhook/event flows with explicit validation and branch behavior
- auditing integrations (e.g., Sheets/Gmail) for field mapping and error handling
- preparing operational artifacts: test payloads, rollback snapshot notes, handoff docs

Do not use this skill for general architecture decisions outside n8n workflow design.

## Working principles

- Model workflows as clear stages: input, validation, processing, output, alerting.
- Keep node naming explicit and operationally readable.
- Validate required fields early; fail fast with actionable messages.
- Define branch logic and error paths before optimization.
- Document webhook contracts (method, path, payload shape, auth expectations).
- Track Google Sheets and Gmail dependencies with field-level mapping notes.
- Keep rollback snapshots for critical workflow revisions.
- Include realistic test payloads for success and failure paths.

## Output format

Return sections in this order:
1. Workflow objective and boundaries
2. Node-by-node architecture summary
3. Data contracts and validations
4. Failure handling and alerts
5. Test payload set
6. Rollback snapshot guidance
7. Operations documentation checklist

## Anti-patterns / what to avoid

- Unnamed or ambiguously named nodes
- Validation only at final nodes
- Missing error branches and alerting behavior
- Undocumented field mappings for Sheets or Gmail
- Deploying changes without rollback snapshot references
- Treating workflow documentation as optional after implementation
