# Comparing `tmp/NeuroR-1.6.4.tar.gz` & `tmp/NeuroR-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroR-1.6.4.tar", last modified: Thu Mar 30 14:36:28 2023, max compression
+gzip compressed data, was "NeuroR-1.7.0.tar", last modified: Tue May 28 07:11:04 2024, max compression
```

## Comparing `NeuroR-1.6.4.tar` & `NeuroR-1.7.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.929164 NeuroR-1.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.921163 NeuroR-1.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.github/workflows/mirror-ebrains.yml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.github/workflows/upload-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-30 14:36:20.000000 NeuroR-1.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-30 14:36:20.000000 NeuroR-1.6.4/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 14:36:20.000000 NeuroR-1.6.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-30 14:36:20.000000 NeuroR-1.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-30 14:36:20.000000 NeuroR-1.6.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-30 14:36:20.000000 NeuroR-1.6.4/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-30 14:36:20.000000 NeuroR-1.6.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/NeuroR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 14:36:28.000000 NeuroR-1.6.4/NeuroR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-30 14:36:28.929164 NeuroR-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-30 14:36:20.000000 NeuroR-1.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    69178 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/_images/BlueBrainNeuroR.png
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/_images/distrib_1d.png
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/doc/source/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/cli/cut-plane.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/cli/neuror.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/cli/sanitize.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/cli/unravel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-30 14:36:20.000000 NeuroR-1.6.4/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-30 14:36:20.000000 NeuroR-1.6.4/examples/cut-plane-detection.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.921163 NeuroR-1.6.4/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.921163 NeuroR-1.6.4/examples/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.925164 NeuroR-1.6.4/examples/data/input/to-be-repaired/
--rwxr-xr-x   0 runner    (1001) docker     (123)   556932 2023-03-30 14:36:20.000000 NeuroR-1.6.4/examples/data/input/to-be-repaired/Neuron_slice.h5
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-30 14:36:20.000000 NeuroR-1.6.4/examples/repair.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.929164 NeuroR-1.6.4/neuror/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/axon.py
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:36:28.929164 NeuroR-1.6.4/neuror/cut_plane/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/cut_leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/dash.css
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/legacy_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/planes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/cut_plane/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/full.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10728 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/unravel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-03-30 14:36:20.000000 NeuroR-1.6.4/neuror/zero_diameter_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 14:36:28.929164 NeuroR-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-30 14:36:20.000000 NeuroR-1.6.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-30 14:36:20.000000 NeuroR-1.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.042707 NeuroR-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.030707 NeuroR-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.034707 NeuroR-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.github/workflows/mirror-ebrains.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.github/workflows/upload-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 07:11:00.000000 NeuroR-1.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 07:11:00.000000 NeuroR-1.7.0/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 07:11:00.000000 NeuroR-1.7.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-28 07:11:00.000000 NeuroR-1.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 07:11:00.000000 NeuroR-1.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 07:11:00.000000 NeuroR-1.7.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 07:11:00.000000 NeuroR-1.7.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/NeuroR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-28 07:11:03.000000 NeuroR-1.7.0/NeuroR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-28 07:11:04.000000 NeuroR-1.7.0/NeuroR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:11:03.000000 NeuroR-1.7.0/NeuroR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 07:11:03.000000 NeuroR-1.7.0/NeuroR.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 07:11:03.000000 NeuroR-1.7.0/NeuroR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 07:11:03.000000 NeuroR-1.7.0/NeuroR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-28 07:11:04.042707 NeuroR-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-28 07:11:00.000000 NeuroR-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69178 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/_images/BlueBrainNeuroR.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/_images/distrib_1d.png
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/doc/source/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/cli/cut-plane.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/cli/neuror.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/cli/sanitize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/cli/unravel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 07:11:00.000000 NeuroR-1.7.0/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-28 07:11:00.000000 NeuroR-1.7.0/examples/cut-plane-detection.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.034707 NeuroR-1.7.0/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.034707 NeuroR-1.7.0/examples/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.038707 NeuroR-1.7.0/examples/data/input/to-be-repaired/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   556932 2024-05-28 07:11:00.000000 NeuroR-1.7.0/examples/data/input/to-be-repaired/Neuron_slice.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-28 07:11:00.000000 NeuroR-1.7.0/examples/repair.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.042707 NeuroR-1.7.0/neuror/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/axon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:11:04.042707 NeuroR-1.7.0/neuror/cut_plane/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/cut_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/dash.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/legacy_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/planes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/cut_plane/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/full.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10826 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/unravel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-28 07:11:00.000000 NeuroR-1.7.0/neuror/zero_diameter_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:11:04.042707 NeuroR-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-28 07:11:00.000000 NeuroR-1.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-28 07:11:00.000000 NeuroR-1.7.0/tox.ini
```

### Comparing `NeuroR-1.6.4/.github/workflows/mirror-ebrains.yml` & `NeuroR-1.7.0/.github/workflows/mirror-ebrains.yml`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/.github/workflows/run-tox.yml` & `NeuroR-1.7.0/.github/workflows/run-tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7","3.8","3.9","3.10","3.11"]
+        python-version: ["3.8","3.9","3.10","3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
+
     - name: Run tox
       run: |
         tox
```

