---
title: SuNeRF
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [cme, magnetic-field, nerf, neural-field, pinn, python, software, solar-physics]
sources: [https://github.com/RobertJaro/SuNeRF]
confidence: medium
---

# SuNeRF

Source URL: https://github.com/RobertJaro/SuNeRF

Input grouping: `Jarolim`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `RobertJaro/SuNeRF`. Source: https://github.com/RobertJaro/SuNeRF
- Inspected README file `README.md` from the repository. Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md
- Inspected git tree with approximately 212 tracked paths. Source: https://github.com/RobertJaro/SuNeRF
- Dominant file extensions in the inspected tree include `.py`:132, `.yaml`:47, `.sh`:20, `[no-ext]`:3, `.txt`:3, `.geny`:3, `.fits`:2, `.md`:1. Source: https://github.com/RobertJaro/SuNeRF
- Top-level repository entries include `.gitignore`, `LICENSE`, `README.md`, `config`, `data`, `requirements.txt`, `scripts`, `sunerf`. Source: https://github.com/RobertJaro/SuNeRF/tree/main
- README note: Solar Neural Radiance Fields for 3D Tomography** Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md
- README note: EUV emission tomography** of the solar corona Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md
- README note: White-light CME tomography** using **Thomson scattering** Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md
- README note: conda create -n sunerf python=3.10 -y Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md
- README note: pip install -r requirements.txt Source: https://github.com/RobertJaro/SuNeRF/blob/main/README.md

## Inspected artifacts

- `README.md`. Source: https://github.com/RobertJaro/SuNeRF

- `requirements.txt`. Source: https://github.com/RobertJaro/SuNeRF


## Code/documentation structure sample

- `requirements.txt`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/baseline/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/baseline/reprojection.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/convert/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/convert/sunerf_to_vtk.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/convert/vtk.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/dataset.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/date_util.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/download_aia.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/download_eui.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/download_euvi.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/download_jsoc.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/download_suvi.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/helio_concurrent_aia_stereo.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/sdo_jsoc.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/sdo_single_wl.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/solo_eui.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/download/synoptic_map.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/__init__.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/convert_stereo_to_sdo.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/convert_stereo_to_sdo_full.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/find_coordinate.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/load_aia_response_function.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/load_eui_response_function.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/load_euvi_response_function.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/prep_aia.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main

- `sunerf/data/euv/prep_aia_v2.py`. Source: https://github.com/RobertJaro/SuNeRF/tree/main


## Related wiki pages

- [[coronal-magnetic-field-modeling]], [[solar-data-access]]
