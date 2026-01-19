---
trigger: always_on
---

# Agent Instructions

A Next.js 16.1 application (App Router) with PostgreSQL and Prisma.
All commands must use **PowerShell** (Windows).

## Essential Commands

- **Install:** `pnpm install`
- **Dev:** `pnpm dev`
- **Build:** `pnpm build`
- **DB:** `pnpm db:generate`, `pnpm db:migrate`

## Documentation Index

Detailed instructions are split by topic in the `docs/` folder:

- **[Tech Stack](../docs/tech-stack.md):** Frameworks, libraries, and versions.
- **[Project Structure](../docs/project-structure.md):** File layout and key files.
- **[Frontend Guidelines](../docs/frontend-guidelines.md):** React components, styling, and coding standards.
- **[Git Workflow](../docs/git-workflow.md):** Commit message conventions.
- **[SEO Strategy](../docs/seo-strategy.md):** Keywords, metadata, and structured data.
- **[Troubleshooting](../docs/troubleshooting.md):** Common errors and resolution steps.

## Critical Rules

1. **Always use PowerShell.**
2. **Diagnose Context:** If an error occurs, checking `next-devtools` tools or `troubleshooting.md` first.
3. **Progressive Disclosure:** Refer to specific docs above when diving into a specific task domain.