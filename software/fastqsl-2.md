---
title: FastQSL
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [field-line-tracing, magnetic-field, python, qsl, software, solar-physics]
sources: [https://github.com/peijin94/FastQSL]
confidence: medium
---

# FastQSL

Source URL: https://github.com/peijin94/FastQSL

Input grouping: `QSL`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `peijin94/FastQSL`. Source: https://github.com/peijin94/FastQSL
- Inspected README file `README.md` from the repository. Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- Inspected git tree with approximately 120 tracked paths. Source: https://github.com/peijin94/FastQSL
- Dominant file extensions in the inspected tree include `.html`:24, `.png`:20, `.js`:19, `.ipynb`:15, `.py`:11, `.pdf`:8, `[no-ext]`:4, `.cu`:4. Source: https://github.com/peijin94/FastQSL
- Top-level repository entries include `.gitattributes`, `.gitignore`, `Doxyfile`, `LICENSE`, `MANIFEST.in`, `Q.fits`, `README.md`, `demo`, `doc`, `fastqslpy`, `grad_unit_vec_B.f90`, `out-pdf`, `pyvistaPlot`, `setup.py`, `test_interp.py`, `test_script.py`. Source: https://github.com/peijin94/FastQSL/tree/main
- README note: The idea is to do the most computational intensive work in GPU with compiled code (TraceBline.cu), and do the rest of the complex but not computational intensive work in Python. Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- README note: Buy a computer with Nvidia GPU Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- README note: Install GPU driver, [https://www.nvidia.com/Download/index.aspx](https://www.nvidia.com/Download/index.aspx), for 'apt' based Linux, try ```sudo ubuntu-drivers autoinstall```. Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- README note: [https://developer.nvidia.com/Cuda-downloads](https://developer.nvidia.com/Cuda-downloads) Download cuda **v10.2! (don't install the newest)** Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- README note: Install anaconda [https://docs.anaconda.com/anaconda/install/windows/](https://docs.anaconda.com/anaconda/install/windows/) Source: https://github.com/peijin94/FastQSL/blob/main/README.md
- Packaging/configuration file `setup.py` was inspected, indicating installable or configured software components. Source: https://github.com/peijin94/FastQSL/blob/main/setup.py

## Inspected artifacts

- `README.md`. Source: https://github.com/peijin94/FastQSL

- `setup.py`. Source: https://github.com/peijin94/FastQSL


## Code/documentation structure sample

- `demo/Q_RK4.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPy.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPy3D.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPy3DScott.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyPlane.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyScott.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyStretch.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyTolTest.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyTolTestScott.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyTwist.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyTwistPlane.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45CuPyTwist_new.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/Q_RKF45MixCuPyDiffScott.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `demo/npzinputRKF45CuPyTwist.ipynb`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/_trace_bline_8cu.html`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/_trace_bline_8cuh.html`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/_trace_bline_adaptive_8cuh.html`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/bc_s.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/bdwn.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/closed.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/doc.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/doxygen.css`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/doxygen.svg`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/dynsections.js`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/files.html`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/folderclosed.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/folderopen.png`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/globals.html`. Source: https://github.com/peijin94/FastQSL/tree/main

- `doc/html/globals_defs.html`. Source: https://github.com/peijin94/FastQSL/tree/main


## Related wiki pages

- [[qsl-and-field-line-topology]], [[coronal-magnetic-field-modeling]]
