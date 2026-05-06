# Environment Setup

<!-- Fill in what applies. Remove sections that don't. -->

## Prerequisites
- Node.js <!-- e.g. >= 20 -->
- Docker + Docker Compose <!-- remove if not used -->
- <!-- Any other tools: pnpm, bun, etc. -->

## Local Setup

```bash
cp .env.example .env.local   # copy env template
npm install                   # install dependencies
npm run dev                   # start dev server
```

## Environment Variables

<!-- Document every variable the project uses. -->
<!-- Format: VAR_NAME — what it does — required/optional — example value -->

| Variable | Description | Required | Example |
|----------|-------------|----------|---------|
| NEXT_PUBLIC_API_URL | URL base de la API | YES |  |

> Copy this table to `.env.example` with placeholder values (never real secrets).

## Environments

| Environment | How to run | Notes |
|-------------|------------|-------|
| Local | `npm run dev` | Uses `.env.local` |
| Docker | `docker-compose up` | Uses `docker-compose.yml` env |
| Production | <!-- deploy command --> | <!-- Notes --> |

## External Services
<!-- List services the app depends on: databases, APIs, auth providers, etc. -->
<!-- Remove this section if there are none. -->

<!-- Service name → purpose → how to get credentials for local dev -->
- GoGuest API -> fuente de los datos de capacidad de la actividad -> obtener API key en la URL
  
## Notes for Agent
- Never hardcode env values in source code
- Never commit `.env.local` or any file with real secrets
- If a new variable is needed, add it to `.env.example` with a placeholder
