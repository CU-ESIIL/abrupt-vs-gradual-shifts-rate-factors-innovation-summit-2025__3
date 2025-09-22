# Data Access

This page tracks datasets powering the **Abrupt vs Gradual Shifts: Rate Factors** sprint. Store large files in CyVerse and link them here so collaborators know where to find source material and derived products.

## Shared storage
- **CyVerse community folder:** [`Innovation_summit/Group_3`](https://de.cyverse.org/data/ds/iplant/home/shared/esiil/Innovation_summit/Group_3/) — upload shared data products in subfolders such as `shared_data/`, `outputs/`, and `deliverables/`.
- **Personal workspaces:** Team members can mirror key outputs under `i:/iplant/home/<username>/projects/innovation_summit_2025/` for experimentation.

## Core datasets
- **USGS LandTrendr spectral change products** — annual disturbance trajectories and derivative metrics for vegetation transitions. Download through Google Earth Engine or USGS bulk services; document processing notebooks in [`code/`](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/code).
- **SNODAS Snow Water Equivalent (SWE)** — daily gridded snowpack data aggregated to weekly change rates. Store curated subsets in `shared_data/snowpack/` within CyVerse.
- **PRISM climate anomalies** — precipitation and temperature rate-of-change summaries used to contextualize abrupt vs gradual events. Archive processed rasters in `shared_data/climate/`.

## Derived products
- **Rate trigger catalog:** Table summarizing derivative thresholds for each pilot watershed. Save as CSV/Parquet under `outputs/rate_triggers/`.
- **Dashboard assets:** Exported figures, GIFs, and embed-ready JSON for the planned alert dashboard. Publish to `deliverables/dashboard/` and reference them from [`docs/index.md`](index.md).

## Documentation
For each dataset or derived product, include a short README with:
1. Source URL or DOI.
2. Processing steps or scripts used.
3. Contact person for questions.

Feel free to add more sections (e.g., QA/QC notes, data issues) as the sprint progresses.
