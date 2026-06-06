---
title: pinn-me
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [dem, magnetic-field, mhd, nerf, neural-field, pinn, python, software, solar-physics]
sources: [https://github.com/RobertJaro/pinn-me]
confidence: medium
---

# pinn-me

Source URL: https://github.com/RobertJaro/pinn-me

Input grouping: `Jarolim`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `RobertJaro/pinn-me`. Source: https://github.com/RobertJaro/pinn-me
- Inspected README file `README.md` from the repository. Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- Inspected git tree with approximately 73 tracked paths. Source: https://github.com/RobertJaro/pinn-me
- Dominant file extensions in the inspected tree include `.py`:37, `.npz`:11, `.yaml`:10, `.sh`:9, `[no-ext]`:2, `.md`:1, `.jpg`:1, `.png`:1. Source: https://github.com/RobertJaro/pinn-me
- Top-level repository entries include `.gitignore`, `LICENSE`, `README.md`, `config`, `data`, `images`, `pme`, `requirements.txt`, `scripts`, `setup.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main
- README note: A Physics-Informed Neural Network Framework for Accurate Milne-Eddington Inversions of Solar Magnetic Fields Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- README note: PINN ME can be installed via pip. The package is compatible with Python 3.8 and above. Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- README note: The installation requires pyTorch, lightning, sunPy, and WandB. Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- README note: The code is developed for GPU acceleration, and the package will automatically detect the available GPU. If no GPU is available, the code will run on CPU, but it will be significantly slower. Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- README note: Download the Hinode/SOTSP **Level 1** data from the Hinode archive. The data should be a folder with fits files. Source: https://github.com/RobertJaro/pinn-me/blob/main/README.md
- Packaging/configuration file `setup.py` was inspected, indicating installable or configured software components. Source: https://github.com/RobertJaro/pinn-me/blob/main/setup.py

## Inspected artifacts

- `README.md`. Source: https://github.com/RobertJaro/pinn-me

- `setup.py`. Source: https://github.com/RobertJaro/pinn-me

- `requirements.txt`. Source: https://github.com/RobertJaro/pinn-me


## Code/documentation structure sample

- `config/test_set/clear.yaml`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `config/test_set/no_psf.yaml`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `config/test_set/psf.yaml`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `config/test_set/static_clear.yaml`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `config/test_set/static_psf.yaml`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `data/testcase1_200_200.npz`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `data/testcase2_200_200_withPSF_5x5_1.5.npz`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/convert/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/convert/pme_to_npz.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/create_test_set.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/create_test_set_pymilne_comparison.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/crop_psf.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/download.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/download_hmi.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/muram_prep.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/data/muram_sunspot_prep.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/compare_muram.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/compute_uncertainty.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/hinode/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/hinode/compare_hinode.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/hinode/load_time_series.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/loader.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/muram/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/muram/compare_muram.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/parameters.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/test_set/__init__.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main

- `pme/evaluation/test_set/compare_noise.py`. Source: https://github.com/RobertJaro/pinn-me/tree/main


## Related wiki pages

- [[coronal-magnetic-field-modeling]], [[solar-data-access]]