### Comparing `NeuroR-1.6.4/.github/workflows/upload-pypi.yml` & `NeuroR-1.7.0/.github/workflows/upload-pypi.yml`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/.gitlab-ci.yml` & `NeuroR-1.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/.pylintrc` & `NeuroR-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/CONTRIBUTING.md` & `NeuroR-1.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/COPYING` & `NeuroR-1.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/COPYING.LESSER` & `NeuroR-1.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/NeuroR.egg-info/PKG-INFO` & `NeuroR-1.7.0/NeuroR.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroR
-Version: 1.6.4
+Version: 1.7.0
 Summary: A morphology repair tool
 Home-page: https://github.com/bluebrain/neuror
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: |banner|
         
         |build| |license| |docs| |doi|
@@ -24,15 +24,15 @@
         
         
         Acknowledgements
         ----------------
         
         The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
         
-        This research was supported by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+        This work has been partially funded by the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 720270, 785907 (Human Brain Project SGA1/SGA2) and by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
         
         Citation
         --------
         
         Cite NeuroR with the following DOI: |doi|
         
         NeuroR implements the methods discussed in the following paper:
@@ -138,15 +138,15 @@
         License
         -------
         
         NeuroR is licensed under the terms of the GNU Lesser General Public License version 3.
         Refer to `COPYING.LESSER <https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER>`__
         and `COPYING <https://github.com/BlueBrain/NeuroR/blob/master/COPYING>`__ for details.
         
-        Copyright (c) 2019-2023 Blue Brain Project/EPFL
+        Copyright (c) 2019-2024 Blue Brain Project/EPFL
         
         .. |build| image:: https://travis-ci.com/BlueBrain/NeuroR.svg?branch=master
                       :target: https://travis-ci.com/BlueBrain/NeuroR
         
         .. |license| image:: https://img.shields.io/pypi/l/neuror
                         :target: https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER
```

### Comparing `NeuroR-1.6.4/NeuroR.egg-info/SOURCES.txt` & `NeuroR-1.7.0/NeuroR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/PKG-INFO` & `NeuroR-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroR
-Version: 1.6.4
+Version: 1.7.0
 Summary: A morphology repair tool
 Home-page: https://github.com/bluebrain/neuror
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Description: |banner|
         
         |build| |license| |docs| |doi|
@@ -24,15 +24,15 @@
         
         
         Acknowledgements
         ----------------
         
         The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
         
-        This research was supported by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+        This work has been partially funded by the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 720270, 785907 (Human Brain Project SGA1/SGA2) and by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
         
         Citation
         --------
         
         Cite NeuroR with the following DOI: |doi|
         
         NeuroR implements the methods discussed in the following paper:
