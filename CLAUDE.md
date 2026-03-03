# CLAUDE.md

## Project

beardless.io — business card site for Beardless HQ, a technology advisory firm in Stockholm. Deployed to GitHub Pages at beardless.io.

## Stack

- Hugo static site generator (hugo.toml for config)
- Zero JavaScript. All CSS is inlined in the layout templates.
- Fonts: Syne 700 (brand/headings), DM Mono 400 (details) via Google Fonts
- GitHub Actions builds and deploys on push to main

## Design principles

- Nordic minimalist. Edgy, not posh.
- All text lowercase. Brand is "beardless hq".
- Dark background (#0a0a08), warm off-white text (#e8e4df), muted (#5a5550).
- No decorative elements. Typography and whitespace do the work.
- No JS unless absolutely necessary. HTMX is acceptable if interactivity is needed later.

## Key files

- `layouts/index.html` — the entire homepage (HTML + inline CSS)
- `layouts/404.html` — 404 page, same visual language
- `hugo.toml` — site config, params (description, email)
- `static/CNAME` — custom domain mapping
- `.github/workflows/static.yml` — build and deploy pipeline

## Commands

- `hugo server` — local dev server with live reload
- `hugo --minify` — production build to public/

## Rules

- Keep it minimal. Don't add complexity unless explicitly asked.
- public/ is build output, gitignored. Never commit into it.
- Always test with `hugo --minify` before pushing.
- When changing templates, verify both desktop and mobile viewports.
