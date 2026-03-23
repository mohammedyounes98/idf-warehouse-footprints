# Methodological note
## Working inventory of warehouse footprints in Île-de-France, France
### Public release v0.1.0

## 1. Purpose of this note

This note accompanies the first public working release of a spatial inventory of warehouse footprints in Île-de-France. Its purpose is to explain what this release represents, how it was prepared for public dissemination, and how it should be read and used.

The note does not attempt to document every internal processing detail. Rather, it provides the methodological context needed to interpret the present release responsibly.

## 2. Nature of the released dataset

The released dataset is a public working inventory derived from a larger internal master dataset. The internal master includes both retained and rejected candidates, source-derived fields, intermediate processing attributes, and review information. That internal structure is necessary for analysis, auditability, and future refinement, but it is not suitable for public dissemination in its raw form.

For this reason, the public release was produced as a separate derivative layer. Only the retained features were exported, and the attribute schema was reduced to a small set of public-facing fields.

## 3. Conceptual basis of the inventory

This inventory should not be understood as a simple shape-based extraction of large buildings. The released footprints result from a broader multi-criteria workflow combining spatial context, source integration, feature cleaning, and review.

In practical terms, the released layer represents the current public state of an ongoing inventory-building process. The presence of a feature in this version indicates that, at the time of release, it was retained in the curated working set prepared for public communication and exploratory use.

## 4. General workflow behind the release

The broader internal workflow proceeds in several stages.

First, candidate building features are assembled from source data relevant to large building footprints and industrial or logistics-related spatial contexts.

Second, candidate geometries are cleaned and normalised through standard geoprocessing operations intended to improve coherence and reduce artefacts inherited from source layers.

Third, the candidate pool is reduced through a contextual and analytical filtering process. The final public layer is not the raw candidate set but the retained subset resulting from that wider workflow.

Fourth, a release-specific public derivative is prepared. At this stage, only the retained features are exported, geometry quality is checked, duplicate artefacts are reviewed, and the public schema is reduced to a minimal set of stable and interpretable attributes.

## 5. Public release design

The public dataset has been designed with a clear separation between internal analytical provenance and external dissemination.

The internal master dataset preserves detailed processing information, including non-retained candidates and source-derived fields. The public layer, by contrast, is intended to be stable, legible, and citable. It therefore includes only a small number of fields that support identification, versioning, and basic interpretation.

This separation is deliberate. It allows the released dataset to remain understandable to external users while preserving the richer internal structure needed for future revisions.

## 6. Public fields

The current public release includes the following fields:

- `wh_id`: stable public identifier
- `release_version`: public version label
- `release_stage`: release stage
- `method_version`: internal methodological state label associated with this release
- `area_m2`: footprint area in square metres
- `status_pub`: public status label
- `review_flag`: optional review indicator


## 7. Limitations

This is a working release.

It should not be treated as a complete, final, or authoritative inventory of warehouses in Île-de-France. Several kinds of limitation should be kept in mind.

First, the inventory remains subject to omission and revision. Some relevant features may not yet be included, while some retained features may be refined or reinterpreted in later versions.

Second, geometric representation depends on the quality and structure of the underlying source data and on the processing choices used to derive the public layer.

Third, inclusion in the dataset should not be interpreted as legal, cadastral, or administrative proof of warehouse status.

## 8. Versioning and continuity

This public release is versioned as `v0.1.0`. The `0.x` series indicates that the dataset is public but still methodologically in development.

Stable public identifiers are used to support continuity across versions wherever the same real-world feature remains conceptually the same object. At the same time, later releases may introduce revised geometries, new features, removed features, or changes in release logic.

Users should therefore cite the exact version used rather than referring generically to “the dataset”.

## 9. Citation

Mohammed Younes. (2026). *Working inventory of warehouse footprints in Île-de-France, France* (v0.1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.19131942

## 10. Recommended use

This release is well suited to:

- exploratory mapping
- preliminary spatial analysis
- methodological discussion
- transparent citation of the current working state of the inventory

It is less suited to:

- regulatory or legal interpretation
- operational decision-making without independent validation
- claims of exhaustive warehouse coverage

## 11. Future development

Later versions may refine the released geometries, expand or contract the inventory, revise the public schema, or document the method in greater detail.

The present release should therefore be read as a formal public snapshot of an evolving data product rather than as its final state.

## 12. Acknowledgements

This work was produced within the framework of the [Logistics City Chair](https://www.lvmt.fr/chaires/logistics-city/) at Université Gustave Eiffel.
