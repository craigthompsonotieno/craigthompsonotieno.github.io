---
title: "SDG Dataset Matcher"
date: 2024-01-01
description: "A Python data engineering project that matches UN-DESA datasets to official SDMX Sustainable Development Goal indicators using API integration, XML parsing, fuzzy matching, and confidence scoring."
summary: "A Python pipeline that matches UN-DESA datasets to official SDMX SDG indicators using fuzzy matching and confidence scoring."
tags: ["Python", "Pandas", "Data Engineering", "SDGs", "Fuzzy Matching", "API", "Jupyter Notebook"]
categories: ["Projects"]
showDate: false
showAuthor: false
showReadingTime: false
showTableOfContents: true
showRelatedContent: false
featureimage: "images/projects/sdg-dataset-matcher-overview.png"
---

## Overview

The SDG Dataset Matcher is a Python data engineering project designed to link UN-DESA datasets to official SDMX Sustainable Development Goal indicators.

The project addresses a practical data organization problem: large development data catalogs often contain dataset names and descriptions, but they are not always clearly linked to official indicator identifiers. Manual matching is time-consuming, inconsistent, and difficult to scale.

Using **Python, Pandas, Requests, XML parsing, and fuzzy matching**, I built a reproducible pipeline that loads the UN-DESA dataset catalog, retrieves official SDG series metadata from the SDMX Registry API, compares dataset names with SDG indicator metadata, assigns similarity scores, classifies matches by confidence level, and exports structured outputs for validation and reuse.

## Tools

Python | Pandas | Requests | NumPy | lxml | XML Parsing | SequenceMatcher | Jupyter Notebook | CSV Outputs

## What I Did

- Loaded and cleaned a UN-DESA dataset catalog containing 498 datasets
- Queried the SDMX Registry API to retrieve official SDG data structure and series metadata
- Parsed XML responses to extract SDG series IDs, descriptions, and indicator codes
- Used Python’s `SequenceMatcher` to calculate similarity scores between dataset names and SDG series descriptions
- Classified matches into high, medium, and low confidence groups
- Generated match quality summaries and score distribution visuals
- Checked for duplicate mappings and assessed match quality
- Exported matched datasets, confidence-level files, registry metadata, and summary statistics

## Project Workflow

```text
UN-DESA dataset catalog
→ SDMX Registry API request
→ XML parsing and metadata extraction
→ text cleaning and normalization
→ fuzzy matching with SequenceMatcher
→ confidence scoring
→ validation checks
→ CSV exports and summary statistics
```

## Matching Logic

The matching process compares UN-DESA dataset names with official SDG series descriptions from the SDMX Registry.

Exact matching is not enough because dataset titles and official SDG metadata may describe the same topic using different wording. Fuzzy matching helps identify likely relationships even when names are not identical.

The project uses similarity scores between 0 and 1:

- Scores above 0.7 are treated as high-confidence matches
- Scores between 0.5 and 0.7 are treated as medium-confidence matches
- Scores of 0.5 or below are treated as low-confidence matches requiring review

## Match Quality Summary

| Match Category | Threshold | Number of Matches |
|---|---:|---:|
| High confidence | > 0.7 | 17 |
| Medium confidence | 0.5–0.7 | 56 |
| Low confidence | ≤ 0.5 | 425 |
| Total processed | — | 498 |

## Key Results

- Processed and matched **498 UN-DESA dataset records**
- Retrieved metadata for **839 SDMX SDG series**
- Matched **109 unique SDG codes**
- Produced **17 high-confidence matches** suitable for direct review or downstream use
- Produced **56 medium-confidence matches** requiring validation
- Identified **425 low-confidence matches** requiring manual review
- Reduced manual reconciliation effort by creating a reusable automated matching workflow

## Output Files

The pipeline generates structured outputs for validation, review, and reuse:

- `matched_datasets.csv`
- `high_confidence_matches.csv`
- `medium_confidence_matches.csv`
- `low_confidence_matches.csv`
- `dataset_to_series_mapping.csv`
- `summary_statistics.csv`
- `sdmx_registry_data.csv`
- `original_catalog.csv`

## Match Quality Overview

![SDG Dataset Matcher overview](/images/projects/sdg-dataset-matcher-overview.png)

The match quality overview shows the distribution of fuzzy match scores and the breakdown of high-, medium-, and low-confidence matches across the 498 processed datasets.

## Top Matches

![SDG Dataset Matcher top matches](/images/projects/sdg-dataset-matcher-top-matches.png)

The top matches output shows examples of dataset records linked to official SDG series metadata, including similarity scores and confidence classifications.

## Key Findings

- Manual dataset-to-indicator matching is slow, inconsistent, and difficult to scale
- API-based metadata retrieval makes the workflow more reproducible and easier to update
- Fuzzy matching helps identify possible relationships between differently worded dataset titles and official SDG metadata
- Confidence scoring separates stronger matches from records requiring manual validation
- The large number of low-confidence matches shows why human review is still important for final validation
- Structured CSV outputs make the results easier to audit, review, and reuse

## Skills Demonstrated

- Python-based data engineering
- API integration using Requests
- XML parsing using lxml
- Data cleaning and transformation using Pandas
- Fuzzy matching with SequenceMatcher
- Confidence scoring and match classification
- Data quality assessment and duplicate mapping checks
- CSV export and reproducible output generation
- Development data organization and SDG metadata mapping

## Repository

[View the project on GitHub](https://github.com/craigthompsonotieno/SDG-Dataset-Matcher)