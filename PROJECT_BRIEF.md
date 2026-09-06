# Project Brief: Road Network Risk Concentration in Kaduna Metropolis

## Spatial Question
Within Kaduna metropolis, which areas show the highest concentration of major roads
and intersections — a structural proxy for traffic-accident risk — and how does this
relate to the location of markets and motor parks (major traffic generators)?

## Study Area
Kaduna metropolis, comprising Kaduna North and Kaduna South Local Government Areas
(LGAs), Kaduna State, Nigeria.

## Datasets

| # | Dataset | Description | Source |
|---|---------|-------------|--------|
| 1 | Road network (highways, intersections) | Line features tagged `highway=*` for Nigeria, filtered to Kaduna metropolis | [OpenStreetMap via Geofabrik Nigeria extract](https://download.geofabrik.de/africa/nigeria.html) |
| 2 | Traffic generators (markets, motor parks / bus stations) | Point features tagged `amenity=marketplace`, `amenity=bus_station` etc. | [OpenStreetMap via Overpass Turbo](https://overpass-turbo.eu/) (or extracted from the same Geofabrik file) |
| 3 | Administrative boundaries | LGA boundary polygons for Kaduna North & Kaduna South, used to clip the study area | [GADM Nigeria administrative boundaries (Level 2)](https://gadm.org/download_country.html) |

## Method (brief)
1. Clip the Nigeria OSM road network to the Kaduna North/South LGA boundary (GADM).
2. Compute road/intersection density (e.g. line density or kernel density of
   intersection points) across a grid over the study area.
3. Overlay market and motor park point locations on the density surface to see
   whether high-density road areas coincide with major traffic generators.
4. Identify and map the top concentration zones as candidate risk areas.

## Notes on scope
Point-level FRSC crash records are not published as an open dataset (available only
by direct request to FRSC), so this project uses road-network structure and traffic
generator proximity as an observable proxy for accident risk, rather than mapping
reported crash locations directly.
