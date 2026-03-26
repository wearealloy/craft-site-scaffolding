# [project-name]

CraftCMS project with DDEV and Vite.

## Requirements

- [DDEV](https://ddev.readthedocs.io)
- Docker

## Setup

```bash
ddev start
ddev craft up
```

Development

```bash
ddev npm run dev
```

Vite runs on https://[project-name].ddev.site:5173.

Build

```bash
ddev npm run build
```

Useful commands

```bash
ddev craft db/backup          # Back up the database
ddev craft db/restore <file>  # Restore a backup
ddev craft clear-caches/all   # Clear all caches
ddev launch                   # Open site in browser
ddev launch /admin            # Open control panel
```
