# Code Review Checklist

## Functional
- [ ] Code does what it's supposed to do
- [ ] Edge cases are handled
- [ ] Error handling is appropriate
- [ ] No unnecessary code or dead branches

## Quality
- [ ] Code follows project conventions (see `.agents/context/conventions.md`)
- [ ] Variable/function names are clear and consistent
- [ ] Functions are small and focused (single responsibility)
- [ ] No code duplication

## Performance
- [ ] No obvious performance issues
- [ ] Efficient data structures used
- [ ] No unnecessary re-renders (React)
- [ ] Database queries are optimized (if applicable)

## Security
- [ ] No secrets or credentials exposed
- [ ] Input validation is in place
- [ ] Proper authentication/authorization checks
- [ ] No SQL injection / XSS vulnerabilities

## Testing
- [ ] Tests cover the new functionality
- [ ] Tests are meaningful (not just checking truthy)
- [ ] All existing tests still pass

## Documentation
- [ ] Complex logic is commented
- [ ] README updated if needed
- [ ] TypeScript types are accurate

## Next.js Specific
- [ ] Server vs client component usage is correct
- [ ] Data fetching follows best practices
- [ ] Metadata is set for pages
- [ ] Follows Next.js 16 docs (`node_modules/next/dist/docs/`)

## Review Notes
<!-- Additional comments -->
