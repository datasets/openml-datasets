# FRESHNESS CHECK — openml-datasets

- Repo path: `/home/fedora/Projects/up-to-date-datasets/datasets/openml-datasets`
- Checked on: `2026-03-04`

---

## Step 1: Repo Structure

```
openml-datasets/
├── data/                    # 89 subdirectories, one per dataset
│   ├── <dataset-name>/
│   │   ├── <name>.csv
│   │   ├── <name>.arff
│   │   ├── README.md        # per-dataset README with OpenML URL
│   │   └── datapackage.json # per-dataset Frictionless Data descriptor
│   └── ...
└── FRESHNESS_CHECK.md
```

**Findings:**
- No top-level README.md found.
- No top-level datapackage.json found.
- No scripts/ directory or update scripts of any kind found.
- Each of the 89 dataset subdirectories contains its own `README.md` and `datapackage.json`.

---

## Step 2: Dataset Description and Upstream Source

**Description:** A collection of 89 of the most downloaded datasets extracted from [OpenML](https://www.openml.org). Each dataset is stored in both ARFF and CSV format with Frictionless Data `datapackage.json` descriptors.

**GitHub upstream repo:** `https://github.com/datasets/openml-datasets`

**OpenML API upstream:** `https://api.openml.org/api/v1/json/data/<id>`

Each per-dataset README contains a link of the form:
> The resources for this dataset can be found at https://www.openml.org/d/<ID>

OpenML dataset IDs found in this repo range from low integers (e.g. `2` for anneal, `61` for iris) up to `40900` (Satellite).

---

## Step 3: Local Data Examination

### Git Log

The local clone was inspected via `git log`:

| Commit | Date | Message |
|--------|------|---------|
| 33fdb1a | 2018-09-03 15:49:10 +0200 | Added indent to datapackage.json files |
| 1e58ec5 | 2018-08-27 22:13:55 +0200 | [xl] Added datasets under 100 MB |
| 0cb6c64 | 2018-08-27 21:52:43 +0200 | [s] Added adult dataset |
| 9940b9a | 2018-08-27 19:48:20 +0200 | [s] Initial commit Added first dataset |

**Latest local commit date: 2018-09-03**

### Local CSV Row Counts (sample)

| Dataset | Local CSV rows (data only) |
|---------|---------------------------|
| iris | 150 |
| adult | 48,842 |
| airlines | 539,383 |
| Click_prediction_small | 399,482 |
| SpeedDating | 8,378 |
| Satellite | 5,100 |
| abalone | 4,177 |
| IMDB.drama | 120,919 |

All 89 datasets contain CSV files with data (header row + data rows verified).

---

## Step 4: Upstream Source Probing

### GitHub Upstream Repo (https://github.com/datasets/openml-datasets)

Probed via GitHub API (`https://api.github.com/repos/datasets/openml-datasets`):

- **Default branch:** `main`
- **Latest commit:** `33fdb1a8` — 2018-09-03T13:49:10Z — "Added indent to datapackage.json files"
- **pushed_at:** 2024-10-01T11:49:11Z (metadata-only update; code unchanged)
- **updated_at:** 2025-08-16T03:28:15Z (stars/forks activity, not code)
- **Open PRs:** 0

**Result: The GitHub upstream repo has no new commits since 2018-09-03. The local clone is fully in sync.**

### OpenML API (https://api.openml.org/)

Each dataset was probed individually via `https://api.openml.org/api/v1/json/data/<id>`. Key findings:

#### Upload dates of locally-stored dataset versions (v1):

| Dataset | OpenML ID | Version | Upload Date |
|---------|-----------|---------|-------------|
| anneal | 2 | 1 | 2014-04-06 |
| iris | 61 | 1 | 2014-04-06 |
| adult | 179 | 1 | 2014-04-23 |
| airlines | 1169 | 1 | 2014-10-10 |
| SpeedDating | 40536 | 1 | 2016-11-16 |
| Satellite | 40900 | 1 | 2017-09-22 |

The most recent OpenML upload date among stored datasets: **2017-09-22** (Satellite).

#### Newer versions available on OpenML (not in local repo):

| Dataset | Local Version | Latest OpenML Version | Latest Upload Date |
|---------|-------------|----------------------|-------------------|
| iris | v1 | v52 (id=44344) | 2022-11-15 |
| adult | v1 | v4 (id=45068) | 2023-01-27 |
| airlines | v1 | v4 (id=45072) | 2023-01-27 |
| SpeedDating | v1 | v2 (id=42825) | 2021-04-20 |
| Satellite | v1 | v1 only | N/A (no newer version) |

The most recent upload date found on OpenML for any version of these datasets: **2023-01-27** (adult v4 and airlines v4).

#### Row count verification (local vs OpenML API quality metadata):

| Dataset | Local Data Rows | OpenML NumberOfInstances | Match |
|---------|----------------|--------------------------|-------|
| iris | 150 | 150 | YES |
| adult | 48,842 | 48,842 | YES |
| airlines | 539,383 | 539,383 | YES |
| Click_prediction_small | 399,482 | 399,482 | YES |
| SpeedDating | 8,378 | 8,378 | YES |
| Satellite | 5,100 | 5,100 | YES |

**All checked row counts match the OpenML v1 quality metadata exactly.**

---

## Step 5: Staleness Assessment

| Dimension | Local | Upstream |
|-----------|-------|----------|
| GitHub repo last commit | 2018-09-03 | 2018-09-03 (same — fully in sync) |
| OpenML dataset versions stored | v1 of each | Up to v52/v4 available (2023-01-27) |
| Row counts vs OpenML v1 | Match | N/A |

**Verdict: STALE**

The local repo is a perfect mirror of the GitHub upstream repo (`datasets/openml-datasets`), which itself has not been updated since **2018-09-03**. OpenML.org has published newer versions of multiple datasets — for example, `adult` has a v4 uploaded on **2023-01-27** and `airlines` has a v4 uploaded on **2023-01-27**. The stored data in this repo reflects only the v1 snapshots of each OpenML dataset as they existed in 2018.

The data content within the local repo exactly matches the OpenML v1 instances counts, confirming the local copy is a faithful representation of what was downloaded — but those downloads are now approximately 7.5 years old. OpenML has newer versions of at least several datasets.

---

## Summary

- **Latest local date:** 2018-09-03 (last git commit to local/GitHub repo)
- **Latest upstream date (GitHub):** 2018-09-03 (GitHub repo has no new commits)
- **Latest upstream date (OpenML):** 2023-01-27 (adult v4 and airlines v4 on OpenML.org)
- **Is stale:** YES — the GitHub packaging repo is frozen at 2018; OpenML source has newer dataset versions
- **Staleness reason:** The GitHub upstream repo `datasets/openml-datasets` has not had new commits since 2018-09-03. OpenML.org has newer versions of many datasets (e.g., adult v4 uploaded 2023-01-27, airlines v4 uploaded 2023-01-27, iris v52 uploaded 2022-11-15). No update scripts exist to refresh the data.
