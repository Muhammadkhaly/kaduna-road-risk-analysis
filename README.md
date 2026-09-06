# Kaduna Road Network Risk Analysis

A spatial analysis project examining where road network density and major traffic
generators (markets, motor parks) concentrate within Kaduna metropolis, Nigeria, as a
proxy for identifying likely traffic-risk areas.

See [`PROJECT_BRIEF.md`](./PROJECT_BRIEF.md) for the full spatial question, study
area definition, and dataset list with source links.

## Repository structure
```
.
├── README.md              # this file
├── PROJECT_BRIEF.md        # spatial question, study area, datasets + sources
├── data/                   # raw and clipped datasets (or a data/README.md with download instructions, if files are too large to commit)
├── notebooks/ or scripts/  # analysis code
└── outputs/                # maps, figures, results
```

## How to reproduce
1. Download the Nigeria OSM extract from Geofabrik and the GADM Nigeria Level 2
   boundaries (links in `PROJECT_BRIEF.md`).
2. Clip roads and points of interest to the Kaduna North/South LGA boundary.
3. Run the density analysis (see `notebooks/` or `scripts/`) to produce the road
   density surface and overlay traffic generators.
4. Outputs (maps/figures) are saved to `outputs/`.

## Status
[Add a short note here on what's done vs. in progress, e.g. "Data collected and
clipped; density analysis in progress."]
