---
title: proj
created: 2026-06-07
updated: 2026-06-07
type: software
tags: [data-access, forecasting, heliosphere, hmi, jsoc, software, solar-physics, solar-wind]
sources: [https://github.com/JSOC-SDP/proj]
confidence: medium
---

# proj

Source URL: https://github.com/JSOC-SDP/proj

Input grouping: `JSOC`. Source list: [[doc_2592136f325f_Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1]]

## Technical notes

- Repository: `JSOC-SDP/proj`. Source: https://github.com/JSOC-SDP/proj
- Inspected README file `cookbook/ReadMe` from the repository. Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe
- Inspected git tree with approximately 1696 tracked paths. Source: https://github.com/JSOC-SDP/proj
- Dominant file extensions in the inspected tree include `.c`:473, `.f`:196, `.h`:167, `.mk`:145, `.pl`:113, `.f90`:103, `[no-ext]`:97, `.pro`:84. Source: https://github.com/JSOC-SDP/proj
- Top-level repository entries include `cgem`, `cookbook`, `datacapture`, `despike_iris`, `dsdsmigr`, `example`, `export`, `farside`, `flatfield`, `jpe`, `lev0`, `lev1`, `lev1.5_aia`, `lev1.5_hmi`, `lev1_aia`, `lev1_hmi`, `libs`, `limbfit`, `limbfit_aia`, `mag`. Source: https://github.com/JSOC-SDP/proj/tree/main
- README note: smpl_03.c	prints a list of the data series known to DRMS - a simple Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe
- README note: smpl_04.c	prints the number of unique records in a selected data series Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe
- README note: and the number of data segments per record - a simple version of Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe
- README note: smpl_05.c	inserts data records from noaa_ar.dat into series created with Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe
- README note: smpl_06.c	updates data records in series built with smpl_05 with new Source: https://github.com/JSOC-SDP/proj/blob/main/cookbook/ReadMe

## Inspected artifacts

- `cookbook/ReadMe`. Source: https://github.com/JSOC-SDP/proj


## Code/documentation structure sample

- `cgem/pdfi/apps/berciktest_ss.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `cgem/pdfi/apps/cgem_pdfi_test.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `cgem/pdfi/apps/laplacetest_ss.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `cgem/pdfi/apps/pdfi_wrapper4jsoc_test.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `cookbook/Makefile`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `datacapture/scripts/jim.test`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `datacapture/scripts/test.file`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `dsdsmigr/apps/fd_test.map`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `dsdsmigr/apps/set_gaps_missing_test.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/Rules.mk`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/Rules.mk`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/data/dsds.jsd`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/data/nso_igor.gong_mrv_ex1.jsd`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/demo_td08062007.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/f_dup_gong_mrv.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/f_ingest_gong_mrv.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/hello_world.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/helloworld.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/ingest_gong_mrv_lib.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/opendsdsrecs.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/ringfit_ssw.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/scalesegments.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/threadalrm.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/threadsigs.c`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `example/apps/xinterp.f`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `export/scripts/copy-from-rick.py`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `export/scripts/ingest-noaa-active-region-info.py`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `export/webapps/drmsexport/action.py`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `export/webapps/drmsexport/check_address.py`. Source: https://github.com/JSOC-SDP/proj/tree/main

- `export/webapps/drmsexport/check_dbserver.py`. Source: https://github.com/JSOC-SDP/proj/tree/main


## Related wiki pages

- [[solar-data-access]], [[active-region-parameters]]
