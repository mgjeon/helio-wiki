---
title: CHMAP
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [dem, heliosphere, idl, mhd, python, software, solar-physics, solar-wind]
sources: [https://github.com/predsci/CHMAP]
confidence: medium
---

# CHMAP

Source URL: https://github.com/predsci/CHMAP

Input grouping: `Predictive Science`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `predsci/CHMAP`. Source: https://github.com/predsci/CHMAP
- Inspected README file `README.md` from the repository. Source: https://github.com/predsci/CHMAP/blob/master/README.md
- Inspected git tree with approximately 452 tracked paths. Source: https://github.com/predsci/CHMAP
- Dominant file extensions in the inspected tree include `.py`:242, `.png`:124, `.md`:32, `.ipynb`:11, `[no-ext]`:8, `.dot`:4, `.properties`:4, `.sh`:4. Source: https://github.com/predsci/CHMAP
- Top-level repository entries include `.gitignore`, `.idea`, `CITATION.cff`, `LICENSE`, `README.md`, `alembic.ini`, `chmap`, `conda_recipe_chmap.yml`, `mkdocs`, `schema_viz`, `setup.cfg`, `setup.py`, `software`. Source: https://github.com/predsci/CHMAP/tree/master
- README note: CHMAP: Coronal Hole Mapping and Analysis Pipeline Source: https://github.com/predsci/CHMAP/blob/master/README.md
- README note: CHMAP is a python package focused on the detection, mapping, tracking, and Source: https://github.com/predsci/CHMAP/blob/master/README.md
- README note: general analysis of coronal holes in the solar corona. Source: https://github.com/predsci/CHMAP/blob/master/README.md
- README note: Limb Brightening Correction Source: https://github.com/predsci/CHMAP/blob/master/README.md
- README note: Although CHMAP was designed for analyzing coronal hole evolution from seconds to Source: https://github.com/predsci/CHMAP/blob/master/README.md
- Packaging/configuration file `setup.py` was inspected, indicating installable or configured software components. Source: https://github.com/predsci/CHMAP/blob/master/setup.py
- Packaging/configuration file `setup.cfg` was inspected, indicating installable or configured software components. Source: https://github.com/predsci/CHMAP/blob/master/setup.cfg

## Inspected artifacts

- `README.md`. Source: https://github.com/predsci/CHMAP

- `setup.py`. Source: https://github.com/predsci/CHMAP

- `setup.cfg`. Source: https://github.com/predsci/CHMAP


## Code/documentation structure sample

- `chmap/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/env.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/1f2e28f386b1_delete_map_image_assoc_table.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/50d8c4f5653e_update_histogram_table.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/a1efa43a441c_add_meth_id_to_image_combos.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/a7b01b0429ff_create_histogram_table.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/d90be2c7dd2f_rename_meth_defs.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/f016c47d344a_create_var_vals_map_table.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/alembic/versions/f78f77366bda_update_var_vals_table.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/CHD_pipeline_AIAdegrad_replace-all.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/CHD_pipeline_example.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/CHD_pipeline_example_2.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/CHD_save_singles(not_used).py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/chd_funcs.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/compare_MIDM.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/correct_images.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/detection/threshold_testing.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/cluster2.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_apr13.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_counts.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_exe.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_norm.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_position.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/kmeans_prelim.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/defunct/spectral.py`. Source: https://github.com/predsci/CHMAP/tree/master

- `chmap/coronal_holes/ml_detect/examples/__init__.py`. Source: https://github.com/predsci/CHMAP/tree/master


## Related wiki pages

- [[coronal-magnetic-field-modeling]], [[solar-data-access]]
