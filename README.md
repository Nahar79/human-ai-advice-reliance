# Human advice-taking and decision quality

**Real-data secondary analysis ·  portfolio draft · November 2026**

This project replaces simulated demonstrations with an executed analysis of public human-participant records. Read [results/REPORT.md](results/REPORT.md) for results, methods and limitations, or open `results/REPORT.html` for a self-contained visual report.

## Status
- Scripts executed successfully; input checks and hand-verifiable metric checks pass.
- 35,670 source trials, 1,125 participants; 34,711 trials after midpoint exclusion.
- Primary analysis: 567 participants receiving AI-labelled advice.
- Exploratory secondary analysis, **not new data collection or a full paper replication**.
  

## Run
Use Python 3.12 and a virtual environment. Install the pinned dependencies:

```bash
python -m pip install -r requirements.txt
python src/check_metrics.py
python src/analyse.py
```

The original CSV is bundled for offline reproduction. To restore a missing CSV from its pinned source:

```bash
python src/fetch_data.py
```

The analysis runs from any working directory. It regenerates tables, quality checks and PNG figures with a fixed bootstrap seed. `analysis.ipynb` is an optional guided notebook; install Jupyter separately if needed. Paths in it assume the notebook remains in this project directory. Results are precomputed so no notebook installation is required for review.

## Files
- `src/analyse.py`: input validation, descriptive metrics, participant bootstrap, figures and sensitivity checks.
- `src/check_metrics.py`: constructed examples checking beneficial/harmful switches and ties.
- `src/fetch_data.py`: pinned source download with SHA-256 verification.
- `data/provenance.json`: exact source, commit, checksum and citation.
- `data/raw/haiid_dataset.csv`: unmodified public source records; no simulated observations.
- `data/raw/SOURCE_LICENSE.txt`: original repository licence notice, retained unchanged.
- `data/MEASURES.md`: definitions and denominators.
- `results/`: aggregate CSV tables, plots and report. No participant identifiers or demographics are exported in results.
- `LEARNING_GUIDE.md`: preparation for discussing the project.

## Attribution
Data belong to the original research contribution of Vodrahalli, Daneshjou, Gerstenberg and Zou (AIES 2022), DOI https://doi.org/10.1145/3514094.3534150. Source repository: https://github.com/kailas-v/human-ai-interactions. Retain the bundled original MIT notice with source copies. This project adds a small exploratory analysis, not a claim to ownership of the original study.

## Contribution disclosure
The original researchers collected all participant data. 