@@ -138,15 +138,15 @@
         License
         -------
         
         NeuroR is licensed under the terms of the GNU Lesser General Public License version 3.
         Refer to `COPYING.LESSER <https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER>`__
         and `COPYING <https://github.com/BlueBrain/NeuroR/blob/master/COPYING>`__ for details.
         
-        Copyright (c) 2019-2023 Blue Brain Project/EPFL
+        Copyright (c) 2019-2024 Blue Brain Project/EPFL
         
         .. |build| image:: https://travis-ci.com/BlueBrain/NeuroR.svg?branch=master
                       :target: https://travis-ci.com/BlueBrain/NeuroR
         
         .. |license| image:: https://img.shields.io/pypi/l/neuror
                         :target: https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER
```

### Comparing `NeuroR-1.6.4/README.rst` & `NeuroR-1.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 Acknowledgements
 ----------------
 
 The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
 
-This research was supported by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+This work has been partially funded by the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 720270, 785907 (Human Brain Project SGA1/SGA2) and by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
 
 Citation
 --------
 
 Cite NeuroR with the following DOI: |doi|
 
 NeuroR implements the methods discussed in the following paper:
@@ -131,15 +131,15 @@
 License
 -------
 
 NeuroR is licensed under the terms of the GNU Lesser General Public License version 3.
 Refer to `COPYING.LESSER <https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER>`__
 and `COPYING <https://github.com/BlueBrain/NeuroR/blob/master/COPYING>`__ for details.
 
-Copyright (c) 2019-2023 Blue Brain Project/EPFL
+Copyright (c) 2019-2024 Blue Brain Project/EPFL
 
 .. |build| image:: https://travis-ci.com/BlueBrain/NeuroR.svg?branch=master
               :target: https://travis-ci.com/BlueBrain/NeuroR
 
 .. |license| image:: https://img.shields.io/pypi/l/neuror
                 :target: https://github.com/BlueBrain/NeuroR/blob/master/COPYING.LESSER
```

### Comparing `NeuroR-1.6.4/doc/Makefile` & `NeuroR-1.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/doc/source/_images/BlueBrainNeuroR.png` & `NeuroR-1.7.0/doc/source/_images/BlueBrainNeuroR.png`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/doc/source/_images/distrib_1d.png` & `NeuroR-1.7.0/doc/source/_images/distrib_1d.png`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/doc/source/conf.py` & `NeuroR-1.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/examples/cut-plane-detection.ipynb` & `NeuroR-1.7.0/examples/cut-plane-detection.ipynb`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/examples/data/input/to-be-repaired/Neuron_slice.h5` & `NeuroR-1.7.0/examples/data/input/to-be-repaired/Neuron_slice.h5`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/examples/repair.ipynb` & `NeuroR-1.7.0/examples/repair.ipynb`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/axon.py` & `NeuroR-1.7.0/neuror/axon.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         https://bbpgitlab.epfl.ch/nse/morphologyrepair/BlueRepairSDK/-/blob/main/BlueRepairSDK/src/helper_axon.cpp#L83
 
     .. warning::
         I have **absolutely** no clue why sorting by this metric
     '''
     dists = []
     for root in intact_axons:
-        origin = root.points[0]
-        origin_cut = section.points[0]
+        origin = root.points[0, COLS.XYZ]
+        origin_cut = section.points[0, COLS.XYZ]
         diff = origin_cut - origin
         diff[COLS.X] = origin_cut[COLS.X] + origin[COLS.X]
         dists.append(np.linalg.norm(diff))
 
     return intact_axons[np.argmin(dists)]
 
 
@@ -157,22 +157,22 @@
     for branch in branch_pool:
         if (branch in used_axon_branches or strahler_orders[similar] != strahler_orders[branch]):
             continue
 
         L.debug("Pasting axon branch with ID %s", branch.id)
 
         end_point = section.points[-1, COLS.XYZ]
-        appended = section.append_section(branch)
+        appended = section.to_morphio().append_section(branch.to_morphio())
         translation = section.points[-1, COLS.XYZ] - appended.points[0, COLS.XYZ]
         align(appended, translation)
         translate(appended, translation)
 
         # Make sure the child section first point is exactly the end point of the parent section
         appended_points = np.copy(appended.points)
-        appended_points[0] = end_point
+        appended_points[0, COLS.XYZ] = end_point
         appended.points = appended_points
 
         if any(np.any(section.points[:, COLS.Y] > y_extent) for section in appended.iter()):
             L.debug("Discarded, exceeds y-limit")
             morphology.delete_section(appended)
         else:
             L.debug('Section appended')
```

