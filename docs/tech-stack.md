# Technology Stack

## Core
- **Framework:** Next.js 16.1 (App Router) with React 19.2
- **Language:** TypeScript 5
- **Database:** PostgreSQL with Prisma 7 ORM
- **Authentication:** NextAuth.js 5 (beta) with pluggable providers (credentials, GitHub, Google, Azure)
- **Styling:** Tailwind CSS 4 with Radix UI primitives
- **Internationalization:** next-intl with 11 supported locales
- **Icons:** Lucide React
- **Forms:** React Hook Form with Zod validation
- **Package Manager:** pnpm

## Environment Variables
Required in `.env`:
```
DATABASE_URL=           # PostgreSQL connection string
AUTH_SECRET=            # NextAuth secret key
```

Optional for OAuth:
```
AUTH_GITHUB_ID=
AUTH_GITHUB_SECRET=
AUTH_GOOGLE_ID=
AUTH_GOOGLE_SECRET=
AUTH_AZURE_AD_CLIENT_ID=
AUTH_AZURE_AD_CLIENT_SECRET=
AUTH_AZURE_AD_ISSUER=
```

Optional features:
```
OPENAI_API_KEY=         # For AI-powered semantic search
```
