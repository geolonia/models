# Geolonia Models

Data models of Geolonia projects: JSON Schemas, JSON-LD @contexts and vocabularies at https://models.geolonia.com. This is a data model node, built with [datamodels-toolkit](https://github.com/geolonia/datamodels-toolkit) (what a node publishes: [docs/node.md](https://github.com/geolonia/datamodels/blob/main/docs/node.md)). Models that are useful beyond Geolonia can later be proposed to [datamodels.jp](https://datamodels.jp).

- `node.yaml`: the settings.
- `models/smartmap/`: the models of Geolonia's Smart Map (geolonia/models#2). A model is a folder in it with `schema.json`, `catalog.yaml` and `examples/example.json`, laid out as in [datamodels.jp](https://github.com/geolonia/datamodels/tree/main/models).
- `.github/workflows/publish.yml`: checks pull requests, and publishes main to GitHub Pages.
- `catalog-info.yaml`: the Backstage entry (owner: Data Team).

```bash
npx github:geolonia/datamodels-toolkit#v0.2.1 check
npx github:geolonia/datamodels-toolkit#v0.2.1 build   # into _site/
```
