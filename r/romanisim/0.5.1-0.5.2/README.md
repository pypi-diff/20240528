# Comparing `tmp/romanisim-0.5.1.tar.gz` & `tmp/romanisim-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romanisim-0.5.1.tar", last modified: Fri May  3 14:25:23 2024, max compression
+gzip compressed data, was "romanisim-0.5.2.tar", last modified: Tue May 28 14:58:33 2024, max compression
```

## Comparing `romanisim-0.5.1.tar` & `romanisim-0.5.2.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.542558 romanisim-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 14:25:08.000000 romanisim-0.5.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.518558 romanisim-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-03 14:25:08.000000 romanisim-0.5.1/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-03 14:25:08.000000 romanisim-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-03 14:25:08.000000 romanisim-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 14:25:08.000000 romanisim-0.5.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-03 14:25:08.000000 romanisim-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-03 14:25:08.000000 romanisim-0.5.1/JenkinsfileRT_dev
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-03 14:25:08.000000 romanisim-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-03 14:25:23.542558 romanisim-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-03 14:25:08.000000 romanisim-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.522558 romanisim-0.5.1/docs/romanisim/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/apt.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/bandpass.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/catalog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/l1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/l2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/psf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/refs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/romanisim/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 14:25:08.000000 romanisim-0.5.1/docs/rtd_environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-03 14:25:08.000000 romanisim-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 14:25:08.000000 romanisim-0.5.1/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.530557 romanisim-0.5.1/romanisim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/apt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/cr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.530557 romanisim-0.5.1/romanisim/data/
--rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/data/Roman_effarea_20201130.csv
--rw-r--r--   0 runner    (1001) docker     (127)  3936671 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/data/gaia-270-66-2027-06-01.ecsv
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/nonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25518 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)  1213393 2024-05-03 14:25:22.000000 romanisim-0.5.1/romanisim/ramp_fit_casertano.c
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ramp_fit_casertano.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/romanisim/regtest/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/regtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/regtest/test_l1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11427 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/ris_make_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/romanisim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)    31953 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_ris_make_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-05-03 14:25:08.000000 romanisim-0.5.1/romanisim/wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.542558 romanisim-0.5.1/romanisim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:25:22.000000 romanisim-0.5.1/romanisim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 14:25:23.000000 romanisim-0.5.1/romanisim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:25:23.538558 romanisim-0.5.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romancal_make_all_l1s.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romancal_make_regtest_l1s.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2193 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-catalog
--rwxr-xr-x   0 runner    (1001) docker     (127)     5283 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-image
--rwxr-xr-x   0 runner    (1001) docker     (127)    10443 2024-05-03 14:25:08.000000 romanisim-0.5.1/scripts/romanisim-make-stack
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:25:23.542558 romanisim-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 14:25:08.000000 romanisim-0.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-03 14:25:08.000000 romanisim-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.321969 romanisim-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 14:58:19.000000 romanisim-0.5.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.301969 romanisim-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 14:58:19.000000 romanisim-0.5.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.301969 romanisim-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-28 14:58:19.000000 romanisim-0.5.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-28 14:58:19.000000 romanisim-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-28 14:58:19.000000 romanisim-0.5.2/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-28 14:58:19.000000 romanisim-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 14:58:19.000000 romanisim-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 14:58:19.000000 romanisim-0.5.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-28 14:58:19.000000 romanisim-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-28 14:58:19.000000 romanisim-0.5.2/JenkinsfileRT_dev
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 14:58:19.000000 romanisim-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-28 14:58:33.321969 romanisim-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-28 14:58:19.000000 romanisim-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.301969 romanisim-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.305969 romanisim-0.5.2/docs/romanisim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/apt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/bandpass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/catalog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/l1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/l2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/refs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/romanisim/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 14:58:19.000000 romanisim-0.5.2/docs/rtd_environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-28 14:58:19.000000 romanisim-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 14:58:19.000000 romanisim-0.5.2/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.309969 romanisim-0.5.2/romanisim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/apt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14833 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/cr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.313969 romanisim-0.5.2/romanisim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/data/Roman_effarea_20201130.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  3936671 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/data/gaia-270-66-2027-06-01.ecsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/nonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25518 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1213393 2024-05-28 14:58:32.000000 romanisim-0.5.2/romanisim/ramp_fit_casertano.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/ramp_fit_casertano.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.317969 romanisim-0.5.2/romanisim/regtest/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/regtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/regtest/test_l1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11427 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/ris_make_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.321969 romanisim-0.5.2/romanisim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_ris_make_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-28 14:58:19.000000 romanisim-0.5.2/romanisim/wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.321969 romanisim-0.5.2/romanisim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-28 14:58:33.000000 romanisim-0.5.2/romanisim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-28 14:58:33.000000 romanisim-0.5.2/romanisim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:58:33.000000 romanisim-0.5.2/romanisim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:58:32.000000 romanisim-0.5.2/romanisim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-28 14:58:33.000000 romanisim-0.5.2/romanisim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 14:58:33.000000 romanisim-0.5.2/romanisim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:58:33.321969 romanisim-0.5.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-28 14:58:19.000000 romanisim-0.5.2/scripts/romancal_make_all_l1s.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-28 14:58:19.000000 romanisim-0.5.2/scripts/romancal_make_regtest_l1s.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2193 2024-05-28 14:58:19.000000 romanisim-0.5.2/scripts/romanisim-make-catalog
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5283 2024-05-28 14:58:19.000000 romanisim-0.5.2/scripts/romanisim-make-image
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10443 2024-05-28 14:58:19.000000 romanisim-0.5.2/scripts/romanisim-make-stack
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:58:33.321969 romanisim-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-28 14:58:19.000000 romanisim-0.5.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-28 14:58:19.000000 romanisim-0.5.2/tox.ini
```

### Comparing `romanisim-0.5.1/.github/workflows/build.yml` & `romanisim-0.5.2/.github/workflows/build.yml`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,21 @@
   pull_request:
   workflow_dispatch:
 
 jobs:
   build:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish.yml@v1
     with:
-      upload_to_pypi: ${{ (github.event_name == 'release') && (github.event.action == 'released') }}
+      env: |
+        FFTW_DIR: /opt/homebrew/opt/fftw/lib/
       targets: |
         # Linux wheels
         - cp3*-manylinux_x86_64
         # MacOS wheels
         - cp3*-macosx_x86_64
         # Until we have arm64 runners, we can't automatically test arm64 wheels
         - cp3*-macosx_arm64
       sdist: true
+      test_command: python -c "from romanisim import ramp_fit_casertano"
+      upload_to_pypi: ${{ (github.event_name == 'release') && (github.event.action == 'released') }}
     secrets:
       pypi_token: ${{ secrets.PYPI_PASSWORD_STSCI_MAINTAINER }}
```

