# Frontend Guidelines

## Core Principles
- **React 19 & Next.js 16:** Implementation of Server Components, Actions, and async transitions.
- **Performance:** Optimization using `React.memo`, `useMemo`, `useCallback`, and advanced hooks (`useOptimistic`, `useTransition`).
- **Accessibility:** WCAG 2.1/2.2 AA compliance, ARIA patterns, and semantic HTML.
- **Styling:** Tailwind CSS 4, Design Tokens, and responsive design (mobile-first).

## Coding Conventions
### TypeScript
- Use TypeScript strict mode.
- Prefer explicit types over `any`.
- **Interfaces** for object shapes, **Types** for unions/intersections.
- **Naming:**
  - Functions: `camelCase` (e.g., `getUserData`)
  - Components: `PascalCase` (e.g., `PromptCard`)
  - Constants: `UPPER_SNAKE_CASE`
  - Files: `kebab-case.tsx` (components), `camelCase.ts` (utils)

### React/Next.js
- **Server Components** by default. Use `"use client"` only for interactivity.
- **Server Actions** instead of API routes for mutations where possible.
- **Data Fetching:** React Query/TanStack Query for server state (if client-fetched), SWR, or direct Server Component fetching.

### Boundaries
#### Always Do
- Run `pnpm run lint` before committing.
- Use existing UI components from `src/components/ui/`.
- Add translations (next-intl) for user-facing text.

#### Never Do
- Hardcode user-facing strings (use i18n).
- Access `node_modules` directly.
- Commit secrets.

## Component Architecture
1. **Atoms/Molecules:** Build reusable components in `src/components/ui/`.
2. **Feature Components:** Place in `src/components/{feature}/`.
3. **Exports:** Export directly from the file.

## Testing context
- Use React Testing Library for components.
- Playwright/Cypress for E2E.
- Jest for unit tests.
