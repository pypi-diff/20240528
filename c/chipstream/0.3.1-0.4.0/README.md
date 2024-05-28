# Comparing `tmp/chipstream-0.3.1.tar.gz` & `tmp/chipstream-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chipstream-0.3.1.tar", last modified: Wed May 22 22:05:52 2024, max compression
+gzip compressed data, was "chipstream-0.4.0.tar", last modified: Tue May 28 06:08:24 2024, max compression
```

## Comparing `chipstream-0.3.1.tar` & `chipstream-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.347383 chipstream-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.335383 chipstream-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.335383 chipstream-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-22 22:05:49.000000 chipstream-0.3.1/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-22 22:05:49.000000 chipstream-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 22:05:49.000000 chipstream-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-22 22:05:49.000000 chipstream-0.3.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 22:05:49.000000 chipstream-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 22:05:52.347383 chipstream-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-22 22:05:49.000000 chipstream-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.339383 chipstream-0.3.1/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStream.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStream.ico
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStreamLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/ChipStreamLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/hook-chipstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_ChipStream.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_ChipStream.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_chipstream.iss_dummy
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 22:05:49.000000 chipstream-0.3.1/build-recipes/win_make_iss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.339383 chipstream-0.3.1/chipstream/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/cli/cli_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/chipstream/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/img/chipstream_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/gui/table_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-22 22:05:49.000000 chipstream-0.3.1/chipstream/path_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.347383 chipstream-0.3.1/chipstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 22:05:52.000000 chipstream-0.3.1/chipstream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/artwork/chipstream_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 22:05:49.000000 chipstream-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-22 22:05:49.000000 chipstream-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:05:52.347383 chipstream-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:05:52.343383 chipstream-0.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/requirements-full.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_gui_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-22 22:05:49.000000 chipstream-0.3.1/tests/test_path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.118247 chipstream-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.106247 chipstream-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.106247 chipstream-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-28 06:08:16.000000 chipstream-0.4.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-28 06:08:16.000000 chipstream-0.4.0/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-28 06:08:16.000000 chipstream-0.4.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-28 06:08:16.000000 chipstream-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 06:08:16.000000 chipstream-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-28 06:08:16.000000 chipstream-0.4.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 06:08:16.000000 chipstream-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-28 06:08:24.118247 chipstream-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-28 06:08:16.000000 chipstream-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.110247 chipstream-0.4.0/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/ChipStream.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/ChipStream.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/ChipStreamLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/ChipStreamLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/hook-chipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/macos_ChipStream.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/win_ChipStream.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/win_chipstream.iss_dummy
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 06:08:16.000000 chipstream-0.4.0/build-recipes/win_make_iss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.110247 chipstream-0.4.0/chipstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/chipstream/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/cli/cli_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/cli/cli_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/chipstream/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/chipstream/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/img/chipstream_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/gui/table_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 06:08:16.000000 chipstream-0.4.0/chipstream/path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/chipstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 06:08:24.000000 chipstream-0.4.0/chipstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/artwork/chipstream_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/artwork/chipstream_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/artwork/chipstream_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 06:08:16.000000 chipstream-0.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-28 06:08:16.000000 chipstream-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:08:24.118247 chipstream-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:08:24.114247 chipstream-0.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/requirements-full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/test_gui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 06:08:16.000000 chipstream-0.4.0/tests/test_path_cache.py
```

### Comparing `chipstream-0.3.1/.github/workflows/check.yml` & `chipstream-0.4.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/.github/workflows/deploy_github.yml` & `chipstream-0.4.0/.github/workflows/deploy_github.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/.github/workflows/deploy_pypi.yml` & `chipstream-0.4.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/.gitignore` & `chipstream-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/CHANGELOG` & `chipstream-0.4.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.4.0
+ - feat: CLI by default creates output file that contains no redundant
+   data and uses the input file as a basin; old behavior can be brought
+   back with the "--drain-basins" command-line option
+ - feat: implement same behavior for GUI as for CLI, with the
+   "Exploit basins" checkbox
+ - fix: show correct data PPID in CLI
+ - setup: bump dcnum from 0.19.1 to 0.20.1
+ - docs: add tool tips for most controls
 0.3.1
  - ref: migrate from QTableView to QTableWidget (issues with Windows 11)
 0.3.0
  - BREAKING CHANGE: major changes in dcnum postprocessing
  - feat: allow to select whether volume should be computed
  - feat: allow to select whether flickering correction should be done
  - feat: allow to specify number of events to analyze in CLI
