# CNNpred Replication

Replication and critical extension of Hoseinzade & Haratizadeh (2019),
"CNNpred: CNN-based stock market prediction using a diverse set of variables"
(Expert Systems With Applications 129).


## Structure

- `data/raw/` — raw downloaded CSVs (not in git, see Drive folder)
- `data/processed/` — cleaned per-index Parquet files (not in git)
- `notebooks/` — exploratory analysis
- `src/data/` — data pipeline (download + merge)
- `src/models/` — CNNpred and baselines
- `src/eval/` — metrics, trading simulation
- `results/` — output tables and figures
- `deck/` — presentation files

## Setup

```bash
conda create -n cnnpred python=3.11 -y
conda activate cnnpred
pip install -r requirements.txt
```

Copy `.env.example` to `.env` and fill in your FRED API key.

## Links

- Decisions log: [Google Doc link]
- Raw data drive: https://drive.google.com/drive/folders/1LVNJ4dpWOllAPKvWtvw7KeAlvhmqgJOQ?usp=drive_link
- Original paper: https://doi.org/10.1016/j.eswa.2019.03.029
