# Website Architecture

## Stack
- React 19 + TypeScript + Vite
- Tailwind CSS
- React Router

## Implemented pages
`/`, `/demo`, `/download`, `/github`, `/docs`, `/security`, `/releases`, etc.

## Current caveats
- `src/config/project.ts` contains placeholder links and default API base URL (`https://api.voiceshield.example.com`).
- Some UI API response assumptions differ from current backend `/api/v1/analyze` schema.
