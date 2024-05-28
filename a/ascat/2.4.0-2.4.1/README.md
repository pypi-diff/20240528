# Comparing `tmp/ascat-2.4.0.tar.gz` & `tmp/ascat-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascat-2.4.0.tar", last modified: Wed May 15 12:57:12 2024, max compression
+gzip compressed data, was "ascat-2.4.1.tar", last modified: Tue May 28 09:09:29 2024, max compression
```

## Comparing `ascat-2.4.0.tar` & `ascat-2.4.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 12:57:06.000000 ascat-2.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.550478 ascat-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.554479 ascat-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 12:57:06.000000 ascat-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 12:57:06.000000 ascat-2.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 12:57:06.000000 ascat-2.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 12:57:06.000000 ascat-2.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-15 12:57:06.000000 ascat-2.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-15 12:57:06.000000 ascat-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-15 12:57:12.582479 ascat-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-15 12:57:06.000000 ascat-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/ascat_bufr_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/docs_env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/org/
--rw-r--r--   0 runner    (1001) docker     (127)    33620 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/org/xarray_readers_tutorial.org
--rw-r--r--   0 runner    (1001) docker     (127)    92416 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/read_cgls_swi_ts_files/
--rw-r--r--   0 runner    (1001) docker     (127)    65951 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   578048 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.566479 ascat-2.4.0/docs/read_eumetsat_files/
--rw-r--r--   0 runner    (1001) docker     (127)    99279 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   151416 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_5_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   151239 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_8_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   719257 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.566479 ascat-2.4.0/docs/read_hsaf_cdr_files/
--rw-r--r--   0 runner    (1001) docker     (127)    68510 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    77447 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    78359 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
--rw-r--r--   0 runner    (1001) docker     (127)   162796 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    78897 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    65970 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
--rw-r--r--   0 runner    (1001) docker     (127)  1256504 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/docs/read_hsaf_nrt_files/
--rw-r--r--   0 runner    (1001) docker     (127)   173484 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   168175 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)   165841 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
--rw-r--r--   0 runner    (1001) docker     (127)   171571 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
--rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   186561 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1289682 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/xarray_readers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 12:57:06.000000 ascat-2.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 12:57:06.000000 ascat-2.4.0/environment_win.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 12:57:06.000000 ascat-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-15 12:57:12.582479 ascat-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 12:57:06.000000 ascat-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.554479 ascat-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/aggregators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/cgls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/download/
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/download/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/download/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/eumetsat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/level1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/level2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29708 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/h_saf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.574478 ascat-2.4.0/src/ascat/read_native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21703 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/cdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/eps_native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.578479 ascat-2.4.0/src/ascat/read_native/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/ccsds.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps.dtd
--rw-r--r--   0 runner    (1001) docker     (127)    67604 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    34467 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63559 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63563 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    66425 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    66555 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    39840 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    37290 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36662 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44139 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44137 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    42843 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25966 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31948 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    89975 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/ragged_array_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)    57936 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/xarray_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.578479 ascat-2.4.0/src/ascat/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/src/ascat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/get_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/skip_test_ragged_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_cgls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_h_saf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_level1.py
--rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_level2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-15 12:57:06.000000 ascat-2.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 09:09:19.000000 ascat-2.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.886756 ascat-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.890756 ascat-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-28 09:09:19.000000 ascat-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:09:19.000000 ascat-2.4.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 09:09:19.000000 ascat-2.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 09:09:19.000000 ascat-2.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-28 09:09:19.000000 ascat-2.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 09:09:19.000000 ascat-2.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-28 09:09:29.922756 ascat-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-28 09:09:19.000000 ascat-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.898756 ascat-2.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/ascat_bufr_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/docs_env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    33620 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/org/xarray_readers_tutorial.org
+-rw-r--r--   0 runner    (1001) docker     (127)    92416 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_cgls_swi_ts_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    65951 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   578048 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_eumetsat_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    99279 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151416 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151239 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_8_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   719257 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_hsaf_cdr_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    68510 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77447 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78359 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162796 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78897 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65970 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1256504 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.906756 ascat-2.4.1/docs/read_hsaf_nrt_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   173484 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168175 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165841 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171571 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186561 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1289682 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/xarray_readers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 09:09:19.000000 ascat-2.4.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 09:09:19.000000 ascat-2.4.1/environment_win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 09:09:19.000000 ascat-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-28 09:09:29.922756 ascat-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 09:09:19.000000 ascat-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.886756 ascat-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.906756 ascat-2.4.1/src/ascat/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/cgls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/download/
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/download/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/download/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/eumetsat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29708 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/h_saf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/read_native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21703 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/cdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73255 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/eps_native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.918756 ascat-2.4.1/src/ascat/read_native/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/ccsds.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)    67604 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    34467 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63559 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63563 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66425 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66555 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39840 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    37290 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36662 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44139 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44137 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42843 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25966 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31948 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89975 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/ragged_array_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57936 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/xarray_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.918756 ascat-2.4.1/src/ascat/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/src/ascat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/get_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/skip_test_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_cgls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_h_saf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 09:09:19.000000 ascat-2.4.1/tox.ini
```

### Comparing `ascat-2.4.0/.coveragerc` & `ascat-2.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/.github/workflows/ubuntu.yml` & `ascat-2.4.1/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/.github/workflows/upload_pypi.yml` & `ascat-2.4.1/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/.github/workflows/windows.yml` & `ascat-2.4.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/.gitignore` & `ascat-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/CHANGELOG.rst` & `ascat-2.4.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 2.4.1
+=============
+
+- Add keyword to ignore ASCAT Level 1b flag noise out of limits
+
 Version 2.4.0
 =============
 
 - Update file handling read_period
 - Refactor xarray readers/writers into SwathFileCollection, CellFileCollection,
   and CellFileCollectionStack
 - Add tutorial for xarray readers/writers