### Comparing `romanisim-0.5.1/.github/workflows/ci.yml` & `romanisim-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/.github/workflows/ci_cron.yml` & `romanisim-0.5.2/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/.gitignore` & `romanisim-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/.readthedocs.yaml` & `romanisim-0.5.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/CODE_OF_CONDUCT.md` & `romanisim-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/JenkinsfileRT_dev` & `romanisim-0.5.2/JenkinsfileRT_dev`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/LICENSE` & `romanisim-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/PKG-INFO` & `romanisim-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.5.1
+Version: 0.5.2
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `romanisim-0.5.1/README.md` & `romanisim-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/Makefile` & `romanisim-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/conf.py` & `romanisim-0.5.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,14 @@
 html_theme_path = [stsci_rtd_theme.get_html_theme_path()]
 html_domain_indices = True
 html_sidebars = {"**": ["globaltoc.html", "relations.html", "searchbox.html"]}
 html_use_index = True
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/',
-               (None, 'http://data.astropy.org/intersphinx/python3.inv')),
+               (None, 'https://data.astropy.org/intersphinx/python3.inv')),
     'astropy': ('https://docs.astropy.org/en/stable/', None),
     'galsim': ('https://galsim-developers.github.io/GalSim/_build/html/', None),
     'coord': ('https://lsstdesc.org/Coord/_build/html/', None),
 }
 
 nitpicky = True
```