### Comparing `NeuroR-1.6.4/neuror/cli.py` & `NeuroR-1.7.0/neuror/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
               help='Force the detection along the given plane')
 def folder(input_dir, output_dir, width, display, plane):
     '''Compute cut planes for all morphology in INPUT_DIR and save them into OUTPUT_DIR
 
     See "cut-plane compute --help" for more information'''
     for inputfilename in iter_morphology_files(input_dir):
         L.info('Seaching cut plane for file: %s', inputfilename)
-        outfilename = os.path.join(output_dir, inputfilename.with_suffix('.json'))
+        outfilename = os.path.join(output_dir, inputfilename.with_suffix('.json').name)
         try:
             _export_cut_plane(inputfilename, outfilename, width, display=display,
                               searched_axes=(plane or ('X', 'Y', 'Z')),
                               fix_position=None)
         except Exception as e:  # noqa, pylint: disable=broad-except
             L.warning('Cut plane computation for %s failed', inputfilename)
             L.warning(e, exc_info=True)
```

### Comparing `NeuroR-1.6.4/neuror/cut_plane/cut_leaves.py` & `NeuroR-1.7.0/neuror/cut_plane/cut_leaves.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/cut_plane/dash.css` & `NeuroR-1.7.0/neuror/cut_plane/dash.css`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/cut_plane/detection.py` & `NeuroR-1.7.0/neuror/cut_plane/detection.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/cut_plane/legacy_detection.py` & `NeuroR-1.7.0/neuror/cut_plane/legacy_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     '''
     axis = {'x': COLS.X, 'y': COLS.Y, 'z': COLS.Z}[axis.lower()]
 
     cut = defaultdict(lambda key: False)
     side = cut_detect(neuron, cut, 0, axis)
 
     # reclassify cut points in tuft,based on apical point position
-    apical_section_id, point_id = apical_point_section_segment(neuron)
+    apical_section_id, point_id = apical_point_section_segment(neuron.to_morphio())
     if apical_section_id is not None:
         apical_section = neuron.sections[apical_section_id]
         apical_offset = apical_section.points[point_id, axis]
         cut_mark(children_ids(apical_section), cut, apical_offset, side, axis)
     else:
         apical_section = None
```

### Comparing `NeuroR-1.6.4/neuror/cut_plane/planes.py` & `NeuroR-1.7.0/neuror/cut_plane/planes.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/cut_plane/viewer.py` & `NeuroR-1.7.0/neuror/cut_plane/viewer.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/full.py` & `NeuroR-1.7.0/neuror/full.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/main.py` & `NeuroR-1.7.0/neuror/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 '''
 import copy
 import logging
 from collections import Counter, OrderedDict, defaultdict
 from enum import Enum
 from itertools import chain
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 import jsonschema
 import morphio
 import neurom as nm
 import numpy as np
 from morph_tool import apical_point_section_segment
 from morph_tool.spatial import point_to_section_segment
 from morphio import PointLevel, SectionType
 from neurom import NeuriteType, iter_neurites, iter_sections, load_morphology
 from neurom.core.dataformat import COLS