```

### Comparing `ascat-2.4.0/LICENSE.txt` & `ascat-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/PKG-INFO` & `ascat-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.4.0
+Version: 2.4.1
 Summary: Read and visualize for data from the Advanced Scatterometer (ASCAT)
 Home-page: https://tuwien.at/mg/geo/rs
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, https://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.4.0/README.md` & `ascat-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/Makefile` & `ascat-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/ascat_bufr_format.rst` & `ascat-2.4.1/docs/ascat_bufr_format.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/conf.py` & `ascat-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/examples.rst` & `ascat-2.4.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/index.rst` & `ascat-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/org/xarray_readers_tutorial.org` & `ascat-2.4.1/docs/org/xarray_readers_tutorial.org`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_cgls_swi_ts.ipynb` & `ascat-2.4.1/docs/read_cgls_swi_ts.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_cgls_swi_ts.rst` & `ascat-2.4.1/docs/read_cgls_swi_ts.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png` & `ascat-2.4.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_eumetsat.ipynb` & `ascat-2.4.1/docs/read_eumetsat.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_eumetsat.rst` & `ascat-2.4.1/docs/read_eumetsat.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_19_0.png` & `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_19_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_5_0.png` & `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_5_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_8_0.png` & `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_8_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr.ipynb` & `ascat-2.4.1/docs/read_hsaf_cdr.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr.rst` & `ascat-2.4.1/docs/read_hsaf_cdr.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png` & `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt.ipynb` & `ascat-2.4.1/docs/read_hsaf_nrt.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt.rst` & `ascat-2.4.1/docs/read_hsaf_nrt.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png` & `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/docs/xarray_readers_tutorial.ipynb` & `ascat-2.4.1/docs/xarray_readers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/setup.cfg` & `ascat-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/setup.py` & `ascat-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/__init__.py` & `ascat-2.4.1/src/ascat/__init__.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/aggregate/aggregators.py` & `ascat-2.4.1/src/ascat/aggregate/aggregators.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/aggregate/interface.py` & `ascat-2.4.1/src/ascat/aggregate/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/cgls.py` & `ascat-2.4.1/src/ascat/cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/download/connectors.py` & `ascat-2.4.1/src/ascat/download/connectors.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/download/interface.py` & `ascat-2.4.1/src/ascat/download/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/eumetsat/level1.py` & `ascat-2.4.1/src/ascat/eumetsat/level1.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 Readers for ASCAT Level 1b data for various file formats.
 """
 
 import os
-from datetime import timedelta
 from collections import defaultdict
 
 import numpy as np
 
 from ascat.read_native.nc import AscatL1bNcFile
 from ascat.read_native.hdf5 import AscatL1bHdf5File
 from ascat.read_native.bufr import AscatL1bBufrFile
@@ -74,15 +73,15 @@
         elif self.file_format in [".bfr", ".bfr.gz", ".buf", "buf.gz"]:
             self.fid = AscatL1bBufrFile(self.filename)
         elif self.file_format in [".h5", ".h5.gz"]:
             self.fid = AscatL1bHdf5File(self.filename)
         else:
             raise RuntimeError("ASCAT Level 1b file format unknown")
 
-    def read(self, toi=None, roi=None, generic=True, to_xarray=False):
+    def read(self, toi=None, roi=None, generic=True, to_xarray=False, **kwargs):
         """
         Read ASCAT Level 1b data.
 
         Parameters
         ----------
         toi : tuple of datetime, optional
             Filter data for given time of interest (default: None).
@@ -100,15 +99,15 @@
         Returns
         -------
         data : xarray.Dataset or numpy.ndarray
             ASCAT data.
         metadata : dict
             Metadata.
         """
-        data, metadata = self.fid.read(generic=generic, to_xarray=to_xarray)
+        data, metadata = self.fid.read(generic=generic, to_xarray=to_xarray, **kwargs)
 
         if toi:
             data = get_toi_subset(data, toi)
 
         if roi:
             data = get_roi_subset(data, roi)
```

### Comparing `ascat-2.4.0/src/ascat/eumetsat/level2.py` & `ascat-2.4.1/src/ascat/eumetsat/level2.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/file_handling.py` & `ascat-2.4.1/src/ascat/file_handling.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/h_saf.py` & `ascat-2.4.1/src/ascat/h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/bufr.py` & `ascat-2.4.1/src/ascat/read_native/bufr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/cdr.py` & `ascat-2.4.1/src/ascat/read_native/cdr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/eps_native.py` & `ascat-2.4.1/src/ascat/read_native/eps_native.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,27 @@
 import xarray as xr
 import lxml.etree as etree
 from cadati.jd_date import jd2dt
 from datetime import datetime
 from datetime import timedelta
 
 from ascat.utils import get_toi_subset, get_roi_subset
+from ascat.utils import get_bit, set_bit
 
 short_cds_time = np.dtype([("day", ">u2"), ("time", ">u4")])
 long_cds_time = np.dtype([("day", ">u2"), ("ms", ">u4"), ("mms", ">u2")])
 
 long_nan = np.iinfo(np.int32).min
 ulong_nan = np.iinfo(np.uint32).max
 int_nan = np.iinfo(np.int16).min
 uint_nan = np.iinfo(np.uint16).max
-int8_nan = np.iinfo(np.int8).max
+int8_nan = np.iinfo(np.int8).min
 uint8_nan = np.iinfo(np.uint8).max
-int32_nan = np.iinfo(np.int32).max
+int32_nan = np.iinfo(np.int32).min
+uint32_nan = np.iinfo(np.uint32).max
 float32_nan = -999999.
 
 # 2000-01-01 00:00:00
 julian_epoch = 2451544.5
 
 
 class AscatL1bEpsSzfFile:
@@ -71,15 +73,16 @@
         Parameters
         ----------
         filename : str
             Filename.
         """
         self.filename = filename
 
