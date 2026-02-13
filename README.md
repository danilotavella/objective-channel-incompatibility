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

The notebook `simulation.ipynb` contains:

- Synthetic data generation (Drift Diffusion Model)
- Separate optimization under restricted objectives
- Comparison of recovered parameter sets
- Likelihood evaluation under cross-objective settings

---

## License

MIT License
