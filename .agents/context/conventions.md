# Code Conventions

## General
- **Language**: TypeScript (strict mode)
- **File naming**: kebab-case for files, PascalCase for components
- **Imports**: Grouped (external → internal → relative), sorted alphabetically

## Components
- Functional components with explicit return types
- Props typed with `interface`, not `type`
- Co-locate styles with components when possible

## App Router
- Use server components by default
- Mark client components with `'use client'` only when needed
- API routes under `app/api/`

## Styling
- Tailwind CSS utilities first
- CSS modules for complex component-specific styles
- Avoid inline styles

## Testing
- Write tests alongside source files
- Name test files with `.test.ts` or `.test.tsx` suffix

## Commit Messages
- Conventional commits: `type(scope): description`
- Types: `feat`, `fix`, `refactor`, `docs`, `chore`, `test`
