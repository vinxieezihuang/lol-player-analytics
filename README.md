# League of Legends Player Analytics

## 1. Project Overview
This project is a personal showcase project built with Python, Jupyter Notebook, and the Riot Games API.

Its purpose is to demonstrate an end-to-end data pipeline for:
- connecting to the Riot API,
- retrieving player account data,
- collecting match history,
- extracting player-level match statistics,
- and exporting structured data for future analysis.

The project was first validated on a personal Riot account and later extended to a high-activity public account to build a larger dataset for analysis.

---

## 2. Project Goals
The main goals of this project are:

- Authenticate with the Riot API using a developer key
- Convert Riot ID into player `puuid`
- Retrieve summoner profile information
- Fetch recent match history
- Extract player-specific statistics from match details
- Export match data into CSV format
- Build a foundation for future analysis, visualization, and dashboard development

---

## 3. Current Status
The current project version has successfully completed the following:

### Completed
- VS Code project setup
- Python virtual environment setup
- Dependency installation
- `.env` configuration for Riot API key
- Riot ID to `puuid` lookup
- Summoner profile retrieval
- Recent match history retrieval
- Single-match detail extraction
- Batch extraction workflow validation
- Manual CSV export for stable output
- Public account dataset extraction with 100 matches

### Current Progress
The project was first tested on a personal Riot account, where only one recent match was available. This was sufficient to validate the API pipeline.

The workflow was then successfully scaled to the public account `Hide on bush#KR1`, from which 100 matches were retrieved and exported as a structured dataset.

### Current Limitation
A pandas compatibility issue was encountered in the current local environment, so CSV export was temporarily completed using Python's built-in CSV writer instead of a DataFrame-based workflow.

### Planned Improvement
In the next phase, the environment can be cleaned up to restore full pandas-based analysis, and the extracted dataset can be used for exploratory analysis, visualization, and performance profiling.

---

## 4. Project Structure
```text
lol-player-analytics/
│
├─ .venv/
├─ .env
├─ .gitignore
├─ requirements.txt
├─ README.md
├─ notebooks/
│  ├─ 01_api_test.ipynb
│  ├─ 02_match_history.ipynb
│  └─ 03_bulk_match_extract.ipynb
├─ src/
├─ data/
│  ├─ raw/
│  ├─ interim/
│  └─ processed/
└─ outputs/
