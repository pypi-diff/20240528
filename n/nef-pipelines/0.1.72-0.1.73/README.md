# Comparing `tmp/nef_pipelines-0.1.72.tar.gz` & `tmp/nef_pipelines-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.72.tar", last modified: Tue May 14 10:25:03 2024, max compression
+gzip compressed data, was "nef_pipelines-0.1.73.tar", last modified: Tue May 28 14:30:29 2024, max compression
```

## Comparing `nef_pipelines-0.1.72.tar` & `nef_pipelines-0.1.73.tar`

### file list

```diff
@@ -1,516 +1,520 @@
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.820339 nef_pipelines-0.1.72/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.708521 nef_pipelines-0.1.72/.github/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.860477 nef_pipelines-0.1.72/.github/workflows/
--rw-r--r--   0 garyt      (501) staff       (20)     1119 2024-04-18 20:49:16.000000 nef_pipelines-0.1.72/.github/workflows/test.yml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.884608 nef_pipelines-0.1.72/.idea/
--rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.72/.idea/.gitignore
--rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.72/.idea/.name
--rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.72/.idea/NFC.iml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.892947 nef_pipelines-0.1.72/.idea/inspectionProfiles/
--rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.72/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.72/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.72/.idea/modules.xml
--rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.72/.idea/vcs.xml
--rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.72/.pre-commit-config.yaml
--rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.72/.readthedocs.yml
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.72/AUTHORS.md
--rw-r--r--   0 garyt      (501) staff       (20)     9901 2024-05-14 10:24:39.000000 nef_pipelines-0.1.72/CHANGELOG.md
--rw-r--r--   0 garyt      (501) staff       (20)      334 2024-05-07 13:30:02.000000 nef_pipelines-0.1.72/CITATION.cff
--rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.72/CONTRIBUTING.md
--rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.72/LICENSE.txt
--rw-r--r--   0 garyt      (501) staff       (20)    10388 2024-05-14 10:25:03.819780 nef_pipelines-0.1.72/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)     8849 2024-04-09 13:03:05.000000 nef_pipelines-0.1.72/README.md
--rw-r--r--   0 garyt      (501) staff       (20)      833 2024-04-18 08:20:22.000000 nef_pipelines-0.1.72/TODO.md
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.911404 nef_pipelines-0.1.72/docs/
--rw-r--r--   0 garyt      (501) staff       (20)    15643 2024-05-01 22:05:57.000000 nef_pipelines-0.1.72/docs/design_overview.md
--rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.72/pyproject.toml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.925343 nef_pipelines-0.1.72/references/
--rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.72/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.72/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.72/references/kosol idps molecules-18-10802.pdf
--rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.72/release_to_pypi.sh
--rw-r--r--   0 garyt      (501) staff       (20)      472 2024-05-12 21:27:26.000000 nef_pipelines-0.1.72/requirements.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1809 2024-05-14 10:25:03.823319 nef_pipelines-0.1.72/setup.cfg
--rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.72/setup.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.713765 nef_pipelines-0.1.72/src/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.957530 nef_pipelines-0.1.72/src/nef_pipelines/
--rw-r--r--   0 garyt      (501) staff       (20)        6 2024-04-09 11:38:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/VERSION
--rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:01.993540 nef_pipelines-0.1.72/src/nef_pipelines/data/
--rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/ambiguity_translations.json
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.298447 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/
--rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
--rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
--rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
--rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
--rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
--rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
--rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.363779 nef_pipelines-0.1.72/src/nef_pipelines/lib/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      124 2024-04-24 21:11:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    20551 2024-04-24 21:37:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-05-01 19:23:42.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    26343 2024-05-04 20:19:37.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     6467 2024-05-13 18:00:53.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    14141 2024-04-24 21:12:53.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garyt      (501) staff       (20)    11906 2024-04-18 08:17:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.385794 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/chem_comp.py
--rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/io.py
--rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/object_iter.py
--rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/translator.py
--rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garyt      (501) staff       (20)    27862 2024-05-07 17:44:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     5594 2024-05-12 19:18:26.000000 nef_pipelines-0.1.72/src/nef_pipelines/main.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.389247 nef_pipelines-0.1.72/src/nef_pipelines/nef_app/
--rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.406734 nef_pipelines-0.1.72/src/nef_pipelines/tests/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.416854 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     5010 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.424034 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr-xr-x   0 garyt      (501) staff       (20)      473 2024-04-18 08:20:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garyt      (501) staff       (20)    10043 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garyt      (501) staff       (20)      192 2024-04-18 08:18:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.432370 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.438079 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
--rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     5018 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.440711 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.444504 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)     3625 2024-04-18 08:20:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.450660 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:34.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.549908 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rw-r--r--   0 garyt      (501) staff       (20)      582 2024-04-24 21:14:16.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa.nef
--rw-r--r--   0 garyt      (501) staff       (20)      708 2024-04-24 21:14:16.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef
--rwxr--r--   0 garyt      (501) staff       (20)       44 2024-05-03 08:09:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_header.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
--rw-r--r--   0 garyt      (501) staff       (20)      588 2024-04-24 21:14:16.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef
--rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rw-r--r--   0 garyt      (501) staff       (20)     1141 2024-05-04 17:47:19.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_export_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4296 2024-05-04 17:49:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_import_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.565416 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.572038 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
--rwxr-xr-x   0 garyt      (501) staff       (20)     2560 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_delete.py
--rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_filter.py
--rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_tabulate.py
--rwxr-xr-x   0 garyt      (501) staff       (20)    17207 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_unassign.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.595643 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.640216 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     8824 2024-04-16 20:00:43.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/short_co.neff
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sparky_all.out
--rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1386 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     6225 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.653461 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.753549 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr-xr-x   0 garyt      (501) staff       (20)      814 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4097 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4458 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.755518 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:50:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.763128 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
--rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.788461 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.840399 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)     2578 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     2535 2024-04-18 08:22:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     3819 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     3851 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4675 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.845006 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.851682 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garyt      (501) staff       (20)     2689 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     2013 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.857638 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.914804 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
--rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)     4616 2024-04-18 08:20:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4320 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.918632 nef_pipelines-0.1.72/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      743 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.922068 nef_pipelines-0.1.72/src/nef_pipelines/tests/simulate/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/simulate/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7057 2024-05-01 22:01:47.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/simulate/test_simulate_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:02.935056 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.031443 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)    12668 2024-04-28 20:42:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     4198 2024-04-18 08:20:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2665 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.039453 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.086061 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
--rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
--rw-r--r--   0 garyt      (501) staff       (20)     5589 2024-04-28 19:39:11.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     1889 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_import_order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)     5829 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_import_restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3306 2024-04-28 19:38:49.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_secondary_structure.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.106035 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/header.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1643 2024-05-06 16:49:31.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/multi.nef
--rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     9436 2024-04-18 18:18:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_nef_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     9402 2024-05-07 20:03:52.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_save.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     7766 2024-05-04 20:18:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.111036 nef_pipelines-0.1.72/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xcamshift/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     1830 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.155957 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.166499 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
--rw-r--r--   0 garyt      (501) staff       (20)     3396 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1555 2024-04-18 08:20:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     9051 2024-04-28 20:42:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.226057 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:15.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.264630 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garyt      (501) staff       (20)     8230 2024-04-28 19:36:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     6669 2024-04-28 19:35:07.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     1987 2024-04-28 19:32:11.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     1465 2024-04-18 08:18:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3298 2024-04-18 08:20:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    11180 2024-04-28 19:29:44.000000 nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.311656 nef_pipelines-0.1.72/src/nef_pipelines/tools/
--rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.324085 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2614 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     2670 2024-04-21 14:47:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-04-21 14:47:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.363363 nef_pipelines-0.1.72/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.367864 nef_pipelines-0.1.72/src/nef_pipelines/tools/fit/
--rw-r--r--   0 garyt      (501) staff       (20)      349 2024-05-12 19:22:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/fit/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     4408 2024-05-14 10:02:26.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/fit/exponential.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.389537 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garyt      (501) staff       (20)     8836 2024-04-16 20:56:19.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/filter.py
--rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-04-21 14:47:08.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     8044 2024-04-09 11:39:47.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garyt      (501) staff       (20)    18446 2024-04-21 14:59:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/unassign.py
--rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.395265 nef_pipelines-0.1.72/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/peaks/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/res_assign.py_unused
--rw-r--r--   0 garyt      (501) staff       (20)     8831 2024-05-13 18:00:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/save.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.401028 nef_pipelines-0.1.72/src/nef_pipelines/tools/series/
--rw-r--r--   0 garyt      (501) staff       (20)      356 2024-05-12 19:20:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/series/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    20047 2024-05-12 19:20:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/series/build.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.407873 nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/
--rw-r--r--   0 garyt      (501) staff       (20)      393 2024-05-01 21:57:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    13608 2024-05-01 21:56:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    26519 2024-05-13 17:55:38.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/unlabelling.py
--rw-r--r--   0 garyt      (501) staff       (20)      291 2024-05-13 18:00:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.410936 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.412111 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.420058 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.422488 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.425254 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.427133 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.504120 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     4514 2024-05-03 07:54:44.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.507235 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11238 2024-05-04 20:17:59.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.509657 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garyt      (501) staff       (20)     1071 2024-05-01 17:55:31.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.520596 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garyt      (501) staff       (20)     2942 2024-05-01 17:53:56.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     6096 2024-04-16 20:00:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.530351 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2156 2024-05-01 17:55:07.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    12049 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.534986 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.569039 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.574662 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/
--rw-r--r--   0 garyt      (501) staff       (20)      682 2024-05-12 21:19:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.584527 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     9591 2024-05-13 16:47:47.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/project.py
--rw-r--r--   0 garyt      (501) staff       (20)     6039 2024-05-04 20:21:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    24793 2024-05-04 20:17:59.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.614405 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.622040 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.634401 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16845 2024-04-17 08:40:33.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2359 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     5808 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.635979 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.640379 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.644419 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.648668 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     4875 2024-04-28 20:42:25.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.651111 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.655510 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.657795 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.660621 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.665933 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.669476 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.701767 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     6470 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     9064 2024-05-04 20:18:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.706093 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/
--rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.709410 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8155 2024-04-18 19:39:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.718864 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5150 2024-04-24 21:15:48.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
--rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/talos_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.721007 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.724207 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.731642 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.783243 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     2950 2024-04-28 19:38:31.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-04-28 19:42:01.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.796276 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.802247 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.811699 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-14 10:25:03.815908 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/
--rw-r--r--   0 garyt      (501) staff       (20)    10388 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)    22012 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garyt      (501) staff       (20)       48 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garyt      (501) staff       (20)      546 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garyt      (501) staff       (20)       19 2024-05-14 10:25:01.000000 nef_pipelines-0.1.72/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.72/tox.ini
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.533783 nef_pipelines-0.1.73/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.173845 nef_pipelines-0.1.73/.github/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.263009 nef_pipelines-0.1.73/.github/workflows/
+-rw-r--r--   0 garyt      (501) staff       (20)     1119 2024-04-18 20:49:16.000000 nef_pipelines-0.1.73/.github/workflows/test.yml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.271333 nef_pipelines-0.1.73/.idea/
+-rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.73/.idea/.gitignore
+-rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.73/.idea/.name
+-rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.73/.idea/NFC.iml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.276073 nef_pipelines-0.1.73/.idea/inspectionProfiles/
+-rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.73/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.73/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.73/.idea/modules.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.73/.idea/vcs.xml
+-rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.73/.pre-commit-config.yaml
+-rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.73/.readthedocs.yml
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.73/AUTHORS.md
+-rw-r--r--   0 garyt      (501) staff       (20)    10275 2024-05-28 14:24:40.000000 nef_pipelines-0.1.73/CHANGELOG.md
+-rw-r--r--   0 garyt      (501) staff       (20)      334 2024-05-07 13:30:02.000000 nef_pipelines-0.1.73/CITATION.cff
+-rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.73/CONTRIBUTING.md
+-rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.73/LICENSE.txt
+-rw-r--r--   0 garyt      (501) staff       (20)    10388 2024-05-28 14:30:29.532826 nef_pipelines-0.1.73/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)     8849 2024-04-09 13:03:05.000000 nef_pipelines-0.1.73/README.md
+-rw-r--r--   0 garyt      (501) staff       (20)      833 2024-04-18 08:20:22.000000 nef_pipelines-0.1.73/TODO.md
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.278334 nef_pipelines-0.1.73/docs/
+-rw-r--r--   0 garyt      (501) staff       (20)    15643 2024-05-01 22:05:57.000000 nef_pipelines-0.1.73/docs/design_overview.md
+-rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.73/pyproject.toml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.289314 nef_pipelines-0.1.73/references/
+-rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.73/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.73/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.73/references/kosol idps molecules-18-10802.pdf
+-rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.73/release_to_pypi.sh
+-rw-r--r--   0 garyt      (501) staff       (20)      472 2024-05-12 21:27:26.000000 nef_pipelines-0.1.73/requirements.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1809 2024-05-28 14:30:29.536099 nef_pipelines-0.1.73/setup.cfg
+-rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.73/setup.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.175203 nef_pipelines-0.1.73/src/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.301934 nef_pipelines-0.1.73/src/nef_pipelines/
+-rw-r--r--   0 garyt      (501) staff       (20)        6 2024-04-09 11:38:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/VERSION
+-rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.336769 nef_pipelines-0.1.73/src/nef_pipelines/data/
+-rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/ambiguity_translations.json
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.574990 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/
+-rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
+-rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
+-rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
+-rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
+-rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.601857 nef_pipelines-0.1.73/src/nef_pipelines/lib/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      124 2024-04-24 21:11:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20551 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    26343 2024-05-16 22:05:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6467 2024-05-13 18:00:53.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14141 2024-04-24 21:12:53.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11906 2024-04-18 08:17:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.610483 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/chem_comp.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/io.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/object_iter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/translator.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garyt      (501) staff       (20)    27878 2024-05-21 22:58:33.000000 nef_pipelines-0.1.73/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5594 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/main.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.612669 nef_pipelines-0.1.73/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.626663 nef_pipelines-0.1.73/src/nef_pipelines/tests/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.688641 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5010 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.695194 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)      473 2024-04-18 08:20:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)    10043 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garyt      (501) staff       (20)      192 2024-04-18 08:18:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.698802 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.703973 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5018 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.706011 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.711218 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     3625 2024-04-18 08:20:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.715278 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:34.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.731675 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       10 2024-05-16 07:22:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)      582 2024-04-24 21:14:16.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2024-04-24 21:14:16.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef
+-rwxr--r--   0 garyt      (501) staff       (20)       44 2024-05-16 07:35:50.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_header.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)      588 2024-04-24 21:14:16.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef
+-rwxr--r--   0 garyt      (501) staff       (20)       22 2024-05-16 07:30:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       85 2024-05-16 22:15:38.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_x2_header.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       85 2024-05-16 22:15:38.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_x2_header_repeat_chains.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)     1141 2024-05-04 17:47:19.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_export_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     7429 2024-05-17 12:55:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_import_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.747540 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.755145 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2560 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_filter.py
+-rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)    17207 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.762326 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.776323 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     8824 2024-04-16 20:00:43.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/short_co.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1386 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6225 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.786508 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.810454 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garyt      (501) staff       (20)     1878 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)      814 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4097 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4458 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.812036 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:50:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.837808 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
+-rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.850153 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.879317 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2578 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2535 2024-04-18 08:22:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3819 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3851 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4675 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.882819 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.887873 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2689 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2013 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.891418 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.919698 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)   388315 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1k0o.cif
+-rw-r--r--   0 garyt      (501) staff       (20)   304357 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1k0o.pdb
+-rw-r--r--   0 garyt      (501) staff       (20)    29541 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
+-rw-r--r--   0 garyt      (501) staff       (20)    19578 2024-05-17 21:38:59.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4795 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4795 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4195 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2395 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2254 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
+-rwxr-xr-x   0 garyt      (501) staff       (20)      800 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)     7622 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4320 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.921828 nef_pipelines-0.1.73/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      743 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.923695 nef_pipelines-0.1.73/src/nef_pipelines/tests/simulate/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/simulate/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7057 2024-05-01 22:01:47.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/simulate/test_simulate_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.954714 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.984804 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)    12668 2024-04-28 20:42:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4198 2024-04-18 08:20:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2665 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:28.991252 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.085995 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     5589 2024-04-28 19:39:11.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1889 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_import_order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5829 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_import_restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3306 2024-04-28 19:38:49.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_secondary_structure.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.101997 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/header.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1643 2024-05-06 16:49:31.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/multi.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     9436 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9402 2024-05-07 20:03:52.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_save.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     7766 2024-05-04 20:18:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.106237 nef_pipelines-0.1.73/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xcamshift/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1830 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.113331 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.120088 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
+-rw-r--r--   0 garyt      (501) staff       (20)     3396 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1555 2024-04-18 08:20:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9051 2024-04-28 20:42:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.133211 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:15.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.184496 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)     8230 2024-04-28 19:36:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6669 2024-04-28 19:35:07.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1987 2024-04-28 19:32:11.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1465 2024-04-18 08:18:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2024-04-18 08:20:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11180 2024-04-28 19:29:44.000000 nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.202199 nef_pipelines-0.1.73/src/nef_pipelines/tools/
+-rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.210640 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2614 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2670 2024-04-21 14:47:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-04-21 14:47:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.214342 nef_pipelines-0.1.73/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.217507 nef_pipelines-0.1.73/src/nef_pipelines/tools/fit/
+-rw-r--r--   0 garyt      (501) staff       (20)      349 2024-05-12 19:22:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/fit/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4408 2024-05-14 10:02:26.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/fit/exponential.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.234744 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8836 2024-04-16 20:56:19.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/filter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-04-21 14:47:08.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8044 2024-04-09 11:39:47.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garyt      (501) staff       (20)    18446 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.238415 nef_pipelines-0.1.73/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/peaks/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/res_assign.py_unused
+-rw-r--r--   0 garyt      (501) staff       (20)     8831 2024-05-13 18:00:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/save.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.242797 nef_pipelines-0.1.73/src/nef_pipelines/tools/series/
+-rw-r--r--   0 garyt      (501) staff       (20)      356 2024-05-12 19:20:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/series/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20047 2024-05-12 19:20:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/series/build.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.247859 nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/
+-rw-r--r--   0 garyt      (501) staff       (20)      393 2024-05-01 21:57:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    13608 2024-05-01 21:56:32.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    26519 2024-05-13 17:55:38.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/unlabelling.py
+-rw-r--r--   0 garyt      (501) staff       (20)      291 2024-05-13 18:00:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.250416 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.251088 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.276001 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.278390 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.280629 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.282078 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.284596 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4514 2024-05-03 07:54:44.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.306917 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14306 2024-05-23 13:35:40.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.348781 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)     1071 2024-05-01 17:55:31.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.357579 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2942 2024-05-01 17:53:56.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6096 2024-04-16 20:00:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.365416 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    12049 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.369849 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.375728 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2374 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22750 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.398017 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)      682 2024-05-12 21:19:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.405308 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9591 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/project.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6039 2024-05-04 20:21:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    24793 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.409510 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.416342 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.422221 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16845 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2359 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5808 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.423863 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.429743 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.434630 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)      454 2024-05-17 20:58:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.436663 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     4875 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    35346 2024-05-28 14:16:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.438156 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.440557 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.442401 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.446198 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.449909 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.452729 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.458690 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6470 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9064 2024-05-04 20:18:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.461768 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.466931 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8155 2024-04-18 19:39:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.474936 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5150 2024-04-24 21:15:48.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/talos_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.476228 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.479258 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.484414 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.491523 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     2950 2024-04-28 19:38:31.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-04-28 19:42:01.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.497243 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.519623 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.528313 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-28 14:30:29.530664 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garyt      (501) staff       (20)    10388 2024-05-28 14:30:27.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)    22242 2024-05-28 14:30:28.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2024-05-28 14:30:27.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       48 2024-05-28 14:30:27.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garyt      (501) staff       (20)      546 2024-05-28 14:30:27.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       19 2024-05-28 14:30:27.000000 nef_pipelines-0.1.73/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.73/tox.ini
```

### Comparing `nef_pipelines-0.1.72/.github/workflows/test.yml` & `nef_pipelines-0.1.73/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.73/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/.pre-commit-config.yaml` & `nef_pipelines-0.1.73/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/CHANGELOG.md` & `nef_pipelines-0.1.73/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -318,7 +318,16 @@
 - handling fo the default file path in save wasn't working
 - simulate unaleblling improved help text
 - incosistent use of DataType in streamfitter and fit expoenetial was corrected
 - DataType replaced with IntensityMeasuremenType
 
 ## version 0.1.71
 improved error handling when `streamfitter` does load into `fit exponential`
