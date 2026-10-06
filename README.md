# Arcadia

An Astro website for **Fin de siècle**.

## Development

Use Node.js 24 and install dependencies with `npm ci`.

| Command                           | Purpose                                             |
| --------------------------------- | --------------------------------------------------- |
| `npm run dev -- --background`     | Start the development server in the background      |
| `npm run format`                  | Format source and configuration files with Prettier |
| `npm run format:check`            | Check formatting without changing files             |
| `npm run check`                   | Check Astro and TypeScript diagnostics              |
| `npm run build`                   | Build the static website into `dist/`               |
| `npm run preview -- --background` | Preview the production build in the background      |

## Automation

GitHub Actions runs formatting, type checks, and the build for pushes to
`master` and pull requests targeting `master`. The workflow can also be run
manually. It checks the project; deployment is not configured.

Dependabot checks npm dependencies and GitHub Actions every Monday. npm minor
and patch updates are grouped; major npm updates are proposed separately.
Updates are reviewed and merged manually.
