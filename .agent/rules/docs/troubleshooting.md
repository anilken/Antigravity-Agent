# Troubleshooting Guide

## Common Issues

### Next.js & Prisma
When encountering errors related to Prisma Client, modules, or runtime:
1. **Verify Environment:** Check `nodejs` vs `edge` runtime usage.
2. **Check Configuration:** Ensure `next.config.ts` and `prisma.schema` are aligned.
3. **Adapter:** Verify properly configured database adapter and `accelerateUrl` if using Prisma Accelerate.

### Diagnostic Tools
Use Next.js MCP tools to:
- Inspect runtime environment.
- Verify Prisma engine type.
- Detect missing configurations.

## Resolution Steps
1. Identify root cause (build vs runtime).
2. Check recent changes in `package.json` or `prisma/schema.prisma`.
3. Run `pnpm run db:generate` to refresh client.
4. Consult `docs/tech-stack.md` for version compatibility.