### Comparing `romanisim-0.5.1/docs/index.rst` & `romanisim-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/apt.rst` & `romanisim-0.5.2/docs/romanisim/apt.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/bandpass.rst` & `romanisim-0.5.2/docs/romanisim/bandpass.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/catalog.rst` & `romanisim-0.5.2/docs/romanisim/catalog.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/image.rst` & `romanisim-0.5.2/docs/romanisim/image.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/install.rst` & `romanisim-0.5.2/docs/romanisim/install.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/l1.rst` & `romanisim-0.5.2/docs/romanisim/l1.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/l2.rst` & `romanisim-0.5.2/docs/romanisim/l2.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/overview.rst` & `romanisim-0.5.2/docs/romanisim/overview.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/parameters.rst` & `romanisim-0.5.2/docs/romanisim/parameters.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/psf.rst` & `romanisim-0.5.2/docs/romanisim/psf.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/refs.rst` & `romanisim-0.5.2/docs/romanisim/refs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/running.rst` & `romanisim-0.5.2/docs/romanisim/running.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/docs/romanisim/wcs.rst` & `romanisim-0.5.2/docs/romanisim/wcs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/pyproject.toml` & `romanisim-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -125,7 +125,10 @@
     "if __name__ == \"__main__\":",
 ]
 
 [tool.ruff]
 extend-ignore = [
     "E501",
 ]
+
+[tool.cibuildwheel.macos]
+before-build = "brew install eigen fftw"
```

### Comparing `romanisim-0.5.1/requirements-dev.txt` & `romanisim-0.5.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/__init__.py` & `romanisim-0.5.2/romanisim/__init__.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/apt.py` & `romanisim-0.5.2/romanisim/apt.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/bandpass.py` & `romanisim-0.5.2/romanisim/bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/catalog.py` & `romanisim-0.5.2/romanisim/catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/cr.py` & `romanisim-0.5.2/romanisim/cr.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/data/Roman_effarea_20201130.csv` & `romanisim-0.5.2/romanisim/data/Roman_effarea_20201130.csv`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/data/gaia-270-66-2027-06-01.ecsv` & `romanisim-0.5.2/romanisim/data/gaia-270-66-2027-06-01.ecsv`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/gaia.py` & `romanisim-0.5.2/romanisim/gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/image.py` & `romanisim-0.5.2/romanisim/image.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/l1.py` & `romanisim-0.5.2/romanisim/l1.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/nonlinearity.py` & `romanisim-0.5.2/romanisim/nonlinearity.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/parameters.py` & `romanisim-0.5.2/romanisim/parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,31 @@
                 'vparity': -1,
                 'v3yangle': -60.0,
                 # I don't know what vparity and v3yangle should really be,
                 # but they are always -1 and -60 in existing files.
                 },
     'aperture': {'name': 'WFI_CEN',
                  'position_angle': 0
+                 },
+}
+
+# Default metadata for level 3 mosaics
+default_mosaic_parameters_dictionary = {
+    'basic': {'time_mean_mjd': Time('2026-01-01T00:00:00').mjd,
+              'optical_element': 'F184',
+              },
+    'wcsinfo': {'ra_ref': 270.0,
+                'dec_ref': 66.0,
+                'v2_ref': 0,
+                'v3_ref': 0,
+                'roll_ref': 0,
+                'vparity': -1,
+                'v3yangle': -60.0,
+                # I don't know what vparity and v3yangle should really be,
+                # but they are always -1 and -60 in existing files.
                 },
 }
 
 reference_data = {
     "dark": 0.01 * u.electron / u.s,
     "distortion": None,
     "flat": None,
```

### Comparing `romanisim-0.5.1/romanisim/persistence.py` & `romanisim-0.5.2/romanisim/persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/psf.py` & `romanisim-0.5.2/romanisim/psf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/ramp.py` & `romanisim-0.5.2/romanisim/ramp.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/ramp_fit_casertano.c` & `romanisim-0.5.2/romanisim/ramp_fit_casertano.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "romanisim.ramp_fit_casertano",
         "sources": [
             "romanisim/ramp_fit_casertano.pyx"
         ]
     },
     "module_name": "romanisim.ramp_fit_casertano"
