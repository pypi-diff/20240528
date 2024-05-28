# Comparing `tmp/astrocut-0.8.tar.gz` & `tmp/astrocut-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cbrasseur/Documents/githubRepos/astrocut/dist/tmp157thofl/astrocut-0.8.tar", last modified: Fri Jul  2 19:11:45 2021, max compression
+gzip compressed data, was "/Users/cbrasseur/Documents/githubRepos/astrocut/dist/tmp_nzq0ftk/astrocut-0.9.tar", last modified: Tue Aug 10 15:23:48 2021, max compression
```

## Comparing `astrocut-0.8.tar` & `astrocut-0.9.tar`

### file list

```diff
@@ -1,76 +1,87 @@
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.097642 astrocut-0.8/
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.081328 astrocut-0.8/.github/
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.085974 astrocut-0.8/.github/workflows/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     3003 2021-06-15 19:48:02.000000 astrocut-0.8/.github/workflows/ci_workflows.yml
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      733 2020-10-13 18:41:29.000000 astrocut-0.8/.gitignore
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      171 2020-10-13 18:41:29.000000 astrocut-0.8/.readthedocs.yml
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1443 2021-07-02 19:08:45.000000 astrocut-0.8/CHANGES.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      361 2020-10-13 18:41:29.000000 astrocut-0.8/MANIFEST.in
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5000 2021-07-02 19:11:45.097777 astrocut-0.8/PKG-INFO
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4654 2021-06-10 03:11:31.000000 astrocut-0.8/README.rst
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.088188 astrocut-0.8/astrocut/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1042 2021-06-15 19:48:02.000000 astrocut-0.8/astrocut/__init__.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      613 2021-06-10 03:11:31.000000 astrocut-0.8/astrocut/_astropy_init.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1957 2020-10-13 18:41:29.000000 astrocut-0.8/astrocut/conftest.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    35485 2020-10-13 18:41:29.000000 astrocut-0.8/astrocut/cube_cut.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    16075 2021-07-02 18:38:50.000000 astrocut-0.8/astrocut/cutout_processing.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    30198 2021-06-15 19:48:02.000000 astrocut-0.8/astrocut/cutouts.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.090094 astrocut-0.8/astrocut/data/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      246 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/data/README.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      827 2020-01-13 20:17:19.000000 astrocut-0.8/astrocut/exceptions.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.090314 astrocut-0.8/astrocut/extern/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      366 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/extern/__init__.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    13683 2020-10-13 18:41:29.000000 astrocut-0.8/astrocut/make_cube.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.092057 astrocut-0.8/astrocut/tests/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      108 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/tests/__init__.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.092287 astrocut-0.8/astrocut/tests/data/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5760 2021-06-10 03:11:31.000000 astrocut-0.8/astrocut/tests/data/ex_ffi_wcs.txt
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      299 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/tests/setup_package.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    12760 2020-10-13 18:41:29.000000 astrocut-0.8/astrocut/tests/test_cube_cut.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     9582 2021-06-15 19:48:02.000000 astrocut-0.8/astrocut/tests/test_cutout_processing.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    17927 2021-06-15 19:48:02.000000 astrocut-0.8/astrocut/tests/test_cutouts.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     3444 2020-10-13 18:41:29.000000 astrocut-0.8/astrocut/tests/test_make_cube.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     6743 2021-06-15 19:48:02.000000 astrocut-0.8/astrocut/tests/utils_for_test.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.092742 astrocut-0.8/astrocut/utils/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      148 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/utils/__init__.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.093000 astrocut-0.8/astrocut/utils/tests/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        0 2019-06-21 15:38:43.000000 astrocut-0.8/astrocut/utils/tests/__init__.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    15799 2020-05-06 19:15:38.000000 astrocut-0.8/astrocut/utils/wcs_fitting.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      335 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut/version.py
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.089858 astrocut-0.8/astrocut.egg-info/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5000 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/PKG-INFO
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1450 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/SOURCES.txt
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        1 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/dependency_links.txt
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)       83 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/entry_points.txt
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        1 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/not-zip-safe
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)       72 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/requires.txt
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        9 2021-07-02 19:11:45.000000 astrocut-0.8/astrocut.egg-info/top_level.txt
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.094142 astrocut-0.8/docs/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4581 2019-06-21 15:38:43.000000 astrocut-0.8/docs/Makefile
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.094935 astrocut-0.8/docs/_static/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    45012 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_static/AstroCut_medium.png
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    14264 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_static/AstroCut_thumb.png
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      217 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_static/astrocut.css
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.082688 astrocut-0.8/docs/_templates/
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.095807 astrocut-0.8/docs/_templates/autosummary/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      250 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      251 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      252 2019-06-21 15:38:43.000000 astrocut-0.8/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.096262 astrocut-0.8/docs/astrocut/
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.096757 astrocut-0.8/docs/astrocut/imgs/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4400 2019-11-18 19:30:16.000000 astrocut-0.8/docs/astrocut/imgs/color_ex_cutout.png
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    34276 2019-11-18 19:30:16.000000 astrocut-0.8/docs/astrocut/imgs/png_ex_cutout.png
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    12521 2020-10-13 18:41:29.000000 astrocut-0.8/docs/astrocut/index.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      720 2020-10-13 18:41:29.000000 astrocut-0.8/docs/astrocut/install.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     7441 2020-10-13 18:41:29.000000 astrocut-0.8/docs/conf.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      860 2019-09-17 18:52:13.000000 astrocut-0.8/docs/index.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      169 2019-06-21 15:38:43.000000 astrocut-0.8/docs/license.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4513 2019-06-21 15:38:43.000000 astrocut-0.8/docs/make.bat
-drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-07-02 19:11:45.097448 astrocut-0.8/licenses/
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1495 2019-06-21 15:38:43.000000 astrocut-0.8/licenses/LICENSE.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      372 2019-06-21 15:38:43.000000 astrocut-0.8/licenses/README.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1659 2019-06-21 15:38:43.000000 astrocut-0.8/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      132 2020-10-13 18:41:29.000000 astrocut-0.8/pyproject.toml
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1548 2021-07-02 19:11:45.098537 astrocut-0.8/setup.cfg
--rwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)     1957 2020-10-13 18:41:29.000000 astrocut-0.8/setup.py
--rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     2707 2021-06-15 19:48:02.000000 astrocut-0.8/tox.ini
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.905755 astrocut-0.9/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      319 2021-08-10 14:49:04.000000 astrocut-0.9/.codecov.yml
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.878669 astrocut-0.9/.github/
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.885282 astrocut-0.9/.github/workflows/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     3003 2021-08-10 14:49:04.000000 astrocut-0.9/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      733 2020-10-13 18:41:29.000000 astrocut-0.9/.gitignore
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      157 2021-07-22 15:36:03.000000 astrocut-0.9/.readthedocs.yml
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1521 2021-08-10 15:22:39.000000 astrocut-0.9/CHANGES.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      361 2020-10-13 18:41:29.000000 astrocut-0.9/MANIFEST.in
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5197 2021-08-10 15:23:48.905943 astrocut-0.9/PKG-INFO
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4851 2021-07-22 15:36:03.000000 astrocut-0.9/README.rst
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.888572 astrocut-0.9/astrocut/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1137 2021-08-10 14:49:04.000000 astrocut-0.9/astrocut/__init__.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      613 2021-06-10 03:11:31.000000 astrocut-0.9/astrocut/_astropy_init.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1957 2020-10-13 18:41:29.000000 astrocut-0.9/astrocut/conftest.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    35561 2021-08-10 14:49:04.000000 astrocut-0.9/astrocut/cube_cut.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    22805 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/cutout_processing.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    26801 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/cutouts.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.891308 astrocut-0.9/astrocut/data/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      246 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/data/README.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      827 2020-01-13 20:17:19.000000 astrocut-0.9/astrocut/exceptions.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.891659 astrocut-0.9/astrocut/extern/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      366 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/extern/__init__.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    13683 2020-10-13 18:41:29.000000 astrocut-0.9/astrocut/make_cube.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.894429 astrocut-0.9/astrocut/tests/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      108 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/tests/__init__.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.894769 astrocut-0.9/astrocut/tests/data/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5760 2021-06-10 03:11:31.000000 astrocut-0.9/astrocut/tests/data/ex_ffi_wcs.txt
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      299 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/tests/setup_package.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    12764 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/tests/test_cube_cut.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    13230 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/tests/test_cutout_processing.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    12327 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/tests/test_cutouts.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     3444 2020-10-13 18:41:29.000000 astrocut-0.9/astrocut/tests/test_make_cube.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5816 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/tests/test_utils.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     6730 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/tests/utils_for_test.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.895852 astrocut-0.9/astrocut/utils/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      148 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/utils/__init__.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.896207 astrocut-0.9/astrocut/utils/tests/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        0 2019-06-21 15:38:43.000000 astrocut-0.9/astrocut/utils/tests/__init__.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     7677 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/utils/utils.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    15795 2021-08-10 14:49:05.000000 astrocut-0.9/astrocut/utils/wcs_fitting.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      335 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut/version.py
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.890957 astrocut-0.9/astrocut.egg-info/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     5197 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/PKG-INFO
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1766 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/SOURCES.txt
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        1 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/dependency_links.txt
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)       83 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/entry_points.txt
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        1 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/not-zip-safe
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      125 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/requires.txt
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)        9 2021-08-10 15:23:48.000000 astrocut-0.9/astrocut.egg-info/top_level.txt
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.897557 astrocut-0.9/docs/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4581 2019-06-21 15:38:43.000000 astrocut-0.9/docs/Makefile
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.899058 astrocut-0.9/docs/_static/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    45012 2019-06-21 15:38:43.000000 astrocut-0.9/docs/_static/AstroCut_medium.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    14264 2019-06-21 15:38:43.000000 astrocut-0.9/docs/_static/AstroCut_thumb.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      461 2021-07-22 15:36:03.000000 astrocut-0.9/docs/_static/astrocut.css
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1962 2021-07-22 15:36:03.000000 astrocut-0.9/docs/_static/main.css
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.899390 astrocut-0.9/docs/_templates/
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.900567 astrocut-0.9/docs/_templates/autosummary/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      250 2019-06-21 15:38:43.000000 astrocut-0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      251 2019-06-21 15:38:43.000000 astrocut-0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      252 2019-06-21 15:38:43.000000 astrocut-0.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      559 2021-07-22 15:36:03.000000 astrocut-0.9/docs/_templates/layout.html
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.902673 astrocut-0.9/docs/astrocut/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      147 2021-07-22 15:36:03.000000 astrocut-0.9/docs/astrocut/api.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      159 2021-08-10 14:49:05.000000 astrocut-0.9/docs/astrocut/contents.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    12057 2021-07-22 15:36:03.000000 astrocut-0.9/docs/astrocut/file_formats.rst
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.904389 astrocut-0.9/docs/astrocut/imgs/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4400 2019-11-18 19:30:16.000000 astrocut-0.9/docs/astrocut/imgs/color_ex_cutout.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     8325 2021-08-10 14:49:05.000000 astrocut-0.9/docs/astrocut/imgs/hapcut_combined.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     6110 2021-08-10 14:49:05.000000 astrocut-0.9/docs/astrocut/imgs/hapcut_left.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     6946 2021-08-10 14:49:05.000000 astrocut-0.9/docs/astrocut/imgs/hapcut_right.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    34276 2019-11-18 19:30:16.000000 astrocut-0.9/docs/astrocut/imgs/png_ex_cutout.png
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)    21354 2021-08-10 14:49:05.000000 astrocut-0.9/docs/astrocut/index.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      580 2021-07-22 15:36:03.000000 astrocut-0.9/docs/astrocut/install.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      172 2021-07-22 15:36:03.000000 astrocut-0.9/docs/astrocut/license.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     7420 2021-07-22 15:36:03.000000 astrocut-0.9/docs/conf.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1840 2021-07-22 15:36:03.000000 astrocut-0.9/docs/index.html
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     4513 2019-06-21 15:38:43.000000 astrocut-0.9/docs/make.bat
+drwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)        0 2021-08-10 15:23:48.905472 astrocut-0.9/licenses/
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1495 2019-06-21 15:38:43.000000 astrocut-0.9/licenses/LICENSE.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      372 2019-06-21 15:38:43.000000 astrocut-0.9/licenses/README.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1659 2019-06-21 15:38:43.000000 astrocut-0.9/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)      132 2020-10-13 18:41:29.000000 astrocut-0.9/pyproject.toml
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     1610 2021-08-10 15:23:48.906917 astrocut-0.9/setup.cfg
+-rwxr-xr-x   0 cbrasseur  (1650) STSCI\science  (1031)     1957 2020-10-13 18:41:29.000000 astrocut-0.9/setup.py
+-rw-r--r--   0 cbrasseur  (1650) STSCI\science  (1031)     2730 2021-08-10 14:49:05.000000 astrocut-0.9/tox.ini
```

### Comparing `astrocut-0.8/.github/workflows/ci_workflows.yml` & `astrocut-0.9/.github/workflows/ci_workflows.yml`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,18 @@
             toxargs: -v --develop
 
           - name: Python 3.6 with oldest supported version of all dependencies
             os: ubuntu-16.04
             python: 3.6
             toxenv: py36-test-oldestdeps   
             
-          - name: Python 3.7 with numpy 1.17 and full coverage
+          - name: Python 3.7 with numpy 1.21 and full coverage
             os: ubuntu-latest
             python: 3.7
-            toxenv: py37-test-alldeps-numpy117-cov
+            toxenv: py37-test-alldeps-numpy121-cov
 
           - name: Python 3.8 with all optional dependencies (Windows)
             os: windows-latest
             python: 3.8
             toxenv: py38-test-alldeps
             
           - name: Python 3.7 with all optional dependencies (MacOS X)
```

