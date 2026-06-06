---
title: Parameter_Estimation_Solar_Wind
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [forecasting, gong, heliosphere, magnetic-field, pfss, python, software, solar-physics, solar-wind]
sources: [https://github.com/opaliss/Parameter_Estimation_Solar_Wind]
confidence: medium
---

# Parameter_Estimation_Solar_Wind

Source URL: https://github.com/opaliss/Parameter_Estimation_Solar_Wind

Input grouping: `Ambient Solar Wind Model`. Source list: [[doc_2f75ba2ae09c_Solar-Physics-Codes-Solar-Wind-CME_1]]

## Technical notes

- Repository: `opaliss/Parameter_Estimation_Solar_Wind`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind
- Inspected README file `README.md` from the repository. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md
- Inspected git tree with approximately 123 tracked paths. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind
- Dominant file extensions in the inspected tree include `.ipynb`:38, `.png`:34, `.npy`:20, `.py`:18, `.gz`:11, `.md`:1, `.pdf`:1. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind
- Top-level repository entries include `ACE_tools`, `GONG`, `HUX`, `MCMC_analysis`, `MCMC_simulation`, `PFSS`, `README.md`, `SA_analysis`, `SA_evaluate_samples`, `SA_tools`, `ensemble_simulation`, `figs`, `model_chain.py`, `model_chain_results`, `profiling_model_chain_computation.pdf`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main
- README note: Bayesian Inference and Global Sensitivity Analysis for Ambient Solar Wind Prediction Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md
- README note: 1. GONG CR Synoptic Maps: available online at https://gong.nso.edu/data/magmap/crmap.html. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md
- README note: Note*: ACE *in-situ* messurements are directly imported in the code using the [*heliopy*](https://heliopy.readthedocs.io/en/0.15.3/) package and the GONG synoptic maps for CR2048-CR2058 are saved in the folder **GONG**. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md
- README note: The code roadmap to run the UQ framework: sensitivity analysis $\to$ MCMC $\to$ ensemble forecasting: Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md
- README note: SA_tools/generate_samples.py** $\to$ **SA_evaluate_samples** $\to$ **SA_analysis** $\to$ **MCMC_simulation** $\to$ **MCMC_analysis** $\to$ **ensemble_simulation** Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/blob/main/README.md

## Inspected artifacts

- `README.md`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind


## Code/documentation structure sample

- `ACE_tools/interpolate.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `HUX/hux_propagation.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/.ipynb_checkpoints/MCMC_CR2048-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/.ipynb_checkpoints/MCMC_CR2052-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/.ipynb_checkpoints/MCMC_CR2053-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/.ipynb_checkpoints/MCMC_CR2054-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/.ipynb_checkpoints/MCMC_CR2056-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2049.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2050.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2052.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2053.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2054.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2055.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2056.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2057.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/MCMC_CR2058.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_analysis/histogram_mcmc_evolution.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2048.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2049.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2050.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2052.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2053.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2054.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2055.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2056.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2057.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `MCMC_simulation/MCMC_CR2058.py`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `SA_analysis/.ipynb_checkpoints/GSA_CR2048_LHS-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `SA_analysis/.ipynb_checkpoints/GSA_CR2048_LHS_Time_Dependent_QoI-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main

- `SA_analysis/.ipynb_checkpoints/GSA_CR2053_LHS-checkpoint.ipynb`. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind/tree/main


## Related wiki pages

- [[ambient-solar-wind-modeling]], [[heliosphere-model]]
