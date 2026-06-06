---
title: NF2
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [hmi, magnetic-field, nerf, neural-field, pinn, python, software, solar-physics]
sources: [https://github.com/RobertJaro/NF2]
confidence: medium
---

# NF2

Source URL: https://github.com/RobertJaro/NF2

Input grouping: `Jarolim`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `RobertJaro/NF2`. Source: https://github.com/RobertJaro/NF2
- Inspected README file `README.md` from the repository. Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- Inspected git tree with approximately 118 tracked paths. Source: https://github.com/RobertJaro/NF2
- Dominant file extensions in the inspected tree include `.py`:57, `.md`:33, `.yaml`:12, `.ipynb`:5, `[no-ext]`:3, `.jpg`:2, `.txt`:2, `.in`:1. Source: https://github.com/RobertJaro/NF2
- Top-level repository entries include `.gitignore`, `.readthedocs.yaml`, `INSTALL.md`, `LICENSE`, `MANIFEST.in`, `README.md`, `conda-recipe`, `docs`, `environment.yml`, `examples`, `images`, `nf2`, `pyproject.toml`, `requirements.txt`, `tests`. Source: https://github.com/RobertJaro/NF2/tree/main
- README note: Neural Network Force-Free Magnetic Field Extrapolation - NF2 Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- README note: The framework is designed for solar-physics analyses with HMI/SHARP, full-disk, synoptic, and benchmark data, while keeping the training, export, and evaluation interfaces consistent across geometries. Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- README note: NF2 supports Python 3.11 and 3.12. Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- README note: For GPU-enabled PyTorch installs, select your CUDA version at [pytorch.org/get-started/locally](https://pytorch.org/get-started/locally/). For CUDA 12.6, run: Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- README note: pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu126 Source: https://github.com/RobertJaro/NF2/blob/main/README.md
- Packaging/configuration file `pyproject.toml` was inspected, indicating installable or configured software components. Source: https://github.com/RobertJaro/NF2/blob/main/pyproject.toml
- Documentation material exists at `docs/analytical.md`. Source: https://github.com/RobertJaro/NF2/blob/main/docs/analytical.md

## Inspected artifacts

- `README.md`. Source: https://github.com/RobertJaro/NF2

- `pyproject.toml`. Source: https://github.com/RobertJaro/NF2

- `environment.yml`. Source: https://github.com/RobertJaro/NF2

- `requirements.txt`. Source: https://github.com/RobertJaro/NF2

- `docs/analytical.md`. Source: https://github.com/RobertJaro/NF2

- `docs/api.md`. Source: https://github.com/RobertJaro/NF2

- `docs/cartesian.md`. Source: https://github.com/RobertJaro/NF2

- `docs/conf.py`. Source: https://github.com/RobertJaro/NF2

- `docs/configuration.md`. Source: https://github.com/RobertJaro/NF2

- `docs/downloads.md`. Source: https://github.com/RobertJaro/NF2


## Code/documentation structure sample

- `docs/_static/.gitkeep`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/_static/logo.jpg`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/analytical.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/api.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/cartesian.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/conf.py`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/configuration.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/downloads.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/evaluation.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/exporting.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/extrapolations.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/faq.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/generate_reference.py`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/generated/cli_reference.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/generated/configuration_reference.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/generated/datasets_reference.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/generated/export_metrics_reference.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/index.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/installation.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/metrics.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/notebooks.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/publications.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/quickstart.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/reference.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/requirements.txt`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/series.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/spherical.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/training.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `docs/usage.md`. Source: https://github.com/RobertJaro/NF2/tree/main

- `environment.yml`. Source: https://github.com/RobertJaro/NF2/tree/main


## Related wiki pages

- [[coronal-magnetic-field-modeling]], [[solar-data-access]]
