## Project

CraftCMS with DDEV, Vite (nystudio107/craft-vite), Tailwind CSS v4, and Twig
templates.

## Commands

This is a DDEV project — prefix all CLI commands with `ddev`:

```bash
ddev craft <command>       # Craft CLI
ddev composer <command>    # Composer
ddev npm <command>         # npm (or use ddev exec npm)
ddev exec <command>        # Run inside the web container
```

Frontend

- Entry point: `src/entrypoint.ts`
- Styles: `src/css/`
- Scripts: `src/ts/`
- Config: `vite.config.ts`
- Dev server: `ddev npm run dev` → available at https://[project].ddev.site:5173
- Build: `ddev npm run build` → outputs to public_html/dist/

Templates

Twig templates live in templates/. Structure:

- `_base/` — base layouts
- `_meta/` — <head> meta partials
- `_partials/` — reusable components
- `index.twig` — homepage

Craft config

- Vite plugin config: `config/vite.php`
- General config: `config/general.php`
- DB config: `config/db.php`

Environment

Secrets and environment-specific values live in .env. Never commit .env.