@@ -1669,177 +1669,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1872,42 +1872,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18161,261 +18161,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18424,29 +18424,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18457,15 +18457,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18474,29 +18474,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18507,15 +18507,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18524,29 +18524,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18557,15 +18557,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18574,29 +18574,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18607,15 +18607,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18624,29 +18624,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18657,217 +18657,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18883,15 +18883,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18899,68 +18899,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18968,15 +18968,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18991,15 +18991,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19015,15 +19015,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19031,68 +19031,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19100,15 +19100,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19123,15 +19123,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19147,15 +19147,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19163,68 +19163,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19232,15 +19232,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19255,170 +19255,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22709,26 +22709,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-yunaauch/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-9q57nl6_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `romanisim-0.5.1/romanisim/ramp_fit_casertano.pyx` & `romanisim-0.5.2/romanisim/ramp_fit_casertano.pyx`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/ris_make_utils.py` & `romanisim-0.5.2/romanisim/ris_make_utils.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_bandpass.py` & `romanisim-0.5.2/romanisim/tests/test_bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_catalog.py` & `romanisim-0.5.2/romanisim/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_cr.py` & `romanisim-0.5.2/romanisim/tests/test_cr.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_gaia.py` & `romanisim-0.5.2/romanisim/tests/test_gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_image.py` & `romanisim-0.5.2/romanisim/tests/test_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 """
 
 import os
 import copy
 import numpy as np
 import galsim
 from galsim import roman
-from romanisim import image, parameters, catalog, psf, util, wcs, persistence, ramp, l1
+from romanisim import image, parameters, catalog, psf, util, wcs, persistence, ramp, l1, l3
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 from astropy.time import Time
 from astropy import table
 import asdf
 import webbpsf
 from astropy.modeling.functional_models import Sersic2D
 import pytest
 from metrics_logger.decorators import metrics_logger
 from romanisim import log
 from roman_datamodels.stnode import WfiScienceRaw, WfiImage
+import roman_datamodels.maker_utils as maker_utils
 import romanisim.bandpass
 
 
 def test_in_bounds():
     bounds = galsim.BoundsI(0, 1000, 0, 1000)
     xx = np.random.rand(1000) * 1000
     yy = np.random.rand(1000) * 1000
@@ -750,7 +751,99 @@
     if artifactdir is not None:
         af = asdf.AsdfFile()
         af.tree = {'originalimage': origimage,
                    'newimage': newimage,
                    'flux': flux,
                    'tij': tij}
         af.write_to(os.path.join(artifactdir, 'dms231.asdf'))
+
+
+@metrics_logger("DMS232")
+@pytest.mark.soctests
+def test_inject_sources_into_mosaic():
+    """Inject sources into a mosaic.
+    """
+
+    # Set constants and metadata
+    galsim.roman.n_pix = 200
+    rng_seed = 42
+    metadata = copy.deepcopy(parameters.default_mosaic_parameters_dictionary)
+    metadata['basic']['optical_element'] = 'F158'
+
+    # Create WCS
+    twcs = wcs.get_mosaic_wcs(metadata)
+
+    # Create initial Level 3 mosaic
+
+    # Create Four-quadrant pattern of gaussian noise, centered around one
+    # Each quadrant's gaussian noise scales like total exposure time
+    # (total files contributed to each quadrant)
+
+    # Create gaussian noise generators
+    g1 = galsim.GaussianDeviate(rng_seed, mean=1.0, sigma=0.01)
+    g2 = galsim.GaussianDeviate(rng_seed, mean=1.0, sigma=0.02)
+    g3 = galsim.GaussianDeviate(rng_seed, mean=1.0, sigma=0.05)
+    g4 = galsim.GaussianDeviate(rng_seed, mean=1.0, sigma=0.1)
+
+    # Create level 3 mosaic model
+    l3_mos = maker_utils.mk_level3_mosaic(shape=(galsim.roman.n_pix, galsim.roman.n_pix))
+
+    # Update metadata in the l3 model
+    for key in metadata.keys():
+        if key in l3_mos.meta:
+            l3_mos.meta[key].update(metadata[key])
+
+    # Populate the mosaic data array with gaussian noise from generators
+    g1.generate(l3_mos.data.value[0:100, 0:100])
+    g2.generate(l3_mos.data.value[0:100, 100:200])
+    g3.generate(l3_mos.data.value[100:200, 0:100])
+    g4.generate(l3_mos.data.value[100:200, 100:200])
+
+    # Define Poisson Noise of mosaic
+    l3_mos.var_poisson.value[0:100, 0:100] = 0.01**2
+    l3_mos.var_poisson.value[0:100, 100:200] = 0.02**2
+    l3_mos.var_poisson.value[100:200, 0:100] = 0.05**2
+    l3_mos.var_poisson.value[100:200, 100:200] = 0.1**2
+
+    # Create normalized psf source catalog (same source in each quadrant)
+    sc_dict = {"ra": 4 * [0.0], "dec": 4 * [0.0], "type": 4 * ["PSF"], "n": 4 * [-1.0],
+               "half_light_radius": 4 * [0.0], "pa": 4 * [0.0], "ba": 4 * [1.0], "F158": 4 * [1.0]}
+    sc_table = table.Table(sc_dict)
+
+    xpos, ypos = 50, 50
+    sc_table["ra"][0], sc_table["dec"][0] = (twcs._radec(xpos, ypos) * u.rad).to(u.deg).value
+    xpos, ypos = 50, 150
+    sc_table['ra'][1], sc_table['dec'][1] = (twcs._radec(xpos, ypos) * u.rad).to(u.deg).value
+    xpos, ypos = 150, 50
+    sc_table['ra'][2], sc_table['dec'][2] = (twcs._radec(xpos, ypos) * u.rad).to(u.deg).value
+    xpos, ypos = 150, 150
+    sc_table['ra'][3], sc_table['dec'][3] = (twcs._radec(xpos, ypos) * u.rad).to(u.deg).value
+
+    source_cat = catalog.table_to_catalog(sc_table, ["F158"])
+
+    # Copy original Mosaic before adding sources
+    l3_mos_orig = l3_mos.copy()
+
+    # Add source_cat objects to mosaic
+    l3.add_objects_to_l3(l3_mos, source_cat, seed=rng_seed)
+
+    # Ensure that every data pixel value has increased or
+    # remained the same with the new sources injected
+    assert np.all(l3_mos.data.value >= l3_mos_orig.data.value)
+
+    # Ensure that every pixel's poisson variance has increased or
+    # remained the same with the new sources injected
+    # Numpy isclose is needed to determine equality, due to float precision issues
+    close_mask = np.isclose(l3_mos.var_poisson.value, l3_mos_orig.var_poisson.value, rtol=1e-06)
+    assert np.all(l3_mos.var_poisson.value[~close_mask] > l3_mos_orig.var_poisson.value[~close_mask])
+
+    # Create log entry and artifacts
+    log.info('DMS232 successfully injected sources into a mosiac at points (50,50), (50,150), (150,50), (150,150).')
+
+    artifactdir = os.environ.get('TEST_ARTIFACT_DIR', None)
+    if artifactdir is not None:
+        af = asdf.AsdfFile()
+        af.tree = {'l3_mos': l3_mos,
+                   'l3_mos_orig': l3_mos_orig,
+                   'source_cat_table': sc_table,
+                   }
+        af.write_to(os.path.join(artifactdir, 'dms232.asdf'))
```

### Comparing `romanisim-0.5.1/romanisim/tests/test_l1.py` & `romanisim-0.5.2/romanisim/tests/test_l1.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_linear.py` & `romanisim-0.5.2/romanisim/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_persistence.py` & `romanisim-0.5.2/romanisim/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_psf.py` & `romanisim-0.5.2/romanisim/tests/test_psf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_ramp.py` & `romanisim-0.5.2/romanisim/tests/test_ramp.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_ris_make_utils.py` & `romanisim-0.5.2/romanisim/tests/test_ris_make_utils.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_util.py` & `romanisim-0.5.2/romanisim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/tests/test_wcs.py` & `romanisim-0.5.2/romanisim/tests/test_wcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from astropy import units as u
 from astropy.time import Time
 from romanisim import wcs, util, parameters
 import galsim
 import pytest
 
 import roman_datamodels
-try:
-    import roman_datamodels.maker_utils as maker_utils
-except ImportError:
-    import roman_datamodels.testing.utils as maker_utils
+import roman_datamodels.maker_utils as maker_utils
 
 
 def make_fake_distortion_function():
     """A very simple distortion function.
 
     This returns a very simple distortion function that scales pixels
     by roughly their angular size on the sky and does a tangent plane
