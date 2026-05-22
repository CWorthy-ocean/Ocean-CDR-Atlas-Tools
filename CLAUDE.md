# Project notes

Analysis notebooks for [C]Worthy's Ocean CDR Atlas datasets (OAE & DOR efficiency
maps). Research-grade WIP — notebooks are reproducible workflows, the intended deliverable, not a published package.

## How to run

- Conda env: `atlas-calcs` (has xarray, cartopy, pop_tools, s3fs, cftime, matplotlib).
  Activate with `source ~/miniconda3/etc/profile.d/conda.sh && conda activate atlas-calcs`.
- Execute a notebook end-to-end:
  `jupyter nbconvert --to notebook --execute --inplace notebooks/<name>.ipynb`
- After editing a notebook, always re-execute and inspect rendered figures before
  declaring done. Prefer `NotebookEdit` to whole-file rewrites so cell IDs survive.

## Domain shorthand

- OAE = Ocean Alkalinity Enhancement; DOR = Direct Ocean Removal;
  ACE = combined Alkalinity + CO₂ Enhancement (ERW / RAE / AWL).
- γ_OAE, γ_DOR, γ_ACE = dimensionless efficiency vs time since injection.
- Zhou et al. eq. 6:  γ_ACE(t) = γ_OAE(t) − R · γ_DOR(t),
  where R = I_DIC / I_Alk. R=1 is the canonical HCO₃⁻ input.
- Full theory: `reference/Zhou_et_al-main.pdf`.


## Don't, without asking

- Don't commit, push, or create branches.
- Notebooks must run on vanilla Colab with a pip-install cell.
