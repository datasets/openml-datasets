# Update Script Maintenance Report

Date: 2026-03-04

- Reviewed repository structure and confirmed there is no centralized update pipeline:
  - no `scripts/` directory,
  - no top-level datapackage,
  - 89 per-dataset folders with static `.csv`/`.arff` snapshots.
- Verified upstream drift is primarily due to newer OpenML dataset *versions* (not a simple single-source refresh).
- No safe automated bulk refresh was introduced in this pass because a correct update requires:
  - per-dataset OpenML version selection policy,
  - regeneration of 89 dataset subfolders,
  - compatibility checks across per-dataset README/datapackage descriptors.
- Recommendation: perform this repository as a dedicated migration task rather than incremental script patching.