-    def read(self, toi=None, roi=None, generic=True, to_xarray=False):
+    def read(self, toi=None, roi=None, generic=True, to_xarray=False,
+             ignore_noise_ool=False):
         """
         Read ASCAT Level 1b data.
 
         Parameters
         ----------
         toi : tuple of datetime, optional
             Filter data for given time of interest (default: None).
@@ -89,28 +92,32 @@
             e.g. latmin, lonmin, latmax, lonmax
         generic : boolean, optional
             Convert original data field names to generic field names
             (default: True).
         to_xarray : boolean, optional
             Convert data to xarray.Dataset otherwise numpy.ndarray will be
             returned (default: False).
+        ignore_noise_ool : bool, optional
+            Ignore noise out of limit flag (default: False).
 
         Returns
         -------
         data : xarray.Dataset or numpy.ndarray
             ASCAT data.
         metadata : dict
             Metadata.
         """
-        data, metadata = read_eps_l1b(self.filename,
-                                      generic,
-                                      to_xarray,
-                                      full=False,
-                                      unsafe=True,
-                                      scale_mdr=False)
+        data, metadata = read_eps_l1b(
+            self.filename,
+            generic,
+            to_xarray,
+            full=False,
+            unsafe=True,
+            scale_mdr=False,
+            ignore_noise_ool=ignore_noise_ool)
 
         if toi:
             data = get_toi_subset(data, toi)
 
         if roi:
             data = get_roi_subset(data, roi)
 
@@ -155,15 +162,15 @@
         Parameters
         ----------
         filename : str
             Filename.
         """
         self.filename = filename
 
-    def read(self, generic=False, to_xarray=False):
+    def read(self, generic=False, to_xarray=False, **kwargs):
         """
         Read ASCAT Level 1b data.
 
         Parameters
         ----------
         generic : boolean, optional
             Convert original data field names to generic field names
@@ -175,15 +182,15 @@
         Returns
         -------
         data : xarray.Dataset or numpy.ndarray
             ASCAT data.
         metadata : dict
             Metadata.
         """
-        return read_eps_l1b(self.filename, generic, to_xarray)
+        return read_eps_l1b(self.filename, generic, to_xarray, **kwargs)
 
     def close(self):
         """
         Close file.
         """
         pass
 
@@ -353,16 +360,16 @@
             if ((prev_grh["record_class"] != grh["record_class"]) or
                 (prev_grh["record_subclass"] != grh["record_subclass"])):
 
                 # compute record start position of previous record
                 start_pos = (abs_pos - prev_grh["record_size"] * record_count)
                 self.fid.seek(start_pos)
 
-                if full or (prev_grh["record_class"] == 8
-                            or prev_grh["record_class"] == 1):
+                if full or (prev_grh["record_class"] == 8 or
+                            prev_grh["record_class"] == 1):
                     # read previous record, because new one is coming
                     self.read_record_class(prev_grh, record_count)
 
                 # reset record class count
                 record_count = 1
             else:
                 # same record class as before, increase count
@@ -427,17 +434,16 @@
         # sphr (Secondary Product Header Record)
         elif grh["record_class"] == 2:
             self.fid.seek(grh.itemsize, 1)
             self._read_sphr(grh)
 
         # ipr (Internal Pointer Record)
         elif grh["record_class"] == 3:
-            data = np.fromfile(self.fid,
-                               dtype=self.ipr_dtype,
-                               count=record_count)
+            data = np.fromfile(
+                self.fid, dtype=self.ipr_dtype, count=record_count)
             self.aux["ipr"].append(data)
 
         # geadr (Global External Auxiliary Data Record)
         elif grh["record_class"] == 4:
             data = self._read_pointer(record_count)
             self.aux["geadr"].append(data)
 
@@ -446,17 +452,16 @@
             data = self._read_pointer(record_count)
             self.aux["veadr"].append(data)
 
         # viadr (Variable Internal Auxiliary Data Record)
         elif grh["record_class"] == 7:
             template, scaled_template, sfactor = self._read_xml_viadr(
                 grh["record_subclass"])
-            viadr_element = np.fromfile(self.fid,
-                                        dtype=template,
-                                        count=record_count)
+            viadr_element = np.fromfile(
+                self.fid, dtype=template, count=record_count)
 
             viadr_element_sc = self._scaling(viadr_element, scaled_template,
                                              sfactor)
 
             # store viadr_grid separately
             if grh["record_subclass"] == 8:
                 self.aux["viadr_grid"].append(viadr_element)
@@ -464,21 +469,19 @@
             else:
                 self.aux["viadr"].append(viadr_element)
                 self.aux["viadr_scaled"].append(viadr_element_sc)
 
         # mdr (Measurement Data Record)
         elif grh["record_class"] == 8:
             if grh["instrument_group"] == 13:
-                self.dummy_mdr = np.fromfile(self.fid,
-                                             dtype=self.mdr_template,
-                                             count=record_count)
+                self.dummy_mdr = np.fromfile(
+                    self.fid, dtype=self.mdr_template, count=record_count)
             else:
-                self.mdr = np.fromfile(self.fid,
-                                       dtype=self.mdr_template,
-                                       count=record_count)
+                self.mdr = np.fromfile(
+                    self.fid, dtype=self.mdr_template, count=record_count)
                 self.mdr_counter = record_count
         else:
             raise RuntimeError("Record class not found.")
 
     def _scaling(self, unscaled_mdr, scaled_template, sfactor):
         """
         Scale the MDR.
@@ -577,16 +580,16 @@
             if child.tag == "delimiter":
                 continue
 
             child_items = dict(child.items())
             name = child_items.pop("name")
 
             # check if the item is of type longtime
-            longtime_flag = ("type" in child_items
-                             and "longtime" in child_items["type"])
+            longtime_flag = ("type" in child_items and
+                             "longtime" in child_items["type"])
 
             # append the length if it isn"t the special case of type longtime
             try:
                 var_len = child_items.pop("length")
                 if not longtime_flag:
                     length.append(np.int64(var_len))
             except KeyError:
