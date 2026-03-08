# Original Notebooks (Google Colab Versions)

This folder contains the **original versions** of the project notebooks as they were developed in **Google Colab**, using Google Drive mounting for data access.

## What's in here

| File | Description |
|------|-------------|
| `NETIX_CSCI323_Regression.ipynb` | Original regression notebook (Colab version) |
| `NETIX_CSCI323_Classification.ipynb` | Original classification notebook (Colab version) |

## Why are there two versions?

The project was initially built and iterated on in **Google Colab**, where datasets were loaded by mounting Google Drive:

```python
from google.colab import drive
drive.mount("/content/drive")
RAW_DIR = Path("/content/drive/MyDrive/CSV/data_raw/regression")
```

For submission and reproducibility, the notebooks were **migrated to a local VS Code folder structure** — those updated versions live in the `notebooks/` folder at the project root. The Drive mounting was replaced with relative `pathlib` paths that resolve automatically based on the repo's folder structure, meaning anyone who clones this repo can run the notebooks without needing access to a specific Google Drive.

## How to run the project

Use the notebooks in the **`notebooks/` folder**, not the ones here. See the root `README.md` for setup instructions.

---

> These originals are kept for reference and version history only.
