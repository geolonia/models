# Geolonia Models

Data models of Geolonia projects: JSON Schemas, JSON-LD @contexts and vocabularies at https://models.geolonia.com. This is a data model node, built with [datamodels-toolkit](https://github.com/geolonia/datamodels-toolkit) (what a node publishes: [docs/node.md](https://github.com/geolonia/datamodels/blob/main/docs/node.md)). Models that are useful beyond Geolonia can later be proposed to [datamodels.jp](https://datamodels.jp).

- `node.yaml`: the settings.
- `models/`: one folder per subject. A model is a folder in a subject with `schema.json`, `catalog.yaml` and `examples/example.json`, laid out as in [datamodels.jp](https://github.com/geolonia/datamodels/tree/main/models).
  - `smartmap/`: the models of Geolonia's Smart Map (geolonia/models#2).
  - `geocoding/`: the results of a geocoder, such as abr-geocoder (geolonia/models#21). The address itself is datamodels.jp's JapaneseAddress.
- `.github/workflows/publish.yml`: checks pull requests, and publishes main to GitHub Pages.
- `package.json`: pins the toolkit CLI for running the commands below locally. Dependabot bumps it, and the Action in `publish.yml`.
- `catalog-info.yaml`: the Backstage entry (owner: Data Team).

Licence: [CC0-1.0](LICENSE).

```bash
npm ci           # the toolkit CLI, pinned in package.json
npm run check
npm run build    # into _site/
```
