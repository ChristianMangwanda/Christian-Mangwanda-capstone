# Christian Mangwanda capstone

Exploratory data analysis and cohort construction for a multi-label retinal disease study on the MuReD fundus dataset.

## Contents

| Path | What it is |
| --- | --- |
| `EDA.ipynb` | Exploratory data analysis of MuReD: label tables, sources, label prevalence, co-occurrence, labels by source, and a same-eye duplicate audit. |
| `eda/` | EDA outputs: figures, per-image measurements, and the checked duplicate candidates. |
| `phase0.ipynb` | Phase 0: cohort build, duplicate audit, cross-validation folds, inner-validation sets, and nested training subsets. |
| `phase0/source/` | The MuReD label tables and the data-cleaning records. |
| `phase0/artifacts/` | The cohort, folds, splits, subsets, provenance record, and the 224 px image cache. |
| `phase0/reports/` | Phase 0 checks: crop audit, prevalence per split, subset label support. |

## Running the notebooks

- `EDA.ipynb` needs the MuReD images in an `images/` folder at the repository root.
- `phase0.ipynb` starts with `%run definitions.ipynb`. That notebook is not in this repository, so `phase0.ipynb` is here to read, not to run.

## Data

MuReD (Multi-Label Retinal Diseases) dataset, doi:[10.17632/pc4mb3h8hz.1](https://doi.org/10.17632/pc4mb3h8hz.1). The files in `phase0/artifacts/image_cache/` and the example images in the notebooks and figures are derived from MuReD images.