+
+## version 0.1.72
+
+- better handling of NEF-Pipelines fasta headers for round tripping
+- many more fasta format headers supported
+- correct error in handling beta sheet records in pdb files
+- pdbx reader takes sequence from SEQRES records as default
+- add initial chemical shift averager [alpha quality]
+- unassign supports creating ccpn style residue -1 entries e.g @32-1
```

### Comparing `nef_pipelines-0.1.72/CONTRIBUTING.md` & `nef_pipelines-0.1.73/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/LICENSE.txt` & `nef_pipelines-0.1.73/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/PKG-INFO` & `nef_pipelines-0.1.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.72
+Version: 0.1.73
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.72/README.md` & `nef_pipelines-0.1.73/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/TODO.md` & `nef_pipelines-0.1.73/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/docs/design_overview.md` & `nef_pipelines-0.1.73/docs/design_overview.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.73/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.73/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/references/kosol idps molecules-18-10802.pdf` & `nef_pipelines-0.1.73/references/kosol idps molecules-18-10802.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/release_to_pypi.sh` & `nef_pipelines-0.1.73/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/setup.cfg` & `nef_pipelines-0.1.73/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/setup.py` & `nef_pipelines-0.1.73/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/ambiguity_translations.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/ambiguity_translations.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json` & `nef_pipelines-0.1.73/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.73/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/chem_comp.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/chem_comp.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/io.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/io.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/object_iter.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/object_iter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/translation/translator.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/translation/translator.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.73/src/nef_pipelines/lib/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 UNKNOWN_INPUT_SOURCE = "unknown"
 
 FOUR_SPACES = " " * 4
 
 STDIN = Path("-")
 STDOUT = Path("-")
 
