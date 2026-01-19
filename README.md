# Antigravity Agent Configuration

This repository hosts the configuration, rules, and skills for the Antigravity Agent, customized for a **Next.js 16.1 (App Router)** development environment using **PostgreSQL** and **Prisma**.

## 🧠 Agent Brain (`.agent`)

The core of the agent's behavior is defined in the `.agent` directory.

### 📜 Rules & Instructions
Located in `.agent/rules/`, these define how the agent interacts with the codebase.

- **`AGENTS.md`**: The primary entry point containing critical rules and essential commands.
  - **Tech Stack**: Next.js 16.1, React 19, TailwindCSS, Prisma, PostgreSQL.
  - **Environment**: PowerShell (Windows) is the required shell for all commands.
  - **Philosophy**: Follows a "Progressive Disclosure" approach, referring to specific docs only when needed.

#### Documentation Modules
Detailed guidelines are modularized in `.agent/rules/docs/`:
- **Tech Stack**: Frameworks and library versions.
- **Project Structure**: File layout conventions.
- **Frontend Guidelines**: Component and styling standards.
- **Git Workflow**: Commit message conventions.
- **SEO Strategy**: Metadata and keyword optimization.
- **Troubleshooting**: Common error resolutions.

### 🛠️ Skills
Specialized capabilities are stored in `.agent/skills/`:

- **`creating-skills`**: A skill to generate high-quality, predictable, and efficient skills for the agent environment.
- **`redesigning-ui`**: A specialized workflow for performing rigorous design refactors ensuring modern, premium aesthetics.

## 🚀 Usage

To use this configuration with your Antigravity Agent:

1. Ensure this repository is cloned or accessible as your `.agent` source.
2. The agent will automatically load `AGENTS.md` and apply the defined rules.
3. Use the defined skills by asking the agent (e.g., "Create a new skill for..." or "Redesign the UI for...").

## ⚡ Essential Commands Defined

The agent is aware of these project-specific commands:

- **Install**: `pnpm install`
- **Dev**: `pnpm dev`
- **Build**: `pnpm build`
- **Database**: `pnpm db:generate`, `pnpm db:migrate`
