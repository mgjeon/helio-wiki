---
title: demregpy
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [dem, idl, python, remote-sensing, software, solar-physics]
sources: [https://github.com/alasdairwilson/demregpy]
confidence: medium
---

# demregpy

Source URL: https://github.com/alasdairwilson/demregpy

Input grouping: `DEM`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `alasdairwilson/demregpy`. Source: https://github.com/alasdairwilson/demregpy
- Inspected README file `README.rst` from the repository. Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- Inspected git tree with approximately 159 tracked paths. Source: https://github.com/alasdairwilson/demregpy
- Dominant file extensions in the inspected tree include `.fits`:66, `.py`:46, `.rst`:19, `[no-ext]`:5, `.yml`:5, `.yaml`:3, `.dat`:3, `.txt`:3. Source: https://github.com/alasdairwilson/demregpy
- Top-level repository entries include `.codecov.yaml`, `.codespellrc`, `.coveragerc`, `.cruft.json`, `.flake8`, `.github`, `.gitignore`, `.isort.cfg`, `.pre-commit-config.yaml`, `.readthedocs.yaml`, `.rtd-environment.yml`, `.ruff.toml`, `CHANGELOG.rst`, `LICENSE.rst`, `MANIFEST.in`, `README.rst`, `benchmarks`, `changelog`, `demregpy`, `docs`. Source: https://github.com/alasdairwilson/demregpy/tree/main
- README note: This is a python implementation of Hannah & Kontar (2012)'s regularised inversion method. Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- README note: The code is tightly based on the IDL mapping version of the DEM reg-inv code found at https://github.com/ianan/demreg in addition, the code enforces a positivity constraint on the DEM (hence pos). Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- README note: Since then the code has been significantly optimised and expanded with new features while retaining numerical agreement with the original implementation. Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- README note: To calculate a DEM you first need: Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- README note: Data and associated error for a range of channels: e.g. in dn/s/px or counts/s Source: https://github.com/alasdairwilson/demregpy/blob/main/README.rst
- Packaging/configuration file `pyproject.toml` was inspected, indicating installable or configured software components. Source: https://github.com/alasdairwilson/demregpy/blob/main/pyproject.toml
- Packaging/configuration file `setup.py` was inspected, indicating installable or configured software components. Source: https://github.com/alasdairwilson/demregpy/blob/main/setup.py
- Documentation material exists at `docs/api.rst`. Source: https://github.com/alasdairwilson/demregpy/blob/main/docs/api.rst
- Documentation material exists at `docs/conf.py`. Source: https://github.com/alasdairwilson/demregpy/blob/main/docs/conf.py

## Inspected artifacts

- `README.rst`. Source: https://github.com/alasdairwilson/demregpy

- `pyproject.toml`. Source: https://github.com/alasdairwilson/demregpy

- `setup.py`. Source: https://github.com/alasdairwilson/demregpy

- `docs/api.rst`. Source: https://github.com/alasdairwilson/demregpy

- `docs/conf.py`. Source: https://github.com/alasdairwilson/demregpy

- `docs/index.rst`. Source: https://github.com/alasdairwilson/demregpy

- `docs/installation.rst`. Source: https://github.com/alasdairwilson/demregpy

- `docs/method.rst`. Source: https://github.com/alasdairwilson/demregpy

- `docs/todo.rst`. Source: https://github.com/alasdairwilson/demregpy


## Code/documentation structure sample

- `.rtd-environment.yml`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `benchmarks/profile_dem.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `benchmarks/timeit_aia_cutouts.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `benchmarks/timeit_dem.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/__init__.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/_dev/__init__.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/_dev/scm_version.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/demmap.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/dn2dem.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/plotting.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/synthetic.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/__init__.py`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_094.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_131.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_171.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_193.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_211.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia/aia_synoptic_2014-01-01T00-00-00_335.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-00_211.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-02_094.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-03_335.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-07_193.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-09_131.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-44-12_171.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-00_211.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-02_094.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-03_335.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-07_193.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-09_131.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main

- `demregpy/tests/data/aia_flare/aia_flare_2011-02-15T01-46-12_171.fits`. Source: https://github.com/alasdairwilson/demregpy/tree/main


## Related wiki pages

- [[differential-emission-measure]], [[coronal-heating-and-loop-synthesis]]
