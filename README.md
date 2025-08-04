# Code and data used for Cheung et al.

This repository contains the data, code, and documentation for the study: **“Racialized Economic Segregation and Storm-Related Injuries and Deaths in the United States, 2005–2022”**

# Overview
This study investigates whether counties with higher levels of racialized economic segregation, as measured by ICE, experience greater storm-related injuries and deaths. By linking ICE with NOAA’s Storm Events Database, we test the hypothesis that stronger racialized economic segregation is associated with increased vulnerability to storm-attributed health harms, independent of population size. Importantly, we frame this investigation within a socioecological model of public health, which emphasizes the interaction between individual, community, institutional, and policy-level factors in shaping health outcomes. Racialized economic segregation (as operationalized through ICE) does not operate in isolation. It interacts with systems of housing, transportation, healthcare, and emergency preparedness to create cumulative and spatially patterned risks. Neighborhood segregation, disinvestment, discriminatory housing policies, and unequal access to basic services jointly determine which populations are most vulnerable to harm and which have the capacity to recover 49. This systems-level perspective moves beyond explanations that focus solely on individual behavior or hazard exposure, highlighting the deeply rooted nature of climate vulnerability.

# Data Sources
## 1. Storm Events Data (2005–2022)
Source: National Oceanic and Atmospheric Administration (NOAA) Storm Events Database

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

All code is reproducible and documented with comments. Scripts are intended to be run sequentially.

**Please contact Jason Cheung (jasoncheung@uchicago.edu) with any questions about this code.**
