---
title: MAS
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [cme, forecasting, fortran, heliosphere, magnetic-field, mhd, software, solar-physics, solar-wind]
sources: [https://github.com/predsci/MAS]
confidence: medium
---

# MAS

Source URL: https://github.com/predsci/MAS

Input grouping: `Predictive Science`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `predsci/MAS`. Source: https://github.com/predsci/MAS
- Inspected README file `README.md` from the repository. Source: https://github.com/predsci/MAS/blob/main/README.md
- Inspected git tree with approximately 242 tracked paths. Source: https://github.com/predsci/MAS
- Dominant file extensions in the inspected tree include `.out`:60, `.dat`:46, `.h5`:41, `.in`:22, `[no-ext]`:16, `.py`:14, `.conf`:8, `.err`:8. Source: https://github.com/predsci/MAS
- Top-level repository entries include `.gitignore`, `LICENSE`, `README.md`, `bin`, `build.sh`, `conf`, `doc`, `examples`, `load_mas_env.sh`, `src`, `testsuite`. Source: https://github.com/predsci/MAS/tree/main
- README note: Magnetohydrodynamic Algorithm outside a Sphere Source: https://github.com/predsci/MAS/blob/main/README.md
- README note: For more information on MAS, including model/computational details and references, see [here](https://predsci.com/mas). Source: https://github.com/predsci/MAS/blob/main/README.md
- README note: ==> Please contact PSI at support@predsci.com if you plan to use this code for research purposes. <== Source: https://github.com/predsci/MAS/blob/main/README.md
- README note: NVIDIA's `nvfortran` v26.1 (both CPU and GPU) Source: https://github.com/predsci/MAS/blob/main/README.md
- README note: NOTE: MAS does not work on NVIDIA GPUs with nvfortran 25.5 or 25.9, please use 25.7 or >=26.1. Source: https://github.com/predsci/MAS/blob/main/README.md

## Inspected artifacts

- `README.md`. Source: https://github.com/predsci/MAS


## Code/documentation structure sample

- `bin/mas_compare_run.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/mas_compare_run_diags.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/mas_hel_prep.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/mas_merge_runs.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/mas_plot_histories.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_data_reader_2d.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_data_reader_3d.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_get_2D_grid_info.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_get_3D_grid_info.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_interp2d_tp.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psi_io.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psimath.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/psipals.py`. Source: https://github.com/predsci/MAS/tree/main

- `bin/remesh_mas_run.py`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_bast_vis_sml.png`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_grid_schematic.pdf`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_input_parameter_documentation.txt`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_logo.png`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_logo_text.png`. Source: https://github.com/predsci/MAS/tree/main

- `doc/mas_units.txt`. Source: https://github.com/predsci/MAS/tree/main

- `examples/corona_polytropic_cr2124_steadystate/mas.in`. Source: https://github.com/predsci/MAS/tree/main

- `examples/corona_thermo_hm1_cr2124_steadystate/mas.in`. Source: https://github.com/predsci/MAS/tree/main

- `examples/corona_thermo_hm1_tilted_dipole_steadystate/mas.in`. Source: https://github.com/predsci/MAS/tree/main

- `examples/corona_thermo_hm2_cr2124_steadystate/closed_field_mask_pfss.h5`. Source: https://github.com/predsci/MAS/tree/main

- `examples/corona_thermo_hm2_cr2124_steadystate/mas.in`. Source: https://github.com/predsci/MAS/tree/main

- `examples/heliosphere_tmhdhm1_bc_cr2124_steadystate/bc/slice_tp001_bp002.h5`. Source: https://github.com/predsci/MAS/tree/main

- `examples/heliosphere_tmhdhm1_bc_cr2124_steadystate/bc/slice_tp001_br002.h5`. Source: https://github.com/predsci/MAS/tree/main

- `examples/heliosphere_tmhdhm1_bc_cr2124_steadystate/bc/slice_tp001_bt002.h5`. Source: https://github.com/predsci/MAS/tree/main

- `examples/heliosphere_tmhdhm1_bc_cr2124_steadystate/bc/slice_tp001_rho002.h5`. Source: https://github.com/predsci/MAS/tree/main

- `examples/heliosphere_tmhdhm1_bc_cr2124_steadystate/bc/slice_tp001_t002.h5`. Source: https://github.com/predsci/MAS/tree/main


## Related wiki pages

- [[coronal-magnetic-field-modeling]], [[solar-data-access]]