@@ -671,17 +674,17 @@
             if child.tag == "delimiter":
                 continue
 
             child_items = dict(child.items())
             name = child_items.pop("name")
 
             # check if the item is of type bitfield
-            bitfield_flag = ("type" in child_items
-                             and ("bitfield" in child_items["type"]
-                                  or "time" in child_items["type"]))
+            bitfield_flag = ("type" in child_items and
+                             ("bitfield" in child_items["type"] or
+                              "time" in child_items["type"]))
 
             # append the length if it isn"t the special case of type
             # bitfield or time
             try:
                 var_len = child_items.pop("length")
                 if not bitfield_flag:
                     length.append(np.int64(var_len))
@@ -691,16 +694,16 @@
             data[name] = child_items
 
             if child.tag == "array":
                 for arr in child.iterdescendants():
                     arr_items = dict(arr.items())
 
                     # check if the type is bitfield
-                    bitfield_flag = ("type" in arr_items
-                                     and "bitfield" in arr_items["type"])
+                    bitfield_flag = ("type" in arr_items and
+                                     "bitfield" in arr_items["type"])
 
                     if bitfield_flag:
                         data[name].update(arr_items)
                         break
                     else:
                         if arr.tag == "field":
                             data[name].update(arr_items)
@@ -775,15 +778,14 @@
         Metadata.
 
     Returns
     -------
     data : dict of numpy.ndarray
         Converted dataset.
     """
-
     for var_name in skip_fields:
         data.pop(var_name, None)
 
     for var_name, (new_name, new_dtype, valid_range,
                    nan_val) in gen_fields_lut.items():
         if new_dtype is None:
             data[new_name] = np.ma.array(data.pop(var_name))
@@ -897,96 +899,112 @@
 
 
 def read_eps_l1b(filename,
                  generic=False,
                  to_xarray=False,
                  full=True,
                  unsafe=False,
-                 scale_mdr=True):
+                 scale_mdr=True,
+                 ignore_noise_ool=False):
     """
     Level 1b reader and data preparation.
 
     Parameters
     ----------
     filename : str
         ASCAT Level 1b file name in EPS Native format.
     generic : bool, optional
         "True" reading and converting into generic format or
         "False" reading original field names (default: False).
     to_xarray : bool, optional
         "True" return data as xarray.Dataset
         "False" return data as numpy.ndarray (default: False).
