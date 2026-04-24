# Polpo Claude Skills Repository

This repository is a version-controlled library of reusable Claude Code skills used by Polpo.

It is the source of truth for shared skills that guide technical work, prompt quality, workflow design, frontend implementation, and client delivery.

## What this repository contains

- Reusable skills in `skills/`
- Reusable prompt templates in `templates/claude-code/`
- Installation guidance in `docs/INSTALL.md`
- Usage guidance in `docs/USAGE.md`
- Version history in `docs/CHANGELOG.md`

## Skill vs template vs `CLAUDE.md` vs task prompt

### Skill
A skill is a reusable instruction module stored in `SKILL.md` with a clear scope and output expectations. Skills are meant to be reused across many tasks and projects.

### Template
A template is a copy/paste prompt scaffold with placeholders (for example `[PROJECT]`, `[OBJECTIVE]`, `[FILES]`, `[CONSTRAINTS]`) used to quickly prepare recurring task requests for Claude Code or Codex.

### `CLAUDE.md`
`CLAUDE.md` is project-level guidance for a specific repository or environment. It defines local rules, constraints, and conventions for work inside that repo.

### Task prompt
A task prompt is the request for one concrete job (for example, "refactor this file" or "draft a client handoff"). It should use skills, templates, and project context when relevant.

## Included skills

- `polpo-technical-operator`
- `polpo-claude-prompt-auditor`
- `polpo-n8n-architect`
- `polpo-frontend-implementation`
- `polpo-client-delivery`

## Included templates (`templates/claude-code/`)

- `implementation-prompt.md`
- `review-prompt.md`
- `prompt-audit.md`
- `n8n-workflow-review.md`
- `frontend-change.md`
- `client-delivery-summary.md`

> Before expanding the library with new skills, audit existing skills for trigger precision and boundary clarity to avoid overlap.

## Recommended installation approaches

### Option 1: Global user skills
Copy or symlink selected skill folders into:

- `~/.claude/skills/`

This makes skills available across repositories.

### Option 2: Project-specific skills
Copy selected skill folders into:

- `<repo>/.claude/skills/`

This keeps skills scoped to a single project.

See detailed commands in `docs/INSTALL.md`.
