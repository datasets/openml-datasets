# OpenML Datasets

Curated tabular datasets sourced from the [OpenML](https://www.openml.org/) data repository.

## Contents

- `datapackage.json`: top-level data package descriptor for all CSV resources in this dataset.
- `data/`: one directory per dataset.
  - Each dataset directory contains:
    - a CSV file
    - an ARFF file
    - a dataset-level `datapackage.json`
    - a dataset-level `README.md`

## Structure

```text
data/
  [DATASET-NAME]/
    [DATASET-NAME].csv
    [DATASET-NAME].arff
    datapackage.json
    README.md
```

## Source

- OpenML: https://www.openml.org/search?type=data