+    full : bool, optional
+        Read full file content (True) or just Main Product Header
+        Record (MPHR) and Main Data Record (MDR) (False). Default: True
+    unsafe : bool, optional
+        If True it is (unsafely) assumed that MDR are continuously
+        stacked until the end of file. Makes reading a lot faster.
+        Default: False
+    scale_mdr : bool, optional
+        Compute scaled MDR (True) or not (False). Default: True
+    ignore_noise_ool : bool, optional
+        Ignore noise out of limit flag (default: False).
 
     Returns
     -------
     ds : xarray.Dataset, dict of xarray.Dataset
         ASCAT Level 1b data.
     """
-    eps_file = read_eps(filename,
-                        full=full,
-                        unsafe=unsafe,
-                        scale_mdr=scale_mdr)
+    eps_file = read_eps(
+        filename, full=full, unsafe=unsafe, scale_mdr=scale_mdr)
 
     ptype = eps_file.mphr["PRODUCT_TYPE"]
     fmv = int(eps_file.mphr["FORMAT_MAJOR_VERSION"])
 
     if ptype == "SZF":
 
         if fmv == 12:
-            data, metadata = read_szf_fmv_12(eps_file)
+            data, metadata = read_szf_fmv_12(eps_file, ignore_noise_ool)
 
             skip_fields = [
                 "utc_localisation-days", "utc_localisation-milliseconds",
                 "degraded_inst_mdr", "degraded_proc_mdr", "flagfield_rf1",
                 "flagfield_rf2", "flagfield_pl", "flagfield_gen1",
                 "flagfield_gen2"
             ]
 
             gen_fields_lut = {
                 "inc_angle_full": ("inc", np.float32, (0, 90), float32_nan),
                 "azi_angle_full": ("azi", np.float32, (0, 360), float32_nan),
-                "sigma0_full": ("sig", np.float32, (-35, 35), float32_nan),
+                "sigma0_full": ("sig", np.float32, (-50, 50), float32_nan),
                 "sat_track_azi":
-                ("sat_track_azi", np.float32, (0, 360), float32_nan),
+                    ("sat_track_azi", np.float32, (0, 360), float32_nan),
                 "beam_number": ("beam_number", np.int8, (1, 6), int8_nan),
                 "swath_indicator":
-                ("swath_indicator", np.int8, (0, 1), int8_nan),
+                    ("swath_indicator", np.int8, (0, 1), int8_nan),
                 "land_frac": ("land_frac", np.float32, (0, 1), float32_nan),
                 "f_usable": ("f_usable", np.int8, (0, 2), int8_nan),
                 "as_des_pass": ("as_des_pass", np.uint8, (0, 1), uint8_nan),
                 "time": ("time", None, (np.datetime64("1900-01-01"),
                                         np.datetime64("2100-01-01")), 0),
                 "lon": ("lon", np.float32, (-180, 180), float32_nan),
-                "lat": ("lat", np.float32, (-90, 90), float32_nan)
+                "lat": ("lat", np.float32, (-90, 90), float32_nan),
+                "flagfield":
+                    ("flagfield", None, (0, uint32_nan - 1), uint32_nan),
             }
 
         elif fmv == 13:
-            data, metadata = read_szf_fmv_13(eps_file)
+            data, metadata = read_szf_fmv_13(eps_file, ignore_noise_ool)
 
             skip_fields = [
-                "utc_localisation-days", "utc_localisation-milliseconds",
-                "degraded_inst_mdr", "degraded_proc_mdr", "flagfield"
+                "utc_localisation-days",
+                "utc_localisation-milliseconds",
+                "degraded_inst_mdr",
+                "degraded_proc_mdr",
             ]
 
             gen_fields_lut = {
                 "inc_angle_full": ("inc", np.float32, (0, 90), float32_nan),
                 "azi_angle_full": ("azi", np.float32, (0, 360), float32_nan),
-                "sigma0_full": ("sig", np.float32, (-35, 35), float32_nan),
+                "sigma0_full": ("sig", np.float32, (-50, 50), float32_nan),
                 "sat_track_azi":
-                ("sat_track_azi", np.float32, (0, 360), float32_nan),
+                    ("sat_track_azi", np.float32, (0, 360), float32_nan),
                 "beam_number": ("beam_number", np.int8, (1, 6), int8_nan),
                 "swath_indicator":
-                ("swath_indicator", np.int8, (0, 1), int8_nan),
+                    ("swath_indicator", np.int8, (0, 1), int8_nan),
                 # "land_frac": ("land_frac", np.float32, (0, 1), float32_nan),
                 "f_usable": ("f_usable", np.int8, (0, 2), int8_nan),
                 "as_des_pass": ("as_des_pass", np.uint8, (0, 1), uint8_nan),
                 "time": ("time", None, (np.datetime64("1900-01-01"),
                                         np.datetime64("2100-01-01")), 0),
                 "lon": ("lon", np.float32, (-180, 180), float32_nan),
-                "lat": ("lat", np.float32, (-90, 90), float32_nan)
+                "lat": ("lat", np.float32, (-90, 90), float32_nan),
+                "flagfield":
+                    ("flagfield", None, (0, uint32_nan - 1), uint32_nan),
             }
         else:
             raise RuntimeError("L1b SZF format version not supported.")
 
         rename_coords = {"longitude_full": "lon", "latitude_full": "lat"}
 
         for k, v in rename_coords.items():
@@ -1050,16 +1068,16 @@
                     elif len(data[var_name][subset].shape) > 1:
                         dtype.append(
                             (var_name, data[var_name][subset].dtype.str,
                              data[var_name][subset].shape[1:]))
 
                     fill_values[var_name] = data[var_name].fill_value
 
-                ds[beam] = np.ma.empty(data["time"][subset].size,
-                                       dtype=np.dtype(dtype))
+                ds[beam] = np.ma.empty(
+                    data["time"][subset].size, dtype=np.dtype(dtype))
 
                 for var_name, v in data.items():
                     if var_name == "beam_number" and generic:
                         continue
                     ds[beam][var_name] = v[subset]
                     ds[beam][var_name].set_fill_value(fill_values[var_name])
 
@@ -1318,16 +1336,16 @@
 
     for f, nan_val in fields:
         data[f] = raw_data[f.upper()].reshape(n_records, 3)
         valid = raw_unscaled[f.upper()].reshape(n_records, 3) != nan_val
         data[f][~valid] = nan_val
 
     # modify longitudes from (0, 360) to (-180,180)
-    mask = np.logical_and(data["longitude"] != long_nan,
-                          data["longitude"] > 180)
+    mask = np.logical_and(data["longitude"] != long_nan, data["longitude"]
+                          > 180)
     data["longitude"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     mask = (data["azi_angle_trip"] != int_nan) & (data["azi_angle_trip"] < 0)
     data["azi_angle_trip"][mask] += 360
 
     data["node_num"] = np.tile((np.arange(n_node_per_line) + 1),
@@ -1404,16 +1422,16 @@
 
     for f, nan_val in fields:
         data[f] = raw_data[f.upper()].reshape(n_records, 3)
         valid = raw_unscaled[f.upper()].reshape(n_records, 3) != nan_val
         data[f][~valid] = nan_val
 
     # modify longitudes from (0, 360) to (-180,180)
-    mask = np.logical_and(data["longitude"] != long_nan,
-                          data["longitude"] > 180)
+    mask = np.logical_and(data["longitude"] != long_nan, data["longitude"]
+                          > 180)
     data["longitude"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     mask = (data["azi_angle_trip"] != int_nan) & (data["azi_angle_trip"] < 0)
     data["azi_angle_trip"][mask] += 360
 
     data["node_num"] = np.tile((np.arange(n_node_per_line) + 1),
@@ -1424,15 +1442,15 @@
     data["as_des_pass"] = (data["sat_track_azi"] < 270).astype(np.uint8)
 
     data["swath_indicator"] = data.pop("swath indicator")
 
     return data, metadata
 
 
-def read_szf_fmv_12(eps_file):
+def read_szf_fmv_12(eps_file, ignore_noise_ool=False):
     """
     Read SZF format version 12.
 
     beam_num
     - 1 Left Fore Antenna
     - 2 Left Mid Antenna
     - 3 Left Aft Antenna
@@ -1448,14 +1466,16 @@
     - 0 Left
     - 1 Right
 
     Parameters
     ----------
     eps_file : EPSProduct object
         EPS Product object.
+    ignore_noise_ool : bool, optional
+        Ignore noise out of limit flag (default: False).
 
     Returns
     -------
     data : numpy.ndarray
         SZF data.
     """
     data = {}
@@ -1515,16 +1535,16 @@
     for f in fields:
         if eps_file.mdr_sfactor[f.upper()] == 1:
             data[f] = eps_file.mdr[f.upper()].flatten()[idx_nodes]
         else:
             data[f] = (eps_file.mdr[f.upper()].flatten() * 1. /
                        eps_file.mdr_sfactor[f.upper()])[idx_nodes]
 
-    data["swath_indicator"] = (data["beam_number"].flatten() > 3).astype(
-        np.uint8)
+    data["swath_indicator"] = (data["beam_number"].flatten()
+                               > 3).astype(np.uint8)
     data["as_des_pass"] = (data["sat_track_azi"] < 270).astype(np.uint8)
 
     fields = [("longitude_full", long_nan), ("latitude_full", long_nan),
               ("sigma0_full", long_nan), ("inc_angle_full", uint_nan),
               ("azi_angle_full", int_nan), ("land_frac", uint_nan),
               ("flagfield_gen2", int8_nan)]
 
@@ -1543,15 +1563,18 @@
     data["longitude_full"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     idx = (data["azi_angle_full"] != int_nan) & (data["azi_angle_full"] < 0)
     data["azi_angle_full"][idx] += 360
 
     # set flags
-    data["f_usable"] = set_flags(data)
+    data["f_usable"] = set_flags(data, ignore_noise_ool)
+
+    # create flagflield
+    data["flagfield"] = gen_flagfield(data)
 
     return data, metadata
 
 
 def read_smx_fmv_12(eps_file):
     """
     Read SMO/SMR format version 12.
