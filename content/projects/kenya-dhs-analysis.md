---
title: "Kenya DHS MNCAH Equity Analysis"
date: 2024-01-01
description: "A survey-weighted R and Power BI project analyzing maternal, newborn, child, adolescent, and household health indicators across Kenya using DHS 2014 microdata."
summary: "A survey-weighted health equity analysis of MNCAH and household indicators across Kenya’s 47 counties using DHS 2014 microdata."
tags: ["R", "DHS", "Survey Analysis", "Public Health", "Health Equity", "Geospatial Analysis", "Power BI"]
categories: ["Projects"]
showDate: false
showAuthor: false
showReadingTime: false
showTableOfContents: true
showRelatedContent: false
featureimage: "images/projects/kenya-dhs-mncah-overview.png"
---

## Overview

The Kenya DHS MNCAH Equity Analysis is a public health data analysis project focused on maternal, newborn, child, adolescent, and household health indicators across Kenya’s 47 counties.

Using **Kenya DHS 2014 microdata**, I applied survey-weighted analysis in R to estimate county-level health indicators, generate confidence intervals, visualize subnational disparities, and prepare outputs for interactive Power BI reporting.

The project demonstrates how complex survey data can be transformed into decision-ready insights for health equity monitoring, county-level planning, and evidence-based public health decision-making.

## Tools

R | DHS Microdata | survey | srvyr | tidyverse | ggplot2 | sf | geodata | Power BI | Excel

## What I Did

- Loaded and cleaned Kenya DHS 2014 microdata for maternal, child, adolescent, household, and geographic analysis
- Applied DHS sampling weights and complex survey design methods in R
- Computed county-level estimates for MNCAH and household health indicators
- Generated 95% confidence intervals to show uncertainty around subnational estimates
- Produced county-level maps, ranking charts, equity gap visuals, and drill-down outputs
- Built Power BI dashboard pages to make the results easier to explore and communicate
- Exported structured outputs for reporting, visualization, and further analysis

## Project Workflow

```text
DHS microdata preparation
→ survey design specification
→ weighted indicator estimation
→ county-level confidence intervals
→ geospatial mapping
→ Power BI dashboard development
→ health equity insights
```

## Indicators Covered

### Maternal Health

- ANC 4+ visits
- Skilled birth attendance
- Facility delivery
- Postnatal care

### Child Health

- Full immunization coverage
- Stunting prevalence
- Wasting prevalence
- Diarrhea treatment with ORS

### Adolescent Health

- Modern contraceptive use among adolescents
- Adolescents who have begun childbearing
- ANC 4+ among adolescents with a recent birth

### Household and Environmental Health

- Improved drinking water source
- Improved sanitation facility
- Household electricity access

## Dashboard Overview

![Kenya DHS MNCAH dashboard overview](/images/projects/kenya-dhs-mncah-overview.png)

The overview dashboard summarizes selected MNCAH and household health indicators across Kenya’s 47 counties, including headline indicators, county rankings, and key insights.

## Thematic Dashboard Pages

<div class="not-prose" style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; margin-top: 1.5rem; margin-bottom: 1.5rem;">

  <div>
    <img src="/images/projects/kenya-dhs-mncah-maternal-health.png"
         alt="Maternal health dashboard"
         style="width: 100%; border-radius: 10px; display: block;">
    <p style="margin-top: 8px; font-size: 0.9rem; text-align: center;">Maternal Health</p>
  </div>

  <div>
    <img src="/images/projects/kenya-dhs-mncah-child-health.png"
         alt="Child health dashboard"
         style="width: 100%; border-radius: 10px; display: block;">
    <p style="margin-top: 8px; font-size: 0.9rem; text-align: center;">Child Health</p>
  </div>

  <div>
    <img src="/images/projects/kenya-dhs-mncah-adolescent-environmental.png"
         alt="Adolescent and environmental dashboard"
         style="width: 100%; border-radius: 10px; display: block;">
    <p style="margin-top: 8px; font-size: 0.9rem; text-align: center;">Adolescent & Environmental</p>
  </div>

</div>


These dashboard pages present maternal health, child health, adolescent health, and household environmental indicators through county-level summaries and visual comparisons.

## Equity Analysis

![Kenya DHS MNCAH equity analysis dashboard](/images/projects/kenya-dhs-mncah-equity-analysis.png)

The equity analysis page compares the best- and worst-performing counties for selected indicators, highlighting performance gaps that may be hidden when only national averages are reported.

## Key Findings

- National averages can hide major county-level differences in maternal, child, adolescent, and household health outcomes
- Survey weights are essential when analyzing DHS microdata to avoid biased estimates
- Confidence intervals help communicate uncertainty, especially for county-level estimates with smaller sample sizes
- Geospatial and dashboard-based visualization makes health inequalities easier to identify and communicate
- Equity gap analysis helps highlight counties and indicators requiring targeted policy attention
- County-level outputs support localized interpretation and planning

## Skills Demonstrated

- Complex survey data analysis using R
- DHS sample weighting and survey design specification
- County-level health indicator estimation
- Confidence interval estimation
- Data cleaning and transformation using tidyverse
- Geospatial mapping using sf, geodata, and ggplot2
- Power BI dashboard design and data storytelling
- Health equity and subnational disparity analysis
- Translating statistical outputs into decision-ready insights

## Repository

[View the project on GitHub](https://github.com/craigthompsonotieno/MNCAH_Kenya_DHS)