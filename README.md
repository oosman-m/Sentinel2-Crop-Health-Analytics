# Multi-Temporal Sentinel-2 Crop Health Assessment & Spatial Stress Detection

**Author:** Muhammad Usman  
**Tools & Tech:** QGIS 3.x, R Programming (`ggplot2`, `dplyr`)  
**Dataset:** Sentinel-2 Satellite Multispectral Imagery (ESA Copernicus - Level 2A)  
**Spatial Resolution:** 10 Meters / Pixel (Bands 4 & 8)  

---

## 📌 Executive Summary
This case study establishes a satellite remote sensing and statistical analytics framework to monitor spatial crop health variations. Using Sentinel-2 imagery, map algebra was executed in QGIS to calculate the Normalized Difference Vegetation Index (NDVI), followed by statistical modeling in R to evaluate seasonal canopy shifts and confirm significant vigor changes.

$$\text{NDVI} = \frac{\text{Band 8 (NIR)} - \text{Band 4 (Red)}}{\text{Band 8 (NIR)} + \text{Band 4 (Red)}}$$

---

## 📊 Key Findings & Analytics Output

1. **Spatial Stress Zoning (QGIS):** Identified clear stress pockets ($\text{NDVI} < 0.3$) along field boundaries versus dense green foliage ($\text{NDVI} > 0.6$) in central irrigated plots.
2. **Statistical Hypothesis Testing (R):** A paired t-test confirmed a statistically significant seasonal increase in canopy vigor from March ($\text{Mean} \approx 0.37$) to July ($\text{Mean} \approx 0.76$) with $p < 0.001$.

---

## 📂 Repository Deliverables

- 📄 **[`/docs`](./docs/):** Contains the complete PDF Case Study Report (`Geospatial_NDVI_Crop_Health_Case_Study.pdf`).
- 💻 **[`/scripts`](./scripts/):** R script (`ndvi_statistical_analysis.R`) for reproducing boxplots, density distribution curves, and t-tests.
- 📊 **[`/data`](./data/):** Sampled spatial pixel points extracted from raster layers (`ndvi_march_samples.csv` & `ndvi_july_samples.csv`).
- 🖼️ **[`/maps_and_plots`](./maps_and_plots/):** High-resolution exported QGIS spatial maps and R visualization plots.

---

## 💡 Practical Value & Agricultural Impact
- **Variable-Rate Fertilization:** Enables targeted application of fertilizers to underperforming stress zones, reducing input costs by 15–20%.
- **Targeted Irrigation:** Identifies localized moisture deficits before visual crop damage occurs.
- **Yield Forecasting:** Serves as an early warning metric 4–6 weeks prior to harvest.
