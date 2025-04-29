# Capstone Project: The Urban Heat Island (UHI) Effect in Madrid

## Project Overview
This repository contains the final code for my undergraduate capstone project. The project investigates the **Urban Heat Island (UHI) effect** in Madrid, analyzing how **vegetation coverage** and **socioeconomic vulnerability** influence nighttime land surface temperatures across different neighborhoods.

The project uses satellite data, socioeconomic data, and statistical modeling to answer:
- How is heat exposure distributed across Madrid?
- Does vegetation help mitigate the UHI effect?
- Are vulnerable neighborhoods disproportionately exposed to higher temperatures?

## Methodology
**Data Sources:**
- Landsat 8 & 9: Daytime Land Surface Temperature (LST) and NDVI
- MODIS: Nighttime Land Surface Temperature
- Sentinel-2: Vegetation indices (NDVI)
- Dynamic World: Land cover classification
- OpenStreetMap (OSM): Urban structures
- Municipal data (Iguala Madrid and Portal Estadístico): Socioeconomic indicators

**Tools and Libraries:**
- Google Earth Engine (GEE) – Satellite data processing
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy) – Data analysis and visualization
- QGIS – Mapping and geospatial analysis
- Google Colab – Notebook execution environment

**Statistical Analyses:**
- Descriptive statistics (mean, minimum, maximum, distribution)
- Pearson correlation analysis
- Ordinary Least Squares (OLS) regression
- Interaction models (analyzing if vegetation's cooling effect varies across neighborhoods)

## Main Analytical Steps
- **Data preprocessing:** Cloud masking, unit conversions (Kelvin → Celsius), land classification.
- **Vegetation Analysis:** 
  - Calculate and visualize NDVI (Normalized Difference Vegetation Index).
  - Compare NDVI across region, city, and selected neighborhoods.
- **Temperature Analysis:** 
  - Compare daytime (Landsat) and nighttime (MODIS) LST across urban and rural areas.
- **Urban Heat Island (UHI) Analysis:** 
  - Calculate UHI intensity (urban temperature - rural temperature).
  - Map spatial patterns of UHI.
- **Socioeconomic Analysis:** 
  - Assess correlation between UHI intensity, vegetation levels, and socioeconomic indicators (income, unemployment, vulnerability index).

## Key Findings
- Vegetated areas consistently show lower nighttime temperatures.
- The UHI effect is stronger in southeastern neighborhoods of Madrid (e.g., Usera, Puente de Vallecas).
- Socioeconomic vulnerability correlates with greater heat exposure, even when controlling for vegetation.

## Repository 
- `FINAL_CODE_CAPSTONE.ipynb`: Complete code for data preprocessing, analysis, and visualization.

---

> **Note:** The project focuses on summer months (June–August) between 2018–2024, when UHI effects are most pronounced.
