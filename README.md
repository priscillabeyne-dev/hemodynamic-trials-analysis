# Perioperative Hemodynamic Trials: Outcome Measures, 2015–2025

A descriptive analysis of primary outcome measures in perioperative hemodynamic monitoring and goal-directed therapy trials registered on ClinicalTrials.gov between 2015 and 2025.

**Author:** Priscilla Beyne
**Course:** CHIP 690-335, Milestone 02

## Research question

Among clinical trials related to perioperative hemodynamic monitoring and goal-directed therapy registered between 2015 and 2025, which primary outcome measures appear most often, and how does the mix of outcomes differ between 2015–2019 and 2020–2025?

## Why this project

I work on BD's Advanced Patient Monitoring Clinical Services Group, which partners with Integrated Delivery Networks on hemodynamic monitoring quality improvement projects. When our clinical champions plan to publish QI results, knowing which outcome measures are commonly used in registered trials helps us select endpoints that are credible to a clinical audience and aligned with current research practice.

## Approach

The analysis follows these steps:

1. Query the ClinicalTrials.gov v2 API across five clinical keywords (hemodynamic monitoring, goal-directed therapy, perioperative hypotension, hypotension prediction, fluid responsiveness).
2. Combine the results and deduplicate by NCT ID.
3. Filter to trials with surgical or perioperative terminology in the title or primary outcomes.
4. Restrict to start dates between January 1, 2015 and December 31, 2025.
5. Categorize each trial's primary outcome(s) into one of 14 categories using documented keyword matching rules.
6. Count outcome categories in two time periods (2015–2019 vs. 2020–2025) and visualize the comparison.

## Files in this repository

- `analysis.ipynb` — the main Jupyter notebook with all code, explanation, and the final chart
- `outcomes_by_period.png` — the visualization (also embedded in the notebook)
- `trials_clean.csv` — the cleaned and deduplicated dataset used for the analysis
- `requirements.txt` — Python libraries needed to run the notebook
- `README.md` — this file

## How to run the notebook

These instructions assume macOS. The same workflow works on Linux with minor changes; on Windows, replace `source venv/bin/activate` with `venv\Scripts\activate`.