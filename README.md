# NSW Fire Data Analysis  
*Applied Project for MATH7002 – Advanced Statistical Methods*  
**Author:** Midhun Shyam (Student ID: 22058122)  
**Date:** 28 October 2024  

## 📖 Overview  
This repository contains an applied statistical analysis of New South Wales (NSW) fire data, examining spatial patterns, environmental drivers, and operational implications for fire‐rescue services. Analyses include:

1. **Preliminary Exploration & Chi‑square Test**  
2. **Task 1: Spatial Density (Mixture Models & Kernel Density)**  
3. **Task 2: Humidity’s Effect on Fire Duration (Mixture of Regression Models)**  
4. **Task 3: Equipment Allocation by Fire Duration (Conditional Probabilities)**  
5. **Task 4: Seasonal Effects (Mixture Models on Temperature)**


## 🔍 Repository Structure  

├── MATH7002_22058122.pdf ← Final rendered report (40 pages)
├── 22058122.Rmd ← R Markdown source


##  Requirements  

- **R** ≥ 4.3.1  
- The following R packages (install via `install.packages()`):  
  - `mixtools`, `mvtnorm`, `MASS`  
  - `hexbin`, `ggplot2`, `dplyr`  
  - `leaflet`, `leaflet.extras`, `htmltools`  
- **Pandoc** (for knitting to PDF)  
- A LaTeX distribution (e.g. TeX Live or TinyTeX) for PDF rendering  


## Getting Started  

1. **Clone this repo**  
   ```bash
   git clone https://github.com/midhunshyam/NSW-Fire-Analysis.git
   cd NSW-Fire-Analysis

## File Descriptions

**22058122.Rmd**
-The fully annotated R Markdown source. This Contains code chunks for data import, EDA, statistical testing, modeling, plotting, and mapping.
Organised into numbered “Task” sections, each with clear hypotheses, methodology, results, and conclusions.

**MATH7002_22058122.pdf**
-A polished 40‑page PDF report derived from the .Rmd. Includes table of contents, inline code output, figures (boxplots, density plots, maps), and narrative interpretation.

## Key Findings

-Fire-type distribution is significantly non‑uniform (χ² = 224.94, p < 2.2e‑16).
-Spatial density: A 3‑component Gaussian mixture captures clusters; estimated fire density at WSU Parramatta South is ~0.18.
-Humidity–duration relationship fits best with k = 3 regression mixtures, supporting hidden environmental factors.
-Equipment allocation for 35–45 min fires: roughly 56 % desert, 43 % forest, and minimal grassland retardants.
-Seasonal temperature patterns resolve into three clusters, insufficient to cleanly identify four seasons via mixture models.

---
##License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).
You are free to use, adapt, and share this work with proper attribution.
