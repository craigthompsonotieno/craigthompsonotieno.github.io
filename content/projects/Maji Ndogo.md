---
title: "Maji Ndogo: Water Access Analysis"
date: 2024-01-01
description: "A SQL, Python, and Power BI project analyzing water access, infrastructure gaps, queue times, data quality, and corruption risks in a fictional African nation."
summary: "A SQL, Python, and Power BI project analyzing water access, infrastructure gaps, queue times, and data integrity in a fictional African nation."
tags: ["SQL", "MySQL", "Power BI", "Python", "Jupyter Notebook", "Data Cleaning", "Data Analysis", "Water Access"]
categories: ["Projects"]
showDate: false
showAuthor: false
showReadingTime: false
showTableOfContents: true
showRelatedContent: false
featureimage: "images/projects/maji-ndogo-national-analysis.png"
---

## Overview

Maji Ndogo is a story-driven data analysis project completed as part of the **ALX Africa Data Science programme**. The project is set in a fictional African nation facing a severe water access crisis.

Using a **60,000+ record MySQL database**, I analyzed water sources, field visits, employee records, water quality scores, locations, and an independent auditor report to identify infrastructure gaps, service delivery challenges, data quality issues, and corruption risks.

## Tools

SQL | MySQL | Python | Pandas | Jupyter Notebook | Power BI | Matplotlib

## What I Did

- Queried and explored a relational MySQL database containing water access and field survey data
- Cleaned employee records, standardized email addresses, and corrected formatting issues
- Analyzed water source types, population served, queue times, and geographic service gaps
- Used SQL joins, views, CTEs, aggregations, and window functions to rank infrastructure repair priorities
- Compared surveyor scores with independent auditor scores to detect data integrity issues
- Built a Power BI dashboard to communicate national, provincial, queue-time, and gender-related insights

## Project Workflow

```text
MySQL database analysis
→ SQL cleaning and transformation
→ Python and Jupyter analysis
→ audit validation
→ Power BI dashboard
→ insights and recommendations
````

## Dashboard Preview

![Maji Ndogo national analysis dashboard](/images/projects/maji-ndogo-national-analysis.png)

The national dashboard summarizes water source distribution, population served, rural and urban patterns, and town-level differences across Maji Ndogo.

## Queue Analysis

![Maji Ndogo queue analysis dashboard](/images/projects/maji-ndogo-queue-analysis.png)

This view highlights waiting time patterns by province, day of week, and hour of day, helping identify where service bottlenecks are most severe.

## Gender and Social Risk Insights

![Maji Ndogo gender trails dashboard](/images/projects/maji-ndogo-gender-trails.png)

This dashboard explores gender-related patterns in water collection and water-related risks, showing how the burden of water access is unevenly distributed.

## Key Findings

* Many citizens rely on shared taps, rivers, wells, or broken home taps rather than reliable clean water at home
* Queue times at shared taps can become extremely long in high-burden locations
* Rural communities experience greater water access challenges than urban areas
* Women and children carry a disproportionate burden in water collection
* Independent audit comparisons revealed data quality issues and possible survey manipulation
* SQL-based ranking helped identify priority water sources for repair and infrastructure improvement

## Skills Demonstrated

* SQL querying, joins, views, CTEs, and window functions
* MySQL database analysis and cleaning
* Python-based analysis in Jupyter Notebook
* Data validation and audit comparison
* Infrastructure prioritization analysis
* Power BI dashboard design and storytelling
* Translating technical findings into decision-ready insights

## Repository

[View the project on GitHub](https://github.com/craigthompsonotieno/Maji_Ndogo)

 