```

### Comparing `chipstream-0.3.1/LICENSE` & `chipstream-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/PKG-INFO` & `chipstream-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.3.1
+Version: 0.4.0
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: dcnum>=0.19.1
+Requires-Dist: dcnum>=0.20.1
 Requires-Dist: h5py<4,>=3.0.0
 Requires-Dist: numpy<2,>=1.21
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == "cli"
 Provides-Extra: gui
 Requires-Dist: pyqt6; extra == "gui"
```

### Comparing `chipstream-0.3.1/README.rst` & `chipstream-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/ChipStream.icns` & `chipstream-0.4.0/build-recipes/ChipStream.icns`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/ChipStream.ico` & `chipstream-0.4.0/build-recipes/ChipStream.ico`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/Readme.md` & `chipstream-0.4.0/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/hook-chipstream.py` & `chipstream-0.4.0/build-recipes/hook-chipstream.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/macos_ChipStream.spec` & `chipstream-0.4.0/build-recipes/macos_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/macos_build_app.sh` & `chipstream-0.4.0/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/win_ChipStream.spec` & `chipstream-0.4.0/build-recipes/win_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/win_chipstream.iss_dummy` & `chipstream-0.4.0/build-recipes/win_chipstream.iss_dummy`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/build-recipes/win_make_iss.py` & `chipstream-0.4.0/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/__init__.py` & `chipstream-0.4.0/chipstream/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/cli/cli_common.py` & `chipstream-0.4.0/chipstream/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/cli/cli_main.py` & `chipstream-0.4.0/chipstream/cli/cli_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,18 @@
                    "extraction [µm].")
 @click.option("--limit-events", type=str, default="0",
               help="Limit events of events to analyze. This can be either "
                    "a number (e.g. '5000') or a range (e.g. '5000-7000'). "
                    "You can also specify a step size (e.g. '5000-7000-2' for "
                    "every second event). The convention follows Python slices "
                    "with 'n' substituting for 'None'.")
+@click.option("--drain-basins", type=str, is_flag=True,
+              help="Write all basin features from input to output file. This "
+                   "option trades computation time and small file size for "
+                   "an output file that contains all available features.")
 @click.option("-r", "--recursive", is_flag=True,
               help="Recurse into subdirectories.")
 @click.option("--num-cpus",
               type=click.IntRange(min=1, max=mp.cpu_count(), clamp=True),
               help="Number of processes to create."
               )
 @click.option("--dry-run", is_flag=True,
@@ -125,28 +129,28 @@
     background_kwargs=None,
     segmentation_method="thresh",
     segmentation_kwargs=None,
     feature_kwargs=None,
     gate_kwargs=None,
     pixel_size=0,
     limit_events="0",
+    drain_basins=False,
     recursive=False,
     num_cpus=None,
     dry_run=False,
     verbose=False,
     debug=False,
 ):
 
     if debug:
         click.secho("Running in debug mode (this will be slow)",
                     fg="yellow")
         verbose = True
 
     # Parse limit_frames to get the HDF5Data index_mapping
-
     if limit_events == "0":
         index_mapping = None
     elif limit_events.count("-"):
         vals = limit_events.split("-")
         assert len(vals) in [2, 3], "slice definition must have length 2 or 3"
         start = None if vals[0] == "n" else int(vals[0])
         stop = None if vals[1] == "n" else int(vals[1])
@@ -171,16 +175,17 @@
         background_method=background_method,
         background_kwargs=background_kwargs,
         segmentation_method=segmentation_method,
         segmentation_kwargs=segmentation_kwargs,
         feature_kwargs=feature_kwargs,
         gate_kwargs=gate_kwargs,
         pixel_size=pixel_size,
-        # Below this line are arguments that do not define the pipeline ID
         index_mapping=index_mapping,
+        # Below this line are arguments that do not define the pipeline ID
+        basin_strategy="drain" if drain_basins else "tap",
         num_cpus=num_cpus or mp.cpu_count(),
         dry_run=dry_run,
         debug=debug,
         )
 
     if recursive:
         failed = 0  # keeps track of files that failed to process
```

