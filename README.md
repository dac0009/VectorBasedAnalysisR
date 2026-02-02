# VectorBasedAnalysisR

Spatial analysis of U.S. vector data using **R**, [`sf`](https://r-spatial.github.io/sf/), and [`tmap`](https://r-tmap.github.io/tmap/). This project demonstrates how to perform core GIS workflows in R including spatial joins, buffers, intersections, dissolves, and map visualizations. Designed for teaching and exploring key GIS workflows using modern `tmap v4` syntax.

---

## Overview

This project covers:

- Loading and inspecting shapefiles and GeoPackage layers
- Performing spatial joins and point-in-polygon analysis
- Creating buffers and clip/intersection operations
- Generating Voronoi diagrams and convex hulls
- Dissolving geometries by attributes
- Calculating line length within polygons and density
- Mapping spatial layers with clean, modern cartography using `tmap`

---

### Packages

Install the following R packages:

```r
install.packages(c(
  "sf", 
  "tmap", 
  "tidyverse", 
  "ggthemes", 
  "tmaptools"
))
```
### Structure
VectorBasedAnalysisR/
├── data/
│   └── vector_analysis/  # Contains shapefiles and GPKG data
├── output/
│   └── *.shp / *.gpkg / *.png  # Exported results (buffers, maps, etc.)
├── scripts/
│   └── analysis.R  # Main spatial workflow
├── README.md

- Interstate buffers overlaid on states
- Cities per state (point-in-polygon)
- Line density by state (interstates/km²)
- Dissolved subregions
- Geometric operations (union, erase, symmetric difference)

### Learning Goals

- Understand spatial relationships using sf geometry types
- Practice spatial operations like st_intersection(), st_union(), and st_difference()
- Visualize and explore spatial data using tmap v4
- Gain hands-on experience with real-world U.S. vector data