+NEWLINE = "\n"
+
 
 def _get_loop_by_category_or_none(frame: Saveframe, category: str) -> Loop:
 
     result = None
     if f"_{category}" in frame.loop_dict.keys():
         result = frame.get_loop(category)
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/main.py` & `nef_pipelines-0.1.73/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_export_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/fasta/test_export_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/fasta/test_import_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_sequence.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,169 +1,154 @@
 import typer
-from typer.testing import CliRunner
 
 from nef_pipelines.lib.nef_lib import NEF_MOLECULAR_SYSTEM
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
-from nef_pipelines.transcoders.fasta.importers.sequence import sequence
+from nef_pipelines.transcoders.rcsb.importers.sequence import sequence
 
-runner = CliRunner()
 app = typer.Typer()
 app.command()(sequence)
 
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 EXPECTED_3AA = """\
-save_nef_molecular_system
-   _nef_molecular_system.sf_category   nef_molecular_system
-   _nef_molecular_system.sf_framecode  nef_molecular_system
-
-   loop_
-      _nef_sequence.index
-      _nef_sequence.chain_code
-      _nef_sequence.sequence_code
-      _nef_sequence.residue_name
-      _nef_sequence.linking
-      _nef_sequence.residue_variant
-      _nef_sequence.cis_peptide
-
-     1   A   1   ALA   start    .   .
-     2   A   2   ALA   middle   .   .
-     3   A   3   ALA   end      .   .
+    save_nef_molecular_system
+        _nef_molecular_system.sf_category   nef_molecular_system
+        _nef_molecular_system.sf_framecode  nef_molecular_system
+
+        loop_
+            _nef_sequence.index
+            _nef_sequence.chain_code
+            _nef_sequence.sequence_code
+            _nef_sequence.residue_name
+            _nef_sequence.linking
+            _nef_sequence.residue_variant
+            _nef_sequence.cis_peptide
+
+            1   A   1   ALA   start    .   .
+            2   A   2   ALA   middle   .   .
+            3   A   3   ALA   end      .   .
 
-   stop_
+        stop_
 
-save_"""
+    save_
+"""
 
 
 # noinspection PyUnusedLocal
 def test_3aa():
 
-    path = path_in_test_data(__file__, "3aa.fasta")
-    result = run_and_report(app, [path])
-
-    mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
-
-    assert_lines_match(EXPECTED_3AA, mol_sys_result)
-
-
-def test_3aa_spaces():
-
-    path = path_in_test_data(__file__, "3aa_spaces.fasta")
-    result = run_and_report(app, [path])
+    path = path_in_test_data(__file__, "3aa.pdb")
+    result = run_and_report(app, [path], input=HEADER)
 
+    assert result.exit_code == 0
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3AA, mol_sys_result)
 
 
 EXPECTED_3A_AB = """\