### Comparing `chipstream-0.3.1/chipstream/cli/cli_proc.py` & `chipstream-0.4.0/chipstream/cli/cli_proc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pathlib
 import time
-from typing import List
+from typing import List, Literal
 
 import click
 import dcnum.logic
 from dcnum.meta import ppid
 import dcnum.read
 
 
@@ -21,30 +21,33 @@
     background_method: str,
     background_kwargs: List[str],
     segmentation_method: str,
     segmentation_kwargs: List[str],
     feature_kwargs: List[str],
     gate_kwargs: List[str],
     pixel_size: float,
-    # Below this line are arguments that do not affect the pipeline ID
     index_mapping: int | slice | None,
+    # Below this line are arguments that do not affect the pipeline ID
+    basin_strategy: Literal["drain", "tap"],
     num_cpus: int,
     dry_run: bool,
     debug: bool,
 ):
     # Make sure the pixel size makes sense
     if pixel_size == 0:
         pixel_size = validate_pixel_size(data_path=path_in)
 
     if path_out is None:
         path_out = path_in.with_name(path_in.stem + "_dcn.rtdc")
     path_out.parent.mkdir(parents=True, exist_ok=True)
 
     # data keyword arguments
-    with dcnum.read.HDF5Data(path_in, pixel_size=pixel_size) as data:
+    data_kwargs = {"pixel_size": pixel_size,
+                   "index_mapping": index_mapping}
+    with dcnum.read.HDF5Data(path_in, **data_kwargs) as data:
         dat_id = data.get_ppid()
     click.echo(f"Data ID:\t{dat_id}")
 
     # background keyword arguments
     bg_kwargs = validate_background_kwargs(background_method,
                                            background_kwargs)
     bg_cls = cm.bg_methods[background_method]
@@ -84,25 +87,24 @@
         click.echo("Dry run complete")
         return 0
 
     job = dcnum.logic.DCNumPipelineJob(
         path_in=path_in,
         path_out=path_out,
         data_code="hdf",
-        data_kwargs={"pixel_size": pixel_size,
-                     "index_mapping": index_mapping},
+        data_kwargs=data_kwargs,
         background_code=bg_cls.get_ppid_code(),
         background_kwargs=bg_kwargs,
         segmenter_code=seg_cls.get_ppid_code(),
         segmenter_kwargs=seg_kwargs,
         feature_code=feat_cls.get_ppid_code(),
         feature_kwargs=feat_kwargs,
         gate_code=gate_cls.get_ppid_code(),
         gate_kwargs=gate_kwargs,
-        no_basins_in_output=True,
+        basin_strategy=basin_strategy,
         num_procs=num_cpus,
         debug=debug,
     )
 
     runner = dcnum.logic.DCNumJobRunner(job)
     runner.start()
     strlen = 0
```

### Comparing `chipstream-0.3.1/chipstream/cli/cli_valid.py` & `chipstream-0.4.0/chipstream/cli/cli_valid.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/gui/__init__.py` & `chipstream-0.4.0/chipstream/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/gui/img/chipstream_icon.png` & `chipstream-0.4.0/chipstream/gui/img/chipstream_icon.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/gui/main_window.py` & `chipstream-0.4.0/chipstream/gui/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,16 @@
             "feature_kwargs": {
                 "brightness": self.checkBox_feat_bright.isChecked(),
                 "haralick": self.checkBox_feat_haralick.isChecked(),
                 "volume": self.checkBox_feat_volume.isChecked(),
                 },
             "gate_code": "norm",
             "gate_kwargs": {},
