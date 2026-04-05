# Project Name : COVID19 DASHBOARD

The project is an interactive COVID19 Dashboard built to visualize and analyze the global spread of COVID-19 from January 2020 to March 2023, featuring key metrics such as confirmed cases, death cases, and infection rates across countries.

## Project Objective : Problem Statement

The COVID-19 pandemic generated massive volumes of global health data that were difficult to interpret at a glance. The objective of this project is to provide a clear, interactive, and data-driven overview of the pandemic's impact worldwide by:

Tracking the total number of confirmed cases and death cases globally
Identifying the Top 5 countries most affected by COVID-19
Highlighting the Bottom 5 countries with the lowest prevalence
Monitoring cumulative trends on both a yearly and monthly basis
Enabling dynamic filtering by Year, Month, and Day for time-specific analysis


## Data Sourcing

The data used in this dashboard was sourced directly from the Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE) official COVID-19 GitHub repository:

📁 Source : JHU CSSE COVID-19 Time Series Data

This repository contains time-series CSV files tracking the global spread of COVID-19, specifically:

- time_series_covid19_confirmed_global.csv — Daily cumulative confirmed cases by country/region
- time_series_covid19_deaths_global.csv — Daily cumulative death cases by country/region
- time_series_covid19_recovered_global.csv — Daily cumulative recovered cases by country/region

The dataset covers 180+ countries and territories with daily updates from January 2020 through March 2023, maintained and regularly updated by the JHU Whiting School of Engineering.

## Data Transformation

Raw data was cleaned and transformed prior to visualization, including the following steps:

Data Cleaning — Removed null/missing values, corrected inconsistent country names (e.g., "Noth Koread" normalized), and standardized date formats
Aggregation — Summarized daily records into monthly and yearly cumulative totals
Rate Calculation — Computed the global infection rate (confirmed cases vs. world population), resulting in a 1% rate
Ranking — Sorted countries by total confirmed cases to derive Top 5 (US, India, France, Germany, Brazil) and Bottom 5 (Tuvalu, Holy See, MS Zaandam, Antarctica, North Korea) rankings
Filtering Logic — Implemented slicer/filter functionality by Year (2021–2023), Month (Jan–Mar), and Day for dynamic dashboard interactivity


## Data Visualization

The final dashboard was built with the following visual components:
- VisualDescriptionKPI CardsConfirmed Cases (316.9B),
- Death Cases (4.4B),
- Rate (1%)Horizontal
- Bar ChartTop 5 countries by highest confirmed casesVertical
- Bar ChartBottom 5 countries by lowest confirmed casesLine
- Chart (Yearly) Cumulative yearly confirmed cases from 2020–2023Line
- Chart (Monthly) Cumulative monthly confirmed cases across all months
- Slicers / Filters : Interactive filters by Year, Month, and Day

### Key Insights:

  - The United States recorded the highest prevalence with ~58.8 billion confirmed cases
  - North Korea recorded the lowest prevalence with just 300 confirmed cases
  - The peak yearly surge occurred in 2022, as seen in the cumulative yearly line chart
North Korea recorded the lowest prevalence with just 300 confirmed cases
The peak yearly surge occurred in 2022, as seen in the cumulative yearly line chart
