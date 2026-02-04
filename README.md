# Ozone-Project
This repository contains a Python project for analyzing surface ozone data to produce trends, exceedance context, and decision-support visualizations. The project focuses on building a reproducible workflow from data retrieval through QA/QC, analysis, and reporting using EPA monitoring datasets.

# Features
Data Retrieval: Pulls ozone monitoring data from EPA AQS (and supports adding other sources).
QA/QC: Handles missing values, unit consistency, time alignment, flags, and outlier screening.
Analysis: Computes trend summaries, seasonal patterns, and exceedance-context metrics.
Visualization: Generates clear time-series plots and summary graphics for reporting.
Reproducible Outputs: Produces analysis-ready tables and figure outputs with documented assumptions.

# Data Sources
EPA AQS: MDA8 ozone (surface monitoring data)
EPA Meteorology: station/site meteorological files used alongside ozone analyses
MERRA-2 Reanalysis: planetary boundary layer height (PBLH) and supporting meteorological fields
Satellite: OMI and TROPOMI products used for chemical-regime diagnostics
Emissions: NEI (National Emissions Inventory) for emissions context and interpretation

# Project Structure
data/: Data files (CSV, TXT, NetCDF4) used in the notebooks.
notebooks/: Jupyter notebooks demonstrating QA/QC, analysis, and visualization
src/: Python modules for data retrieval, processing, analysis, and plotting
outputs/: Generated figures and tables (gitignored or versioned selectively)

# Tools and Libraries
Python 3.10+
pandas, numpy, scipy
xarray
matplotlib, plotly 
scikit-learn
cartopy
