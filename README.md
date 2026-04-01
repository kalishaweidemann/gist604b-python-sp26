# Python for GIS: pandas, GeoPandas, and Rasterio

## Overview
This repository demonstrates a structured workflow for working with tabular, vector, and raster GIS data using Python. The project integrates pandas, GeoPandas, and Rasterio within a reproducible development environment using GitHub Codespaces.

The assignment emphasizes separating exploratory analysis (notebooks) from reusable implementations (Python scripts), along with validating functionality through automated testing.


## Skills demonstrated
- Working with tabular data using pandas
- Processing and analyzing spatial vector data with GeoPandas
- Performing raster-based workflows using Rasterio
- Implementing reusable Python functions from notebook workflows
- Validating code using pytest
- Managing a structured repository in a containerized environment (Codespaces)


## Workflow
The project follows a consistent workflow across all components:

1. Develop and test logic in Jupyter Notebooks  
2. Implement reusable functions in `src/`  
3. Validate functionality using `pytest` (pandas and GeoPandas)  
4. Complete raster analysis directly within the Rasterio notebook  

This approach reinforces the transition from exploratory analysis to reproducible, testable code.


## Repository structure
```text
.
├── notebooks/
│   ├── pandas/
│   │   ├── 01_function_load_and_explore_gis_data.ipynb
│   │   ├── 02_function_filter_environmental_data.ipynb
│   │   ├── 03_function_calculate_station_statistics.ipynb
│   │   └── 04_function_join_station_data.ipynb
│   ├── geopandas/
│   │   ├── 00_download_real_data.ipynb
│   │   ├── 01_function_load_spatial_data.ipynb
│   │   ├── 02_function_explore_properties.ipynb
│   │   ├── 03_function_transform_crs.ipynb
│   │   ├── 04_function_geometry_operations.ipynb
│   │   ├── 05_function_spatial_relationships.ipynb
│   │   ├── 06_function_spatial_joins.ipynb
│   │   └── 07_function_overlay_and_visualize.ipynb
│   └── rasterio/
│       └── remote_sensing_workflow.ipynb
├── src/
│   ├── download_real_data.py
│   ├── geopandas_basics.py
│   └── pandas_basics.py
├── tests/
│   ├── test_geopandas_basics.py
│   └── test_pandas_basics.py
├── data/
│   ├── cities/
│   │   └── ne_cities_us.geojson
│   ├── ecoregions/
│   │   └── epa_level3_western_us.geojson
│   ├── protected_areas/
│   │   └── national_parks_major.geojson
│   ├── neighborhood_samples.geojson
│   ├── temperature_readings.csv
│   └── weather_stations.csv
├── .devcontainer/
│   ├── devcontainer.json
│   └── Dockerfile
├── .gitignore
├── pyproject.toml
├── uv.lock
└── README.md
```


## Notes
- Jupyter Notebooks are used for exploration and method development
- Core functionality is implemented in the `src/` directory
- Automated tests ensure correctness for pandas and GeoPandas workflows
- Raster analysis is completed entirely within the Rasterio notebook