# Redefining NFL Offensive Efficiency Metrics

## Project Overview
This repository contains the code and methodology for an advanced analytics evaluation of National Football League (NFL) offensive efficiency. Historically, NFL analysts have relied on legacy thresholds for Success Rate (40%/60%/100%) and Explosive Plays (10+ yard runs / 20+ yard passes). This project evaluates regular-season data from the nflverse dataset to find the optimal thresholds to use for these metrics. 

By analyzing Expected Points Added (EPA) and game-script differentials, this analysis proposes and statistically validates a mathematically calibrated framework:
* **Revised Success Rate:** 50% of required yardage on 1st down, 70% on 2nd down, 90% on 3rd down, and 100% on 4th down.
* **Revised Explosive Plays:** A play-agnostic threshold of 15+ yards gained.

Regression modeling demonstrates that this revised framework outperforms traditional metrics in explaining variations in season-level Points Per Game (PPG).

## Data Source
All play-by-play data is sourced from the open-source [nflverse](https://github.com/nflverse/nflverse-data) repository, accessed via the `nflreadpy` Python library.

## Repository Structure
* `analysis.ipynb`: The primary Jupyter Notebook containing data ingestion, preprocessing, feature engineering, and visualization.
* `requirements.txt` / `environment.yml`: Dependency files for reproducing the local environment.
* `README.md`: Project documentation and setup instructions.

---

## Setup & Installation Instructions

This analysis was originally developed in Google Colab but can be run in any local Jupyter environment. Choose the setup method that best fits your workflow.

### Option 1: Running Locally (Recommended)

**1. Clone the repository**
```bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
cd YOUR_REPOSITORY_NAME
