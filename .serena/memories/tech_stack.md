# Tech stack

- YAML / JSON Schema / JSON-LD only; no package.json. Tooling = `@geolonia/datamodels` (datamodels-toolkit) run via npx and as a GitHub Action.
- Toolkit version is pinned in several places that must move together: both `uses: geolonia/datamodels-toolkit@<sha> # vX.Y.Z` lines in publish.yml and the `npx @geolonia/datamodels@X.Y.Z` lines in README.md and AGENTS.md. Upgrade with `npx @geolonia/datamodels@latest upgrade [--to vX.Y.Z]` (rewrites all of them); Dependabot only bumps the workflow lines, so its PRs leave README/AGENTS out of sync.

Serena: no symbol-level code; `.serena/project.yml` uses the `yaml` language server.
