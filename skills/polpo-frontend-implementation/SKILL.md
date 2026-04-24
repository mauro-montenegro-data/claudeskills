---
name: polpo-frontend-implementation
description: Use for Polpo and client frontend execution across Next.js, React, Tailwind, shadcn/ui, UX flows, forms, and mobile-first delivery.
---

## Purpose

Guide practical frontend implementation decisions for Polpo projects with focus on usability, delivery speed, and maintainable component structure.

## When to use

Use this skill when:
- planning or implementing Next.js and React interfaces
- building landing pages or institutional websites
- creating form flows and conversion-oriented UX sections
- applying Tailwind and shadcn/ui in production-ready structures
- reviewing frontend readiness for Vercel deployments

## Working principles

- Start mobile-first; scale up for tablet and desktop intentionally.
- Prioritize clear information hierarchy and conversion paths.
- Keep components small, composable, and easy to reuse.
- Favor Tailwind utility clarity over complex styling indirection.
- Use shadcn/ui as base primitives, then customize minimally.
- Keep copy concise, concrete, and aligned with business value.
- Consider performance basics early (image sizing, rendering strategy, bundle awareness).
- Check deployment constraints that affect Vercel behavior.

## Output format

Return sections in this order:
1. UI objective and audience context
2. Proposed page or component structure
3. UX and copy guidance
4. Implementation notes (Next.js/React/Tailwind/shadcn)
5. Responsiveness and accessibility checks
6. Deployment awareness notes (Vercel)

## Anti-patterns / what to avoid

- Desktop-first layouts adapted late to mobile
- Excessive custom UI before using existing primitives
- Long generic marketing copy without clear CTA intent
- Styling patterns that reduce maintainability
- Ignoring deployment/runtime constraints until the end