```

### Comparing `romanisim-0.5.1/romanisim/util.py` & `romanisim-0.5.2/romanisim/util.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/romanisim/wcs.py` & `romanisim-0.5.2/romanisim/wcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         parameters['pointing']['ra_v1'])
 
     parameters['pointing']['dec_v1'] = coord.dec.to(u.deg).value
     parameters['wcsinfo']['dec_ref'] = (
         parameters['pointing']['dec_v1'])
 
     # Romanisim uses ROLL_REF = PA_APER - V3IdlYAngle
-    V3IdlYAngle = -60 # this value should eventually be taken from the SIAF
-    parameters['wcsinfo']['roll_ref'] = pa_aper - V3IdlYAngle 
+    V3IdlYAngle = -60  # this value should eventually be taken from the SIAF
+    parameters['wcsinfo']['roll_ref'] = pa_aper - V3IdlYAngle
 
     if boresight:
         parameters['wcsinfo']['v2_ref'] = 0
         parameters['wcsinfo']['v3_ref'] = 0
         parameters['aperture']['name'] = 'BORESIGHT'
     else:
         from .parameters import v2v3_wficen
@@ -144,14 +144,16 @@
         distortion = dist_model.coordinate_distortion_transform
 
     if distortion is not None:
         wcs = make_wcs(util.skycoord(world_pos), distortion,
                        v2_ref=image_mod.meta.wcsinfo.v2_ref,
                        v3_ref=image_mod.meta.wcsinfo.v3_ref,
                        roll_ref=image_mod.meta.wcsinfo.roll_ref)
