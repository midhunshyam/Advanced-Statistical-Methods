# Advanced Statistical Methods: NSW Fire Data (2024)   

This repository contains an applied statistical analysis of New South Wales (NSW) fire data (2024), examining spatial patterns, environmental drivers, and operational implications for fire‐rescue services. 

Analyses include:

1. **Preliminary Exploration & Chi‑square Test**  
2. **Task 1: Spatial Density (Mixture Models & Kernel Density)**  
3. **Task 2: Humidity’s Effect on Fire Duration (Mixture of Regression Models)**  
4. **Task 3: Equipment Allocation by Fire Duration (Conditional Probabilities)**  
5. **Task 4: Seasonal Effects (Mixture Models on Temperature)**


## Repository Structure

- `Statistical-Report-MATH7002-22058122.pdf`  
  Final rendered report (40 pages)

The `Statistical-Report-MATH7002-22058122.pdf` contains the detailed report with the mathematical equations for the statistical models. This is a polished 40‑page PDF report derived from the .Rmd including table of contents, inline code output, figures (boxplots, density plots, maps), and narrative interpretation.

- `Statistical-Report-MATH7002-22058122.Rmd`  
  R Markdown source for the report

`Statistical-Report-MATH7002-22058122.Rmd` is the fully annotated R Markdown source. This Contains code chunks for data import, EDA, statistical testing, modeling, plotting, and mapping.Organised into numbered “Task” sections, each with clear hypotheses, methodology, results, and conclusions.

##  Requirements  

- **R** ≥ 4.3.1  
- The following R packages (install via `install.packages()`):  
  - `mixtools`, `mvtnorm`, `MASS`  
  - `hexbin`, `ggplot2`, `dplyr`  
  - `leaflet`, `leaflet.extras`, `htmltools`  

## Key Findings

- Fire-type distribution is significantly non‑uniform (χ² = 224.94, p < 2.2e‑16).
- Spatial density: A 3‑component Gaussian mixture captures clusters; estimated fire density at WSU Parramatta South is ~0.18.
- Humidity–duration relationship fits best with k = 3 regression mixtures, supporting hidden environmental factors.
- Equipment allocation for 35–45 min fires: roughly 50 % desert, 40 % forest, and minimal grassland retardants.
- Seasonal temperature patterns resolve into three clusters, insufficient to cleanly identify four seasons via mixture models.
