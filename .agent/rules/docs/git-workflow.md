# Git Workflow

## Conventional Commits
Use the following format for commit messages:
```
<type>(<scope>): <short description>

<detailed description (optional)>
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Formatting changes (indentation, etc.)
- `refactor`: Code change that neither fixes a bug nor adds a feature
- `perf`: Performance improvement
- `test`: Adding or correcting tests
- `chore`: Build/tooling changes
- `ci`: CI configuration changes
- `build`: Build system changes

### Examples
`feat(auth): add user login functionality`
`fix(api): handle null pointer in user endpoint`

## Rules
- Do NOT commit secrets (API keys, passwords).
- Do NOT force push.
- Respect `.gitignore`.
- Run `pnpm lint` before committing.