+        shape = image_mod.data.shape
+        wcs.bounding_box = ((-0.5, shape[-1] - 0.5), (-0.5, shape[-2] - 0.5))
         wcs = GWCS(wcs)
     else:
         # use galsim.roman
         # galsim.roman does something smarter with choosing the roll
         # angle to optimize the solar panels given the target, and
         # therefore requires a date.
         wcs_dict = roman.getWCS(world_pos=util.celestialcoord(world_pos),
@@ -256,16 +258,16 @@
         """
         return self._origin
 
     def _radec(self, x, y, color=None):
         x1 = np.atleast_1d(x)
         y1 = np.atleast_1d(y)
 
-        coord = self.wcs.pixel_to_world(x1, y1)
-        r, d = coord.ra.to(u.rad).value, coord.dec.to(u.rad).value
+        coord = self.wcs(x1, y1, with_bounding_box=False)
+        r, d = (np.radians(c) for c in coord)
 
         if np.ndim(x) == np.ndim(y) == 0:
             return r[0], d[0]
         else:
             if (np.ndim(x) != np.ndim(y)):
                 raise ValueError(
                     f"np.ndim(x) != np.ndim(y) => {np.ndim(x)} != {np.ndim(y)}")
@@ -278,15 +280,15 @@
         # _xy accepts ra/dec in radians; we decorate r1, d1 appropriately.
         r1 = np.atleast_1d(ra) * u.rad
         d1 = np.atleast_1d(dec) * u.rad
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             # x, y = self.wcs.world_to_pixel(r1, d1)
-            x, y = self.wcs.numerical_inverse(r1, d1)
+            x, y = self.wcs.numerical_inverse(r1, d1, with_bounding_box=False)
 
         if np.ndim(ra) == np.ndim(dec) == 0:
             return x[0], y[0]
         else:
             if (np.ndim(ra) != np.ndim(dec)):
                 raise ValueError(
                     f"np.ndim(ra) != np.ndim(dec) => "
@@ -400,7 +402,48 @@
     wcs.GWCS corresponding to wcs.
     """
     if isinstance(wcs, GWCS):
         return wcs.wcs
     else:
         # make a gwcs WCS from a galsim.roman WCS
         return wcs_from_fits_header(wcs.header.header)
+
+
+def get_mosaic_wcs(mosaic):
+    """Get a WCS object for a given sca or set of CRDS parameters.
+
+    Parameters
+    ----------
+    mosaic : roman_datamodels.datamodels.MosaicModel or dict
+        Mosaic model or dictionary containing WCS parameters.
+
+    Returns
+    -------
+    galsim.CelestialWCS for the mosaic
+    """
+
+    # If sent a dictionary, create a temporary model for data interface
+    if (type(mosaic) is not roman_datamodels.datamodels.MosaicModel):
+        mosaic_node = maker_utils.mk_level3_mosaic()
+        for key in mosaic.keys():
+            if isinstance(mosaic[key], dict):
+                mosaic_node['meta'][key].update(mosaic[key])
+            else:
+                mosaic_node['meta'][key] = mosaic[key]
+        mosaic_node = roman_datamodels.datamodels.MosaicModel(mosaic_node)
+    else:
+        mosaic_node = mosaic
+
+    world_pos = astropy.coordinates.SkyCoord(
+        mosaic_node.meta.wcsinfo.ra_ref * u.deg,
+        mosaic_node.meta.wcsinfo.dec_ref * u.deg)
+
+    # Create a tangent plane WCS for the mosaic
+    # The affine parameters below should be reviewed and updated
+    affine = galsim.AffineTransform(
+        0.1, 0, 0, 0.1, origin=galsim.PositionI(mosaic_node.data.shape[0] / 2.0,
+                                                mosaic_node.data.shape[1] / 2.0,),
+        world_origin=galsim.PositionD(0, 0))
+    wcs = galsim.TanWCS(affine,
+                        util.celestialcoord(world_pos))
+
+    return wcs
```

### Comparing `romanisim-0.5.1/romanisim.egg-info/PKG-INFO` & `romanisim-0.5.2/romanisim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.5.1
+Version: 0.5.2
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `romanisim-0.5.1/romanisim.egg-info/SOURCES.txt` & `romanisim-0.5.2/romanisim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 romanisim/apt.py
 romanisim/bandpass.py
 romanisim/catalog.py
 romanisim/cr.py
 romanisim/gaia.py
 romanisim/image.py
 romanisim/l1.py
+romanisim/l3.py
 romanisim/nonlinearity.py
 romanisim/parameters.py
 romanisim/persistence.py
 romanisim/psf.py
 romanisim/ramp.py
 romanisim/ramp_fit_casertano.c
 romanisim/ramp_fit_casertano.pyx
```

### Comparing `romanisim-0.5.1/scripts/romancal_make_all_l1s.sh` & `romanisim-0.5.2/scripts/romancal_make_all_l1s.sh`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/scripts/romancal_make_regtest_l1s.sh` & `romanisim-0.5.2/scripts/romancal_make_regtest_l1s.sh`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/scripts/romanisim-make-catalog` & `romanisim-0.5.2/scripts/romanisim-make-catalog`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/scripts/romanisim-make-image` & `romanisim-0.5.2/scripts/romanisim-make-image`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/scripts/romanisim-make-stack` & `romanisim-0.5.2/scripts/romanisim-make-stack`

 * *Files identical despite different names*

### Comparing `romanisim-0.5.1/tox.ini` & `romanisim-0.5.2/tox.ini`

 * *Files identical despite different names*

