# models (Geolonia data model node → https://models.geolonia.com)

Data-only repo: no code. A datamodels-toolkit "node"; README.md and node.yaml say what it is. Model layout and rules = same as the datamodels.jp catalog (geolonia/datamodels README, docs/node.md there).

- Subjects: `models/smartmap/` (HazardArea) and `models/geocoding/` (GeocodingResult).
- `node.yaml`: `baseUrl` and `iris` are baked into every published IRI — never change. `nodes:` lists datamodels.jp so contexts may import catalog contexts (geocoding imports datamodels.jp `common`).
- CI: `.github/workflows/publish.yml` (written by `datamodels init`) runs the toolkit Action: check on PRs, build + GitHub Pages deploy on main.

Further: `mem:tech_stack`, `mem:suggested_commands`, `mem:conventions`, `mem:task_completion`.