+from neurom.core.types import tree_type_checker
 from neurom.core import Neurite, Section
 from neurom.features.section import branch_order, section_path_length
-from nptyping import NDArray, Shape, Float
 from scipy.spatial.distance import cdist
 
 from neuror import axon, cut_plane
 from neuror.exceptions import NeuroRError
 from neuror.utils import RepairType, direction, repair_type_map, rotation_matrix, section_length
 
 _PARAMS = {
@@ -276,28 +276,39 @@
     )
     direction_ /= np.linalg.norm(direction_)
 
     coord = sec.points[-1, COLS.XYZ] + direction_ * params["seg_length"]
     # we apply tapering function + minimum diameter
     radius = max(tip_radius, sec.points[-1, COLS.R] - taper)
     new_point = np.append(coord, radius)
-    sec.points = np.vstack((sec.points, new_point))
+    sec_pts = np.vstack((sec.points, new_point))
+    sec.to_morphio().points = sec_pts[:, COLS.XYZ]
+    sec.to_morphio().diameters = sec_pts[:, COLS.R] * 2
 
 
 def _y_cylindrical_extent(section):
     '''Returns the distance from the last section point to the origin in the XZ plane.'''
     xz_last_point = section.points[-1, [0, 2]]
     return np.linalg.norm(xz_last_point)
 
 
 def _max_y_dendritic_cylindrical_extent(neuron):
     '''Return the maximum distance of dendritic section ends and the origin in the XZ plane.'''
-    return max((_y_cylindrical_extent(section) for section in neuron.iter()
-                if section.type in {SectionType.basal_dendrite, SectionType.apical_dendrite}),
-               default=0)
+    return max(
+        (
+            _y_cylindrical_extent(section)
+            for section in iter_sections(
+                neuron,
+                section_filter=tree_type_checker(
+                    SectionType.basal_dendrite, SectionType.apical_dendrite
+                ),
+            )
+        ),
+        default=0,
+    )
 
 
 class Repair(object):
     '''Repair the input morphology.
 
     The repair algorithm uses sholl analysis of intact branches to grow new branches from cut
     leaves. The algorithm is fairly complex, but can be controled via a few parameters in the
@@ -335,18 +346,18 @@
         https://bbpgitlab.epfl.ch/nse/morphologyrepair/BlueRepairSDK/-/blob/main/BlueRepairSDK/src/repair.cpp#L469
     '''
 
     def __init__(self,  # pylint: disable=too-many-arguments
                  inputfile: Path,
                  axons: Optional[Path] = None,
                  seed: Optional[int] = 0,
-                 cut_leaves_coordinates: Optional[NDArray[Shape["3"], Any]] = None,
+                 cut_leaves_coordinates: Optional[np.ndarray] = None,
                  legacy_detection: bool = False,
                  repair_flags: Optional[Dict[RepairType, bool]] = None,
-                 apical_point: NDArray[Shape["3"], Float] = None,
+                 apical_point: np.ndarray = None,
                  params: Dict = None,
                  validate_params=False):
         np.random.seed(seed)
         self.legacy_detection = legacy_detection
         self.inputfile = inputfile
         self.axon_donors = axons or []
         self.donated_intact_axon_sections = []
@@ -362,27 +373,30 @@
         if legacy_detection:
             self.cut_leaves = CutPlane.find_legacy(inputfile, 'z').cut_leaves_coordinates
         elif cut_leaves_coordinates is None:
             self.cut_leaves = CutPlane.find(inputfile, bin_width=15).cut_leaves_coordinates
         else:
             self.cut_leaves = np.asarray(cut_leaves_coordinates)
 
-        self.neuron = load_morphology(inputfile)
+        self.neuron = load_morphology(inputfile, mutable=True)
         self.repair_type_map = {}
         self.max_y_cylindrical_extent = _max_y_dendritic_cylindrical_extent(self.neuron)
         self.max_y_extent = max(np.max(section.points[:, COLS.Y])
-                                for section in self.neuron.iter())
+                                for section in self.neuron.to_morphio().iter())
 
         self.info = {}
         apical_section_id = None
         if apical_point != -1:
             if apical_point:
