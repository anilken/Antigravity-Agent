# Project Structure

## Directory Layout
```
/
├── prisma/                 # Database schema and migrations
│   ├── schema.prisma       # Prisma schema definition
│   ├── migrations/         # Database migrations
│   └── seed.ts             # Database seeding script
├── public/                 # Static assets (logos, favicon)
├── src/
│   ├── app/                # Next.js App Router pages
│   │   ├── (auth)/         # Auth pages (login, register)
│   │   ├── admin/          # Admin dashboard
│   │   ├── api/            # API routes
│   ├── components/         # React components
│   │   ├── admin/          # Admin-specific components
│   │   ├── auth/           # Authentication components
│   │   ├── categories/     # Category components
│   │   ├── layout/         # Layout components
│   │   ├── providers/      # React context providers
│   │   ├── settings/       # Settings components
│   │   └── ui/             # Base UI components
│   ├── lib/                # Utility libraries
│   │   ├── ai/             # AI integration
│   │   ├── auth/           # NextAuth configuration
│   │   ├── config/         # Config type definitions
│   │   ├── plugins/        # Plugin system (auth, storage)
│   │   ├── db.ts           # Prisma client instance
│   │   └── utils.ts        # Utility functions (cn)
├── next.config.ts          # Main application configuration
└── package.json            # Dependencies and scripts
```

## Key Files
| File | Purpose |
|------|---------|
| `next.config.ts` | Main app configuration |
| `prisma/schema.prisma` | Database schema |
| `src/lib/auth/index.ts` | NextAuth configuration |
| `src/lib/db.ts` | Prisma client singleton |
| `src/app/layout.tsx` | Root layout with providers |
| `src/components/ui/` | Base UI components |

## Plugin System
Authentication and storage use a plugin architecture:
- **Auth:** `src/lib/plugins/auth/` (credentials, github, google, azure)
- **Storage:** `src/lib/plugins/storage/` (url, s3)
