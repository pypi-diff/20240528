# Comparing `tmp/gaussian_step-2024.5.27.tar.gz` & `tmp/gaussian_step-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussian_step-2024.5.27.tar", last modified: Mon May 27 23:36:00 2024, max compression
+gzip compressed data, was "gaussian_step-2024.5.8.tar", last modified: Thu May  9 10:32:05 2024, max compression
```

## Comparing `gaussian_step-2024.5.27.tar` & `gaussian_step-2024.5.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.539948 gaussian_step-2024.5.27/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-27 23:36:00.539948 gaussian_step-2024.5.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.531948 gaussian_step-2024.5.27/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.535948 gaussian_step-2024.5.27/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.535948 gaussian_step-2024.5.27/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.535948 gaussian_step-2024.5.27/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.535948 gaussian_step-2024.5.27/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.535948 gaussian_step-2024.5.27/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.543948 gaussian_step-2024.5.27/gaussian_step/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 23:36:00.543948 gaussian_step-2024.5.27/gaussian_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.539948 gaussian_step-2024.5.27/gaussian_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/data/gaussian.ini
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/gaussian_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    37116 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/substep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/tk_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/gaussian_step/tk_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.539948 gaussian_step-2024.5.27/gaussian_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 23:36:00.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:35:46.000000 gaussian_step-2024.5.27/gaussian_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 23:36:00.543948 gaussian_step-2024.5.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:36:00.539948 gaussian_step-2024.5.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/tests/test_gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-27 23:35:39.000000 gaussian_step-2024.5.27/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.529320 gaussian_step-2024.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/gaussian.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36943 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/substep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:31:52.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/test_gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/versioneer.py
```

### Comparing `gaussian_step-2024.5.27/CONTRIBUTING.rst` & `gaussian_step-2024.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/HISTORY.rst` & `gaussian_step-2024.5.8/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 =======
 History
 =======
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.27/LICENSE` & `gaussian_step-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/PKG-INFO` & `gaussian_step-2024.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.5.27
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,18 +86,14 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.27/README.rst` & `gaussian_step-2024.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/Makefile` & `gaussian_step-2024.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/SEAMM inverted.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/SEAMM logo.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/molssi_main_logo.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/molssi_main_logo_inverted_white.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/molssi_square.png` & `gaussian_step-2024.5.8/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/_static/nsf.png` & `gaussian_step-2024.5.8/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/conf.py` & `gaussian_step-2024.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/developer_guide/installation.rst` & `gaussian_step-2024.5.8/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/getting_started/index.rst` & `gaussian_step-2024.5.8/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/index.rst` & `gaussian_step-2024.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/docs/make.bat` & `gaussian_step-2024.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/__init__.py` & `gaussian_step-2024.5.8/gaussian_step/__init__.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/data/gaussian.ini` & `gaussian_step-2024.5.8/gaussian_step/data/gaussian.ini`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/data/references.bib` & `gaussian_step-2024.5.8/gaussian_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/energy.py` & `gaussian_step-2024.5.8/gaussian_step/energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,31 +244,24 @@
             if restricted:
                 if multiplicity == 1:
                     keywords.add(f"RHF/{basis}")
                 else:
                     keywords.add(f"ROHF/{basis}")
             else:
                 keywords.add(f"UHF/{basis}")
-            # keywords.add("Guess=Mix")
         elif method[0:2] == "MP":
-            if restricted:
-                if multiplicity == 1:
-                    keywords.add(f"R{method}/{basis}")
-                else:
-                    keywords.add(f"RO{method}/{basis}")
+            if restricted and multiplicity != 1 and isinstance(self, Energy):
+                keywords.add(f"RO{method}/{basis}")
             else:
-                keywords.add(f"U{method}/{basis}")
+                keywords.add(f"{method}/{basis}")
         elif method in ("CCSD", "CCSD(T)"):
-            if restricted:
-                if multiplicity == 1:
-                    keywords.add(f"R{method}/{basis}")
-                else:
-                    keywords.add(f"RO{method}/{basis}")
+            if restricted and multiplicity != 1 and isinstance(self, Energy):
+                keywords.add(f"RO{method}/{basis}")
             else:
-                keywords.add(f"U{method}/{basis}")
+                keywords.add(f"{method}/{basis}")
         elif method in ("CBS-4M", "CBS-QB3"):
             if isinstance(self, Energy):
                 if restricted and multiplicity != 1:
                     keywords.add(f"RO{method}")
                 else:
                     keywords.add(f"{method}")
             else:
@@ -323,20 +316,20 @@
             table = {
                 "Property": [],
                 "Value": [],
                 "Units": [],
             }
 
         metadata = gaussian_step.metadata["results"]
-        if "energy" not in data:
+        if "Total Energy" not in data:
             text += "Gaussian did not produce the energy. Something is wrong!"
             printer.normal(__(text, indent=self.indent + 4 * " "))
 
         for key in (
-            "energy",
+            "Total Energy",
             "Virial Ratio",
             "RMS Density",
             "Cluster Energy with triples",
             "Cluster Energy",
             "MP5 Energy",
             "MP4 Energy",
             "MP4SDQ Energy",
```

### Comparing `gaussian_step-2024.5.27/gaussian_step/energy_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/energy_step.py` & `gaussian_step-2024.5.8/gaussian_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/gaussian_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/gaussian_step.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/metadata.py` & `gaussian_step-2024.5.8/gaussian_step/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,20 +233,14 @@
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "gradients",
         "dimensionality": [3, "natoms"],
         "type": "float",
         "units": "E_h/a0",
         "format": ".6f",
     },
-    "nsteps": {
-        "calculation": ["optimization"],
-        "description": "optimization nsteps",
-        "dimensionality": "scalar",
-        "type": "integer",
-    },
     "model": {
         "description": "The model string",
         "dimensionality": "scalar",
         "type": "string",
     },
     "Virial Ratio": {
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
```

### Comparing `gaussian_step-2024.5.27/gaussian_step/optimization.py` & `gaussian_step-2024.5.8/gaussian_step/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,14 @@
         _, configuration = self.get_system_configuration(None)
 
         if configuration.n_atoms == 1:
             text += "System is an atom, so nothing to optimize."
         else:
             # Information about the optimization
             n_steps = data["Optimization Number of geometries"][0]
-            data["nsteps"] = n_steps
             if data["Geometry Optimization Converged"]:
                 text += f"The geometry optimization converged in {n_steps} steps."
             else:
                 text += (
                     f"Warning: The geometry optimization did not converge in {n_steps} "
                     "steps."
                 )
```

### Comparing `gaussian_step-2024.5.27/gaussian_step/optimization_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/optimization_step.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/substep.py` & `gaussian_step-2024.5.8/gaussian_step/substep.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/tk_energy.py` & `gaussian_step-2024.5.8/gaussian_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/tk_gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step/tk_optimization.py` & `gaussian_step-2024.5.8/gaussian_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/gaussian_step.egg-info/PKG-INFO` & `gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.5.27
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,18 +86,14 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.27/gaussian_step.egg-info/SOURCES.txt` & `gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/setup.py` & `gaussian_step-2024.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.27/versioneer.py` & `gaussian_step-2024.5.8/versioneer.py`

 * *Files identical despite different names*

