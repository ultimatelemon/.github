# Contributing to UltimateLemon

Thanks for helping out! This guide applies to every UltimateLemon repository that doesn't have its own `CONTRIBUTING.md`. A repository's own `README.md` and `CLAUDE.md` always win over this file.

## Before you start

- Work happens in **Linear**. Pick up an issue there, or create one first for anything bigger than a small fix.
- Cross-repository conventions are recorded as architecture decisions in [`ultimatelemon/decisions`](https://github.com/ultimatelemon/decisions). Check them before you pick a tool, library or setup. Want to do it differently? Propose a new decision instead of quietly deviating.

## Working on a change

1. Branch off `main`. Direct pushes to `main` are for organisation admins only.
2. Keep the change focused: one pull request does one thing.
3. Run the checks locally before you push. CI runs the same scripts: `format:check`, `lint`, `typecheck`, `test`, `build` and `verify`, whichever the repository has.
4. Open a pull request, fill in the template and ask for a review.
5. Merge once the `quality` check is green and the review is approved. `main` deploys automatically.

## The short version of our conventions

| Topic | Convention |
| --- | --- |
| Package manager | npm, with npm workspaces for monorepos |
| Node | Node 26: `node:26-alpine` images and `"engines": { "node": ">=26" }` |
| Formatting and linting | [`@ultimatelemon-eu/prettier-config`](https://github.com/ultimatelemon/packages/tree/main/packages/prettier-config) and [`@ultimatelemon-eu/eslint-config`](https://github.com/ultimatelemon/packages/tree/main/packages/eslint-config), referenced, never copied |
| Tests | Vitest, behind a `test` script |
| Database | PostgreSQL with its own role per app; Drizzle with migrations in `drizzle/`, applied at container start |
| Go services | Fiber, sqlc on pgx/v5, `log/slog`, binaries in `cmd/`, code in `internal/` |
| Configuration and secrets | Everything in Infisical, never in the repository or in `.env` files that get committed |
| Files | Cloudflare R2, EU jurisdiction |
| CI and deploys | GitHub Actions through [`shared-actions`](https://github.com/ultimatelemon/shared-actions), images on GHCR, rolled out by Dokploy |

Need something that more repositories could use? Put it in [`packages`](https://github.com/ultimatelemon/packages) as a new `@ultimatelemon-eu` package instead of copying code between repositories.

## Workflows

New repositories can start from our workflow templates: **Actions** → **New workflow** → *By UltimateLemon*. They follow the naming in `shared-actions`:

- `code-quality.yml` (`Code Quality`) runs the checks on every pull request.
- `deployment.yml` (`Deployment`) runs the checks, publishes the image and deploys on every push to `main`.

In a monorepo, prefix both with the app: `web-code-quality.yml` / `Web Code Quality`.

## Writing style

- Dates as `11-10-2026`, times in 24-hour notation.
- No em dashes.
