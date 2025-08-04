# Codes and data used for Cheung et al. (submitted to Nature Communications).

This repository contains the data, code, and documentation for the study:
# “Structural Inequality and Storm-Related Injuries and Deaths in the United States: A County-Year Panel Analysis (2005–2022)”

# Overview
This project investigates the association between racialized economic segregation and storm-related injuries and fatalities across U.S. counties using a socioecological framework. We integrate storm event data with structural inequality metrics to assess how structural disadvantage shapes vulnerability to climate-driven extreme weather.

# Data Sources
## 1. Storm Events Data (2005–2022)
Source: NOAA Storm Events Database

Event Types Included: Hurricanes (Typhoons), Tropical Storms, Storm Surge/Tide, Coastal Floods, Flash Floods, High Winds, and Tornadoes.

Variables Used: Event type, county (FIPS), year, direct and indirect injuries, direct and indirect deaths.

## 2. Index of Concentration at the Extremes (ICE)
Source: IPUMS Contextual Determinants of Health Dataset

Metric: ICE for race-income (non-Hispanic White high-income vs. Black low-income households)

Time Frame: Overlapping 5-year ACS windows (e.g., 2005–2009, 2006–2010...)

Assignment: Each storm event is matched to the ICE window centered around its event year.

## 3. County-Level Population Data
Source: American Community Survey (ACS)

Use: Offset term in count models and calculation of rates.

# Software & Reproducibility
Language: R (version 4.5.0)

Key packages: tidyverse, mgcv, pscl, sf, ggplot2, ggiraphExtra, glmmTMB

All code is reproducible and documented with comments. Scripts are intended to be run sequentially.
