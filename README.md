[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18632836.svg)](https://doi.org/10.5281/zenodo.18632836)

# objective-channel-incompatibility
Minimal diagnostic simulation of multi-objective non-transitivity in model fitting.
# Objective-Channel Incompatibility in Model Fitting

This repository provides a minimal diagnostic simulation illustrating structural incompatibility in multi-objective model fitting.

The experiment demonstrates that:

- Parameter estimates optimized under different objective channels (e.g., accuracy-only vs reaction-time-only)
- May remain internally consistent within each objective
- Yet fail to admit globally coherent joint optimization

The purpose of this repository is strictly diagnostic.

No new algorithms, learning procedures, or optimization frameworks are proposed.

The simulation highlights how partially non-transitive constraints across objective channels can generate parameter divergence even when the generative process remains stable.

---

## Scope

This repository:

- Does not introduce new models
- Does not propose new fitting procedures
- Does not claim impossibility results
- Does not assert domain-specific conclusions

It provides a minimal structural stress test.

---

## Reproducibility

The notebook `objective_channel_incompatibility_ddm.ipynb` contains:

- Synthetic data generation (Drift Diffusion Model)
- Separate optimization under restricted objectives
- Comparison of recovered parameter sets
- Likelihood evaluation under cross-objective settings

This notebook demonstrates that parameter sets that perfectly satisfy single-objective evaluation criteria (e.g., accuracy-only or mean RT-only) may fail dramatically under full trial-level likelihood evaluation.

The example illustrates structural multi-objective non-transitivity in a minimal DDM setting.

To reproduce the minimal structural incompatibility example, run:

`objective_channel_incompatibility_ddm.ipynb`