@@ -1624,16 +1647,16 @@
         data[f][~valid] = new_nan_val
 
     # sat_track_azi (uint)
     data["as_des_pass"] = \
         np.array(raw_data["SAT_TRACK_AZI"].flatten()[idx_nodes] < 270)
 
     # modify longitudes from [0,360] to [-180,180]
-    mask = np.logical_and(data["longitude"] != long_nan,
-                          data["longitude"] > 180)
+    mask = np.logical_and(data["longitude"] != long_nan, data["longitude"]
+                          > 180)
     data["longitude"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     mask = (data["azi_angle_trip"] != int_nan) & (data["azi_angle_trip"] < 0)
     data["azi_angle_trip"][mask] += 360
 
     fields = ["param_db_version", "warp_nrt_version"]
@@ -1645,15 +1668,15 @@
     data["node_num"] = np.tile((np.arange(n_node_per_line) + 1), n_lines)
 
     data["line_num"] = idx_nodes
 
     return data, metadata
 
 
-def read_szf_fmv_13(eps_file):
+def read_szf_fmv_13(eps_file, ignore_noise_ool=False):
     """
     Read SZF format version 13.
 
     beam_num
     - 1 Left Fore Antenna
     - 2 Left Mid Antenna
     - 3 Left Aft Antenna
@@ -1669,14 +1692,16 @@
     - 0 Left
     - 1 Right
 
     Parameters
     ----------
     eps_file : EPSProduct object
         EPS Product object.
+    ignore_noise_ool : bool, optional
+        Ignore noise out of limit flag (default: False).
 
     Returns
     -------
     data : numpy.ndarray
         SZF data.
     """
     data = {}
@@ -1741,16 +1766,16 @@
     for f in fields:
         if eps_file.mdr_sfactor[f.upper()] == 1:
             data[f] = eps_file.mdr[f.upper()].flatten()[idx_nodes]
         else:
             data[f] = (eps_file.mdr[f.upper()].flatten() * 1. /
                        eps_file.mdr_sfactor[f.upper()])[idx_nodes]
 
-    data["swath_indicator"] = (data["beam_number"].flatten() > 3).astype(
-        np.uint8)
+    data["swath_indicator"] = (data["beam_number"].flatten()
+                               > 3).astype(np.uint8)
     data["as_des_pass"] = (data["sat_track_azi"] < 270).astype(np.uint8)
 
     fields = [("longitude_full", long_nan), ("latitude_full", long_nan),
               ("sigma0_full", long_nan), ("inc_angle_full", uint_nan),
               ("azi_angle_full", int_nan), ("flagfield", int_nan)]
 
     for f, nan_val in fields:
@@ -1768,15 +1793,15 @@
     data["longitude_full"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     idx = (data["azi_angle_full"] != int_nan) & (data["azi_angle_full"] < 0)
     data["azi_angle_full"][idx] += 360
 
     # set flags
-    data["f_usable"] = set_flags_fmv13(data["flagfield"])
+    data["f_usable"] = set_flags_fmv13(data["flagfield"], ignore_noise_ool)
 
     return data, metadata
 
 
 def read_szx_fmv_13(eps_file):
     """
     Read SZO/SZR format version
@@ -1841,16 +1866,16 @@
 
     for f, nan_val in fields:
         data[f] = raw_data[f.upper()].reshape(n_records, 3)
         valid = raw_unscaled[f.upper()].reshape(n_records, 3) != nan_val
         data[f][~valid] = nan_val
 
     # modify longitudes from (0, 360) to (-180,180)
-    mask = np.logical_and(data["longitude"] != long_nan,
-                          data["longitude"] > 180)
+    mask = np.logical_and(data["longitude"] != long_nan, data["longitude"]
+                          > 180)
     data["longitude"][mask] += -360.
 
     # modify azimuth from (-180, 180) to (0, 360)
     mask = (data["azi_angle_trip"] != int_nan) & (data["azi_angle_trip"] < 0)
     data["azi_angle_trip"][mask] += 360
 
     data["node_num"] = np.tile((np.arange(n_node_per_line) + 1),
@@ -1883,15 +1908,15 @@
     jd : float
         Julian date.
     """
     offset = days + (milliseconds / 1000.) / (24. * 60. * 60.)
     return julian_epoch + offset
 
 
-def set_flags(data):
+def set_flags(data, ignore_noise_ool=False):
     """
     Compute summary flag for each measurement with a value of 0, 1 or 2
     indicating nominal, slightly degraded or severely degraded data.
 
     The format of ASCAT products is defined by
     "EPS programme generic product format specification" (EPS.GGS.SPE.96167)
     and "ASCAT level 1 product format specification" (EPS.MIS.SPE.97233).
@@ -1956,37 +1981,127 @@
         "flagfield_rf1": np.array([1, 1, 2, 1, 2, 0, 0, 0]),
         "flagfield_rf2": np.array([2, 2, 0, 0, 0, 0, 0, 0]),
         "flagfield_pl": np.array([2, 2, 2, 2, 0, 0, 0, 0]),
         "flagfield_gen1": np.array([0, 2, 0, 0, 0, 0, 0, 0]),
         "flagfield_gen2": np.array([1, 0, 2, 0, 0, 0, 0, 0])
     }
 
+    if ignore_noise_ool:
+        # remove "noise out of limits" as red flag
+        flag_status_bit["flagfield_rf"] = np.array([2, 0, 0, 0, 0, 0, 0, 0])
+
     f_usable = np.zeros(data["flagfield_rf1"].size, dtype=np.uint8)
 
     for flagfield, bitmask in flag_status_bit.items():
         subset = np.nonzero(data[flagfield])[0]
 
         if subset.size > 0:
             unpacked_bits = np.fliplr(
                 np.unpackbits(data[flagfield][subset]).reshape(-1,
                                                                8).astype(bool))
 
-            flag = np.ma.array(np.tile(bitmask,
-                                       unpacked_bits.shape[0]).reshape(-1, 8),
-                               mask=~unpacked_bits,
-                               fill_value=0)
-
-            f_usable[subset] = np.max(np.vstack(
-                (f_usable[subset], flag.filled().max(axis=1))),
-                                      axis=0)
+            flag = np.ma.array(
+                np.tile(bitmask, unpacked_bits.shape[0]).reshape(-1, 8),
+                mask=~unpacked_bits,
+                fill_value=0)
+
+            f_usable[subset] = np.max(
+                np.vstack((f_usable[subset], flag.filled().max(axis=1))),
+                axis=0)
 
     return f_usable
 
 
-def set_flags_fmv13(flagfield):
+def gen_flagfield(data):
+    """
+    The new flagfield collects the fields previously split across the RF1 /
+    RF2 / PL / GEN1 / GEN2 flagfields. Its structure is described in the PFS,
+    Tab. 14: Structure of FLAGFIELD.
+
+    The old RF1 flagfield (related to the quality of the raw echo correction
+    functions) contains the following bit flags and maps to the v11 flagfield
+    as follows :
+
+    RF1 Bit  Flag      v11 Bit  Description
+    0        F_NOISE   0        Noise measurement missing, interpolated value used
+    1        F_PG      1        Degraded power gain product
+    2        V_PG      2        Very degraded power gain product
+    3        F_FILTER  3        Degraded filter shape
+    4        V_FILTER  4        Very degraded filter shape
+
+    RF2 Bit  Flag         v11 Bit  Description
+    0        F_PGP        5        Estimated power gain product outside limits
+    1        F_NP         6        Measured noise outside limits
+    2        F_PGP_DROP   7        Small drop in power gain product detected
+
+    PL Bit   Flag          v11 Bit  Description
+    0        F_ORBIT       n/a      Orbit height used for the NRCS normalisation is outside limits
+    1        F_ATTITUDE    8        No yaw steering
+    2        F_OMEGA       9        Unexpected instrument configuration
+    3        F_MAN         10       Satellite manoeuvre
+    4        F_OSV         11       Input orbit prediction file missing, OSV taken from L0 header
+
+    GEN1 Bit  Flag           v11 Bit  Description
+    0         F_E_TEL_PRES   12       Instrument or platform HKTM missing
+    1         F_E_TEL_IR     13       Instrument or platform HKTM out of limits
+    2         F_CE           n/a
+    3         V_CE           n/a
+    4         F_OA           n/a      Quality of satellite orbit and attitute
+    5         F_TEL          n/a
+    6         F_REF          14
+
+    GEN2 Bit  Flag     v11 Bit  Description
+    0         F_S_A    15       Potential interference from solar array
+    1         F_LAND   16       Measurement over land in the generation of NCRS value
+    2         F_GEO    17       Geolocation algorithm failed
+    3         F_SIGN   18       The NRCS value is negative
+    """
+    flag_table = {
+        "rf1": {
+            0: 0,
+            1: 1,
+            2: 2,
+            3: 3,
+            4: 4
+        },
+        "rf2": {
+            0: 5,
+            1: 6,
+            2: 7
+        },
+        "pl": {
+            1: 8,
+            2: 9,
+            3: 10,
+            4: 11
+        },
+        "gen1": {
+            0: 12,
+            1: 13,
+            6: 14
+        },
+        "gen2": {
+            0: 15,
+            1: 16,
+            2: 17,
+            3: 18
+        }
+    }
+
+    flagfield = np.zeros(data["flagfield_rf1"].size, dtype=np.uint32)
+
+    for flag, table in flag_table.items():
+        for sbit, tbit in table.items():
+            pos = np.nonzero(get_bit(data[f"flagfield_{flag}"], sbit+1))[0]
+            flagfield[pos] = set_bit(flagfield[pos], tbit+1)
+
+    return flagfield
+
+
+def set_flags_fmv13(flagfield, ignore_noise_ool=False):
     """
     Compute summary flag for each measurement with a value of 0, 1 or 2
     indicating nominal, slightly degraded or severely degraded data.
 
     The format of ASCAT products is defined by
     "EPS programme generic product format specification" (EPS.GGS.SPE.96167)
     and "ASCAT level 1 product format specification" (EPS.MIS.SPE.97233).
@@ -2037,14 +2152,18 @@
         Flag indicating nominal (0), minor degraded (1) or major degraded (2).
     """
     # 0..ok, 1..minor/amber alert, 2..major/red alert
     bitmask = np.array(
         [1, 1, 2, 1, 2, 2, 2, 1, 2, 2, 2, 0, 1, 2, 0, 1, 0, 2, 0, 0],
         dtype=np.int8)
 
+    if ignore_noise_ool:
+        # remove "noise out of limits" as red flag
+        bitmask[6] = 0
+
     # create look-up table
     def unpack(b):
         return np.clip(np.arange(2**bitmask.size) & 2**b, 0, 1) * bitmask[b]
 
     lut = np.max(list(map(unpack, list(range(bitmask.size)))), axis=0)
     f_usable = lut[flagfield].astype(np.int8)
```

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/ccsds.xml` & `ascat-2.4.1/src/ascat/read_native/formats/ccsds.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps.dtd` & `ascat-2.4.1/src/ascat/read_native/formats/eps.dtd`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps.xsl` & `ascat-2.4.1/src/ascat/read_native/formats/eps.xsl`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml` & `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/hdf5.py` & `ascat-2.4.1/src/ascat/read_native/hdf5.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/nc.py` & `ascat-2.4.1/src/ascat/read_native/nc.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/ragged_array_ts.py` & `ascat-2.4.1/src/ascat/read_native/ragged_array_ts.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/read_native/xarray_io.py` & `ascat-2.4.1/src/ascat/read_native/xarray_io.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/regrid/interface.py` & `ascat-2.4.1/src/ascat/regrid/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/regrid/regrid.py` & `ascat-2.4.1/src/ascat/regrid/regrid.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/src/ascat/utils.py` & `ascat-2.4.1/src/ascat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,57 @@
 from gzip import GzipFile
 from tempfile import NamedTemporaryFile
 
 import numpy as np
 import xarray as xr
 
 
+def get_bit(a, bit_pos):
+    """
+    Returns 1 or 0 if bit is set or not.
+
+    Parameters
+    ----------
+    a : int or numpy.ndarray
+      Input array.
+    bit_pos : int
+      Bit position. First bit position is right.
+
+    Returns
+    -------
+    b : numpy.ndarray
+      1 if bit is set and 0 if not.
+    """
+    return np.clip(np.bitwise_and(a, 2**(bit_pos - 1)), 0, 1)
+
+
+def set_bit(a, bit_pos, value=1):
+    """
+    Set bit at given position.
+
+    Parameters
+    ----------
+    a : int or numpy.ndarray
+      Input array.
+    bit_pos : int
+      Bit position. First bit starts right.
+    value : 1 or 0, optional
+      Set bit either to 1 or 0 (default: 1).
+
+    Returns
+    -------
+    a : numpy.ndarray
+      Modified input array with bit=value.
+    """
+    if value == 1:
+        return np.bitwise_or(np.atleast_1d(a), 2**(bit_pos - 1))
+    else:
+        return np.bitwise_and(np.atleast_1d(a), ~(2**(bit_pos - 1)))
+
+
 def daterange(start_date, end_date):
     """
     Generator for daily datetimes.
 
     Parameters
     ----------
     start_date : datetime
@@ -244,16 +287,16 @@
                 ds[key] = None
             else:
                 if isinstance(ds[key], xr.Dataset):
                     ds[key] = ds[key].sel(obs=np.nonzero(subset.values)[0])
                 elif isinstance(ds[key], np.ndarray):
                     ds[key] = ds[key][subset]
     else:
-        subset = np.where((ds['time'] > np.datetime64(toi[0])) &
-                          (ds['time'] < np.datetime64(toi[1])))[0]
+        subset = np.where((ds['time'] > np.datetime64(toi[0]))
+                          & (ds['time'] < np.datetime64(toi[1])))[0]
         if subset.size == 0:
             ds = None
         else:
             if isinstance(ds, xr.Dataset):
                 ds = ds.sel(obs=np.nonzero(subset.values)[0])
             elif isinstance(ds, np.ndarray):
                 ds = ds[subset]
@@ -275,26 +318,28 @@
     Returns
     -------
     ds : xarray.Dataset
         Filtered dataset.
     """
     if isinstance(ds, dict):
         for key in ds.keys():
-            subset = np.where((ds[key]['lat'] > roi[0]) & (ds[key]['lat'] < roi[2]) &
-                      (ds[key]['lon'] > roi[1]) & (ds[key]['lon'] < roi[3]))[0]
+            subset = np.where((ds[key]['lat'] > roi[0])
+                              & (ds[key]['lat'] < roi[2])
+                              & (ds[key]['lon'] > roi[1])
+                              & (ds[key]['lon'] < roi[3]))[0]
             if subset.size == 0:
                 ds[key] = None
             else:
                 if isinstance(ds[key], xr.Dataset):
                     ds[key] = ds[key].sel(obs=np.nonzero(subset.values)[0])
                 elif isinstance(ds[key], np.ndarray):
                     ds[key] = ds[key][subset]
     else:
-        subset = np.where((ds['lat'] > roi[0]) & (ds['lat'] < roi[2]) &
-                  (ds['lon'] > roi[1]) & (ds['lon'] < roi[3]))[0]
+        subset = np.where((ds['lat'] > roi[0]) & (ds['lat'] < roi[2])
+                          & (ds['lon'] > roi[1]) & (ds['lon'] < roi[3]))[0]
         if subset.size == 0:
             ds = None
         else:
             if isinstance(ds, xr.Dataset):
                 ds = ds.sel(obs=np.nonzero(subset.values)[0])
             elif isinstance(ds, np.ndarray):
                 ds = ds[subset]
```

### Comparing `ascat-2.4.0/src/ascat.egg-info/PKG-INFO` & `ascat-2.4.1/src/ascat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.4.0
+Version: 2.4.1
 Summary: Read and visualize for data from the Advanced Scatterometer (ASCAT)
 Home-page: https://tuwien.at/mg/geo/rs
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, https://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.4.0/src/ascat.egg-info/SOURCES.txt` & `ascat-2.4.1/src/ascat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/get_path.py` & `ascat-2.4.1/tests/get_path.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/skip_test_ragged_array.py` & `ascat-2.4.1/tests/skip_test_ragged_array.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_cgls.py` & `ascat-2.4.1/tests/test_cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_download.py` & `ascat-2.4.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_file_handling.py` & `ascat-2.4.1/tests/test_file_handling.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_h_saf.py` & `ascat-2.4.1/tests/test_h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_level1.py` & `ascat-2.4.1/tests/test_level1.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tests/test_level2.py` & `ascat-2.4.1/tests/test_level2.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.0/tox.ini` & `ascat-2.4.1/tox.ini`

 * *Files identical despite different names*