-                apical_section_id = point_to_section_segment(self.neuron, apical_point)[0]
+                apical_section_id = point_to_section_segment(
+                    self.neuron.to_morphio(),
+                    apical_point,
+                )[0]
             else:
-                apical_section_id = apical_point_section_segment(self.neuron)[0]
+                apical_section_id = apical_point_section_segment(self.neuron.to_morphio())[0]
 
         if apical_section_id:
             self.apical_section = self.neuron.sections[apical_section_id]
         else:
             self.apical_section = None
 
         # record the tip radius as a lower bound for diameters with taper, excluding axons
@@ -425,25 +439,26 @@
 
         Args:
             outputfile: path to the output morphology
             plot_file: path to the output figure
         '''
         if self.cut_leaves.size == 0:
             L.warning('No cut leaves. Nothing to repair for morphology %s', self.inputfile)
-            self.neuron.write(outputfile)
+            self.neuron.to_morphio().write(outputfile)
             return
 
         # See https://github.com/BlueBrain/MorphIO/issues/161
         keep_axons_alive = []
 
         for axon_donor in self.axon_donors:
             if self.legacy_detection:
                 plane = cut_plane.CutPlane.find_legacy(axon_donor, 'z')
             else:
                 plane = cut_plane.CutPlane.find(axon_donor)
+            plane.morphology = load_morphology(plane.morphology, mutable=True)
             keep_axons_alive.append(plane)
             self.donated_intact_axon_sections.extend(
                 [section for section in iter_sections(plane.morphology)
                  if section.type == SectionType.axon and
                  is_branch_intact(section, plane.cut_leaves_coordinates)])
 
         self._fill_repair_type_map()
@@ -496,15 +511,16 @@
         if plot_file is not None:
             try:
                 from neuror.view import plot_repaired_neuron
                 plot_repaired_neuron(self.neuron, cut_leaves_ids, plot_file)
             except ImportError:
                 L.warning('Skipping writing plots as [plotly] extra is not installed')
 
-        self.neuron.write(outputfile)
+        self.neuron.to_morphio().remove_unifurcations()
+        self.neuron.to_morphio().write(outputfile)
         L.debug('Repair successful for %s', self.inputfile)
 
     def _find_intact_obliques(self):
         '''Find root sections of all intact obliques.
 
         Root obliques are obliques with a section parent of type 'trunk'.
 
@@ -696,15 +712,15 @@
         for child_diameter in child_diameters:
             child_start = section.points[-1, COLS.XYZ]
             points = [child_start.tolist(),
                       (child_start + shuffle_direction(last_segment_vec) *
                        self.params['seg_length']).tolist()]
             prop = PointLevel(points, [current_diameter, child_diameter])
 
-            child = section.append_section(prop)
+            child = section.to_morphio().append_section(prop)
             L.debug('section appended: %s', child.id)
 
     def _grow(self, section, order_offset, origin):
         '''Grow main method.
 
         Will either:
             - continue growing the section
@@ -775,15 +791,15 @@
         self.repair_type_map = repair_type_map(self.neuron, self.apical_section)
 
 
 def repair(inputfile: Path,  # pylint: disable=too-many-arguments
            outputfile: Path,
            axons: Optional[List[Path]] = None,
            seed: int = 0,
-           cut_leaves_coordinates: Optional[NDArray[Shape["3"], Any]] = None,
+           cut_leaves_coordinates: Optional[np.ndarray] = None,
            legacy_detection: bool = False,
            plot_file: Optional[Path] = None,
            repair_flags: Optional[Dict[RepairType, bool]] = None,
            apical_point: List = None,
            params: Dict = None,
            validate_params=False):
     '''The repair function.