+            "basin_strategy":
+                "tap" if self.checkBox_basins.isChecked() else "drain",
             "num_procs": self.spinBox_procs.value(),
         }
 
         # special case for copy-segmenter
         if segmenter == "copy":
             job_kwargs["no_basins_in_output"] = \
                 not self.checkBox_basin_based.isChecked()
```

### Comparing `chipstream-0.3.1/chipstream/gui/main_window.ui` & `chipstream-0.4.0/chipstream/gui/main_window.ui`

 * *Files 6% similar despite different names*

#### Comparing `chipstream-0.3.1/chipstream/gui/main_window.ui` & `chipstream-0.4.0/chipstream/gui/main_window.ui`

```diff
@@ -153,14 +153,17 @@
                 <widget class="QGroupBox" name="groupBox">
                   <property name="title">
                     <string>Background Image</string>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout_2">
                     <item>
                       <widget class="QCheckBox" name="checkBox_bg_flickering">
+                        <property name="toolTip">
+                          <string>Use this option if the input dataset exhibits global temporal brightness variations of a few grayscal values</string>
+                        </property>
                         <property name="text">
                           <string>flickering correction</string>
                         </property>
                         <property name="checked">
                           <bool>true</bool>
                         </property>
                       </widget>
@@ -202,23 +205,26 @@
                             </item>
                           </layout>
                         </widget>
                         <widget class="QWidget" name="page_2">
                           <layout class="QGridLayout" name="gridLayout_3">
                             <item row="0" column="0">
                               <widget class="QLabel" name="label">
+                                <property name="toolTip">
+                                  <string>Mask-generating threshold for the background-corrected image.</string>
+                                </property>
                                 <property name="text">
                                   <string>Threshold</string>
                                 </property>
                               </widget>
                             </item>
                             <item row="0" column="1">
                               <widget class="QSpinBox" name="spinBox_thresh">
                                 <property name="toolTip">
-                                  <string>Mask-generating threshold for the background-corrected image.</string>
+                                  <string>Values smaller than zero are allowed</string>
                                 </property>
                                 <property name="minimum">
                                   <number>-10</number>
                                 </property>
                                 <property name="maximum">
                                   <number>-1</number>
                                 </property>
@@ -238,14 +244,17 @@
                         </property>
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
+                        <property name="toolTip">
+                          <string>Select the segmentation method to use</string>
+                        </property>
                         <item>
                           <property name="text">
                             <string>Disabled (from input file)</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
@@ -267,46 +276,58 @@
                   </property>
                   <property name="title">
                     <string>Feature Extraction</string>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout_7">
                     <item>
                       <widget class="QCheckBox" name="checkBox_feat_bright">
+                        <property name="toolTip">
+                          <string>Compute brightness features, such as mean event brightness</string>
+                        </property>
                         <property name="text">
                           <string>Image brightness features</string>
                         </property>
                         <property name="checked">
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QCheckBox" name="checkBox_feat_volume">
+                        <property name="toolTip">
+                          <string>Estimate the event volume using volrevolve algorithm</string>
+                        </property>
                         <property name="text">
                           <string>Volume</string>
                         </property>
                         <property name="checked">
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QCheckBox" name="checkBox_feat_haralick">
+                        <property name="toolTip">
+                          <string>Compute the haralick texture features (computationally expensive)</string>
+                        </property>
                         <property name="text">
                           <string>Haralick texture features</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <layout class="QHBoxLayout" name="horizontalLayout_2">
                         <property name="topMargin">
                           <number>0</number>
                         </property>
                         <item>
                           <widget class="QCheckBox" name="checkBox_pixel_size">
