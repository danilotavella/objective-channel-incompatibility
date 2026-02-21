# Objective-Channel Incompatibility

Minimal reproducible structural stress test in Drift Diffusion Model (DDM) parameter estimation.

This repository demonstrates ...
...
The example is strictly diagnostic.

## Why this matters

Multi-objective fitting is widely assumed to admit coherent joint improvement 
when objectives are compatible.

This example shows that local objective consistency 
does not imply global likelihood coherence.

The incompatibility arises from structural properties of the fitting interface,
not from noise, model misspecification, or data instability.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18632836.svg)](https://doi.org/10.5281/zenodo.18632836)

## What this repository shows

This repository provides a minimal, fully reproducible example demonstrating objective-channel incompatibility in Drift Diffusion Model (DDM) parameter estimation.

Specifically, it shows that:

- Parameter sets optimized under restricted objectives (accuracy-only or mean RT-only) can appear locally consistent.
- The same parameter sets may fail dramatically when evaluated under full trial-level likelihood.
- Multi-objective non-transitivity emerges as a structural property of the fitting interface.

The notebook `objective_channel_incompatibility_ddm.ipynb` contains the full reproducible pipeline.

Minimal diagnostic simulation of multi-objective non-transitivity in model fitting.

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

