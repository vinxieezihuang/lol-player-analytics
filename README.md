# League of Legends Player Analytics

A portfolio analytics project built with Python, Jupyter Notebook, and the Riot Games API. The project demonstrates an end-to-end workflow for collecting, structuring, analyzing, and visualizing League of Legends player match data.

## Overview

This project covers:

- Riot API connectivity and account lookup
- Match history and match-level data extraction
- Batch collection of player performance records
- CSV-based data structuring for analysis
- Exploratory analysis and visual insights in Jupyter Notebook

## Notebooks

- `01_api_test.ipynb` — Riot API connection test, Riot ID lookup, PUUID retrieval, summoner profile check
- `02_match_history.ipynb` — recent match IDs, single-match details, sample player-level extraction
- `03_bulk_match_extract.ipynb` — batch match collection and raw CSV export
- `04_basic_analysis.ipynb` — summary metrics, champion-level analysis, processed outputs
- `05_visual_insights.ipynb` — charts for champion usage, win/loss results, KDA distribution, and gold vs damage patterns

## Outputs

- `data/processed/champion_summary.csv`
- `data/processed/top_champion_visual_summary.csv`

## Tech Stack

- Python
- Jupyter Notebook
- Riot Games API
- riotwatcher
- pandas
- numpy
- matplotlib

## Skills Demonstrated

- API-based data extraction
- Data cleaning and structuring
- Exploratory data analysis
- Data visualization
- Reproducible analytics workflow design
- Debugging API and environment issues

## Notes

- Raw and intermediate data files are excluded from version control.
- Some raw fields may contain noisy values such as `Invalid`, reflecting source data quality rather than pipeline failure.
- CSV export was used as a stable intermediate output format during development.
