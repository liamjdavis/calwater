# Cal Water Los Altos Suburban: Well Inventory

Inventory of municipal well permits inside the California Water Service (Cal Water)
Los Altos Suburban district, built from public data. Prepared to evaluate the
alternative sites analysis in the EIR for Cal Water's proposed well at Carlisle Way,
Sunnyvale (agenda item 26-0484).

**Interactive map:** https://liamjdavis.github.io/calwater/

## Findings

96 municipal well permits fall within the district boundary:

| Status | Count |
|---|---|
| Water Supply – Active | 22 |
| Destroyed | 40 |
| Abandoned | 12 |
| Other (env. extraction, other-active, other-producing) | 22 |

## Contents

- `wells_water_system_join.ipynb`: full pipeline: downloads SWRCB water-system
  boundaries, spatially joins Valley Water well permits, renders the map
- `WELLS.csv`: Valley Water well permits, filtered to purpose *Municipal*
- `WELLS_with_water_system.csv`: permits joined to their water system
- `index.html` / `los_altos_wells_map.html`: interactive Folium map, wells colored by status

## Data sources

- [Valley Water well permits](https://data-valleywater.opendata.arcgis.com/datasets/43743ae1dbfa4172a3c4a0d6481093b7_0/explore)
- [SWRCB Drinking Water System Area Boundaries](https://gispublic.waterboards.ca.gov/portalserver/rest/services/Drinking_Water/California_Drinking_Water_System_Area_Boundaries/FeatureServer/0)
