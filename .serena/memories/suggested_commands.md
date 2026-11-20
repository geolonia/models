# Commands

Use the toolkit version pinned in publish.yml (see `mem:tech_stack`):
- `npx @geolonia/datamodels@<ver> check` — validate the node. CI on PRs also passes `--base origin/main`, which compares with the base branch and rejects changed or removed published releases; add it locally to match.
- `npx @geolonia/datamodels@<ver> build` — build into `_site/` (gitignored).
- `npx @geolonia/datamodels@<ver> add|extend …` — add a model instead of creating folders by hand.