```

### Comparing `NeuroR-1.6.4/neuror/sanitize.py` & `NeuroR-1.7.0/neuror/sanitize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Dict, List, Tuple
 
 import numpy as np
 from morphio import MorphioError, SomaType, set_maximum_warnings
 from morphio.mut import Morphology  # pylint: disable=import-error
 from neurom.check import morphology_checks as mc
 from neurom.check import CheckResult
+from neurom.core.soma import get_center, get_radius, check_overlaps
 from neurom.apps.annotate import annotate
 from neurom import load_morphology
 from tqdm import tqdm
 
 from neuror.exceptions import CorruptedMorphology
 from neuror.exceptions import ZeroLengthRootSection
 
@@ -252,30 +253,30 @@
     Args:
         morph: the morphology
 
     Returns:
         ``True`` if at least one point was changed, else ``False``.
     """
     changed = False
-    for root_sec in morph.root_sections:
+    for root_sec in morph.to_morphio().root_sections:
         sec_pts = root_sec.points
-        in_soma = np.argwhere(morph.soma.overlaps(sec_pts)).flatten()
+        in_soma = np.argwhere(check_overlaps(morph.soma, sec_pts)).flatten()
 
         if in_soma.size > 0:
             changed = True
 
             last_in_soma = in_soma[-1]
 
             if last_in_soma >= len(sec_pts) - 1:
                 raise CorruptedMorphology("An entire section is located inside the soma")
 
             in_pt = sec_pts[last_in_soma]
             out_pt = sec_pts[last_in_soma + 1]
             vec = out_pt - in_pt
-            new_pt = morph.soma.center + vec / np.linalg.norm(vec) * morph.soma.radius
+            new_pt = get_center(morph.soma) + vec / np.linalg.norm(vec) * get_radius(morph.soma)
             if np.linalg.norm(new_pt - root_sec.points[last_in_soma + 1]) <= _ZERO_LENGTH:
                 new_sec_pts = root_sec.points[last_in_soma + 1:]
                 last_in_soma += 1
             else:
                 new_sec_pts = np.concatenate([[new_pt], root_sec.points[last_in_soma + 1:]])
             root_sec.points = new_sec_pts
             root_sec.diameters = root_sec.diameters[last_in_soma:]
```

### Comparing `NeuroR-1.6.4/neuror/unravel.py` & `NeuroR-1.7.0/neuror/unravel.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/utils.py` & `NeuroR-1.7.0/neuror/utils.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/view.py` & `NeuroR-1.7.0/neuror/view.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/neuror/zero_diameter_fixer.py` & `NeuroR-1.7.0/neuror/zero_diameter_fixer.py`

 * *Files identical despite different names*

### Comparing `NeuroR-1.6.4/setup.py` & `NeuroR-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     long_description_content_type="text/x-rst",
     url="https://github.com/bluebrain/neuror",
     license="LGPLv3",
     install_requires=[
         'click>=6.7',
         'jsonschema',
         'matplotlib>=2.2.3',
-        'morph-tool>=2.9.0,<3.0',
+        'morph-tool>=2.11.0,<3.0',
         'morphio>=3.0.0,<4.0',
-        'neurom>=3.0.1,<4.0',
+        'neurom>=4.0.0',
         'numpy>=1.19.2',
         'nptyping>=2',
         'pandas>=0.24.2',
         'pyquaternion>=0.9.2',
         'scipy>=1.2.0',
     ],
     extras_require={
         'plotly': [
             'dash-core-components>=0.46.0',  # HTML components
             'dash-table>=3.6.0',  # Interactive DataTable component (new!)
             'dash>=0.41.0',  # The core dash backend
-            'plotly-helper>=0.0.8,<1.0',
+            'plotly-helper>=0.0.9,<1.0',
         ],
         'docs': [
             'sphinx-autorun>=1.1.1',
             'sphinx-bluebrain-theme>=0.2.4',
             'sphinx-click>=2.5.0',
             'sphinx>=2.0.0',
         ],
```