-save_nef_molecular_system
-   _nef_molecular_system.sf_category   nef_molecular_system
-   _nef_molecular_system.sf_framecode  nef_molecular_system
-
-   loop_
-      _nef_sequence.index
-      _nef_sequence.chain_code
-      _nef_sequence.sequence_code
-      _nef_sequence.residue_name
-      _nef_sequence.linking
-      _nef_sequence.residue_variant
-      _nef_sequence.cis_peptide
-
-     1   A    1   ALA   start    .   .
-     2   A    2   ALA   middle   .   .
-     3   A    3   ALA   end      .   .
-     4   B    1   ALA   start    .   .
-     5   B    2   ALA   middle   .   .
-     6   B    3   ALA   end      .   .
+    save_nef_molecular_system
+        _nef_molecular_system.sf_category   nef_molecular_system
+        _nef_molecular_system.sf_framecode  nef_molecular_system
+
+        loop_
+            _nef_sequence.index
+            _nef_sequence.chain_code
+            _nef_sequence.sequence_code
+            _nef_sequence.residue_name
+            _nef_sequence.linking
+            _nef_sequence.residue_variant
+            _nef_sequence.cis_peptide
+
+            1   A    1   ALA   start    .   .
+            2   A    2   ALA   middle   .   .
+            3   A    3   ALA   end      .   .
+            4   B   11   ALA   start    .   .
+            5   B   12   ALA   middle   .   .
+            6   B   13   ALA   end      .   .
 
