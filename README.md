# Satellite Imagery and Machine Learning Workshop

[![Launch RStudio on Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mpardy/harvard_workshop/main?urlpath=rstudio)

Welcome to the **Satellite Imagery and Machine Learning Workshop**!

This repository contains the interactive materials, satellite dataset references, land-use boundaries, and code for running satellite imagery classification in R.

---

## 🚀 Launching Online with Binder

You can run all the code directly in your browser without installing R or GIS packages locally!

- **Click to launch RStudio on Binder**:  
  [![Launch RStudio on Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mpardy/harvard_workshop/main?urlpath=rstudio)

*Note: The first launch may take 2–5 minutes while Binder builds the container with spatial libraries (GDAL, GEOS, PROJ) and R packages.*

---

## 📁 Repository Overview

- `Satellite_imagery_ML.Rmd`: Main R Markdown document covering Landsat 8 data processing, spectral index calculation (NDVI), unsupervised classification (K-means), and supervised learning (Decision Trees via `rpart`).
- `London/`: Data directory containing Landsat satellite imagery bands and London ward boundary files.
- `.binder/`: Environment build specifications for MyBinder.org (`runtime.txt`, `apt.txt`, `install.R`).

---

## 💻 Running Locally

If you prefer running locally on your computer:
1. Clone this repository:
   ```bash
   git clone https://github.com/mpardy/harvard_workshop.git
   ```
2. Open `Satellite_imagery_ML.Rmd` in RStudio.
3. Install the required R packages if you haven't already:
   ```R
   install.packages(c("tidyverse", "sf", "terra", "tmap", "leaflet", "viridis", "rpart", "rpart.plot", "caret", "mapedit", "patchwork"))
   ```