### Comparing `astrocut-0.8/.gitignore` & `astrocut-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/CHANGES.rst` & `astrocut-0.9/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.9 (2021-08-10)
+----------------
+
+- Add cutout combine functionality [#45]
+
+
 0.8 (2021-07-02)
 ----------------
 
 - Add moving target cutout functionality [#40]
   
 
 0.7 (2020-08-19)
```

### Comparing `astrocut-0.8/PKG-INFO` & `astrocut-0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: astrocut
-Version: 0.8
-Summary: Cutout tools for astronomical images
-Home-page: https://astrocut.readthedocs.io
-Author: MAST Archive Developers
-Author-email: archive@stsci.edu
-License: BSD 3-Clause
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Provides-Extra: test
-Provides-Extra: docs
-License-File: licenses/LICENSE.rst
-
 Cutout tools for astronomical images
 ------------------------------------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
     
@@ -23,17 +9,21 @@
     :target: https://badge.fury.io/py/astrocut
     :alt: PyPi Status
     
 .. image:: https://readthedocs.org/projects/astrocut/badge/?version=latest
     :target: https://astrocut.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-Tools for making image cutouts from sets of TESS full frame images.
+Astrocut provides tools for making cutouts from sets of astronomical images with shared footprints. It is under active development.
+
+Three main areas of functionality are included:
 
-This package is under active development, and will ultimately grow to encompass a range of cutout activities relevant to images from many missions, however at this time it is focussed on the specific problem of creating Target Pixel File cutouts from sectors of TESS full frame images.
+- Solving the specific problem of creating image cutouts from sectors of Transiting Exoplanet Survey Satellite (TESS) full-frame images.
+- General fits file cutouts incuding from single images and sets of images with the shared WCS/pixel scale.
+- Cutout post-processing functionality, including centering cutouts along a path (for moving targets) and combining cutouts.
 
 Documentation is at https://astrocut.readthedocs.io.
 
 Project Status
 --------------
 .. image:: https://github.com/spacetelescope/astrocut/workflows/CI/badge.svg?branch=master
     :target: https://github.com/spacetelescope/astrocut/actions
@@ -143,9 +133,7 @@
 This project is Copyright (c) MAST Archive Developers and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
 the `Astropy package template <https://github.com/astropy/package-template>`_
 which is licensed under the BSD 3-clause licence. See the licenses folder for
 more information.
 
 
-
-
```

### Comparing `astrocut-0.8/README.rst` & `astrocut-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: astrocut
+Version: 0.9
+Summary: Cutout tools for astronomical images
+Home-page: https://astrocut.readthedocs.io
+Author: MAST Archive Developers
+Author-email: archive@stsci.edu
+License: BSD 3-Clause
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Provides-Extra: test
+Provides-Extra: docs
+License-File: licenses/LICENSE.rst
+
 Cutout tools for astronomical images
 ------------------------------------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
     
@@ -9,17 +23,21 @@
     :target: https://badge.fury.io/py/astrocut
     :alt: PyPi Status
     
 .. image:: https://readthedocs.org/projects/astrocut/badge/?version=latest
     :target: https://astrocut.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-Tools for making image cutouts from sets of TESS full frame images.
+Astrocut provides tools for making cutouts from sets of astronomical images with shared footprints. It is under active development.
+
+Three main areas of functionality are included:
 
-This package is under active development, and will ultimately grow to encompass a range of cutout activities relevant to images from many missions, however at this time it is focussed on the specific problem of creating Target Pixel File cutouts from sectors of TESS full frame images.
+- Solving the specific problem of creating image cutouts from sectors of Transiting Exoplanet Survey Satellite (TESS) full-frame images.
+- General fits file cutouts incuding from single images and sets of images with the shared WCS/pixel scale.
+- Cutout post-processing functionality, including centering cutouts along a path (for moving targets) and combining cutouts.
 
 Documentation is at https://astrocut.readthedocs.io.
 
 Project Status
 --------------
 .. image:: https://github.com/spacetelescope/astrocut/workflows/CI/badge.svg?branch=master
     :target: https://github.com/spacetelescope/astrocut/actions
@@ -129,7 +147,9 @@
 This project is Copyright (c) MAST Archive Developers and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
 the `Astropy package template <https://github.com/astropy/package-template>`_
 which is licensed under the BSD 3-clause licence. See the licenses folder for
 more information.
 
 
+
+
```

### Comparing `astrocut-0.8/astrocut/__init__.py` & `astrocut-0.9/astrocut/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 from ._astropy_init import *  # noqa
 # ----------------------------------------------------------------------------
 
 # Enforce Python version check during package import.
 # This is the same check as the one at the top of setup.py
 import sys
 
-__minimum_python_version__ = "3.5"
+__minimum_python_version__ = "3.6"
 
 
 class UnsupportedPythonError(Exception):
     pass
 
 
 if sys.version_info < tuple((int(val) for val in __minimum_python_version__.split('.'))):
     raise UnsupportedPythonError("astrocut does not support Python < {}".format(__minimum_python_version__))
 
 
 if not _ASTROPY_SETUP_:  # noqa
     from .make_cube import CubeFactory  # noqa
     from .cube_cut import CutoutFactory  # noqa
     from .cutouts import fits_cut, img_cut, normalize_img  # noqa
-    from .cutout_processing import center_on_path, path_to_footprints  # noqa
+    from .cutout_processing import (path_to_footprints, center_on_path,  # noqa
+                                    CutoutsCombiner, build_default_combine_function)  # noqa
```

### Comparing `astrocut-0.8/astrocut/_astropy_init.py` & `astrocut-0.9/astrocut/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/conftest.py` & `astrocut-0.9/astrocut/conftest.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/cube_cut.py` & `astrocut-0.9/astrocut/cube_cut.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from astropy import wcs
 
 from . import __version__ 
 from .exceptions import InputWarning, InvalidQueryError
 
-# Note: Use the astropy function if available
+# Note: Use the astropy function if available, TODO: fix > 4.3 astropy fitting
 import astropy
-if astropy.utils.minversion(astropy, "4.0.2"):
+if astropy.utils.minversion(astropy, "4.0.2") and (float(astropy.__version__[:3]) < 4.3):
     from astropy.wcs.utils import fit_wcs_from_points
 else:
     from .utils.wcs_fitting import fit_wcs_from_points
 
 
 class CutoutFactory():
     """
```

### Comparing `astrocut-0.8/astrocut/cutout_processing.py` & `astrocut-0.9/astrocut/cutout_processing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 """This module contains various cutout post-processing tools."""
 
 import numpy as np
+import warnings
 import os
 
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from astropy.table import Table, vstack
 from astropy.wcs import WCS
 from astropy.time import Time
 
 from scipy.interpolate import splprep, splev
 
+from .utils.utils import get_fits
+from .exceptions import DataWarning, InvalidInputError
+
 
 def _combine_headers(headers, constant_only=False):
     """
     Combine any number of fits headers such that keywords that
     have the same values in all input headers are unchanged, while
     keywords whose values vary are saved in new keywords as:
         F<header number>_K<#>: Keyword
@@ -49,22 +53,22 @@
             continue
         
         if (np.array([x[kwd] for x in headers[1:]]) == headers[0][kwd]).all():
             uniform_cards.append(headers[0].cards[kwd])
         else:
             if constant_only:  # Removing non-constant kewords in this case
                 continue
-                
+ 
             n_vk += 1
             for i, hdr in enumerate(headers):
                 varying_keywords.append((f"F{i+1:02}_K{n_vk:02}", kwd, "Keyword"))
                 varying_keywords.append((f"F{i+1:02}_V{n_vk:02}", hdr[kwd], "Value"))
                 varying_keywords.append((f"F{i+1:02}_C{n_vk:02}", hdr.comments[kwd], "Comment"))
 
-                
+    # TODO: Add wcs checking? How?
     return fits.Header(uniform_cards+varying_keywords)
 
 
 def _get_bounds(x, y, size):
     """
     Given an x,y coordinates (single or lists) and size, return the bounds of the
     described area(s) as [[[x_min, x_max],[y_min, y_max]],...].
@@ -113,71 +117,14 @@
     ny = bounds[1, 1]-bounds[1, 0]
     x = nx/2 + bounds[0, 0]
     y = ny/2 + bounds[1, 0]
     return {"coordinates": img_wcs.pixel_to_world(x, y),
             "size": (ny, nx)}
 
 
-# TODO: Put this in utils 
-def path_to_footprints(path, size, img_wcs, max_pixels=10000):
-    """
-    Given a path that intersects with a wcs footprint, return
-    one or more rectangles that fully contain that intersection 
-    (plus padding given by 'size') with each rectangle no more than 
-    max_pixels in size.
-    
-    Parameters
-    ----------
-    path : `~astropy.coordinate.SkyCoord`
-        SkyCoord object list of coordinates that represent a continuous path.
-    size : array
-        Size of the rectangle centered on the path locations that must 
-        be included in the returned footprint(s). Formatted as [ny,nx]
-    img_wcs : `~astropy.wcs.WCS`
-        WCS object the path intersects with. Must include naxis information.
-    max_pixels : int
-        Optional, default 10000. The maximum area in pixels for individual
-        footprints.
-        
-    Returns
-    -------
-    response : list
-       List of footprints, each a dictionary of the form:
-       {'center_coord': `~astropy.coordinate.SkyCoord`, 'size': [ny,nx]}
-    """
-    
-    x, y = img_wcs.world_to_pixel(path)
-    
-    # Removing any coordinates outside of the img wcs
-    valid_locs = ((x >= 0) & (x < img_wcs.array_shape[0])) & ((y >= 0) & (y < img_wcs.array_shape[1]))
-    x = x[valid_locs]
-    y = y[valid_locs]
-    
-    bounds_list = _get_bounds(x, y, size)
-
-    combined_bounds = list()
-    cur_bounds = bounds_list[0]
-    for bounds in bounds_list[1:]:
-        new_bounds = _combine_bounds(cur_bounds, bounds)
-        
-        if _area(new_bounds) > max_pixels:
-            combined_bounds.append(cur_bounds)
-            cur_bounds = bounds
-        else:
-            cur_bounds = new_bounds
-            
-    combined_bounds.append(cur_bounds)
-    
-    footprints = []
-    for bounds in combined_bounds:
-        footprints.append(_get_args(bounds, img_wcs))
-        
-    return footprints 
-
-
 def _moving_target_focus(path, size, cutout_fles, verbose=False):
     """
     Given a moving target path (list of RA/Decs) and size, that intersects with 
     the given cutout(s) make a cutout of requested size centered on the 
     moving target given by the path.
     
     Note: No resampling is done so there will be some jitter in the moving target
@@ -323,14 +270,69 @@
         if any(x in kwd for x in ["WCA", "WCS", "CTY", "CRP", "CRV", "CUN",
                                   "CDL", "11PC", "12PC", "21PC", "22PC"]):  # Skipping column WCS keywords
             continue
 
         new_header.append(shared_keywords.cards[kwd])
 
 
+def path_to_footprints(path, size, img_wcs, max_pixels=10000):
+    """
+    Given a path that intersects with a wcs footprint, return
+    one or more rectangles that fully contain that intersection 
+    (plus padding given by 'size') with each rectangle no more than 
+    max_pixels in size.
+    
+    Parameters
+    ----------
+    path : `~astropy.coordinate.SkyCoord`
+        SkyCoord object list of coordinates that represent a continuous path.
+    size : array
+        Size of the rectangle centered on the path locations that must 
+        be included in the returned footprint(s). Formatted as [ny,nx]
+    img_wcs : `~astropy.wcs.WCS`
+        WCS object the path intersects with. Must include naxis information.
+    max_pixels : int
+        Optional, default 10000. The maximum area in pixels for individual
+        footprints.
+        
+    Returns
+    -------
+    response : list
+       List of footprints, each a dictionary of the form:
+       {'center_coord': `~astropy.coordinate.SkyCoord`, 'size': [ny,nx]}
+    """
+    
+    x, y = img_wcs.world_to_pixel(path)
+    
+    # Removing any coordinates outside of the img wcs
+    valid_locs = ((x >= 0) & (x < img_wcs.array_shape[0])) & ((y >= 0) & (y < img_wcs.array_shape[1]))
+    x = x[valid_locs]
+    y = y[valid_locs]
+    
+    bounds_list = _get_bounds(x, y, size)
+
+    combined_bounds = list()
+    cur_bounds = bounds_list[0]
+    for bounds in bounds_list[1:]:
+        new_bounds = _combine_bounds(cur_bounds, bounds)
+        
+        if _area(new_bounds) > max_pixels:
+            combined_bounds.append(cur_bounds)
+            cur_bounds = bounds
+        else:
+            cur_bounds = new_bounds
+            
+    combined_bounds.append(cur_bounds)
+    
+    footprints = []
+    for bounds in combined_bounds:
+        footprints.append(_get_args(bounds, img_wcs))
+        
+    return footprints 
+
 
 def center_on_path(path, size, cutout_fles, target=None, img_wcs=None,
                    target_pixel_file=None, output_path=".", verbose=True):
     """
     Given a moving target path that crosses through one or more cutout files 
     (as produced by `cube_cut`/tesscut) and size, create a target pixel file 
     containint a cutout of the requested size centered on the moving target 
@@ -424,7 +426,196 @@
         target_pixel_file = (f"{target}_{primary_header['TSTART']}-{primary_header['TSTop']}_"
                              f"{size[0]}-x-{size[1]}_astrocut.fits")
 
     filename = os.path.join(output_path, target_pixel_file)
     mt_hdu_list.writeto(filename, overwrite=True, checksum=True)
 
     return filename
+
+
+def build_default_combine_function(template_hdu_arr, no_data_val=np.nan):
+    """
+    Given an array of `~astropy.io.fits.ImageHdu` objects, 
+    initialize a function to combine an array of the same size/shape 
+    images where each pixel the mean of all images with available
+    data at that pixel.
+
+    Parameters
+    ----------
+    template_hdu_arr : list
+        A list of `~astropy.io.fits.ImageHdu` objects that will be 
+        used to create the image combine function.
+    no_data_val : scaler
+        Optional. The image value that indicates "no data" at a particular pixel.
+        The deavault is `~numpy.nan`.
+
+    Returns
+    -------
+    response : func
+        The combiner function that can be applying to other arrays of images.
+    """
+    
+    img_arrs = np.array([hdu.data for hdu in template_hdu_arr])
+   
+    if np.isnan(no_data_val):
+        templates = (~np.isnan(img_arrs)).astype(float)
+    else:
+        templates = (img_arrs != no_data_val).astype(float)
+
+    multiplier_arr = np.sum(templates, axis=0)
+    multiplier_arr = np.divide(1, multiplier_arr, where=(multiplier_arr != 0))
+    for t_arr in templates:
+        t_arr *= multiplier_arr
+
+    def combine_function(cutout_hdu_arr):
+        """
+        Combiner function that takes an array of `~astropy.io.fits.ImageHdu` 
+        objects and cobines them into a single image.
+
+        Parameters
+        ----------
+        cutout_hdu_arr : list
+            Array of `~astropy.io.fits.ImageHdu` objects that will be 
+            combined into a single image.
+
+        Returns
+        -------
+        response : array
+            The combined image array.
+        """
+        
+        cutout_imgs = np.array([hdu.data for hdu in cutout_hdu_arr])
+        nans = np.bitwise_and.reduce(np.isnan(cutout_imgs), axis=0)
+        
+        cutout_imgs[np.isnan(cutout_imgs)] = 0  # don't want any nans because they mess up multiple/add
+ 
+        combined_img = np.sum(templates*cutout_imgs, axis=0)
+        combined_img[nans] = np.nan  # putting nans back if we need to
+
+        return combined_img
+
+    return combine_function
+
+
+
+class CutoutsCombiner():
+    """
+    Class for combining cutouts.
+    """
+
+    def __init__(self, fits_list=None, exts=None, img_combiner=None):
+
+        self.input_hdulists = None
+        self.center_coord = None
+        if fits_list:
+            self.load(fits_list, exts)
+
+        self.combine_headers = _combine_headers
+
+        if img_combiner:
+            self.combine_images = img_combiner
+        else:  # load up the default combiner
+            self.build_img_combiner(build_default_combine_function,
+                                    builder_args=[self.input_hdulists[0], np.nan])
+        
+            
+    def load(self, fits_list, exts=None):
+        """
+        Load the input cutouts and select the desired fits extensions.
+
+        Parameters
+        ----------
+        fits_list : list
+            List of fits filenames or `~astropy.io.fits.HDUList` objects
+            with cutouts to be combined.
+        exts : list or None
+            Optional. List of fits extensions to combine.
+            Default is None, which means all extensions will be combined.
+            If the first extension is a PrimaryHeader with no data it will
+            be skipped.      
+        """
+
+        if isinstance(fits_list[0], str):  # input is filenames
+            cutout_hdulists = [fits.open(fle) for fle in fits_list]
+        elif isinstance(fits_list[0], fits.HDUList):  # input is HDUList objects
+            cutout_hdulists = fits_list
+        else:
+            raise InvalidInputError("Unsupported input format!")
+        
+        if exts is None:
+            # Go ahead and deal with possible presence of a primaryHeader and no data as first ext
+            if not cutout_hdulists[0][0].data:
+                self.input_hdulists = [hdu[1:] for hdu in cutout_hdulists]
+            else:
+                self.input_hdulists_hdus = cutout_hdulists
+        else:
+            self.input_hdulists = [hdu[exts] for hdu in cutout_hdulists]
+
+        self.input_hdulists = np.transpose(self.input_hdulists)  # Transpose so hdus to be combined on short axis
+
+        # Try to find the center coordinate
+        try:
+            ra = cutout_hdulists[0][0].header['RA_OBJ']
+            dec = cutout_hdulists[0][0].header['DEC_OBJ']
+            self.center_coord = SkyCoord(f"{ra} {dec}", unit='deg')
+            
+        except KeyError:
+            warnings.warn("Could not find RA/Dec header keywords, center coord will be wrong.",
+                          DataWarning)
+            self.center_coord = SkyCoord("0 0", unit='deg')
+            
+        except ValueError:
+            warnings.warn("Invalid RA/Dec values, center coord will be wrong.",
+                          DataWarning)
+            self.center_coord = SkyCoord("0 0", unit='deg')
+
+            
+    def build_img_combiner(self, function_builder, builder_args):
+        """
+        Build the function that will combine cutout extensions.
+
+        Parameters
+        ----------
+        function_builder : func
+            The function that will create the combine function.
+        builder_args : list
+            Array of arguments for the function builder
+        """
+        
+        self.combine_images = function_builder(*builder_args)
+   
+        
+    def combine(self, output_file="./cutout.fits", memory_only=False):
+        """
+        Combine cutouts and either save the output to a FITS file,
+        
+
+        Parameters
+        ----------
+        output_file : str
+            Optional. The filename for the combined cutout file.
+        memory_only : bool
+            Default value False. If set to true, instead of the combined cutout file being 
+            written to disk it is returned as a `~astropy.io.fit.HDUList` object. If set to
+            True, output_file is ignored.
+
+        Returns
+        -------
+        response : str, `~astropy.io.fit.HDUList`
+            The combined cutout filename, or if memory_only is True, the cutout as a
+            `~astropy.io.fit.HDUList` object..
+        """
+
+        hdu_list = []
+
+        for ext_hdus in self.input_hdulists:
+            
+            new_header = self.combine_headers([hdu.header for hdu in ext_hdus])
+        
+            new_img = self.combine_images([hdu.data for hdu in ext_hdus])
+            hdu_list.append(fits.ImageHDU(data=new_img, header=new_header))
+
+        if memory_only:
+            return get_fits(hdu_list, center_coord=self.center_coord)
+        else:
+            get_fits(hdu_list, center_coord=self.center_coord, output_path=output_file)
+            return output_file
```

### Comparing `astrocut-0.8/astrocut/cutouts.py` & `astrocut-0.9/astrocut/cutouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,136 +3,28 @@
 """This module implements cutout functionality similar to fitscut."""
 
 import os
 import warnings
 import numpy as np
 
 from time import time
-from datetime import date
 
 from astropy import log
-from astropy import units as u
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from astropy import wcs
-from astropy.utils.exceptions import AstropyDeprecationWarning
 from astropy.visualization import (SqrtStretch, LogStretch, AsinhStretch, SinhStretch, LinearStretch,
                                    MinMaxInterval, ManualInterval, AsymmetricPercentileInterval)
 
 from PIL import Image
 
-from . import __version__
+from .utils.utils import parse_size_input, get_cutout_limits, get_cutout_wcs, get_fits
 from .exceptions import InputWarning, DataWarning, InvalidQueryError, InvalidInputError
 
 
-#### FUNCTIONS FOR UTILS ####
-def _get_cutout_limits(img_wcs, center_coord, cutout_size):
-    """
-    Takes the center coordinates, cutout size, and the wcs from
-    which the cutout is being taken and returns the x and y pixel limits
-    for the cutout.
-
-    Note: This function does no bounds checking, so the returned limits are not 
-          guaranteed to overlap the original image.
-
-    Parameters
-    ----------
-    img_wcs : `~astropy.wcs.WCS`
-        The WCS for the image that the cutout is being cut from.
-    center_coord : `~astropy.coordinates.SkyCoord`
-        The central coordinate for the cutout
-    cutout_size : array
-        [nx,ny] in with ints (pixels) or astropy quantities
-
-    Returns
-    -------
-    response : `numpy.array`
-        The cutout pixel limits in an array of the form [[xmin,xmax],[ymin,ymax]]
-    """
-        
-    # Note: This is returning the center pixel in 1-up
-    try:
-        center_pixel = center_coord.to_pixel(img_wcs, 1)
-    except wcs.NoConvergence:  # If wcs can't converge, center coordinate is far from the footprint
-        raise InvalidQueryError("Cutout location is not in image footprint!")
-
-    # For some reason you can sometimes get nans without a no convergance error
-    if np.isnan(center_pixel).all():
-        raise InvalidQueryError("Cutout location is not in image footprint!")
-    
-    lims = np.zeros((2, 2), dtype=int)
-
-    for axis, size in enumerate(cutout_size):
-        
-        if not isinstance(size, u.Quantity):  # assume pixels
-            dim = size / 2
-        elif size.unit == u.pixel:  # also pixels
-            dim = size.value / 2
-        elif size.unit.physical_type == 'angle':
-            pixel_scale = u.Quantity(wcs.utils.proj_plane_pixel_scales(img_wcs)[axis],
-                                     img_wcs.wcs.cunit[axis])
-            dim = (size / pixel_scale).decompose() / 2
-
-        lims[axis, 0] = int(np.round(center_pixel[axis] - 1 - dim))
-        lims[axis, 1] = int(np.round(center_pixel[axis] - 1 + dim))
-
-        # The case where the requested area is so small it rounds to zero
-        if lims[axis, 0] == lims[axis, 1]:
-            lims[axis, 0] = int(np.floor(center_pixel[axis] - 1))
-            lims[axis, 1] = lims[axis, 0] + 1
-
-    return lims
-
-        
-def _get_cutout_wcs(img_wcs, cutout_lims):
-    """
-    Starting with the full FFI WCS and adjusting it for the cutout WCS.
-    Adjusts CRPIX values and adds physical WCS keywords.
-
-    Parameters
-    ----------
-    img_wcs : `~astropy.wcs.WCS`
-        WCS for the image the cutout is being cut from.
-    cutout_lims : `numpy.array`
-        The cutout pixel limits in an array of the form [[ymin,ymax],[xmin,xmax]]
-
-    Returns
-    --------
-    response :  `~astropy.wcs.WCS`
-        The cutout WCS object including SIP distortions if present.
-    """
-
-    # relax = True is important when the WCS has sip distortions, otherwise it has no effect
-    wcs_header = img_wcs.to_header(relax=True) 
-
-    # Adjusting the CRPIX values
-    wcs_header["CRPIX1"] -= cutout_lims[0, 0]
-    wcs_header["CRPIX2"] -= cutout_lims[1, 0]
-
-    # Adding the physical wcs keywords
-    wcs_header.set("WCSNAMEP", "PHYSICAL", "name of world coordinate system alternate P")
-    wcs_header.set("WCSAXESP", 2, "number of WCS physical axes")
-    
-    wcs_header.set("CTYPE1P", "RAWX", "physical WCS axis 1 type CCD col")
-    wcs_header.set("CUNIT1P", "PIXEL", "physical WCS axis 1 unit")
-    wcs_header.set("CRPIX1P", 1, "reference CCD column")
-    wcs_header.set("CRVAL1P", cutout_lims[0, 0] + 1, "value at reference CCD column")
-    wcs_header.set("CDELT1P", 1.0, "physical WCS axis 1 step")
-                
-    wcs_header.set("CTYPE2P", "RAWY", "physical WCS axis 2 type CCD col")
-    wcs_header.set("CUNIT2P", "PIXEL", "physical WCS axis 2 unit")
-    wcs_header.set("CRPIX2P", 1, "reference CCD row")
-    wcs_header.set("CRVAL2P", cutout_lims[1, 0] + 1, "value at reference CCD row")
-    wcs_header.set("CDELT2P", 1.0, "physical WCS axis 2 step")
-
-    return wcs.WCS(wcs_header)
-
-#### FUNCTIONS FOR UTILS ####
-
-
 def _hducut(img_hdu, center_coord, cutout_size, correct_wcs=False, verbose=False):
     """
     Takes an ImageHDU (image and associated metatdata in the fits format), as well as a center 
     coordinate and size and make a cutout of that image, which is returned as another ImageHDU,
     including updated  WCS information.
 
 
@@ -186,15 +78,15 @@
 
     img_data = img_hdu.data
 
     if verbose:
         print("Original image shape: {}".format(img_data.shape))
 
     # Get cutout limits
-    cutout_lims = _get_cutout_limits(img_wcs, center_coord, cutout_size)
+    cutout_lims = get_cutout_limits(img_wcs, center_coord, cutout_size)
 
     if verbose:
         print("xmin,xmax: {}".format(cutout_lims[0]))
         print("ymin,ymax: {}".format(cutout_lims[1]))
 
     # These limits are not guarenteed to be within the image footprint
     xmin, xmax = cutout_lims[0]
@@ -227,137 +119,81 @@
     if padding.any():  # only do if we need to pad
         img_cutout = np.pad(img_cutout, padding, 'constant', constant_values=np.nan)
 
     if verbose:
         print("Image cutout shape: {}".format(img_cutout.shape))
 
     # Getting the cutout wcs
-    cutout_wcs = _get_cutout_wcs(img_wcs, cutout_lims)
+    cutout_wcs = get_cutout_wcs(img_wcs, cutout_lims)
 
     # Updating the header with the new wcs info
     if no_sip:
         hdu_header.update(cutout_wcs.to_header(relax=False))
     else:
         hdu_header.update(cutout_wcs.to_header(relax=True))  # relax arg is for sip distortions if they exist
 
-    # Naming the extension
+    # Naming the extension and preserving the original name
+    hdu_header["O_EXT_NM"] = (hdu_header.get("EXTNAME"), "Original extension name.")
     hdu_header["EXTNAME"] = "CUTOUT"
 
     # Moving the filename, if present, into the ORIG_FLE keyword
     hdu_header["ORIG_FLE"] = (hdu_header.get("FILENAME"), "Original image filename.")
     hdu_header.remove("FILENAME", ignore_missing=True)
 
     hdu = fits.ImageHDU(header=hdu_header, data=img_cutout)
 
     return hdu
 
 
-def _save_single_fits(cutout_hdus, output_path, center_coord):
-    """
-    Save a list of cutout hdus to a single fits file.
-
-    Parameters
-    ----------
-    cutout_hdus : list
-        List of `~astropy.io.fits.hdu.image.ImageHDU` objects to be written to a single fits file.
-    output_path : str
-        The full path to the output fits file.
-    center_coord : `~astropy.coordinates.sky_coordinate.SkyCoord`
-        The center coordinate of the image cutouts.
-    """
-
-    # Setting up the Primary HDU
-    primary_hdu = fits.PrimaryHDU()
-    primary_hdu.header.extend([("ORIGIN", 'STScI/MAST', "institution responsible for creating this file"),
-                               ("DATE", str(date.today()), "file creation date"),
-                               ('PROCVER', __version__, 'software version'),
-                               ('RA_OBJ', center_coord.ra.deg, '[deg] right ascension'),
-                               ('DEC_OBJ', center_coord.dec.deg, '[deg] declination')])
-
-    cutout_hdulist = fits.HDUList([primary_hdu] + cutout_hdus)
-
-    # Writing out the hdu often causes a warning as the ORIG_FLE card description is truncated
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore") 
-        cutout_hdulist.writeto(output_path, overwrite=True, checksum=True)
-
-
-def _save_multiple_fits(cutout_hdus, output_paths, center_coord):
-    """
-    Save a list of cutout hdus to individual fits files.
-
-    Parameters
-    ----------
-    cutout_hdus : list
-        List of `~astropy.io.fits.hdu.image.ImageHDU` objects to be written to a single fits file.
-    output_paths : list
-        The cutout filepaths associated with the cutout hdus.
-    center_coord : `~astropy.coordinates.sky_coordinate.SkyCoord`
-        The center coordinate of the image cutouts.
-    """
-
-    if len(output_paths) != len(cutout_hdus):
-        raise InvalidInputError("The number of filenames must match the number of cutouts.")
-
-    # Adding aditional keywords
-    for i, cutout in enumerate(cutout_hdus):
-        # Turning our hdu into a primary hdu
-        hdu = fits.PrimaryHDU(header=cutout.header, data=cutout.data)
-        hdu.header.extend([("ORIGIN", 'STScI/MAST', "institution responsible for creating this file"),
-                           ("DATE", str(date.today()), "file creation date"),
-                           ('PROCVER', __version__, 'software version'),
-                           ('RA_OBJ', center_coord.ra.deg, '[deg] right ascension'),
-                           ('DEC_OBJ', center_coord.dec.deg, '[deg] declination')])
-
-        cutout_hdulist = fits.HDUList([hdu])
-        cutout_hdulist.writeto(output_paths[i], overwrite=True, checksum=True)
-
-    
-def _parse_size_input(cutout_size):
+def _parse_extensions(infile_exts, infile_name, user_exts):
     """
-    Makes the given cutout size into a length 2 array.
+    Given a list of image extensions available in the file with infile_name, cross-match with
+    user input extensions to figure out which extensions to use for cutout.
 
     Parameters
     ----------
-    cutout_size : int, array-like, `~astropy.units.Quantity`
-        The size of the cutout array. If ``cutout_size`` is a scalar number or a scalar 
-        `~astropy.units.Quantity`, then a square cutout of ``cutout_size`` will be created.  
-        If ``cutout_size`` has two elements, they should be in ``(ny, nx)`` order.  Scalar numbers 
-        in ``cutout_size`` are assumed to be in units of pixels. `~astropy.units.Quantity` objects 
-        must be in pixel or angular units.
+    infile_exts : array
+    infile_name : str
+    user_exts : int, list of ints, None, or 'all'
+        Optional, default None. Default is to cutout the first extension that has image data.
+        The user can also supply one or more extensions to cutout from (integers), or "all".
 
     Returns
     -------
     response : array
-        Length two cutout size array, in the form [ny, nx].
+        List of extensions to be cutout.
     """
-
-    # Making size into an array [ny, nx]
-    if np.isscalar(cutout_size):
-        cutout_size = np.repeat(cutout_size, 2)
-
-    if isinstance(cutout_size, u.Quantity):
-        cutout_size = np.atleast_1d(cutout_size)
-        if len(cutout_size) == 1:
-            cutout_size = np.repeat(cutout_size, 2)
-
-    if len(cutout_size) > 2:
-        warnings.warn("Too many dimensions in cutout size, only the first two will be used.",
-                      InputWarning)
-        cutout_size = cutout_size[:2]
-
-    return cutout_size
-
-       
-def fits_cut(input_files, coordinates, cutout_size, correct_wcs=False, drop_after=None, 
-             single_outfile=True, cutout_prefix="cutout", output_dir='.', verbose=False):
+ 
+    if len(infile_exts) == 0:
+        warnings.warn(f"No image extensions with data found in {infile_name}, skipping...",
+                      DataWarning)
+        return []
+            
+    if user_exts is None:
+        cutout_exts = infile_exts[:1]  # Take the first image extension
+    elif user_exts == 'all':
+        cutout_exts = infile_exts  # Take all the extensions
+    else:  # User input extentions
+        cutout_exts = [x for x in infile_exts if x in user_exts]
+        if len(cutout_exts) < len(user_exts):
+            warnings.warn((f"Not all requested extensions in {infile_name} are image extensions or have data, "
+                           f"extension(s) {','.join([x for x in user_exts if x not in cutout_exts])} will be skipped."),
+                          DataWarning)
+
+    return cutout_exts
+
+                    
+def fits_cut(input_files, coordinates, cutout_size, correct_wcs=False, extension=None, 
+             single_outfile=True, cutout_prefix="cutout", output_dir='.',
+             memory_only=False, verbose=False):
     """
     Takes one or more fits files with the same WCS/pointing, makes the same cutout in each file,
-    and returns the result either in a single fitsfile with one cutout per extension or in 
-    individual fits files.
+    and returns the result either in a single FITS file with one cutout per extension or in 
+    individual fits files. The memory_only flag allows the cutouts to be returned as 
+    `~astropy.io.fits.HDUList` objects rather than saving to disk.
 
     Note: No checking is done on either the WCS pointing or pixel scale. If images don't line up
     the cutouts will also not line up.
 
     Parameters
     ----------
     input_files : list
@@ -370,122 +206,180 @@
         `~astropy.units.Quantity`, then a square cutout of ``cutout_size`` will be created.  
         If ``cutout_size`` has two elements, they should be in ``(ny, nx)`` order.  Scalar numbers 
         in ``cutout_size`` are assumed to be in units of pixels. `~astropy.units.Quantity` objects 
         must be in pixel or angular units.
     correct_wcs : bool
         Default False. If true a new WCS will be created for the cutout that is tangent projected
         and does not include distortions.
+    extension : int, list of ints, None, or 'all'
+       Optional, default None. Default is to cutout the first extension that has image data.
+       The user can also supply one or more extensions to cutout from (integers), or 'all'.
     single_outfile : bool 
         Default True. If true return all cutouts in a single fits file with one cutout per extension,
         if False return cutouts in individual fits files. If returing a single file the filename will 
         have the form: <cutout_prefix>_<ra>_<dec>_<size x>_<size y>.fits. If returning multiple files
         each will be named: <original filemame base>_<ra>_<dec>_<size x>_<size y>.fits.
     cutout_prefix : str 
         Default value "cutout". Only used if single_outfile is True. A prefix to prepend to the cutout 
         filename. 
     output_dir : str
-        Defaul value '.'. The directory to save the cutout file(s) to.
+        Default value '.'. The directory to save the cutout file(s) to.
+    memory_only : bool
+        Default value False. If set to true, instead of the cutout file(s) being written to disk
+        the cutout(s) are returned as a list of `~astropy.io.fit.HDUList` objects. If set to
+        True cutout_prefix and output_dir are ignored, however single_outfile can still be used to
+        set the number of returned `~astropy.io.fits.HDUList` objects.
     verbose : bool
         Default False. If true intermediate information is printed.
 
     Returns
     -------
     response : str or list
         If single_outfile is True returns the single output filepath. Otherwise returns a list of all 
         the output filepaths.
+        If memory_only is True a list of `~astropy.io.fit.HDUList` objects is returned instead of
+        file name(s).
     """
 
-    # Dealing with deprecation
-    if drop_after is not None:
-        warnings.warn("Argument 'drop_after' is deprecated and will be ignored",
-                      AstropyDeprecationWarning)
-    
     if verbose:
         start_time = time()
             
     # Making sure we have an array of images
     if type(input_files) == str:
         input_files = [input_files]
 
+    # If a single extension is given, make it a list
+    if isinstance(extension, int):
+        extension = [extension]
+
     if not isinstance(coordinates, SkyCoord):
         coordinates = SkyCoord(coordinates, unit='deg')
 
     # Turning the cutout size into a 2 member array
-    cutout_size = _parse_size_input(cutout_size)
+    cutout_size = parse_size_input(cutout_size)
+
+    if verbose:
+        print(f"Number of input files: {len(input_files)}")
+        print(f"Cutting out {extension} extension(s)")
+        print(f"Center coordinate: {coordinates.to_string()} deg")
+        print(f"Cutout size: {cutout_size}")
 
     # Making the cutouts
     cutout_hdu_dict = {}
     num_empty = 0
+    num_cutouts = 0
     for in_fle in input_files:
         if verbose:
-            print("\n{}".format(in_fle))
+            print("\nCutting out {}".format(in_fle))
 
         warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
         with fits.open(in_fle, mode='denywrite', memmap=True) as hdulist:
-            try:
-                cutout = _hducut(hdulist[0], coordinates, cutout_size,
-                                 correct_wcs=correct_wcs, verbose=verbose)
-            except OSError as err:
-                warnings.warn("Error {} encountered when performing cutout on {}, skipping...".format(err, in_fle),
-                              DataWarning)
-        
-        # Check that there is data in the cutout image
-        if (cutout.data == 0).all() or (np.isnan(cutout.data)).all():
-            cutout.header["EMPTY"] = (True, "Indicates no data in cutout image.")
-            num_empty += 1
-            
-        cutout_hdu_dict[in_fle] = cutout
+
+            # Sorting out which extension(s) to cutout
+            all_inds = np.where([x.is_image and (x.data is not None) for x in hdulist])[0]
+            cutout_inds = _parse_extensions(all_inds, in_fle, extension)
+
+            num_cutouts += len(cutout_inds)
+            for ind in cutout_inds:            
+                try:
+                    cutout = _hducut(hdulist[ind], coordinates, cutout_size,
+                                     correct_wcs=correct_wcs, verbose=verbose)
+
+                    # Check that there is data in the cutout image
+                    if (cutout.data == 0).all() or (np.isnan(cutout.data)).all():
+                        cutout.header["EMPTY"] = (True, "Indicates no data in cutout image.")
+                        num_empty += 1
+
+                    # Adding a few more keywords
+                    cutout.header["ORIG_EXT"] = (ind, "Extension in original file.")
+                    if not cutout.header.get("ORIG_FLE") and hdulist[0].header.get("FILENAME"):
+                        cutout.header["ORIG_FLE"] = hdulist[0].header.get("FILENAME")
+                    
+                    cutout_hdu_dict[in_fle] = cutout_hdu_dict.get(in_fle, []) + [cutout]
+                    
+                except OSError as err:
+                    warnings.warn((f"Error {err} encountered when performing cutout on {in_fle}, "
+                                   f"extension {ind}, skipping..."),
+                                  DataWarning)
+                    num_empty += 1
 
     # If no cutouts contain data, raise exception
-    if num_empty == len(input_files):
+    if num_empty == num_cutouts:
         raise InvalidQueryError("Cutout contains no data! (Check image footprint.)")
 
     # Make sure the output directory exists
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
         
     # Setting up the output file(s) and writing them
+    cutout_path = None
     if single_outfile:
 
-        cutout_path = "{}_{:7f}_{:7f}_{}-x-{}_astrocut.fits".format(cutout_prefix,
-                                                                    coordinates.ra.value,
-                                                                    coordinates.dec.value,
-                                                                    str(cutout_size[0]).replace(' ', ''), 
-                                                                    str(cutout_size[1]).replace(' ', ''))
-        cutout_path = os.path.join(output_dir, cutout_path)
-        cutout_hdus = [cutout_hdu_dict[fle] for fle in input_files]
-        _save_single_fits(cutout_hdus, cutout_path, coordinates)
+        if verbose:
+            print("Returning cutout as single FITS")
 
-    else:
-        cutout_hdus = []
-        cutout_path = []
+        if not memory_only:
+            cutout_path = "{}_{:7f}_{:7f}_{}-x-{}_astrocut.fits".format(cutout_prefix,
+                                                                        coordinates.ra.value,
+                                                                        coordinates.dec.value,
+                                                                        str(cutout_size[0]).replace(' ', ''), 
+                                                                        str(cutout_size[1]).replace(' ', ''))
+            cutout_path = os.path.join(output_dir, cutout_path)
+            if verbose:
+                print("Cutout fits file: {}".format(cutout_path))
+            
+        cutout_hdus = [x for fle in cutout_hdu_dict for x in cutout_hdu_dict[fle]]    
+        cutout_fits = get_fits(cutout_hdus, coordinates, cutout_path)
+        
+        if memory_only:
+            all_hdus = [cutout_fits]
+        else:
+            all_paths = cutout_path
+
+    else:  # one output file per input file
+
+        if verbose:
+            print("Returning cutouts as individual FITS")
+            
+        if memory_only:
+            all_hdus = []
+        else:
+            all_paths = []
+            if verbose:
+                print("Cutout fits files:")
+            
         for fle in input_files:
-            cutout = cutout_hdu_dict[fle]
-            if cutout.header.get("EMPTY"):
-                warnings.warn("Cutout of {} contains to data and will not be written.".format(fle),
+            cutout_list = cutout_hdu_dict[fle]
+            if np.array([x.header.get("EMPTY") for x in cutout_list]).all():
+                warnings.warn(f"Cutout of {fle} contains no data and will not be written.",
                               DataWarning)
                 continue
 
-            cutout_hdus.append(cutout)
-
             filename = "{}_{:7f}_{:7f}_{}-x-{}_astrocut.fits".format(os.path.basename(fle).rstrip('.fits'),
                                                                      coordinates.ra.value,
                                                                      coordinates.dec.value,
                                                                      str(cutout_size[0]).replace(' ', ''), 
                                                                      str(cutout_size[1]).replace(' ', ''))
-            cutout_path.append(os.path.join(output_dir, filename))
-                
-        _save_multiple_fits(cutout_hdus, cutout_path, coordinates)
+            cutout_path = os.path.join(output_dir, filename)
+            cutout_fits = get_fits(cutout_list, coordinates, cutout_path)
 
+            if memory_only:
+                all_hdus.append(cutout_fits)
+            else:
+                all_paths.append(cutout_path)
+                if verbose:
+                    print(cutout_path)
         
     if verbose:
-        print("Cutout fits file(s): {}".format(cutout_path))
         print("Total time: {:.2} sec".format(time()-start_time))
 
-    return cutout_path
+    if memory_only:
+        return all_hdus
+    else:
+        return all_paths
 
 
 def normalize_img(img_arr, stretch='asinh', minmax_percent=None, minmax_value=None, invert=False):
     """
     Apply given stretch and scaling to an image array.
 
     Parameters
@@ -551,15 +445,15 @@
         norm_img = 255 - norm_img
 
     return norm_img
 
 
 def img_cut(input_files, coordinates, cutout_size, stretch='asinh', minmax_percent=None,
             minmax_value=None, invert=False, img_format='jpg', colorize=False,
-            cutout_prefix="cutout", output_dir='.', drop_after=None, verbose=False):
+            cutout_prefix="cutout", output_dir='.', extension=None, verbose=False):
     """
     Takes one or more fits files with the same WCS/pointing, makes the same cutout in each file,
     and returns the result either as a single color image or in individual image files.
 
     Note: No checking is done on either the WCS pointing or pixel scale. If images don't line up
     the cutouts will also not line up.
 
@@ -597,136 +491,126 @@
         Optional, default False.  If True a single color image is produced as output, and it is expected
         that three files are given as input.
     cutout_prefix : str 
         Default value "cutout". Only used when producing a color image. A prefix to prepend to the 
         cutout filename. 
     output_dir : str
         Defaul value '.'. The directory to save the cutout file(s) to.
+    extension : int, list of ints, None, or 'all'
+        Optional, default None. Default is to cutout the first extension that has image data.
+        The user can also supply one or more extensions to cutout from (integers), or "all".
     verbose : bool
         Default False. If true intermediate information is printed.
 
     Returns
     -------
     response : str or list
         If colorize is True returns the single output filepath. Otherwise returns a list of all 
         the output filepaths.
     """
-
-    # Dealing with deprecation
-    if drop_after is not None:
-        warnings.warn("Argument 'drop_after' is deprecated and will be ignored",
-                      AstropyDeprecationWarning)
         
     if verbose:
         start_time = time()
             
     # Making sure we have an array of images
     if type(input_files) == str:
         input_files = [input_files]
-    
-    # Doing image checks for color images
-    if colorize:
-        if len(input_files) < 3:
-            raise InvalidInputError("Color cutouts require 3 imput files (RGB).")
-        if len(input_files) > 3:
-            warnings.warn("Too many inputs for a color cutout, only the first three will be used.",
-                          InputWarning)
-            input_files = input_files[:3]
             
     if not isinstance(coordinates, SkyCoord):
         coordinates = SkyCoord(coordinates, unit='deg')
 
     # Turning the cutout size into a 2 member array
-    cutout_size = _parse_size_input(cutout_size)
+    cutout_size = parse_size_input(cutout_size)
 
     # Applying the default scaling
     if (minmax_percent is None) and (minmax_value is None):
         minmax_percent = [0.5, 99.5]
         
     # Making the cutouts
     cutout_hdu_dict = {}
     for in_fle in input_files:
         if verbose:
             print("\n{}".format(in_fle))
-        hdulist = fits.open(in_fle, mode='denywrite', memmap=True)
-        cutout = _hducut(hdulist[0], coordinates, cutout_size,
-                         correct_wcs=False, verbose=verbose)
-        hdulist.close()
-
-        # We just want the data array
-        cutout = cutout.data
-        
-        # Applying the appropriate normalization parameters
-        normalized_cutout = normalize_img(cutout, stretch, minmax_percent, minmax_value, invert)
-        
-        # Check that there is data in the cutout image
-        if not (cutout == 0).all():
-            cutout_hdu_dict[in_fle] = normalized_cutout
+
+
+        warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
+        with fits.open(in_fle, mode='denywrite', memmap=True) as hdulist:
+
+            # Sorting out which extension(s) to cutout
+            all_inds = np.where([x.is_image and (x.data is not None) for x in hdulist])[0]
+            cutout_inds = _parse_extensions(all_inds, in_fle, extension)
+
+            for ind in cutout_inds:   
+                try:
+                    cutout = _hducut(hdulist[ind], coordinates, cutout_size, correct_wcs=False, verbose=verbose)
+
+                    # We just want the data array
+                    cutout = cutout.data
+        
+                    # Applying the appropriate normalization parameters
+                    normalized_cutout = normalize_img(cutout, stretch, minmax_percent, minmax_value, invert)
+        
+                    # Check that there is data in the cutout image
+                    if not (cutout == 0).all():
+                        cutout_hdu_dict[in_fle] = cutout_hdu_dict.get(in_fle, []) + [normalized_cutout]
+                    
+                except OSError as err:
+                    warnings.warn("Error {} encountered when performing cutout on {}, skipping...".format(err, in_fle),
+                                  DataWarning)
 
     # If no cutouts contain data, raise exception
     if not cutout_hdu_dict:
         raise InvalidQueryError("Cutout contains to data! (Check image footprint.)")
 
     # Make sure the output directory exists
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
         
     # Setting up the output file(s) and writing them
     if colorize:
+        cutouts = [x for fle in input_files for x in cutout_hdu_dict.get(fle, [])]
+        
+        # Doing checks correct number of cutouts
+        if len(cutouts) < 3:
+            raise InvalidInputError(("Color cutouts require 3 input images (RGB)."
+                                     "If you supplied 3 images one of the cutouts may have been empty."))
+        if len(cutouts) > 3:
+            warnings.warn("Too many inputs for a color cutout, only the first three will be used.",
+                          InputWarning)
+            cutouts = cutouts[:3]
 
+            
         cutout_path = "{}_{:7f}_{:7f}_{}-x-{}_astrocut.{}".format(cutout_prefix,
                                                                   coordinates.ra.value,
                                                                   coordinates.dec.value,
                                                                   str(cutout_size[0]).replace(' ', ''), 
                                                                   str(cutout_size[1]).replace(' ', ''),
                                                                   img_format.lower()) 
         cutout_path = os.path.join(output_dir, cutout_path)
 
-        # TODO: This is not elegant or efficient, make it better
-        red = cutout_hdu_dict.get(input_files[0])
-        green = cutout_hdu_dict.get(input_files[1])
-        blue = cutout_hdu_dict.get(input_files[2])
-
-        cshape = ()
-        for cutout in [red, green, blue]:
-            if cutout is not None:
-                cshape = cutout.shape
-                break
-
-        if red is None:
-            red = np.zeros(cshape)
-        if green is None:
-            green = np.zeros(cshape)
-        if blue is None:
-            blue = np.zeros(cshape)
-
-        Image.fromarray(np.dstack([red, green, blue]).astype(np.uint8)).save(cutout_path)
+        Image.fromarray(np.dstack([cutouts[0], cutouts[1], cutouts[2]]).astype(np.uint8)).save(cutout_path)
           
     else:
  
         cutout_path = []
         for fle in input_files:
-            cutout = cutout_hdu_dict.get(fle)
-            if cutout is None:
-                warnings.warn("Cutout of {} contains to data and will not be written.".format(fle),
-                              DataWarning)
-                continue
 
-            file_path = "{}_{:7f}_{:7f}_{}-x-{}_astrocut.{}".format(os.path.basename(fle).rstrip('.fits'),
-                                                                    coordinates.ra.value,
-                                                                    coordinates.dec.value,
-                                                                    str(cutout_size[0]).replace(' ', ''), 
-                                                                    str(cutout_size[1]).replace(' ', ''),
-                                                                    img_format.lower())
-            file_path = os.path.join(output_dir, file_path)
-            cutout_path.append(file_path)
+            for i, cutout in enumerate(cutout_hdu_dict.get(fle)):
+
+
+                file_path = "{}_{:7f}_{:7f}_{}-x-{}_astrocut_{}.{}".format(os.path.basename(fle).rstrip('.fits'),
+                                                                           coordinates.ra.value,
+                                                                           coordinates.dec.value,
+                                                                           str(cutout_size[0]).replace(' ', ''), 
+                                                                           str(cutout_size[1]).replace(' ', ''),
+                                                                           i,
+                                                                           img_format.lower())
+                file_path = os.path.join(output_dir, file_path)
+                cutout_path.append(file_path)
             
-            Image.fromarray(cutout).save(file_path)
+                Image.fromarray(cutout).save(file_path)
         
     if verbose:
         print("Cutout fits file(s): {}".format(cutout_path))
         print("Total time: {:.2} sec".format(time()-start_time))
 
     return cutout_path
-    
-    
-
```

### Comparing `astrocut-0.8/astrocut/exceptions.py` & `astrocut-0.9/astrocut/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/make_cube.py` & `astrocut-0.9/astrocut/make_cube.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/tests/data/ex_ffi_wcs.txt` & `astrocut-0.9/astrocut/tests/data/ex_ffi_wcs.txt`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/tests/test_cube_cut.py` & `astrocut-0.9/astrocut/tests/test_cube_cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     assert "256.880000_6.380000_8x15_astrocut.fits" in out_file
     
     xmin, xmax = myfactory.cutout_lims[0]
     ymin, ymax = myfactory.cutout_lims[1]
     
     assert (xmax-xmin) == 8
     assert (ymax-ymin) == 15
-
+    
     cutout_size = [1*u.arcsec, 5*u.arcsec]
     out_file = myfactory.cube_cut(cube_file, coord, cutout_size, verbose=False)
     assert "256.880000_6.380000_1x1_astrocut.fits" in out_file
     
     xmin, xmax = myfactory.cutout_lims[0]
     ymin, ymax = myfactory.cutout_lims[1]
```

### Comparing `astrocut-0.8/astrocut/tests/test_cutout_processing.py` & `astrocut-0.9/astrocut/tests/test_cutout_processing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import os 
 import numpy as np
-import os
 
 from astropy.io import fits
 from astropy.utils.data import get_pkg_data_filename
 from astropy.wcs import WCS
+from astropy.coordinates import SkyCoord
 from astropy.table import Table
 from astropy.time import Time
 
-from .utils_for_test import create_test_ffis
-from .. import cutout_processing, CubeFactory, CutoutFactory
+from .utils_for_test import create_test_ffis, create_test_imgs
+from .. import cutout_processing, cutouts, CubeFactory, CutoutFactory
+
 
 # Example FFI WCS for testing
 with open(get_pkg_data_filename('data/ex_ffi_wcs.txt'), "r") as FLE:
     WCS_STR = FLE.read()
 
 
 def test_combine_headers():
@@ -97,42 +99,14 @@
     wcs_obj = WCS(WCS_STR, relax=True)
     bounds = np.array([[0, 4], [0, 6]])
 
     args = cutout_processing._get_args(bounds, wcs_obj)
     assert args["coordinates"] == wcs_obj.pixel_to_world(2, 3)
     assert args["size"] == (6, 4)
 
-    
-def test_path_to_footprints():
-
-    img_wcs = WCS(WCS_STR, relax=True)
-    size = [4, 5]
-
-    xs = [10, 20, 30, 40, 50]
-    ys = [1000, 950, 900, 810, 800]
-    path = img_wcs.pixel_to_world(xs, ys)
-
-    footprints = cutout_processing.path_to_footprints(path, size, img_wcs)
-    assert len(footprints) == 1
-
-    assert (np.max(xs) - np.min(xs) + size[0]) == footprints[0]["size"][1]
-    assert (np.max(ys) - np.min(ys) + size[1]) == footprints[0]["size"][0]
-
-    cent_x = (np.max(xs) - np.min(xs) + size[0])//2 + np.min(xs) - size[0]/2 
-    cent_y = (np.max(ys) - np.min(ys) + size[1])//2 + np.min(ys) - size[1]/2 
-    assert (img_wcs.pixel_to_world([cent_x], [cent_y]) == footprints[0]["coordinates"]).all()
-
-    # Lowering the max pixels so we force >1 footprint
-    max_pixels = 100
-    footprints = cutout_processing.path_to_footprints(path, size, img_wcs, max_pixels)
-
-    assert len(footprints) == 5
-    for fp in footprints:
-        assert np.multiply(*fp["size"]) <= max_pixels
-
 
 def test_moving_target_focus(tmpdir):
 
     # Making the test cube/cutout
     cube_maker = CubeFactory()
     
     img_sz = 1000
@@ -164,14 +138,42 @@
     times = Time(Table(fits.getdata(cutout_file, 1))["TIME"].data[:len(coords)*2:2] + 2457000, format="jd")
     path = Table({"time": times, "position": coords})
 
     mt_cutout_table = cutout_processing._moving_target_focus(path, size, [cutout_file])
     assert mt_cutout_table["TIME"].max() == (times.jd[-1] - 2457000)
     assert len(mt_cutout_table) > len(path)
 
+
+def test_path_to_footprints():
+
+    img_wcs = WCS(WCS_STR, relax=True)
+    size = [4, 5]
+
+    xs = [10, 20, 30, 40, 50]
+    ys = [1000, 950, 900, 810, 800]
+    path = img_wcs.pixel_to_world(xs, ys)
+
+    footprints = cutout_processing.path_to_footprints(path, size, img_wcs)
+    assert len(footprints) == 1
+
+    assert (np.max(xs) - np.min(xs) + size[0]) == footprints[0]["size"][1]
+    assert (np.max(ys) - np.min(ys) + size[1]) == footprints[0]["size"][0]
+
+    cent_x = (np.max(xs) - np.min(xs) + size[0])//2 + np.min(xs) - size[0]/2 
+    cent_y = (np.max(ys) - np.min(ys) + size[1])//2 + np.min(ys) - size[1]/2 
+    assert (img_wcs.pixel_to_world([cent_x], [cent_y]) == footprints[0]["coordinates"]).all()
+
+    # Lowering the max pixels so we force >1 footprint
+    max_pixels = 100
+    footprints = cutout_processing.path_to_footprints(path, size, img_wcs, max_pixels)
+
+    assert len(footprints) == 5
+    for fp in footprints:
+        assert np.multiply(*fp["size"]) <= max_pixels
+
     
 def test_configure_bintable_header(tmpdir):
     
 
     # Making the test cube/cutout/table we need
     cube_maker = CubeFactory()
     
@@ -250,15 +252,91 @@
     assert "path" in out_file
 
     hdu = fits.open(out_file)
     assert len(hdu) == 2
     assert hdu[0].header["DATE"] == Time.now().to_value('iso', subfmt='date')
     assert hdu[0].header["OBJECT"] == ""
     hdu.close()
-    
 
-    
 
-    
+def test_default_combine():
+    """
+    The build_default_combine_function function uses the input hdus
+    to determine which pixels will be used by the combiner function
+    when combining images. The returned combiner function applies
+    that mask before taking the mean of all non-masked pixels to get the
+    output image.
+    """
+
+    hdu_1 = fits.ImageHDU(np.array([[1, 1], [0, 0]]))
+    hdu_2 = fits.ImageHDU(np.array([[0, 0], [1, 1]]))
+
+    # Two input arrays no overlapping pixels
+    combine_func = cutout_processing.build_default_combine_function([hdu_1, hdu_2], 0)
+    assert (combine_func([hdu_1, hdu_2]) == 1).all()
+    assert (combine_func([hdu_2, hdu_1]) == 0).all()
+
+    # Three input arrays overlapping pixels
+    hdu_3 = fits.ImageHDU(np.array([[0, 1], [1, 0]]))
+    combine_func = cutout_processing.build_default_combine_function([hdu_1, hdu_2, hdu_3], 0)
+
+    im4 = fits.ImageHDU(np.array([[4, 5], [0, 0]]))
+    im5 = fits.ImageHDU(np.array([[0, 0], [4, 5]]))
+    im6 = fits.ImageHDU(np.array([[0, 3], [8, 0]]))
+    comb_img = combine_func([im4, im5, im6])
+    assert (comb_img == [[4, 4], [6, 5]]).all()
+
+    im4 = fits.ImageHDU(np.array([[4, 5], [-3, 8]]))
+    im5 = fits.ImageHDU(np.array([[5, 2], [4, 5]]))
+    im6 = fits.ImageHDU(np.array([[4, 3], [8, 9]]))
+    assert (combine_func([im4, im5, im6]) == comb_img).all()
+
+    # Two input arrays, with nans and a missing pixel
+    hdu_1 = fits.ImageHDU(np.array([[1, np.nan], [np.nan, np.nan]]))
+    hdu_2 = fits.ImageHDU(np.array([[np.nan, np.nan], [1, 1]]))
+
+    combine_func = cutout_processing.build_default_combine_function([hdu_1, hdu_2])
+    assert np.allclose(combine_func([hdu_1, hdu_2]), [[1, np.nan], [1, 1]], equal_nan=True)
+
+
+def test_combiner(tmpdir):
+
+    test_images = create_test_imgs(50, 6, dir_name=tmpdir)
+    center_coord = SkyCoord("150.1163213 2.200973097", unit='deg')
+    cutout_size = 2
+
+    cutout_file_1 = cutouts.fits_cut(test_images[:3], center_coord, cutout_size, 
+                                     cutout_prefix="cutout_1", output_dir=tmpdir)
+    cutout_file_2 = cutouts.fits_cut(test_images[3:], center_coord, cutout_size, 
+                                     cutout_prefix="cutout_2", output_dir=tmpdir)
+
+    combiner = cutout_processing.CutoutsCombiner([cutout_file_1, cutout_file_2])
+
+    # Checking the load function
+    assert center_coord.separation(combiner.center_coord) == 0
+    assert len(combiner.input_hdulists) == 3
+    assert len(combiner.input_hdulists[0]) == 2
+
+    # Checking the combiner function was set properly
+    comb_1 = combiner.combine_images(combiner.input_hdulists[0])
+    combine_func = cutout_processing.build_default_combine_function(combiner.input_hdulists[0])
+    assert (comb_1 == combine_func(combiner.input_hdulists[0])).all()
+
+    # Running the combine function and checking the results
+    out_fle = combiner.combine(os.path.join(tmpdir, "combination.fits"))
+    comb_hdu = fits.open(out_fle)
+    assert len(comb_hdu) == 4
+    assert (comb_hdu[1].data == comb_1).all()
+    assert np.isclose(comb_hdu[0].header['RA_OBJ'], center_coord.ra.deg)
+    assert np.isclose(comb_hdu[0].header['DEC_OBJ'], center_coord.dec.deg)
+    comb_hdu.close()
+
+    # Checking memory only input and output
+    input_fits_1 = fits.open(cutout_file_1)
+    input_fits_2 = fits.open(cutout_file_2)
+
+    combiner = cutout_processing.CutoutsCombiner([input_fits_1, input_fits_2])
+    assert center_coord.separation(combiner.center_coord) == 0
+    assert len(combiner.input_hdulists) == 3
+    assert len(combiner.input_hdulists[0]) == 2
 
-    
-    
+    comb_hdu = combiner.combine(memory_only=True)
```

### Comparing `astrocut-0.8/astrocut/tests/test_cutouts.py` & `astrocut-0.9/astrocut/tests/test_cutouts.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,117 +4,20 @@
 from os import path
 from re import findall
 
 from astropy.io import fits
 from astropy import wcs
 from astropy.coordinates import SkyCoord
 from astropy import units as u
-from astropy.utils.exceptions import AstropyDeprecationWarning
 
 from PIL import Image
 
 from .utils_for_test import create_test_imgs
 from .. import cutouts
-from ..exceptions import InputWarning, InvalidInputError, InvalidQueryError
-
-
-def test_get_cutout_limits():
-
-    test_img_wcs_kwds = fits.Header(cards=[('NAXIS', 2, 'number of array dimensions'),
-                                           ('NAXIS1', 20, ''),
-                                           ('NAXIS2', 30, ''),
-                                           ('CTYPE1', 'RA---TAN', 'Right ascension, gnomonic projection'),
-                                           ('CTYPE2', 'DEC--TAN', 'Declination, gnomonic projection'),
-                                           ('CRVAL1', 100, '[deg] Coordinate value at reference point'),
-                                           ('CRVAL2', 20, '[deg] Coordinate value at reference point'),
-                                           ('CRPIX1', 10, 'Pixel coordinate of reference point'),
-                                           ('CRPIX2', 15, 'Pixel coordinate of reference point'),
-                                           ('CDELT1', 1.0, '[deg] Coordinate increment at reference point'),
-                                           ('CDELT2', 1.0, '[deg] Coordinate increment at reference point'),
-                                           ('WCSAXES', 2, 'Number of coordinate axes'),
-                                           ('PC1_1', 1, 'Coordinate transformation matrix element'),
-                                           ('PC2_2', 1, 'Coordinate transformation matrix element'),
-                                           ('CUNIT1', 'deg', 'Units of coordinate increment and value'),
-                                           ('CUNIT2', 'deg', 'Units of coordinate increment and value')])
-    
-    test_img_wcs = wcs.WCS(test_img_wcs_kwds)
-
-    center_coord = SkyCoord("100 20", unit='deg')
-    cutout_size = [10, 10]
-
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert (lims[0, 1] - lims[0, 0]) == (lims[1, 1] - lims[1, 0])
-    assert (lims == np.array([[4, 14], [9, 19]])).all()
-
-    cutout_size = [10, 5]
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert (lims[0, 1] - lims[0, 0]) == 10
-    assert (lims[1, 1] - lims[1, 0]) == 5
-
-    cutout_size = [.1, .1]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert (lims[0, 1] - lims[0, 0]) == (lims[1, 1] - lims[1, 0])
-    assert (lims[0, 1] - lims[0, 0]) == 1
-
-    cutout_size = [4, 5]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert (lims[0, 1] - lims[0, 0]) == 4
-    assert (lims[1, 1] - lims[1, 0]) == 5
-
-    center_coord = SkyCoord("90 20", unit='deg')
-    cutout_size = [4, 5]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert lims[0, 0] < 0
-
-    center_coord = SkyCoord("100 5", unit='deg')
-    cutout_size = [4, 5]*u.pixel
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    assert lims[1, 0] < 0
-
-
-def test_get_cutout_wcs():
-    test_img_wcs_kwds = fits.Header(cards=[('NAXIS', 2, 'number of array dimensions'),
-                                           ('NAXIS1', 20, ''),
-                                           ('NAXIS2', 30, ''),
-                                           ('CTYPE1', 'RA---TAN', 'Right ascension, gnomonic projection'),
-                                           ('CTYPE2', 'DEC--TAN', 'Declination, gnomonic projection'),
-                                           ('CRVAL1', 100, '[deg] Coordinate value at reference point'),
-                                           ('CRVAL2', 20, '[deg] Coordinate value at reference point'),
-                                           ('CRPIX1', 10, 'Pixel coordinate of reference point'),
-                                           ('CRPIX2', 15, 'Pixel coordinate of reference point'),
-                                           ('CDELT1', 1.0, '[deg] Coordinate increment at reference point'),
-                                           ('CDELT2', 1.0, '[deg] Coordinate increment at reference point'),
-                                           ('WCSAXES', 2, 'Number of coordinate axes'),
-                                           ('PC1_1', 1, 'Coordinate transformation matrix element'),
-                                           ('PC2_2', 1, 'Coordinate transformation matrix element'),
-                                           ('CUNIT1', 'deg', 'Units of coordinate increment and value'),
-                                           ('CUNIT2', 'deg', 'Units of coordinate increment and value')])
-    
-    test_img_wcs = wcs.WCS(test_img_wcs_kwds)
-
-    center_coord = SkyCoord("100 20", unit='deg')
-    cutout_size = [4, 5]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    cutout_wcs = cutouts._get_cutout_wcs(test_img_wcs, lims)
-    assert (cutout_wcs.wcs.crval == [100, 20]).all()
-    assert (cutout_wcs.wcs.crpix == [3, 4]).all()
-
-    center_coord = SkyCoord("100 5", unit='deg')
-    cutout_size = [4, 5]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    cutout_wcs = cutouts._get_cutout_wcs(test_img_wcs, lims)
-    assert (cutout_wcs.wcs.crval == [100, 20]).all()
-    assert (cutout_wcs.wcs.crpix == [3, 19]).all()
-
-    center_coord = SkyCoord("110 20", unit='deg')
-    cutout_size = [10, 10]*u.deg
-    lims = cutouts._get_cutout_limits(test_img_wcs, center_coord, cutout_size)
-    cutout_wcs = cutouts._get_cutout_wcs(test_img_wcs, lims)
-    assert (cutout_wcs.wcs.crval == [100, 20]).all()
-    assert (cutout_wcs.wcs.crpix == [-3, 6]).all() 
+from ..exceptions import InputWarning, InvalidInputError, InvalidQueryError 
 
 
 def test_fits_cut(tmpdir, capsys):
 
     test_images = create_test_imgs(50, 6, dir_name=tmpdir)
 
     # Single file
@@ -138,41 +41,45 @@
     sra, sdec = cut_wcs.all_pix2world(cutout_size/2, cutout_size/2, 0)
     assert round(float(sra), 4) == round(center_coord.ra.deg, 4)
     assert round(float(sdec), 4) == round(center_coord.dec.deg, 4)
 
     cutout_hdulist.close()
 
     # Multiple files
-    with pytest.warns(AstropyDeprecationWarning):
-        cutout_files = cutouts.fits_cut(test_images, center_coord, cutout_size,
-                                        drop_after="Dummy1", single_outfile=False, output_dir=tmpdir)
+    cutout_files = cutouts.fits_cut(test_images, center_coord, cutout_size, single_outfile=False, output_dir=tmpdir)
 
     assert isinstance(cutout_files, list)
     assert len(cutout_files) == len(test_images)
 
     cutout_hdulist = fits.open(cutout_files[0])
-    assert len(cutout_hdulist) == 1
+    assert len(cutout_hdulist) == 2
     
-    cut1 = cutout_hdulist[0].data
+    cut1 = cutout_hdulist[1].data
     assert cut1.shape == (cutout_size, cutout_size)
     
-    cut_wcs = wcs.WCS(cutout_hdulist[0].header)
+    cut_wcs = wcs.WCS(cutout_hdulist[1].header)
     sra, sdec = cut_wcs.all_pix2world(cutout_size/2, cutout_size/2, 0)
     assert round(float(sra), 4) == round(center_coord.ra.deg, 4)
     assert round(float(sdec), 4) == round(center_coord.dec.deg, 4)
 
     cutout_hdulist.close()
 
     # Output directory that has to be made
     cutout_files = cutouts.fits_cut(test_images, center_coord, cutout_size,
                                     output_dir=path.join(tmpdir, "cutout_files"), single_outfile=False)
 
     assert isinstance(cutout_files, list)
     assert len(cutout_files) == len(test_images)
-    assert "cutout_files" in cutout_files[0] 
+    assert "cutout_files" in cutout_files[0]
+
+    # Memory only flag
+    cutout_list = cutouts.fits_cut(test_images, center_coord, cutout_size, single_outfile=True, memory_only=True)
+    assert isinstance(cutout_list, list)
+    assert len(cutout_list) == 1
+    assert isinstance(cutout_list[0], fits.HDUList)
     
     # Do an off the edge test
     center_coord = SkyCoord("150.1163213 2.2005731", unit='deg')
     cutout_file = cutouts.fits_cut(test_images, center_coord, cutout_size, single_outfile=True, output_dir=tmpdir)
     assert isinstance(cutout_file, str)
     
     cutout_hdulist = fits.open(cutout_file)
@@ -337,32 +244,29 @@
     img_arr = np.array([[1, 0], [.25, .75]])
     norm_img = cutouts.normalize_img(img_arr, stretch='asinh', minmax_percent=[0.7, 99.3])
     with pytest.warns(InputWarning):
         test_img = cutouts.normalize_img(img_arr, stretch='asinh', minmax_value=[5, 2000], minmax_percent=[0.7, 99.3])
     assert (test_img == norm_img).all()
 
 
-
 def test_img_cut(tmpdir, capsys):
 
     test_images = create_test_imgs(50, 6, dir_name=tmpdir)
     center_coord = SkyCoord("150.1163213 2.200973097", unit='deg')
     cutout_size = 10
 
     # Basic jpg image
     jpg_files = cutouts.img_cut(test_images, center_coord, cutout_size, output_dir=tmpdir)
     
     assert len(jpg_files) == len(test_images)
     with open(jpg_files[0], 'rb') as IMGFLE:
         assert IMGFLE.read(3) == b'\xFF\xD8\xFF'  # JPG
 
     # Png (single input file, not as list)
-    with pytest.warns(AstropyDeprecationWarning):
-        img_files = cutouts.img_cut(test_images[0], center_coord, cutout_size, img_format='png',
-                                    output_dir=tmpdir, drop_after="")
+    img_files = cutouts.img_cut(test_images[0], center_coord, cutout_size, img_format='png', output_dir=tmpdir)
     with open(img_files[0], 'rb') as IMGFLE:
         assert IMGFLE.read(8) == b'\x89\x50\x4E\x47\x0D\x0A\x1A\x0A'  # PNG
     assert len(img_files) == 1
 
     # Color image
     color_jpg = cutouts.img_cut(test_images[:3], center_coord, cutout_size, colorize=True, output_dir=tmpdir)
     img = Image.open(color_jpg)
@@ -389,14 +293,13 @@
 
     # test color image where one of the images is all zeros
     hdu = fits.open(test_images[0], mode='update')
     hdu[0].data[:, :] = 0
     hdu.flush()
     hdu.close()
 
-    color_png = cutouts.img_cut(test_images[:3], center_coord, cutout_size, colorize=True,
-                                img_format='png', output_dir=tmpdir)
-    img = Image.open(color_png)
-    assert img.mode == 'RGB'
-    assert (np.asarray(img)[:, :, 0] == 0).all()
+    with pytest.raises(InvalidInputError):
+        cutouts.img_cut(test_images[:3], center_coord, cutout_size,
+                        colorize=True, img_format='png', output_dir=tmpdir)
+
```

### Comparing `astrocut-0.8/astrocut/tests/test_make_cube.py` & `astrocut-0.9/astrocut/tests/test_make_cube.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/astrocut/tests/utils_for_test.py` & `astrocut-0.9/astrocut/tests/utils_for_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def add_keywords(hdu, extname, time_increment, primary=False):
     """
     Add a bunch of required keywords (mostly fake values).
     """
     
-    hdu.header['extname'] = 'CAMERA.CCD 1.1 cal'
+    hdu.header['extname'] = extname
     hdu.header['camera'] = 1
     hdu.header['ccd'] = 1
     hdu.header['tstart'] = float(time_increment)
     hdu.header['tstop'] = float(time_increment+1)
     hdu.header['date-obs'] = '2019-05-11T00:08:26.816Z'
     hdu.header['date-end'] = '2019-05-11T00:38:26.816Z'
     hdu.header['barycorr'] = 5.0085597E-03
```

### Comparing `astrocut-0.8/astrocut/utils/wcs_fitting.py` & `astrocut-0.9/astrocut/utils/wcs_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     # use (1, 0, 0, 1) as initial guess, in case input wcs was passed in
     # and cd terms are way off.
     p0 = np.concatenate([wcs.wcs.cd.flatten(), wcs.wcs.crpix.flatten()])
     
     xpmin, xpmax, ypmin, ypmax = xp.min(), xp.max(), yp.min(), yp.max()
     if xpmin==xpmax: xpmin, xpmax = xpmin-0.5, xpmax+0.5
     if ypmin==ypmax: ypmin, ypmax = ypmin-0.5, ypmax+0.5
-    
+
     fit = least_squares(_linear_wcs_fit, p0,
                         args=(lon, lat, xp, yp, wcs),
                         bounds=[[-np.inf,-np.inf,-np.inf,-np.inf, xpmin, ypmin],
                                 [ np.inf, np.inf, np.inf, np.inf, xpmax, ypmax]])
     wcs.wcs.crpix = np.array(fit.x[4:6])
     wcs.wcs.cd = np.array(fit.x[0:4].reshape((2, 2)))
```

### Comparing `astrocut-0.8/astrocut.egg-info/PKG-INFO` & `astrocut-0.9/astrocut.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrocut
-Version: 0.8
+Version: 0.9
 Summary: Cutout tools for astronomical images
 Home-page: https://astrocut.readthedocs.io
 Author: MAST Archive Developers
 Author-email: archive@stsci.edu
 License: BSD 3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -23,17 +23,21 @@
     :target: https://badge.fury.io/py/astrocut
     :alt: PyPi Status
     
 .. image:: https://readthedocs.org/projects/astrocut/badge/?version=latest
     :target: https://astrocut.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-Tools for making image cutouts from sets of TESS full frame images.
+Astrocut provides tools for making cutouts from sets of astronomical images with shared footprints. It is under active development.
 
-This package is under active development, and will ultimately grow to encompass a range of cutout activities relevant to images from many missions, however at this time it is focussed on the specific problem of creating Target Pixel File cutouts from sectors of TESS full frame images.
+Three main areas of functionality are included:
+
+- Solving the specific problem of creating image cutouts from sectors of Transiting Exoplanet Survey Satellite (TESS) full-frame images.
+- General fits file cutouts incuding from single images and sets of images with the shared WCS/pixel scale.
+- Cutout post-processing functionality, including centering cutouts along a path (for moving targets) and combining cutouts.
 
 Documentation is at https://astrocut.readthedocs.io.
 
 Project Status
 --------------
 .. image:: https://github.com/spacetelescope/astrocut/workflows/CI/badge.svg?branch=master
     :target: https://github.com/spacetelescope/astrocut/actions
```

### Comparing `astrocut-0.8/astrocut.egg-info/SOURCES.txt` & `astrocut-0.9/astrocut.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.codecov.yml
 .gitignore
 .readthedocs.yml
 CHANGES.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
@@ -28,30 +29,40 @@
 astrocut/extern/__init__.py
 astrocut/tests/__init__.py
 astrocut/tests/setup_package.py
 astrocut/tests/test_cube_cut.py
 astrocut/tests/test_cutout_processing.py
 astrocut/tests/test_cutouts.py
 astrocut/tests/test_make_cube.py
+astrocut/tests/test_utils.py
 astrocut/tests/utils_for_test.py
 astrocut/tests/data/ex_ffi_wcs.txt
 astrocut/utils/__init__.py
+astrocut/utils/utils.py
 astrocut/utils/wcs_fitting.py
 astrocut/utils/tests/__init__.py
 docs/Makefile
 docs/conf.py
-docs/index.rst
-docs/license.rst
+docs/index.html
 docs/make.bat
 docs/_static/AstroCut_medium.png
 docs/_static/AstroCut_thumb.png
 docs/_static/astrocut.css
+docs/_static/main.css
+docs/_templates/layout.html
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
+docs/astrocut/api.rst
+docs/astrocut/contents.rst
+docs/astrocut/file_formats.rst
 docs/astrocut/index.rst
 docs/astrocut/install.rst
+docs/astrocut/license.rst
 docs/astrocut/imgs/color_ex_cutout.png
+docs/astrocut/imgs/hapcut_combined.png
+docs/astrocut/imgs/hapcut_left.png
+docs/astrocut/imgs/hapcut_right.png
 docs/astrocut/imgs/png_ex_cutout.png
 licenses/LICENSE.rst
 licenses/README.rst
 licenses/TEMPLATE_LICENCE.rst
```

### Comparing `astrocut-0.8/docs/Makefile` & `astrocut-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/docs/_static/AstroCut_medium.png` & `astrocut-0.9/docs/_static/AstroCut_medium.png`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/docs/_static/AstroCut_thumb.png` & `astrocut-0.9/docs/_static/AstroCut_thumb.png`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/docs/astrocut/imgs/color_ex_cutout.png` & `astrocut-0.9/docs/astrocut/imgs/color_ex_cutout.png`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/docs/astrocut/imgs/png_ex_cutout.png` & `astrocut-0.9/docs/astrocut/imgs/png_ex_cutout.png`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/docs/astrocut/install.rst` & `astrocut-0.9/docs/astrocut/install.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-************
-Installation
-************
 
-
-Requirements
-============
-
-Astrocut has the following requirements:
-
-- `Astropy`_ 
-- `NumPy <http://www.numpy.org/>`_
-
-  
-Installing astrocut
-===================
+*******************  
+Installing Astrocut
+*******************
 
 Using pip
----------
+=========
 
 The easiest way to install Astrocut is using pip::
 
     pip install astrocut
 
 
 From source
------------
+===========
 
 To install the bleeding edge version from github without downloading,
 run the following command::
 
   pip git+https://github.com/spacetelescope/astrocut.git
 
 The latest development version of astrocut can be cloned from github
```

### Comparing `astrocut-0.8/docs/conf.py` & `astrocut-0.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # version in the build directory (if "python setup.py build_sphinx" is used).
 # Thus, any C-extensions that are needed to build the documentation will *not*
 # be accessible, and the documentation will not build correctly.
 
 import datetime
 import os
 import sys
+from importlib import import_module
 
 try:
     from sphinx_astropy.conf.v1 import *  # noqa
 except ImportError:
     print('ERROR: the documentation requires the sphinx-astropy package to be installed')
     sys.exit(1)
 
@@ -52,15 +53,14 @@
 
 # To perform a Sphinx version check that needs to be more specific than
 # major.minor, call `check_sphinx_version("x.y.z")` here.
 # check_sphinx_version("1.2.1")
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns.append('_templates')
 
 # This is added to the end of RST files - a good place to put substitutions to
 # be used globally.
 rst_epilog += """
 """
 
 # -- Project information ------------------------------------------------------
@@ -71,15 +71,15 @@
 copyright = '{0}, {1}'.format(
     datetime.datetime.now().year, setup_cfg['author'])
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
-__import__(setup_cfg['name'])
+import_module(setup_cfg['name'])
 package = sys.modules[setup_cfg['name']]
 
 # The short X.Y version.
 version = package.__version__.split('-', 1)[0]
 # The full version, including alpha/beta/rc tags.
 release = package.__version__
 
@@ -92,31 +92,32 @@
 # the options for this theme can be modified by overriding some of the
 # variables set in the global configuration. The variables set in the
 # global configuration are listed below, commented out.
 
 
 # Add any paths that contain custom themes here, relative to this directory.
 # To use a different custom theme, add the directory containing the theme.
-#html_theme_path = []
+#html_theme_path = ["_themes",]
+
+# Custome template path, adding custom css and home link
+templates_path = ["_templates"]
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
-#html_theme = None
-
+html_theme = 'sphinx_rtd_theme'
 
-html_theme_options = {
-    'logotext1': 'astro',  # white,  semi-bold
-    'logotext2': 'cut',  # orange, light
-    'logotext3': ':docs'   # white,  light
-    }
+def setup_style(app):
+    app.add_stylesheet("astrocut.css")
 
+master_doc='astrocut/contents'
+html_extra_path=['index.html']
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+html_sidebars = { '**': ['globaltoc.html', 'localtoc.html', 'searchbox.html'] }
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 html_logo = '_static/AstroCut_thumb.png'
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
@@ -132,15 +133,15 @@
 html_title = '{0} v{1}'.format(project, release)
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = project + 'doc'
 
 # Static files to copy after template files
 html_static_path = ['_static']
-html_style = 'astrocut.css'
+html_css_files = ['astrocut.css']
 
 
 # -- Options for LaTeX output -------------------------------------------------
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [('index', project + '.tex', project + u' Documentation',
@@ -153,23 +154,20 @@
 # (source start file, name, description, authors, manual section).
 man_pages = [('index', project.lower(), project + u' Documentation',
               [author], 1)]
 
 
 # -- Options for the edit_on_github extension ---------------------------------
 
-if eval(setup_cfg.get('edit_on_github')):
+if setup_cfg.get('edit_on_github').lower() == 'true':
+
     extensions += ['sphinx_astropy.ext.edit_on_github']
 
-    versionmod = __import__(setup_cfg['name'] + '.version')
     edit_on_github_project = setup_cfg['github_project']
-    if versionmod.version.release:
-        edit_on_github_branch = "v" + versionmod.version.version
-    else:
-        edit_on_github_branch = "master"
+    edit_on_github_branch = "main"
 
     edit_on_github_source_root = ""
     edit_on_github_doc_root = "docs"
 
 # -- Resolving issue number to links in changelog -----------------------------
 github_issues_url = 'https://github.com/{0}/issues/'.format(setup_cfg['github_project'])
```

### Comparing `astrocut-0.8/docs/make.bat` & `astrocut-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/licenses/LICENSE.rst` & `astrocut-0.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/licenses/TEMPLATE_LICENCE.rst` & `astrocut-0.9/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/setup.cfg` & `astrocut-0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 console_scripts = 
 	astropy-package-template-example = packagename.example_mod:main
 
 [options.extras_require]
 test = 
 	pytest-astropy
 docs = 
+	sphinx != 4.1.0
+	docutils == 0.16
 	sphinx-astropy
+	sphinx_rtd_theme >= 0.5.2
 
 [options.package_data]
 astrocut.tests = data/*
 
 [tool:pytest]
 testpaths = "astrocut" "docs"
 astropy_header = true
```

### Comparing `astrocut-0.8/setup.py` & `astrocut-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `astrocut-0.8/tox.ini` & `astrocut-0.9/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tox]
 envlist =
     py{36,37,38}-test{,-alldeps,-devdeps}{,-cov}
-    py{36,37,38}-test-numpy{116,117,118}
-    py{36,37,38}-test-astropy{30,40,lts}
+    py{36,37,38}-test-numpy{118,119,121}
+    py{36,37,38}-test-astropy{40,41,lts}
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
@@ -30,30 +30,30 @@
 #
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
-    numpy116: with numpy 1.16.*
-    numpy117: with numpy 1.17.*
     numpy118: with numpy 1.18.*
-    astropy30: with astropy 3.0.*
+    numpy119: with numpy 1.19.*
+    numpy121: with numpy 1.21.*
     astropy40: with astropy 4.0.*
+    astropy41: with astropy 4.1.*
     astropylts: with the latest astropy LTS
 
 # The following provides some specific pinnings for key packages
 deps =
 
-    numpy116: numpy==1.16.*
-    numpy117: numpy==1.17.*
     numpy118: numpy==1.18.*
+    numpy119: numpy==1.19.*
+    numpy121: numpy==1.21.*
 
-    astropy30: astropy==3.0.*
     astropy40: astropy==4.0.*
+    astropy41: astropy==4.1.*
     astropylts: astropy==4.0.*
 
     devdeps: git+https://github.com/numpy/numpy.git#egg=numpy
     devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
@@ -66,14 +66,15 @@
     cov: pytest --pyargs astrocut {toxinidir}/docs --cov astrocut --cov-config={toxinidir}/setup.cfg {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
+deps= sphinx_rtd_theme
 commands =
     pip freeze
     sphinx-build -W -b html . _build/html
 
 [testenv:linkcheck]
 changedir = docs
 description = check the links in the HTML docs
```

