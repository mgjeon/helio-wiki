---
title: EMToolKit
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [dem, python, remote-sensing, software, solar-physics]
sources: [https://github.com/jeplowman/EMToolKit]
confidence: medium
---

# EMToolKit

Source URL: https://github.com/jeplowman/EMToolKit

Input grouping: `DEM`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `jeplowman/EMToolKit`. Source: https://github.com/jeplowman/EMToolKit
- Inspected README file `README.md` from the repository. Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- Inspected git tree with approximately 82 tracked paths. Source: https://github.com/jeplowman/EMToolKit
- Dominant file extensions in the inspected tree include `.py`:30, `.rst`:11, `.md`:7, `.fits`:7, `[no-ext]`:6, `.ipynb`:6, `.yml`:3, `.bat`:2. Source: https://github.com/jeplowman/EMToolKit
- Top-level repository entries include `.DS_Store`, `.github`, `.gitignore`, `.python-version`, `.readthedocs.yml`, `.vscode`, `CITATION.cff`, `CONTRIBUTE.md`, `DEVELOP.md`, `EMToolKit`, `EMToolKit_example_multi_instrument_downsampling.ipynb`, `EMToolKit_example_multi_instrument_matrix.ipynb`, `EMToolKit_example_single_instrument.ipynb`, `INSTALL.md`, `LICENSE`, `MANIFEST.in`, `README.md`, `dashboard.png`, `data`, `docs`. Source: https://github.com/jeplowman/EMToolKit/tree/main
- README note: Documentation Mirror**: [GitHub Pages](https://jeplowman.github.io/EMToolKit/) Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- README note: To use without installing you can run the example notebooks in this directory from a local copy of this directory structure. You will need the following packages: Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- README note: This works from either conda-forge or pip installed packages, except that you may need to install xrtpy via pip even if the rest are installed via conda-forge. Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- README note: To contribute to EMToolKit, please see the [contribute](https://github.com/jeplowman/EMToolKit/blob/main/CONTRIBUTE.md) file for details on how to get involved. Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- README note: This project is licensed under the BSD License. See the [LICENSE](https://github.com/jeplowman/EMToolKit/blob/main/LICENSE) file for more details. Source: https://github.com/jeplowman/EMToolKit/blob/main/README.md
- Packaging/configuration file `pyproject.toml` was inspected, indicating installable or configured software components. Source: https://github.com/jeplowman/EMToolKit/blob/main/pyproject.toml
- Packaging/configuration file `setup.py` was inspected, indicating installable or configured software components. Source: https://github.com/jeplowman/EMToolKit/blob/main/setup.py

## Inspected artifacts

- `README.md`. Source: https://github.com/jeplowman/EMToolKit

- `pyproject.toml`. Source: https://github.com/jeplowman/EMToolKit

- `setup.py`. Source: https://github.com/jeplowman/EMToolKit

- `environment.yml`. Source: https://github.com/jeplowman/EMToolKit

- `requirements.txt`. Source: https://github.com/jeplowman/EMToolKit


## Code/documentation structure sample

- `EMToolKit/EMToolKit.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/__main__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/downsampling_dem_wrapper.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/simple_reg_dem.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/simple_reg_dem_wrapper.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/sparse_em.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/sparse_em_wrapper.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/sparse_matrix_dem_wrapper.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/algorithms/sparse_nlmap_solver.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/examples/EMToolKit_top_example_07252010.ipynb`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/examples/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/examples/examples.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/instruments/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/instruments/aia.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/instruments/xrt.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/notebook_template.ipynb`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/basic_schemas.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/basic_transforms.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/coord_grid.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/element_functions.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/element_grid.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/element_source_responses.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/operators.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/schemas/util.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/util.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/visualization/__init__.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main

- `EMToolKit/visualization/dashboard.py`. Source: https://github.com/jeplowman/EMToolKit/tree/main


## Related wiki pages

- [[differential-emission-measure]], [[coronal-heating-and-loop-synthesis]]
