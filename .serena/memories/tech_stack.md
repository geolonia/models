# Tech stack

- YAML / JSON Schema / JSON-LD only; no package.json. Tooling = `@geolonia/datamodels` (datamodels-toolkit) run via npx and as a GitHub Action.
- Toolkit version is pinned in several places that must move together: both `uses: geolonia/datamodels-toolkit@<sha> # vX.Y.Z` lines in publish.yml and the `npx` lines in README. Upgrades are `chore: datamodels-toolkit X.Y.Z` PRs (`datamodels upgrade` / Dependabot).

Serena: no symbol-level code; `.serena/project.yml` uses the `yaml` language server.
