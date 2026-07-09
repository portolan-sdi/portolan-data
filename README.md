# portolan-data

Tracking the creation of **Portolan catalogs** — cloud-native geospatial data catalogs (STAC + GeoParquet / COG) that anyone can browse, query, and build on.

This repo isn't code — it's a **coordination board**. Each issue is a catalog to create: either an **official** dataset published as a Portolan catalog, or a **mirror** of an existing data source.

## Get involved

- 💡 **Ideas welcome from anyone.** Have a dataset that would make a great Portolan catalog or mirror? [Open an issue](https://github.com/portolan-sdi/portolan-data/issues/new) and propose it.
- 🙋 **Claim an issue.** Anyone is welcome to pick up an open issue, build the catalog, and put it up. Comment on the issue to claim it.
- ☁️ **Free hosting.** Catalogs can be hosted for free on [Source Coop](https://source.coop) — including under the shared Portolan mirrors organization (see [portolan-ops#1](https://github.com/portolan-sdi/portolan-ops/issues/1)).

## Two kinds of catalog

- **Official** — a first-class Portolan catalog for a dataset.
- **Mirror** — a Portolan catalog that mirrors an upstream source. Mirrors include a `via` link to the source (or `canonical` if the source has its own STAC catalog) and record when the mirror was last updated.

## How a catalog gets built

1. Acquire the source data
2. Convert to cloud-native formats (GeoParquet for vector, COG for raster)
3. Build a STAC catalog + `metadata.yaml` per the [Portolan spec](https://github.com/portolan-sdi/portolan-spec)
4. Publish to a cloud bucket
5. Register it on the [Portolan registry](https://github.com/portolan-sdi/portolan-registry)

The [Portolan CLI](https://github.com/portolan-sdi/portolan-cli) helps with most of these steps.

---

Part of [Portolan](https://github.com/portolan-sdi) — tools for cloud-native geospatial Spatial Data Infrastructure.