+                            <property name="toolTip">
+                              <string>Set the pixel size to a fixed value for all input files</string>
+                            </property>
                             <property name="text">
                               <string>Set global pixel size</string>
                             </property>
                           </widget>
                         </item>
                         <item>
                           <widget class="QDoubleSpinBox" name="doubleSpinBox_pixel_size">
@@ -342,16 +363,19 @@
                   </property>
                   <property name="title">
                     <string>Processing</string>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout_8">
                     <item>
                       <widget class="QSpinBox" name="spinBox_procs">
+                        <property name="toolTip">
+                          <string>Number of CPU threads to use, reduce if you need a responsive system</string>
+                        </property>
                         <property name="suffix">
-                          <string>Worker Processes</string>
+                          <string>Worker threads</string>
                         </property>
                         <property name="minimum">
                           <number>2</number>
                         </property>
                         <property name="maximum">
                           <number>64</number>
                         </property>
@@ -367,14 +391,27 @@
                         <item>
                           <property name="text">
                             <string>Select output path...</string>
                           </property>
                         </item>
                       </widget>
                     </item>
+                    <item>
+                      <widget class="QCheckBox" name="checkBox_basins">
+                        <property name="toolTip">
+                          <string>Produce smaller output files faster by referring to the input data via basins</string>
+                        </property>
+                        <property name="text">
+                          <string>Exploit basins</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
                   </layout>
                 </widget>
               </item>
               <item>
                 <widget class="QCommandLinkButton" name="commandLinkButton_run">
                   <property name="text">
                     <string>Run Pipeline</string>
```

### Comparing `chipstream-0.3.1/chipstream/gui/manager.py` & `chipstream-0.4.0/chipstream/gui/manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/gui/table_progress.py` & `chipstream-0.4.0/chipstream/gui/table_progress.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream/path_cache.py` & `chipstream-0.4.0/chipstream/path_cache.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/chipstream.egg-info/PKG-INFO` & `chipstream-0.4.0/chipstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.3.1
+Version: 0.4.0
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: dcnum>=0.19.1
+Requires-Dist: dcnum>=0.20.1
 Requires-Dist: h5py<4,>=3.0.0
 Requires-Dist: numpy<2,>=1.21
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == "cli"
 Provides-Extra: gui
 Requires-Dist: pyqt6; extra == "gui"