-   stop_
+        stop_
 
-save_"""
+    save_
+"""
 
 
 # noinspection PyUnusedLocal
-def test_3aa_x2():
+def test_3a_ab():
 
-    path = path_in_test_data(__file__, "3aa_x2.fasta")
-    result = run_and_report(app, [path])
+    path = path_in_test_data(__file__, "3a_ab.pdb")
+    result = run_and_report(app, [path], input=HEADER)
 
     assert result.exit_code == 0
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3A_AB, mol_sys_result)
 
 
-EXPECTED_3A_AB_B_start_11 = """\
-save_nef_molecular_system
-   _nef_molecular_system.sf_category   nef_molecular_system
-   _nef_molecular_system.sf_framecode  nef_molecular_system
-
-   loop_
-      _nef_sequence.index
-      _nef_sequence.chain_code
-      _nef_sequence.sequence_code
-      _nef_sequence.residue_name
-      _nef_sequence.linking
-      _nef_sequence.residue_variant
-      _nef_sequence.cis_peptide
-
-     1   A    1   ALA   start    .   .
-     2   A    2   ALA   middle   .   .
-     3   A    3   ALA   end      .   .
-     4   B   11   ALA   start    .   .
-     5   B   12   ALA   middle   .   .
-     6   B   13   ALA   end      .   .
+EXPECTED_3A_CCCC_DDDD = """\
+    save_nef_molecular_system
+        _nef_molecular_system.sf_category   nef_molecular_system
+        _nef_molecular_system.sf_framecode  nef_molecular_system
+
+        loop_
+            _nef_sequence.index
+            _nef_sequence.chain_code
+            _nef_sequence.sequence_code
+            _nef_sequence.residue_name
+            _nef_sequence.linking
+            _nef_sequence.residue_variant
+            _nef_sequence.cis_peptide
+
+            1   CCCC    1   ALA   start    .   .
+            2   CCCC    2   ALA   middle   .   .
+            3   CCCC    3   ALA   end      .   .
+            4   DDDD   11   ALA   start    .   .
+            5   DDDD   12   ALA   middle   .   .
+            6   DDDD   13   ALA   end      .   .
 
-   stop_
+        stop_
 
-save_"""
+    save_"""
 
 
 # noinspection PyUnusedLocal
-def test_3aa_x2_off_10_b():
+def test_3a_segid_cccc_dddd():
 
-    path = path_in_test_data(__file__, "3aa_x2.fasta")
-    result = run_and_report(app, ["--starts", "1,11", path])
+    path = path_in_test_data(__file__, "3a_ab.pdb")
+    result = run_and_report(app, ["--segid", path], input=HEADER)
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
-    assert_lines_match(EXPECTED_3A_AB_B_start_11, mol_sys_result)
+    assert_lines_match(EXPECTED_3A_CCCC_DDDD, mol_sys_result)
 
 
-EXPECTED_3AA_HEADER_PARSING = """\
-save_nef_molecular_system
-   _nef_molecular_system.sf_category   nef_molecular_system
-   _nef_molecular_system.sf_framecode  nef_molecular_system
+# noinspection PyUnusedLocal
+def test_3a_force_segid_cccc_dddd():
 
-   loop_
-      _nef_sequence.index
-      _nef_sequence.chain_code
-      _nef_sequence.sequence_code
-      _nef_sequence.residue_name
-      _nef_sequence.linking
-      _nef_sequence.residue_variant
-      _nef_sequence.cis_peptide
+    path = path_in_test_data(__file__, "3a_cccc_dddd.pdb")
+    result = run_and_report(app, [path], input=HEADER)
 
-     1   thx   -2   ALA   start    .   .
-     2   thx   -1   ALA   middle   .   .
-     3   thx    0   ALA   end      .   .
+    assert result.exit_code == 0
 
-   stop_
+    mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
-save_"""
+    assert_lines_match(EXPECTED_3A_CCCC_DDDD, mol_sys_result)
 
 
-def test_3aa_header_parsing():
+# noinspection PyUnusedLocal
+def test_3a_test_no_chain_segid():
 
-    path = path_in_test_data(__file__, "3aa_header.fasta")
-    result = run_and_report(app, [path])
+    path = path_in_test_data(__file__, "3a_no_chain_no_segid.pdb")
+    result = run_and_report(app, [path], input=HEADER, expected_exit_code=1)
 
-    mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
+    assert result.exit_code == 1
 
-    assert result.stdout.startswith("data_wibble")
-    assert_lines_match(EXPECTED_3AA_HEADER_PARSING, mol_sys_result)
+    assert "ERROR" in result.stdout
+    assert "both the chain code and segment id" in result.stdout
+    assert "not present on an ATOM record" in result.stdout
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/frames/test_unassign.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/frames/test_unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/short_co.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/short_co.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/simulate/test_simulate_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/simulate/test_simulate_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/predSS_4.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/predSS_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/protonated_his.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/protonated_his.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/ubi_4.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/ubi_4.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_export_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_import_order_parameters.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_import_order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_import_restraints.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_import_restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/talos/test_secondary_structure.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/talos/test_secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/multi.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/multi.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_save.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/fit/exponential.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/fit/exponential.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/filter.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/filter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/frames/unassign.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/frames/unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/save.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/save.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/series/build.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/series/build.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/simulate/unlabelling.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/simulate/unlabelling.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.73/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from dataclasses import dataclass
 from itertools import chain, cycle, islice
 from pathlib import Path
 from typing import Iterable, List
 
 import typer
 from fastaparser import Reader
