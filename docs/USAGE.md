# Using Polpo Skills in Claude Code

## How skills are used

Skills give Claude Code reusable instructions for specific kinds of work. They help keep output consistent, practical, and aligned with Polpo standards.

Use skills as structured guidance layers. The task prompt still defines the specific job.

## When to invoke a skill directly

Invoke a skill directly when:
- the task clearly matches that skill's scope
- you need consistent output format
- you want to reduce back-and-forth on expectations
- the work has operational or client delivery impact

If a task could match multiple skills, prefer this order:
1. **Domain execution skill first** (`polpo-n8n-architect` or `polpo-frontend-implementation`).
2. **Cross-cutting decision framing second** (`polpo-technical-operator`) if tradeoffs/sequence still need to be decided.
3. **Communication layer last** (`polpo-client-delivery`) when preparing client-facing outputs.
4. **Prompt quality layer anytime** (`polpo-claude-prompt-auditor`) when the prompt itself is the deliverable.

Examples:
- "Use `polpo-n8n-architect` to review this workflow JSON."
- "Use `polpo-client-delivery` to draft a client handoff summary."

## Test if a skill is too broad or too narrow

### Signs a skill is too broad
- It tries to cover unrelated domains.
- Output style changes too much between tasks.
- Instructions contain many optional branches with no defaults.

### Signs a skill is too narrow
- It only works for one exact project setup.
- It fails when small context changes occur.
- It forces unnecessary details before delivering value.

### Practical test
1. Run the same skill on 3 different but related tasks.
2. Check if outputs are consistent in structure.
3. Check if outputs remain useful without rewriting the skill.
4. If not, split scope (too broad) or generalize constraints (too narrow).

## Example prompts by skill

### `polpo-technical-operator`
"Use `polpo-technical-operator` to evaluate this refactor plan and return risks, tradeoffs, and a minimal execution sequence."

### `polpo-claude-prompt-auditor`
"Use `polpo-claude-prompt-auditor` to review this Claude Code prompt and reduce token usage while preserving acceptance criteria and safety constraints."

### `polpo-n8n-architect`
"Use `polpo-n8n-architect` to review this n8n webhook workflow, validate branch logic, and propose rollback and test payload notes."

### `polpo-frontend-implementation`
"Use `polpo-frontend-implementation` to plan a mobile-first Next.js landing page section with Tailwind and shadcn/ui components."

### `polpo-client-delivery`
"Use `polpo-client-delivery` to draft a concise client implementation report with delivered scope, pending items, risks, and next steps."

## Quick boundary guide (to reduce overlap)

- Use **`polpo-technical-operator`** for *how to decide and sequence technical work*.
- Use **`polpo-n8n-architect`** for *n8n workflow structure, validation, and operational safety*.
- Use **`polpo-frontend-implementation`** for *UI/component implementation and readiness checks*.
- Use **`polpo-client-delivery`** for *client-facing reporting and handoff communication*.
- Use **`polpo-claude-prompt-auditor`** for *improving prompts, not executing the underlying task*.
