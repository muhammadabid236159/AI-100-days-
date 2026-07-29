# 100 Days of AI

A day-by-day collection of Jupyter notebooks and supporting resources for learning AI, ML and data science.

## Quick start

```bash
# Clone repository
git clone https://github.com/muhammadabid236159/AI-100-days-.git
cd AI-100-days-

# (Optional) Create a virtual environment
python -m venv env
source env/bin/activate  # Windows: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Jupyter
jupyter notebook
```

## Repository structure (after reorganization)

```
notebooks/
  days/                 # numbered daily notebooks (day_01_*.ipynb)
  projects/             # project-focused notebooks
  README.md             # table of contents for notebooks

data/                   # datasets (CSV, JSON)
resources/              # notes, progress tracker, contributing guide
backups/                # original files kept for safety
.gitignore
requirements.txt
README.md (this file)
```

## How to use

- Browse notebooks in `notebooks/days/` and open them in Jupyter or Colab
- Keep data in `data/` — large datasets should be stored outside the repo or with Git LFS

## Future improvements

- Convert reusable functions into Python modules under `src/` and add unit tests
- Add a GitHub Actions workflow to run a subset of notebooks using `nbconvert` or `papermill`
- Add a `environment.yml` for conda reproducibility and Binder/Colab badges

## Contact

Muhammad Abid — muhammadabid236159@gmail.com
