# Changelog

All notable changes to this repository are documented here.

## v0.2.0

- Added reusable Claude Code prompt templates in `templates/claude-code/` for common Polpo execution workflows.
- Added templates for implementation, review, prompt audit, n8n workflow review, frontend change, and client delivery summary.
- Updated `README.md` to document templates and their purpose.
- Updated `docs/USAGE.md` with guidance on when to use a skill vs a template.

## v0.1.1

- Refined skill trigger descriptions to improve skill selection consistency.
- Clarified "do not use" boundaries to reduce overlap between skills.
- Sharpened anti-pattern guidance so misuse is easier to detect during review.
- Added multi-skill invocation order guidance in `docs/USAGE.md`.

## v0.1.0

- Initial repository structure created.
- Added base documentation files (`README.md`, `docs/INSTALL.md`, `docs/USAGE.md`, `docs/CHANGELOG.md`).
- Added first five Polpo skills:
  - `polpo-technical-operator`
  - `polpo-claude-prompt-auditor`
  - `polpo-n8n-architect`
  - `polpo-frontend-implementation`
  - `polpo-client-delivery`
