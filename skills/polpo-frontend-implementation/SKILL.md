---
name: polpo-frontend-implementation
description: Use for frontend build/review tasks in Next.js/React (Tailwind + shadcn/ui), with concrete focus on component structure, UX flows, and production readiness.
---

## Purpose

Guide practical frontend implementation decisions for Polpo projects with focus on usability, delivery speed, and maintainable component structure.

## When to use

Use this skill when:
- implementing or refactoring real UI components/pages in Next.js + React
- reviewing a screen for mobile-first layout, CTA clarity, and accessibility basics
- structuring form/conversion flows and validating UI states (loading/error/success)
- checking production readiness (performance basics + Vercel deployment constraints)

Do not use this skill for back-end workflow logic or non-UI architecture decisions.

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
- UI recommendations that skip accessibility or state-handling checks
