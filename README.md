# Working inventory of warehouse footprints in Île-de-France, France

This repository contains the first public working release of a curated spatial inventory of warehouse footprints in Île-de-France, France.

Version `v0.1.0` is a working release. It is public, citable, and suitable for exploratory mapping and preliminary analysis, but it should not be treated as a final or exhaustive reference inventory. The dataset derives from a broader internal workflow that includes candidate generation, contextual filtering, feature cleaning, and review. The public release is deliberately lean: it contains the retained features and a reduced attribute schema prepared for external dissemination.

This dataset was produced within the framework of the [Logistics City Chair](https://www.lvmt.fr/chaires/logistics-city/) at Université Gustave Eiffel.

## Release status

- **Release type:** public working release
- **Version:** `v0.1.0`
- **Release date:** `2026-03-23`
- **DOI:** `10.5281/zenodo.19131942`
- **Publisher:** Zenodo

If the Zenodo record has not yet been published, treat the DOI above as reserved. Once the record is published, the same DOI becomes the active archival identifier for this version.

## What is included

This release contains three outward-facing products and one metadata companion:

- `archive/wh_public_v0_1_0.gpkg` — archival GeoPackage
- `web/wh_public_v0_1_0_web.geojson` — lightweight web map product
- `metadata/wh_public_v0_1_0_layer_metadata.xml` — ArcGIS metadata export
- `docs/methodological_note.md` — release note and methodological context

## Spatial scope

The release covers Île-de-France, France.

## Attribute schema

The public schema is intentionally concise. The release includes only the fields needed for identification, version tracking, and basic interpretation.

| Field | Description |
|---|---|
| `wh_id` | Stable public identifier for the released feature |
| `release_version` | Public release version |
| `release_stage` | Release stage, here `working` |
| `method_version` | Label for the internal methodological state used to produce this release |
| `area_m2` | Area of the released footprint in square metres |
| `status_pub` | Public release status label |
| `review_flag` | Optional indicator for features that may require future review |

## How to cite

Please cite the exact version used.

**Citation for this release**

Mohammed Younes. (2026). *Working inventory of warehouse footprints in Île-de-France, France* (v0.1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.19131942

A machine-readable citation file is provided in `CITATION.cff`.

## What this dataset is and is not

This release is a curated working inventory intended to support transparency, exploratory use, and further methodological development. It is not a legal, cadastral, administrative, or operational register of warehouses. Inclusion in the dataset should not be read as definitive confirmation of functional status in every case.

The inventory may contain omissions, boundary imperfections, or classification uncertainty. Future versions may refine geometries, revise inclusion decisions, or expand coverage.

## Versioning policy

This repository follows an explicit versioning logic.

- Patch releases (`0.1.1`, `0.1.2`, etc.) are for small corrections that do not materially alter the substance of the release.
- Minor releases (`0.2.0`, `0.3.0`, etc.) indicate meaningful changes in method, schema, or released content.
- A future `1.0.0` will be reserved for the first stable official release, if and when such a release is declared.

Please cite the exact version used in your work.

## Sources and attribution

This release is derived from a broader workflow that integrates multiple upstream geospatial sources. Source attribution and notices are provided in `NOTICE.md`.

Please preserve source acknowledgements in any redistribution, derivative work, or publication based on this release.

## Licensing

The repository uses a split licensing model.

- **Data files** in `data/release/v0.1.0/archive/` and `data/release/v0.1.0/web/` are released under **ODbL-1.0**. See `LICENSE_DATA.md`.
- **Documentation and metadata files** are released under **CC BY 4.0**. See `LICENSE_DOCS.md`.

Please also preserve the upstream source acknowledgements provided in `NOTICE.md` and `docs/sources-and-attribution.md`.

## Contact

For questions, corrections, or citation issues, please contact:

**Mohammed Younes**  
Email: [mohammed.younes@enpc.fr](mailto:mohammed.younes@enpc.fr)


