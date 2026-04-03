# Mona Mayhem - Project Guidelines

## Project Overview

**Mona Mayhem** is a retro arcade-themed GitHub contribution battle arena built with Astro. The app compares GitHub contribution graphs of two users in a playful, gamified interface inspired by classic arcade battles.

- **Phase**: Scaffold phase (pages, API routes, and styling will be built iteratively)
- **Tech Stack**: Astro v5, Node.js adapter (server-rendered), GitHub API for contribution data
- **Key Files**: `src/pages/index.astro` (main page), `src/pages/api/contributions/[username].ts` (API endpoint)
- **Styling**: Press Start 2P font for retro gaming aesthetic, custom CSS in `src/styles/`

## Build and Dev Commands

```bash
# Development server (live reload)
npm run dev

# Production build
npm run build

# Preview built site locally
npm run preview
```

All commands run the Astro CLI. Development server starts on `http://localhost:3000` by default.

## Astro Best Practices

### File Structure
- **Pages** (`src/pages/`) → Auto-routed to `/` paths; only `.astro`, `.md`, `.mdx`, `.ts` (API)
- **Components** (`src/components/`) → Reusable Astro components (`.astro` files only)
- **API Routes** (`src/pages/api/`) → Server endpoints; return JSON or HTML responses
- **Assets** (`src/assets/` or `public/`) → Images, fonts, static files

### Component Guidelines
- Use `.astro` files for components; they render on the server by default (no JS shipped)
- Props are TypeScript-typed; access via `Astro.props`
- For client-side interactivity, use `client:load`, `client:idle`, or `client:visible` directives sparingly
- Prefer server-side rendering to minimize JavaScript in the browser

### API Routes
- Create endpoints in `src/pages/api/[...].ts` as TypeScript files
- Export default function: `export default function(context: APIContext) { ... }`
- Return `Response` objects or use Astro helpers like `Response.json()`
- Use dynamic routes like `[username].ts` for parameterized endpoints

### Styling
- Co-locate styles with components (inline `<style>` tags or `.css` imports)
- Use CSS cascade and component scoping to avoid conflicts
- Leverage the retro theme: Press Start 2P font, pixel-art aesthetics, arcade colors

### External Data (GitHub API)
- Fetch GitHub contribution data in API routes or at build time
- Cache responses to avoid rate limits (GitHub API: 60 req/hour unauthenticated, 5000 req/hour with token)
- Use `GITHUB_TOKEN` env var for higher rate limits if needed

## Development Workflow

1. **Start dev server**: `npm run dev` before coding
2. **Use Copilot** to scaffold pages, API routes, and components
3. **Test incrementally**: Each feature should be testable in the browser
4. **Build locally**: Run `npm run build` to catch errors before pushing
5. **Refer to workshop**: See `workshop/` folder for step-by-step guidance (for learning context only)

## Notes

- The app is **server-rendered** (Node adapter in standalone mode); all pages load on demand
- *Workshop files are separate* — focus on building the app in `src/` and `public/`; ignore `workshop/` and `docs/` during development
- Keep dependencies minimal; the project only uses Astro and its Node adapter