@@ -19,14 +20,15 @@
     offset_chain_residues,
     sequence_3let_to_res,
     sequence_to_nef_frame,
     translate_1_to_3,
 )
 from nef_pipelines.lib.structures import SequenceResidue
 from nef_pipelines.lib.util import (
+    NEWLINE,
     STDIN,
     exit_error,
     is_int,
     parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.fasta import import_app
 
@@ -156,15 +158,18 @@
     fasta_frames = []
 
     fasta_residues, read_entry_name = _read_sequences(
         file_names, chain_codes, molecule_types, not no_header
     )
 
     if read_entry_name and not entry_name:
-        entry.entry_id = read_entry_name
+        entry_name = "__".join(read_entry_name)
+        if not entry_name:
+            entry_name = "fasta"
+        entry.entry_id = entry_name
     elif entry_name:
         entry.entry_id = entry_name
     else:
         entry.entry_id = "fasta"
 
     read_chain_codes = residues_to_chain_codes(fasta_residues)
 
@@ -211,24 +216,14 @@
     chain_code: str = None
     starts: int = 1
 
 
 # could do with taking a list of offsets
 # noinspection PyUnusedLocal
 #
-# >pdb|4ciw|A
-# >CW42
-# >crab_anapl ALPHA CRYSTALLIN B CHAIN (ALPHA(B)-CRYSTALLIN).
-# >gnl|mdb|bmrb16965:1 HET-s
-# >gggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggg
-# >2DLV_1|Chain A|Regulator of G-protein signaling 18|Homo sapiens (9606)
-# >2SRC_1|Chain A|TYROSINE-PROTEIN KINASE SRC|Homo sapiens (9606)
-# >H1N1 nucleoprotein, monomeric 416A mutant
-
-
 def _parse_fasta(fasta_sequence, parse_header: bool = True) -> Sequence:
     definition = fasta_sequence.formatted_definition_line()
     bar_count = definition.count("|")
     last_part = definition.split()[-1]
     is_bracketed = last_part.startswith("(") and last_part.endswith(")")
     is_last_field_number = last_part.strip("()").isdigit()
 
@@ -248,23 +243,66 @@
                 if is_int(field[-1]):
                     start = int(field.split()[-1])
 
         entry_id, comment = fasta_sequence.id, fasta_sequence.description
 
     elif bar_count == 3 and is_bracketed and is_last_field_number:
         fields = definition.split("|")
-        entry_id = fields[0]
-        comment = "|".join(fields[1:])
+        entry_id = fields[0].lstrip(">")
+        comment = "__".join(fields[1:])
     else:
-        entry_id, comment = fasta_sequence.id, fasta_sequence.description
+        sequence_id = "".join([c if c.isalnum() else "_" for c in fasta_sequence.id])
+        entry_id, comment = sequence_id, fasta_sequence.description
 
     letters = [letter_code.letter_code for letter_code in fasta_sequence.sequence]
     return Sequence(entry_id, comment, letters, chain_code, start)
 
 
+@dataclass
+class SequenceInfo:
+    entry_id: str
+    chain_code: str
+    start: int
+
+
+def _exit_if_there_are_file_and_input_chain_codes(
+    file_chain_codes, input_chain_codes, file_paths
+):
+    input_chain_codes = [
+        chain_code for chain_code in input_chain_codes if chain_code is not None
+    ]
+    file_chain_codes = [
+        chain_code for chain_code in file_chain_codes if chain_code is not None
+    ]
+    if file_chain_codes and input_chain_codes:
+        msg = f"""
+            there are chain codes in the files and input arguments
+            the chain codes in the files are {','.join(file_chain_codes)}
+            the chain codes in the input arguments are {','.join(input_chain_codes)}
+            the files are
+            {NEWLINE.join([str(file_path) for file_path in file_paths])}
+            chain codes must come from files or inputs not both!
+            """
+        exit_error(msg)
+
+
+def _exit_if_there_are_gaps_in_file_chain_codes(file_chain_codes, file_paths):
+
+    file_chain_codes = [
+        chain_code for chain_code in file_chain_codes if chain_code is not None
+    ]
+    if len(file_chain_codes) != len(file_chain_codes):
+        msg = f"""
+            there are sequences without chain codes in the files
+            {NEWLINE.join([str(file_path) for file_path in file_paths])}
+            either all sequences in files must have a chain code or none
+            """
+        exit_error(msg)
+
+
 def _read_sequences(
     file_paths: List[Path],
     chain_codes: Iterable[str],
     molecule_types: List[MoleculeType],
     parse_header=False,
 ) -> List[SequenceResidue]:
 
@@ -297,14 +335,37 @@
         """
         exit_error(msg)
 
     residues = OrderedSet()
     # read as many chain codes as there are sequences
     # https://stackoverflow.com/questions/16188270/get-a-fixed-number-of-items-from-a-generator
 
+    file_chain_codes = [
+        sequence_record.chain_code for sequence_record in sequence_records
+    ]
+
+    _exit_if_there_are_gaps_in_file_chain_codes(file_chain_codes, file_paths)
+
+    # this keeps the default input chain code as A
+    file_chain_codes = [
+        chain_code for chain_code in file_chain_codes if chain_code is not None
+    ]
+    if file_chain_codes and chain_codes == ["A"]:
+        chain_codes = []
+
+    _exit_if_there_are_file_and_input_chain_codes(
+        file_chain_codes, chain_codes, file_paths
+    )
+
+    _exit_if_there_are_replicate_chain_codes_from_files(
+        file_chain_codes, chain_codes, file_paths
+    )
+
+    chain_codes = file_chain_codes if file_chain_codes else chain_codes
+
     chain_code_iter = get_chain_code_iter(chain_codes)
     for sequence_record, chain_code, molecule_type in zip(
         sequence_records, chain_code_iter, molecule_types
     ):
 
         try:
             sequence_3_let = translate_1_to_3(
@@ -324,8 +385,70 @@
         chain_residues = offset_chain_residues(
             chain_residues,
             {sequence_record.chain_code: sequence_record.starts - 1},
         )
 
         residues.update(chain_residues)
 
-    return residues, sequence_records[0].entry_id
+    entry_names = [
+        sequence_record.entry_id
+        for sequence_record in sequence_records
+        if sequence_record.entry_id
+    ]
+
+    return residues, entry_names
+
+
+def _exit_if_there_are_replicate_chain_codes_from_files(
+    file_chain_codes, input_chain_codes, file_paths
+):
+
+    file_chain_counts = Counter(file_chain_codes)
+    file_chain_replicates = {
+        chain_code: count
+        for chain_code, count in file_chain_counts.items()
+        if count > 1 and chain_code is not None
+    }
+    input_chain_counts = Counter(input_chain_codes)
+    input_chain_replicates = {
+        chain_code: count
+        for chain_code, count in input_chain_counts.items()
+        if count > 1
+    }
+
+    if file_chain_replicates:
+        repeats = " ".join(
+            [
+                f"{chain_code} [{count}]"
+                for chain_code, count in file_chain_replicates.items()
+            ]
+        )
+
+        msg = f"""
+                some of the input chain codes are repeated: {repeats}
+                {NEWLINE.join([str(file_path) for file_path in file_paths])}
+                all chain codes must be unique
+            """
+        exit_error(msg)
+
+    if input_chain_replicates:
+        msg = f"""
+            some of the chain codes: {','.join(input_chain_replicates.keys())}
+            are repeated in the input each chain must have a unique chain code
+        """
+
+        exit_error(msg)
+
+    all_chain_counts = Counter(file_chain_codes + input_chain_codes)
+    all_chain_replicates = {
+        chain_code: count
+        for chain_code, count in all_chain_counts.items()
+        if count > 1 and chain_code is not None
+    }
+    if all_chain_replicates:
+        msg = f"""
+                some of the chain codes are repeated: {','.join(all_chain_replicates.keys())}
+                the chain codes come from a combination of the input arguments and the files
+                {NEWLINE.join([str(file_paths) for file_path in file_paths])}
+                all chain_codes_must_be_unique
+            """
+        exit_error(msg)
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/project.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/project.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,36 +11,30 @@
 from pdbx.reader import PdbxReader
 from strenum import LowercaseStrEnum
 
 from nef_pipelines.lib.structures import LineInfo
 from nef_pipelines.lib.util import exit_error
 
 
-class Atom:
-    ...
+class Atom: ...
 
 
-class Chain:
-    ...
+class Chain: ...
 
 
-class Residue:
-    ...
+class Residue: ...
 
 
-class Model:
-    ...
+class Model: ...
 
 
-class Structure:
-    ...
+class Structure: ...
 
 
-class Sequence:
-    ...
+class Sequence: ...
 
 
 @dataclass
 class Atom:  # noqa: F811
     serial: int
     atom_name: str
 
@@ -76,14 +70,15 @@
     segment_id: Optional[str] = None
     sequence: Optional[Sequence] = None
     model: Optional[Model] = None
 
     def __iter__(self):
         return self.residues.__iter__()
 
+
 @dataclass
 class Model:
     serial: int
     chains: Dict[str, Chain] = field(default_factory=dict)
     structure: Optional[Structure] = None
 
     def __iter__(self):
@@ -133,15 +128,14 @@
     )
 
     models: List[Model] = field(default_factory=list)
 
     def __iter__(self):
         return self.models.__iter__()
 
-
     def __getitem__(self, index):
         return self.models[0]
 
 
 current_structure: Optional[Structure] = None
 current_model: Optional[Model] = None
 current_chain: Optional[Chain] = None
@@ -298,18 +292,24 @@
         current_chain, chain_code, segment_id, line_info
     )
 
     _exit_if_no_chain_code_and_no_segment_id(chain_code, segment_id, line_info)
 
     if current_chain:
         new_chain = False
-        if (current_chain.chain_code and chain_code) and current_chain.chain_code != chain_code:
+        if (
+            current_chain.chain_code and chain_code
+        ) and current_chain.chain_code != chain_code:
             new_chain = True
 
-        if current_chain.segment_id and segment_id and current_chain.segment_id != segment_id:
+        if (
+            current_chain.segment_id
+            and segment_id
+            and current_chain.segment_id != segment_id
+        ):
             new_chain = True
 
         if new_chain:
             current_chain = None
 
     if not current_chain:
         chain_segment_key = chain_code if chain_code else segment_id
@@ -442,15 +442,17 @@
         chain_code,
         first_sequence_code,
         last_sequence_code,
         alternative_location,
         PdbSecondaryStructureType.SHEET,
     )
 
-    current_structure.secondary_structure.append(secondary_structure_element)
+    current_structure.secondary_structure.setdefault(chain_code, []).append(
+        secondary_structure_element
+    )
 
 
 def _fixup_sequences(current_structure):
     sequence_index_by_sequences = {}
     sequence_count = 1
     for sequence in current_structure.sequences.values():
         sequence = tuple(sequence.residues)
@@ -479,15 +481,15 @@
 
     for line_no, line in enumerate(lines, start=1):
 
         line = line.rstrip("\n")
 
         line = _pad_line_to_80(line)
 
-        record_type = line.split()[0]
+        record_type = line[0:6].strip()
 
         line_info = PDBLineInfo(
             source, line_no=line_no, line=line, record_type=record_type
         )
 
         if record_type == "ATOM":
             if not current_model:
@@ -914,18 +916,18 @@
             )
 
             current_structure.secondary_structure.setdefault(chain_code, []).append(
                 secondary_structure_element
             )
 
 
-def parse_cif(fh: Iterable[str], source: str) -> Structure:
+def parse_cif(lines: Iterable[str], source: str) -> Structure:
     global current_structure, current_indices
 
-    current_lines = fh.readlines()
+    current_lines = [line for line in lines]
 
     current_indices = _find_last_row_indices(
         current_lines,
         [
             "_atom_site",
         ],
     )
@@ -954,33 +956,36 @@
 
 def _match_sequences_and_set_offsets(structure):
     if structure.sequences:
         matcher = SequenceMatcher()
         chain_matches = {}
         chain_starts = {}
         for chain in structure.models[0].chains.values():
-            chain_segment_id_key = chain.chain_code if chain.chain_code else chain.segment_id
+            chain_segment_id_key = (
+                chain.chain_code if chain.chain_code else chain.segment_id
+            )
             chain_residues = {}
             chain_starts[chain_segment_id_key] = chain.residues[0].sequence_code
 
             for residue in chain.residues:
                 chain_residues[residue.sequence_code] = residue.residue_name
 
-
             min_residue = min(chain_residues.keys())
             max_residue = max(chain_residues.keys())
 
             match_residues = []
             for i in range(min_residue, max_residue + 1):
                 match_residue = chain_residues[i] if i in chain_residues else "."
                 match_residues.append(match_residue)
 
             for index, sequence in structure.sequences.items():
                 matcher.set_seqs(match_residues, sequence.residues)
-                chain_segment_key = chain.chain_code if chain.chain_code else  chain.segment_id
+                chain_segment_key = (
+                    chain.chain_code if chain.chain_code else chain.segment_id
+                )
                 chain_matches.setdefault(chain_segment_key, {})[matcher.ratio()] = (
                     index,
                     matcher.get_opcodes(),
                 )
 
         chain_offsets = {}
         for chain, matches in chain_matches.items():
@@ -1022,62 +1027,102 @@
         monomer_id = row[monomer_id_index]
         current_structure.sequences.setdefault(
             entity_id, Sequence(entity_id, None, structure=current_structure)
         )
 
         current_structure.sequences[entity_id].residues.append(monomer_id)
 
-PDB_RECORD_IDS = set([
 
-    'HEADER', 'OBSLTE', 'TITLE', 'SPLT',
-    'CAVEAT', 'COMPND', 'SOURCE','KEYWDS',
-    'EXPDTA','NUMMDL','MDLTYP','AUTHOR',
-    'REVDAT','SPRSDE','JRNL', 'REMARKS',
-    'DBREF', 'DBREF1', 'DBREF2', 'SEQADV',
-    'SEQRES', 'MODRES', 'HET','FORMUL',
-    'HETNAM','HETSYN', 'HELIX', 'SHEET',
-    'SSBOND', 'LINK', 'CISPEP', 'SITE'
-    'CRYST1', 'MTRIXn', 'ORIGXn', 'SCALEn',
-    'MODEL', 'ANISOU', 'TER', 'ENDMDL',
-    'CONECT', 'MASTER', 'END'
-])
+PDB_RECORD_IDS = set(
+    [
+        "HEADER",
+        "OBSLTE",
+        "TITLE",
+        "SPLT",
+        "CAVEAT",
+        "COMPND",
+        "SOURCE",
+        "KEYWDS",
+        "EXPDTA",
+        "NUMMDL",
+        "MDLTYP",
+        "AUTHOR",
+        "REVDAT",
+        "SPRSDE",
+        "JRNL",
+        "REMARKS",
+        "DBREF",
+        "DBREF1",
+        "DBREF2",
+        "SEQADV",
+        "SEQRES",
+        "MODRES",
+        "HET",
+        "FORMUL",
+        "HETNAM",
+        "HETSYN",
+        "HELIX",
+        "SHEET",
+        "SSBOND",
+        "LINK",
+        "CISPEP",
+        "SITE" "CRYST1",
+        "MTRIXn",
+        "ORIGXn",
+        "SCALEn",
+        "MODEL",
+        "ANISOU",
+        "TER",
+        "ENDMDL",
+        "CONECT",
+        "MASTER",
+        "END",
+    ]
+)
+
 
 class RCSBFileType(LowercaseStrEnum):
-    PDB= auto(),
-    CIF = auto(),
-    UNKNOWN =  auto()
+    PDB = (auto(),)
+    CIF = (auto(),)
+    UNKNOWN = auto()
+
 
-def guess_cif_or_pdb(lines: Iterable[str], file_name: str = '', test_length: int =100):
+def guess_cif_or_pdb(lines: Iterable[str], file_name: str = "", test_length: int = 100):
 
     pdb = 0
     cif = 0
 
     file_path = Path(file_name)
 
-    if file_path.suffix.lower() in ('.cif', '.mmcif', '.pdbx'):
+    if file_path.suffix.lower() in (".cif", ".mmcif", ".pdbx"):
         cif = 1
-    elif file_path.suffix.lower() == '.pdb':
+    elif file_path.suffix.lower() == ".pdb":
         pdb = 1
     else:
         for line in lines[:test_length]:
             fields = line.strip().split()
             if fields[0] in PDB_RECORD_IDS:
-                pdb+=1
-            if fields[0].startswith('data_') or fields[0][0] in ('_', ';') or fields[0] == 'loop_':
-                cif+=1
+                pdb += 1
+            if (
+                fields[0].startswith("data_")
+                or fields[0][0] in ("_", ";")
+                or fields[0] == "loop_"
+            ):
+                cif += 1
 
     if pdb > cif:
         result = RCSBFileType.PDB
     elif cif > pdb:
         result = RCSBFileType.CIF
     else:
         result = RCSBFileType.UNKNOWN
 
     return result
 
+
 if __name__ == "__main__":
     root = Path(
         "/Users/garythompson/Dropbox/nef_pipelines/nef_pipelines/src/nef_pipelines/tests/rcsb/test_data/"
     )
     file_name = random.choice(
         [
             root / Path("1l2y_short.cif"),
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/order_parameters.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/restraints.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/talos/talos_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/talos/talos_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.73/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.73/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.72
+Version: 0.1.73
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.73/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa.nef
 src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef
 src/nef_pipelines/tests/fasta/test_data/3aa_header.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+src/nef_pipelines/tests/fasta/test_data/3aa_x2_header.fasta
+src/nef_pipelines/tests/fasta/test_data/3aa_x2_header_repeat_chains.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_filter.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
 src/nef_pipelines/tests/frames/test_unassign.py
@@ -199,14 +201,16 @@
 src/nef_pipelines/tests/pales/test_template.py
 src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
 src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
 src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
 src/nef_pipelines/tests/rcsb/__init__.py
 src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
 src/nef_pipelines/tests/rcsb/test_sequence.py
+src/nef_pipelines/tests/rcsb/test_data/1k0o.cif
+src/nef_pipelines/tests/rcsb/test_data/1k0o.pdb
 src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
 src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
 src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
 src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
```

### Comparing `nef_pipelines-0.1.72/src/nef_pipelines.egg-info/requires.txt` & `nef_pipelines-0.1.73/src/nef_pipelines.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.72/tox.ini` & `nef_pipelines-0.1.73/tox.ini`

 * *Files identical despite different names*

