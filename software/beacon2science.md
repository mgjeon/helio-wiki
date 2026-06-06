---
title: beacon2science
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [cme, drag-based-model, forecasting, python, software, solar-physics]
sources: [https://github.com/lelouedec/beacon2science]
confidence: medium
---

# beacon2science

Source URL: https://github.com/lelouedec/beacon2science

Input grouping: `CME Propagation Model`. Source list: [[doc_2f75ba2ae09c_Solar-Physics-Codes-Solar-Wind-CME_1]]

## Technical notes

- Repository: `lelouedec/beacon2science`. Source: https://github.com/lelouedec/beacon2science
- Inspected README file `README.md` from the repository. Source: https://github.com/lelouedec/beacon2science/blob/main/README.md
- Inspected git tree with approximately 44 tracked paths. Source: https://github.com/lelouedec/beacon2science
- Dominant file extensions in the inspected tree include `.py`:22, `.0`:10, `.json`:5, `.md`:2, `[no-ext]`:2, `.otf`:1, `.sh`:1, `.txt`:1. Source: https://github.com/lelouedec/beacon2science
- Top-level repository entries include `Data`, `README.md`, `RealTime`, `Sequences_dataset.py`, `Sequences_dataset_rdifs.py`, `TestNN1.py`, `TestNN2.py`, `Tracking`, `TrainNN1.py`, `TrainNN2.py`, `b2s_dataset.py`, `configs`, `dataset_train_final.json`, `models`, `requirements.txt`, `runs`, `sequence_dataset_final_rdifs.json`, `sequences_dataset.json`. Source: https://github.com/lelouedec/beacon2science/tree/main
- README note: Beacon2Science: Enhancing STEREO/HI beacon data with machine learning for efficient CME tracking Source: https://github.com/lelouedec/beacon2science/blob/main/README.md
- README note: Code for the different components of the "Beacon2Science" pipeline. A copy of the python packages used to produce this paper results can be found in requirements.txt Source: https://github.com/lelouedec/beacon2science/blob/main/README.md
- README note: In each folder, the functions.py is an adapted version of the code found in https://github.com/maikebauer/STEREO-HI-Data-Processing , with the core functions remaining the same. Source: https://github.com/lelouedec/beacon2science/blob/main/README.md
- README note: The different train and test .py files enable reproducing the paper's results from scratch once the data is processed and saved. Source: https://github.com/lelouedec/beacon2science/blob/main/README.md
- README note: For training for example: python trainNN1.py configs/config_NN1.json Source: https://github.com/lelouedec/beacon2science/blob/main/README.md

## Inspected artifacts

- `README.md`. Source: https://github.com/lelouedec/beacon2science

- `requirements.txt`. Source: https://github.com/lelouedec/beacon2science


## Code/documentation structure sample

- `Data/Create_L1.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Data/Create_L2.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Data/Create_dataset.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Data/Download_data.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Data/functions.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/RT_b2s.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/Real_timeBot.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/Track_CME.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/data_pipeline.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/functions.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `RealTime/strudl_models.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Sequences_dataset.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Sequences_dataset_rdifs.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `TestNN1.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `TestNN2.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `Tracking/Track_interface.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `TrainNN1.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `TrainNN2.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `b2s_dataset.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `models/ESRGAN.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `models/RIFE.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `models/unet2.py`. Source: https://github.com/lelouedec/beacon2science/tree/main

- `requirements.txt`. Source: https://github.com/lelouedec/beacon2science/tree/main


## Related wiki pages

- [[cme-propagation-models]], [[ambient-solar-wind-modeling]]