```

### Comparing `chipstream-0.3.1/chipstream.egg-info/SOURCES.txt` & `chipstream-0.4.0/chipstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/docs/artwork/chipstream_icon.svg` & `chipstream-0.4.0/docs/artwork/chipstream_icon.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/docs/artwork/chipstream_splash.png` & `chipstream-0.4.0/docs/artwork/chipstream_splash.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/docs/artwork/chipstream_splash.svg` & `chipstream-0.4.0/docs/artwork/chipstream_splash.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/docs/conf.py` & `chipstream-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/pyproject.toml` & `chipstream-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Visualization',
     'Intended Audience :: Science/Research',
 ]
 license = {text = "GPL version 3.0 or later"}
 dependencies = [
-    "dcnum>=0.19.1",
+    "dcnum>=0.20.1",
     "h5py>=3.0.0, <4",
     "numpy>=1.21, <2",  # CVE-2021-33430
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 cli = ["click>=8"]
```

### Comparing `chipstream-0.3.1/tests/conftest.py` & `chipstream-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `chipstream-0.4.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/tests/helper_methods.py` & `chipstream-0.4.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/tests/test_cli.py` & `chipstream-0.4.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,54 @@
 import dcnum.read
 import h5py
+import numpy as np
 
 import pytest
 
 from helper_methods import retrieve_data
 
 
 pytest.importorskip("click")
 
 from chipstream.cli import cli_main  # noqa: E402
 
 
+@pytest.mark.parametrize("drain", [True, False])
+def test_cli_basins(cli_runner, drain):
+    path_temp = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path = path_temp.with_name("input_path.rtdc")
+
+    # create a test file for more than 100 events
+    with dcnum.read.concatenated_hdf5_data(
+        paths=3*[path_temp],
+        path_out=path,
+            compute_frame=True):
+        pass
+
+    path_out = path.with_name("with_pixel_size_dcn.rtdc")
+    args = [str(path),
+            str(path_out),
+            "-s", "thresh",
+            ]
+    if drain:
+        args.append("--drain-basins")
+    result = cli_runner.invoke(cli_main.chipstream_cli, args)
+    assert result.exit_code == 0
+
+    with h5py.File(path_out) as h5:
+        for feat in ["image", "frame"]:
+            if drain:
+                assert feat in h5["events"]
+            else:
+                assert feat not in h5["events"]
+        for feat in ["mask", "deform", "aspect"]:
+            assert feat in h5["events"]
+
+
 @pytest.mark.parametrize("limit_events,dcnum_mapping,dcnum_yield,f0", [
     # this is the default
     ["0", "0", 36, 1],
     ["1-4", "1-4-n", 6, 2],
     ["3-10-5", "3-10-5", 5, 4],
 ])
 def test_cli_limit_events(cli_runner, limit_events, dcnum_yield,
@@ -28,23 +62,28 @@
         paths=3*[path_temp],
         path_out=path,
             compute_frame=True):
         pass
 
     # sanity check
     with h5py.File(path) as h5:
-        assert h5["events/frame"][0] == 1
-        assert h5["events/frame"][1] == 2
+        assert np.all(h5["events/frame"][:]
+                      == np.array([1,  2,  2,  4,  4,  5,  5,  5,  6,  6,
+                                   6,  7,  8,  8, 10, 10, 11, 11, 11, 12,
+                                   12, 12, 13, 14, 14, 16, 16, 17, 17, 17,
+                                   18, 18, 18]))
+        assert "basinmap0" not in h5
 
     path_out = path.with_name("limited_events.rtdc")
     result = cli_runner.invoke(cli_main.chipstream_cli,
                                [str(path),
                                 str(path_out),
                                 "-s", "thresh",
                                 "--limit-events", limit_events,
+                                "--drain-basins",
                                 ])
     assert result.exit_code == 0
 
     with h5py.File(path_out) as h5:
         assert h5["events/frame"][0] == f0
         assert h5.attrs["pipeline:dcnum yield"] == dcnum_yield
         assert h5.attrs["pipeline:dcnum mapping"] == dcnum_mapping
```

### Comparing `chipstream-0.3.1/tests/test_gui.py` & `chipstream-0.4.0/tests/test_gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,14 +36,36 @@
 def test_gui_basic(mw):
     # Just check some known properties in the UI.
     assert mw.spinBox_thresh.value() == -6
     assert mw.checkBox_feat_bright.isChecked()
     assert len(mw.job_manager) == 0
 
 
+@pytest.mark.parametrize("use_basins", [True, False])
+def test_gui_basins(mw, use_basins):
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    mw.append_paths([path])
+    mw.checkBox_basins.setChecked(use_basins)
+    mw.on_run()
+    while mw.job_manager.is_busy():
+        time.sleep(.1)
+    out_path = path.with_name(path.stem + "_dcn.rtdc")
+    assert out_path.exists()
+
+    with h5py.File(out_path) as h5:
+        for feat in ["image", "frame"]:
+            if not use_basins:
+                assert feat in h5["events"]
+            else:
+                assert feat not in h5["events"]
+        for feat in ["mask", "deform", "aspect"]:
+            assert feat in h5["events"]
+
+
 @pytest.mark.parametrize("correct_offset", [True, False])
 def test_gui_correct_offset(mw, correct_offset):
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     mw.append_paths([path])
     mw.checkBox_pixel_size.setChecked(True)
     mw.checkBox_bg_flickering.setChecked(correct_offset)
```

### Comparing `chipstream-0.3.1/tests/test_gui_manager.py` & `chipstream-0.4.0/tests/test_gui_manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.3.1/tests/test_path_cache.py` & `chipstream-0.4.0/tests/test_path_cache.py`

 * *Files identical despite different names*

