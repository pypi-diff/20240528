# Comparing `tmp/cellfinder-1.2.0.tar.gz` & `tmp/cellfinder-1.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.2.0.tar", last modified: Wed May 15 16:11:09 2024, max compression
+gzip compressed data, was "cellfinder-1.3.0rc0.tar", last modified: Tue May 28 15:38:41 2024, max compression
```

## Comparing `cellfinder-1.2.0.tar` & `cellfinder-1.3.0rc0.tar`

### file list

```diff
@@ -1,90 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.346486 cellfinder-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.github/workflows/test_include_guard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-15 16:11:03.000000 cellfinder-1.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 16:11:03.000000 cellfinder-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 16:11:03.000000 cellfinder-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 16:11:09.358486 cellfinder-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-15 16:11:03.000000 cellfinder-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/cli_migration_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/detect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/curation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/detect/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/detect_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/thread_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/input_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/train/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/train_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-15 16:11:09.000000 cellfinder-1.2.0/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-15 16:11:03.000000 cellfinder-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:09.358486 cellfinder-1.2.0/setup.cfg
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.218645 cellfinder-1.3.0rc0/.github/
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/.github/workflows/
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5102 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/.github/workflows/test_and_deploy.yml
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1779 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/.github/workflows/test_include_guard.yaml
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1493 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/.gitignore
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/.napari/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      342 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/.napari/config.yml
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1806 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/CITATION.cff
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1564 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/LICENSE
+-rw-rw-r--   0 adam      (1001) adam      (1001)      320 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/MANIFEST.in
+-rw-r--r--   0 adam      (1001) adam      (1001)     6457 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4180 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1182 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1336 2024-05-28 13:04:31.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2087 2024-05-23 15:52:38.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1302 2024-05-28 14:59:17.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1578 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/cli_migration_warning.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/
+-rw-rw-r--   0 adam      (1001) adam      (1001)       62 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      229 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      287 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      279 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3097 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4249 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3866 2024-05-28 15:02:46.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      287 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      382 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      355 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-312.pyc
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/classify/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      171 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      187 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      175 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4335 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7771 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7149 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3016 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4579 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4128 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    14282 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    24420 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    22810 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7352 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    11288 2024-05-23 15:53:00.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9766 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2364 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3544 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3259 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     6321 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/augment.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3061 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/classify.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)    17125 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/cube_generator.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)    10034 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/resnet.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2560 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/tools.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/config/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/config/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)       56 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/config/cellfinder.conf
+-rw-rw-r--   0 adam      (1001) adam      (1001)      107 2024-01-03 15:53:15.000000 cellfinder-1.3.0rc0/cellfinder/core/config/cellfinder.conf.custom
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      169 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      185 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      173 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7846 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    11736 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    10384 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9592 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/detect.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      177 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      193 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      181 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2038 2024-05-07 15:42:37.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2707 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2500 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-312.pyc
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/
+-rw-rw-r--   0 adam      (1001) adam      (1001)       40 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      233 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      263 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      240 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1449 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1942 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1829 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2808 2024-05-07 15:42:37.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3857 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3665 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3082 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4520 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4496 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1331 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2746 2024-05-07 15:02:11.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3001 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2084 2024-05-07 15:02:11.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/setup_filters.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      200 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      188 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    31524 2024-01-16 13:15:35.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-199.py310.1.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1478 2024-01-16 13:15:35.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-199.py310.nbi
+-rw-rw-r--   0 adam      (1001) adam      (1001)    33890 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.1.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    34146 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.2.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.nbi
+-rw-rw-r--   0 adam      (1001) adam      (1001)    33846 2024-05-23 15:53:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.1.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    34102 2024-05-23 15:53:34.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.2.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-23 15:53:34.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.nbi
+-rw-rw-r--   0 adam      (1001) adam      (1001)    33929 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.1.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    34185 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.2.nbc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.nbi
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9803 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    15888 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    14649 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9893 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    15465 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    14790 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     6806 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    11313 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    10217 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5437 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    10104 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9349 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    13894 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)    11307 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7660 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7035 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/download/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      171 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      187 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      175 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1857 2024-05-09 10:52:26.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2316 2024-05-23 15:17:23.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/cli.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3264 2024-05-09 10:45:04.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4608 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4057 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1764 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/download/cli.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3277 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/download/download.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3625 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/main.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/tools/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2743 2024-05-23 13:35:02.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/IO.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      172 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3065 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4786 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4433 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1325 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1924 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1694 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1869 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/image_processing.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2434 2024-05-23 15:14:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/image_processing.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1831 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2982 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2640 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1153 2024-05-09 10:45:04.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1338 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1282 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2738 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/system.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3303 2024-05-23 15:14:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/system.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1590 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tf.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4167 2024-01-03 15:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tiff.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4889 2024-05-23 15:17:23.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tiff.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5418 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7524 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     6614 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3371 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/array_operations.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1124 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/geometry.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2269 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/image_processing.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2175 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/prep.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)      856 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/source_files.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2232 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/system.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2899 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/tiff.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4867 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/tools.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/train/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      172 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     9635 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    15619 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    13611 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    13260 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/train/train_yml.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)      106 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/types.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/
+-rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-16 12:55:27.000000 cellfinder-1.3.0rc0/cellfinder/napari/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      164 2024-01-16 12:55:32.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      180 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    16221 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/curation.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    26918 2024-05-23 14:14:01.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/curation.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2378 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3071 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2769 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      960 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/sample_data.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     1373 2024-05-23 14:13:10.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/sample_data.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3817 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5550 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4934 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    21447 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/curation.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/detect/
+-rw-rw-r--   0 adam      (1001) adam      (1001)       34 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      215 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      245 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      222 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    10018 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    14902 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    13667 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5225 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     8717 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7387 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3305 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5136 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-311.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4576 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)    13658 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/detect.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5377 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/detect_containers.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3078 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/thread_worker.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     2150 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/input_container.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)      921 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/napari.yaml
+-rw-rw-r--   0 adam      (1001) adam      (1001)      732 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/sample_data.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/train/
+-rw-rw-r--   0 adam      (1001) adam      (1001)       35 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__init__.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/
+-rw-rw-r--   0 adam      (1001) adam      (1001)      215 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)      222 2024-05-23 14:14:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5073 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     7017 2024-05-23 14:14:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4609 2024-05-09 10:51:35.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train_containers.cpython-310.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     6891 2024-05-23 15:15:00.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train_containers.cpython-312.pyc
+-rw-rw-r--   0 adam      (1001) adam      (1001)     5941 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/train.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     4386 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/train_containers.py
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3824 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1001)     6457 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1001)    12378 2024-05-28 15:38:41.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1001)        1 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1001)      247 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1001)      373 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1001)       11 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1001)     3499 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/pyproject.toml
+-rw-rw-r--   0 adam      (1001) adam      (1001)       38 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/setup.cfg
```

### Comparing `cellfinder-1.2.0/.github/workflows/test_include_guard.yaml` & `cellfinder-1.3.0rc0/.github/workflows/test_include_guard.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-name: Test Tensorflow include guards
-# These tests check that the include guards checking for tensorflow's availability
+name: Test Keras include guards
+# These tests check that the include guards checking for Keras availability
 # behave as expected on ubuntu and macOS.
 
 on:
   pull_request:
   push:
     branches:
       - main
 
 jobs:
-  tensorflow_guards:
+  keras_guards:
     name: Test include guards
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest]
     runs-on: ${{ matrix.os }}
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.10'
 
-      - name: Install via pip
-        run: python -m pip install -e .
+      - name: Install cellfinder via pip
+        run: python -m pip install -e "."
 
       - name: Test (working) import
         uses: jannekem/run-python-script-action@v1
+        env:
+          KERAS_BACKEND: torch
         with:
           fail-on-error: true
           script: |
             import cellfinder.core
             import cellfinder.napari
 
-      - name: Uninstall tensorflow-macos on Mac M1
-        if: matrix.os == 'macos-latest'
-        run: python -m pip uninstall -y tensorflow-macos
-
-      - name: Uninstall tensorflow on Ubuntu
-        if: matrix.os == 'ubuntu-latest'
-        run: python -m pip uninstall -y tensorflow
+      - name: Uninstall keras
+        run: python -m pip uninstall -y keras
 
       - name: Test (broken) import
         id: broken_import
         uses: jannekem/run-python-script-action@v1
         with:
           fail-on-error: false
           script: |
```

### Comparing `cellfinder-1.2.0/.gitignore` & `cellfinder-1.3.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/CITATION.cff` & `cellfinder-1.3.0rc0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/LICENSE` & `cellfinder-1.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/PKG-INFO` & `cellfinder-1.3.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.2.0
+Version: 1.3.0rc0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -27,16 +27,16 @@
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
-Requires-Dist: tensorflow-macos<2.12.0,>=2.5.0; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tensorflow<2.12.0,>=2.5.0; platform_system != "Darwin" or platform_machine != "arm64"
+Requires-Dist: keras>=3.0.0
+Requires-Dist: torch>=2.1.0
 Requires-Dist: tifffile
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyinstrument; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `cellfinder-1.2.0/README.md` & `cellfinder-1.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/__init__.py` & `cellfinder-1.3.0rc0/cellfinder/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import os
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
+# Check cellfinder is installed
 try:
     __version__ = version("cellfinder")
 except PackageNotFoundError as e:
     raise PackageNotFoundError("cellfinder package not installed") from e
 
-# If tensorflow is not present, tools cannot be used.
+# If Keras is not present, tools cannot be used.
 # Throw an error in this case to prevent invocation of functions.
 try:
-    TF_VERSION = version("tensorflow")
+    KERAS_VERSION = version("keras")
 except PackageNotFoundError as e:
-    try:
-        TF_VERSION = version("tensorflow-macos")
-    except PackageNotFoundError as e:
-        raise PackageNotFoundError(
-            f"cellfinder tools cannot be invoked without tensorflow. "
-            f"Please install tensorflow into your environment to use cellfinder tools. "
-            f"For more information, please see "
-            f"https://github.com/brainglobe/brainglobe-meta#readme."
-        ) from e
+    raise PackageNotFoundError(
+        f"cellfinder tools cannot be invoked without Keras. "
+        f"Please install Keras with a backend into your environment "
+        f"to use cellfinder tools. "
+        f"For more information on Keras backends, please see "
+        f"https://keras.io/getting_started/#installing-keras-3."
+        f"For more information on brainglobe, please see "
+        f"https://github.com/brainglobe/brainglobe-meta#readme."
+    ) from e
+
+
+# Set the Keras backend to torch
+os.environ["KERAS_BACKEND"] = "torch"
 
 __author__ = "Adam Tyson, Christian Niedworok, Charly Rousseau"
 __license__ = "BSD-3-Clause"
 
 DEFAULT_CELLFINDER_DIRECTORY = Path.home() / ".brainglobe" / "cellfinder"
```

### Comparing `cellfinder-1.2.0/cellfinder/cli_migration_warning.py` & `cellfinder-1.3.0rc0/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/classify/augment.py` & `cellfinder-1.3.0rc0/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/classify/classify.py` & `cellfinder-1.3.0rc0/cellfinder/core/classify/classify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
+import keras
 import numpy as np
 from brainglobe_utils.cells.cells import Cell
 from brainglobe_utils.general.system import get_num_processes
-from tensorflow import keras
 
 from cellfinder.core import logger, types
 from cellfinder.core.classify.cube_generator import CubeGeneratorFromFile
 from cellfinder.core.classify.tools import get_model
 from cellfinder.core.train.train_yml import depth_type, models
 
 
@@ -44,43 +44,42 @@
 
     if callback is not None:
         callbacks = [BatchEndCallback(callback)]
     else:
         callbacks = None
 
     # Too many workers doesn't increase speed, and uses huge amounts of RAM
-    workers = get_num_processes(
-        min_free_cpu_cores=n_free_cpus, n_max_processes=max_workers
-    )
+    workers = get_num_processes(min_free_cpu_cores=n_free_cpus)
 
     logger.debug("Initialising cube generator")
     inference_generator = CubeGeneratorFromFile(
         points,
         signal_array,
         background_array,
         voxel_sizes,
         network_voxel_sizes,
         batch_size=batch_size,
         cube_width=cube_width,
         cube_height=cube_height,
         cube_depth=cube_depth,
+        use_multiprocessing=False,
+        workers=workers,
     )
 
     model = get_model(
         existing_model=trained_model,
         model_weights=model_weights,
         network_depth=models[network_depth],
         inference=True,
     )
 
     logger.info("Running inference")
+    # in Keras 3.0 multiprocessing params are specified in the generator
     predictions = model.predict(
         inference_generator,
-        use_multiprocessing=True,
-        workers=workers,
         verbose=True,
         callbacks=callbacks,
     )
     predictions = predictions.round()
     predictions = predictions.astype("uint16")
 
     predictions = np.argmax(predictions, axis=1)
```

### Comparing `cellfinder-1.2.0/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.3.0rc0/cellfinder/core/classify/cube_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from random import shuffle
 from typing import Dict, List, Optional, Tuple, Union
 
+import keras
 import numpy as np
-import tensorflow as tf
 from brainglobe_utils.cells.cells import Cell, group_cells_by_z
 from brainglobe_utils.general.numerical import is_even
+from keras.utils import Sequence
 from scipy.ndimage import zoom
 from skimage.io import imread
-from tensorflow.keras.utils import Sequence
 
 from cellfinder.core import types
 from cellfinder.core.classify.augment import AugmentationParameters, augment
 
 # TODO: rename, as now using dask arrays -
 #  actually should combine to one generator
 
@@ -52,15 +52,22 @@
         augment_likelihood: float = 0.1,
         flip_axis: Tuple[int, int, int] = (0, 1, 2),
         rotate_max_axes: Tuple[float, float, float] = (1, 1, 1),  # degrees
         # scale=[0.5, 2],  # min, max
         translate: Tuple[float, float, float] = (0.05, 0.05, 0.05),
         shuffle: bool = False,
         interpolation_order: int = 2,
+        *args,
+        **kwargs,
     ):
+        # pass any additional arguments not specified in signature to the
+        # constructor of the superclass (e.g.: `use_multiprocessing` or
+        # `workers`)
+        super().__init__(*args, **kwargs)
+
         self.points = points
         self.signal_array = signal_array
         self.background_array = background_array
         self.batch_size = batch_size
         self.axis_2_pixel_um = float(voxel_sizes[2])
         self.axis_1_pixel_um = float(voxel_sizes[1])
         self.axis_0_pixel_um = float(voxel_sizes[0])
@@ -214,18 +221,18 @@
         signal_stack, background_stack = self.__get_stacks(index)
         images = self.__generate_cubes(
             cell_batch, signal_stack, background_stack
         )
 
         if self.train:
             batch_labels = [cell.type - 1 for cell in cell_batch]
-            batch_labels = tf.keras.utils.to_categorical(
+            batch_labels = keras.utils.to_categorical(
                 batch_labels, num_classes=self.classes
             )
-            return images, batch_labels
+            return images, batch_labels.astype(np.float32)
         elif self.extract:
             batch_info = self.__get_batch_dict(cell_batch)
             return images, batch_info
         else:
             return images
 
     def __get_stacks(self, index: int) -> Tuple[np.ndarray, np.ndarray]:
@@ -248,15 +255,16 @@
     ) -> np.ndarray:
         number_images = len(cell_batch)
         images = np.empty(
             (
                 (number_images,)
                 + (self.cube_height, self.cube_width, self.cube_depth)
                 + (self.channels,)
-            )
+            ),
+            dtype=np.float32,
         )
 
         for idx, cell in enumerate(cell_batch):
             images = self.__populate_array_with_cubes(
                 images, idx, cell, signal_stack, background_stack
             )
 
@@ -346,15 +354,22 @@
         augment_likelihood: float = 0.1,
         flip_axis: Tuple[int, int, int] = (0, 1, 2),
         rotate_max_axes: Tuple[int, int, int] = (45, 45, 45),  # degrees
         # scale=[0.5, 2],  # min, max
         translate: Tuple[float, float, float] = (0.2, 0.2, 0.2),
         train: bool = False,  # also return labels
         interpolation_order: int = 2,
+        *args,
+        **kwargs,
     ):
+        # pass any additional arguments not specified in signature to the
+        # constructor of the superclass (e.g.: `use_multiprocessing` or
+        # `workers`)
+        super().__init__(*args, **kwargs)
+
         self.im_shape = shape
         self.batch_size = batch_size
         self.labels = labels
         self.signal_list = signal_list
         self.background_list = background_list
         self.channels = channels
         self.classes = classes
@@ -406,38 +421,39 @@
         list_signal_tmp = [self.signal_list[k] for k in indexes]
         list_background_tmp = [self.background_list[k] for k in indexes]
 
         images = self.__generate_cubes(list_signal_tmp, list_background_tmp)
 
         if self.train and self.labels is not None:
             batch_labels = [self.labels[k] for k in indexes]
-            batch_labels = tf.keras.utils.to_categorical(
+            batch_labels = keras.utils.to_categorical(
                 batch_labels, num_classes=self.classes
             )
-            return images, batch_labels
+            return images, batch_labels.astype(np.float32)
         else:
             return images
 
     def __generate_cubes(
         self,
         list_signal_tmp: List[Union[str, Path]],
         list_background_tmp: List[Union[str, Path]],
     ) -> np.ndarray:
         number_images = len(list_signal_tmp)
         images = np.empty(
-            ((number_images,) + self.im_shape + (self.channels,))
+            ((number_images,) + self.im_shape + (self.channels,)),
+            dtype=np.float32,
         )
 
         for idx, signal_im in enumerate(list_signal_tmp):
             background_im = list_background_tmp[idx]
             images = self.__populate_array_with_cubes(
                 images, idx, signal_im, background_im
             )
 
-        return images.astype(np.float16)
+        return images
 
     def __populate_array_with_cubes(
         self,
         images: np.ndarray,
         idx: int,
         signal_im: Union[str, Path],
         background_im: Union[str, Path],
```

### Comparing `cellfinder-1.2.0/cellfinder/core/classify/resnet.py` & `cellfinder-1.3.0rc0/cellfinder/core/classify/resnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Callable, Dict, List, Literal, Optional, Tuple, Union
 
-from tensorflow import Tensor
-from tensorflow.keras import Model
-from tensorflow.keras.initializers import Initializer
-from tensorflow.keras.layers import (
+from keras import (
+    KerasTensor as Tensor,
+)
+from keras import Model
+from keras.initializers import Initializer
+from keras.layers import (
     Activation,
     Add,
     BatchNormalization,
     Conv3D,
     Dense,
     GlobalAveragePooling3D,
     Input,
     MaxPooling3D,
     ZeroPadding3D,
 )
-from tensorflow.keras.optimizers import Adam, Optimizer
+from keras.optimizers import Adam, Optimizer
 
 #####################################################################
 # Define the types of ResNet
 
 layer_type = Literal[
     "18-layer", "34-layer", "50-layer", "101-layer", "152-layer"
 ]
@@ -109,15 +111,15 @@
     conv_kernel: Tuple[int, int, int] = (7, 7, 3),
     strides: Tuple[int, int, int] = (2, 2, 2),
     padding: int = 3,
     max_pool_size: Tuple[int, int, int] = (3, 3, 2),
     activation: str = "relu",
     use_bias: bool = False,
     bn_epsilon: float = 1e-5,
-    pooling_padding: str = "same",
+    pooling_padding: str = "valid",
     axis: int = 3,
 ) -> Tensor:
     """
     Non-residual unit from He et al. (2015). Corresponds to "conv1" and the
     max pool.
     """
 
@@ -127,14 +129,15 @@
         conv_kernel,
         strides=strides,
         use_bias=use_bias,
         name="conv1",
     )(x)
     x = BatchNormalization(axis=axis, epsilon=bn_epsilon, name="conv1_bn")(x)
     x = Activation(activation, name="conv1_activation")(x)
+
     x = MaxPooling3D(
         max_pool_size,
         strides=strides,
         padding=pooling_padding,
         name="max_pool",
     )(x)
```

### Comparing `cellfinder-1.2.0/cellfinder/core/classify/tools.py` & `cellfinder-1.3.0rc0/cellfinder/core/classify/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 import os
-from typing import List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import List, Optional, Tuple, Union
 
+import keras
 import numpy as np
-import tensorflow as tf
-from tensorflow.keras import Model
+from keras import Model
 
 from cellfinder.core import logger
 from cellfinder.core.classify.resnet import build_model, layer_type
 
 
 def get_model(
     existing_model: Optional[os.PathLike] = None,
     model_weights: Optional[os.PathLike] = None,
     network_depth: Optional[layer_type] = None,
     learning_rate: float = 0.0001,
     inference: bool = False,
     continue_training: bool = False,
 ) -> Model:
-    """
-    Returns the correct model based on the arguments passed
+    """Returns the correct model based on the arguments passed
     :param existing_model: An existing, trained model. This is returned if it
     exists
     :param model_weights: This file is used to set the model weights if it
     exists
     :param network_depth: This defines the type of model to be created if
     necessary
     :param learning_rate: For creating a new model
     :param inference: If True, will ensure that a trained model exists. E.g.
     by using the default one
     :param continue_training: If True, will ensure that a trained model
     exists. E.g. by using the default one
-    :return: A tf.keras model
+    :return: A keras model
 
     """
     if existing_model is not None or network_depth is None:
         logger.debug(f"Loading model: {existing_model}")
-        return tf.keras.models.load_model(existing_model)
+        return keras.models.load_model(existing_model)
     else:
         logger.debug(f"Creating a new instance of model: {network_depth}")
         model = build_model(
-            network_depth=network_depth, learning_rate=learning_rate
+            network_depth=network_depth,
+            learning_rate=learning_rate,
         )
         if inference or continue_training:
             logger.debug(
-                f"Setting model weights according to: {model_weights}"
+                f"Setting model weights according to: {model_weights}",
             )
             if model_weights is None:
-                raise IOError("`model_weights` must be provided")
+                raise OSError("`model_weights` must be provided")
             model.load_weights(model_weights)
         return model
 
 
 def make_lists(
-    tiff_files: Sequence, train: bool = True
+    tiff_files: Sequence,
+    train: bool = True,
 ) -> Union[Tuple[List, List], Tuple[List, List, np.ndarray]]:
     signal_list = []
     background_list = []
     if train:
         labels = []
 
     for group in tiff_files:
```

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/detect.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/classical_filter.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/download/cli.py` & `cellfinder-1.3.0rc0/cellfinder/core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/download/download.py` & `cellfinder-1.3.0rc0/cellfinder/core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/main.py` & `cellfinder-1.3.0rc0/cellfinder/core/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-"""
-N.B imports are within functions to prevent tensorflow being imported before
-it's warnings are silenced
-"""
-
 import os
 from typing import Callable, List, Optional, Tuple
 
 import numpy as np
 from brainglobe_utils.cells.cells import Cell
-from brainglobe_utils.general.logging import suppress_specific_logs
 
 from cellfinder.core import logger
 from cellfinder.core.download.download import model_type
 from cellfinder.core.train.train_yml import depth_type
 
-tf_suppress_log_messages = [
-    "multiprocessing can interact badly with TensorFlow"
-]
-
 
 def main(
     signal_array: np.ndarray,
     background_array: np.ndarray,
     voxel_sizes: Tuple[int, int, int],
     start_plane: int = 0,
     end_plane: int = -1,
@@ -54,21 +44,19 @@
     """
     Parameters
     ----------
     detect_callback : Callable[int], optional
         Called every time a plane has finished being processed during the
         detection stage. Called with the plane number that has finished.
     classify_callback : Callable[int], optional
-        Called every time tensorflow has finished classifying a point.
+        Called every time a point has finished being classified.
         Called with the batch number that has just finished.
     detect_finished_callback : Callable[list], optional
         Called after detection is finished with the list of detected points.
     """
-    suppress_tf_logging(tf_suppress_log_messages)
-
     from cellfinder.core.classify import classify
     from cellfinder.core.detect import detect
     from cellfinder.core.tools import prep
 
     if not skip_detection:
         logger.info("Detecting cell candidates")
 
@@ -94,15 +82,15 @@
     else:
         points = detected_cells or []  # if None
         detect_finished_callback(points)
 
     if not skip_classification:
         install_path = None
         model_weights = prep.prep_model_weights(
-            model_weights, install_path, model, n_free_cpus
+            model_weights, install_path, model
         )
         if len(points) > 0:
             logger.info("Running classification")
             points = classify.main(
                 points,
                 signal_array,
                 background_array,
@@ -116,21 +104,8 @@
                 trained_model,
                 model_weights,
                 network_depth,
                 callback=classify_callback,
             )
         else:
             logger.info("No candidates, skipping classification")
-
     return points
-
-
-def suppress_tf_logging(tf_suppress_log_messages: List[str]) -> None:
-    """
-    Prevents many lines of logs such as:
-    "2019-10-24 16:54:41.363978: I tensorflow/stream_executor/platform/default
-    /dso_loader.cc:44] Successfully opened dynamic library libcuda.so.1"
-    """
-    os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
-
-    for message in tf_suppress_log_messages:
-        suppress_specific_logs("tensorflow", message)
```

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/array_operations.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/geometry.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/image_processing.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/source_files.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/source_files.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/system.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/tiff.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/tools/tools.py` & `cellfinder-1.3.0rc0/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/core/train/train_yml.py` & `cellfinder-1.3.0rc0/cellfinder/core/train/train_yml.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,28 @@
 from pathlib import Path
 from typing import Dict, Literal
 
 from brainglobe_utils.general.numerical import (
     check_positive_float,
     check_positive_int,
 )
-from brainglobe_utils.general.system import ensure_directory_exists
+from brainglobe_utils.general.system import (
+    ensure_directory_exists,
+    get_num_processes,
+)
 from brainglobe_utils.IO.cells import find_relevant_tiffs
 from brainglobe_utils.IO.yaml import read_yaml_section
 from fancylog import fancylog
 from sklearn.model_selection import train_test_split
 
 import cellfinder.core as program_for_log
 from cellfinder.core import logger
 from cellfinder.core.classify.resnet import layer_type
 from cellfinder.core.download.download import DEFAULT_DOWNLOAD_DIRECTORY
 
-tf_suppress_log_messages = [
-    "sample_weight modes were coerced from",
-    "multiprocessing can interact badly with TensorFlow",
-]
-
 depth_type = Literal["18", "34", "50", "101", "152"]
 
 models: Dict[depth_type, layer_type] = {
     "18": "18-layer",
     "34": "34-layer",
     "50": "50-layer",
     "101": "101-layer",
@@ -314,19 +312,15 @@
     no_augment=False,
     tensorboard=False,
     save_weights=False,
     no_save_checkpoints=False,
     save_progress=False,
     epochs=100,
 ):
-    from cellfinder.core.main import suppress_tf_logging
-
-    suppress_tf_logging(tf_suppress_log_messages)
-
-    from tensorflow.keras.callbacks import (
+    from keras.callbacks import (
         CSVLogger,
         ModelCheckpoint,
         TensorBoard,
     )
 
     from cellfinder.core.classify.cube_generator import CubeGeneratorFromDisk
     from cellfinder.core.classify.tools import get_model, make_lists
@@ -335,15 +329,14 @@
     start_time = datetime.now()
 
     ensure_directory_exists(output_dir)
     model_weights = prep_model_weights(
         model_weights=model_weights,
         install_path=install_path,
         model_name=model,
-        n_free_cpus=n_free_cpus,
     )
 
     yaml_contents = parse_yaml(yaml_file)
 
     tiff_files = get_tiff_files(yaml_contents)
     logger.info(
         f"Found {sum(len(imlist) for imlist in tiff_files)} images "
@@ -357,14 +350,15 @@
         network_depth=models[network_depth],
         learning_rate=learning_rate,
         continue_training=continue_training,
     )
 
     signal_train, background_train, labels_train = make_lists(tiff_files)
 
+    n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
     if test_fraction > 0:
         logger.info("Splitting data into training and validation datasets")
         (
             signal_train,
             signal_test,
             background_train,
             background_test,
@@ -383,32 +377,36 @@
         )
         validation_generator = CubeGeneratorFromDisk(
             signal_test,
             background_test,
             labels=labels_test,
             batch_size=batch_size,
             train=True,
+            use_multiprocessing=False,
+            workers=n_processes,
         )
 
         # for saving checkpoints
-        base_checkpoint_file_name = "-epoch.{epoch:02d}-loss-{val_loss:.3f}.h5"
+        base_checkpoint_file_name = "-epoch.{epoch:02d}-loss-{val_loss:.3f}"
 
     else:
         logger.info("No validation data selected.")
         validation_generator = None
-        base_checkpoint_file_name = "-epoch.{epoch:02d}.h5"
+        base_checkpoint_file_name = "-epoch.{epoch:02d}"
 
     training_generator = CubeGeneratorFromDisk(
         signal_train,
         background_train,
         labels=labels_train,
         batch_size=batch_size,
         shuffle=True,
         train=True,
         augment=not no_augment,
+        use_multiprocessing=False,
+        workers=n_processes,
     )
     callbacks = []
 
     if tensorboard:
         logdir = output_dir / "tensorboard"
         ensure_directory_exists(logdir)
         tensorboard = TensorBoard(
@@ -417,44 +415,50 @@
             write_graph=True,
             update_freq="epoch",
         )
         callbacks.append(tensorboard)
 
     if not no_save_checkpoints:
         if save_weights:
-            filepath = str(output_dir / ("weight" + base_checkpoint_file_name))
+            filepath = str(
+                output_dir
+                / ("weight" + base_checkpoint_file_name + ".weights.h5")
+            )
         else:
-            filepath = str(output_dir / ("model" + base_checkpoint_file_name))
+            filepath = str(
+                output_dir / ("model" + base_checkpoint_file_name + ".keras")
+            )
 
         checkpoints = ModelCheckpoint(
             filepath,
             save_weights_only=save_weights,
         )
         callbacks.append(checkpoints)
 
     if save_progress:
-        filepath = str(output_dir / "training.csv")
-        csv_logger = CSVLogger(filepath)
+        csv_filepath = str(output_dir / "training.csv")
+        csv_logger = CSVLogger(csv_filepath)
         callbacks.append(csv_logger)
 
     logger.info("Beginning training.")
+    # Keras 3.0: `use_multiprocessing` input is set in the
+    # `training_generator` (False by default)
     model.fit(
         training_generator,
         validation_data=validation_generator,
-        use_multiprocessing=False,
         epochs=epochs,
         callbacks=callbacks,
     )
 
     if save_weights:
         logger.info("Saving model weights")
-        model.save_weights(str(output_dir / "model_weights.h5"))
+        model.save_weights(output_dir / "model.weights.h5")
     else:
         logger.info("Saving model")
-        model.save(output_dir / "model.h5")
+        model.save(output_dir / "model.keras")
 
     logger.info(
         "Finished training, " "Total time taken: %s",
         datetime.now() - start_time,
     )
```

### Comparing `cellfinder-1.2.0/cellfinder/napari/curation.py` & `cellfinder-1.3.0rc0/cellfinder/napari/curation.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/detect/detect.py` & `cellfinder-1.3.0rc0/cellfinder/napari/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.3.0rc0/cellfinder/napari/detect/detect_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.3.0rc0/cellfinder/napari/detect/thread_worker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/input_container.py` & `cellfinder-1.3.0rc0/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/napari.yaml` & `cellfinder-1.3.0rc0/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/sample_data.py` & `cellfinder-1.3.0rc0/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/train/train.py` & `cellfinder-1.3.0rc0/cellfinder/napari/train/train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/train/train_containers.py` & `cellfinder-1.3.0rc0/cellfinder/napari/train/train_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder/napari/utils.py` & `cellfinder-1.3.0rc0/cellfinder/napari/utils.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.2.0/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.3.0rc0/cellfinder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.2.0
+Version: 1.3.0rc0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -27,16 +27,16 @@
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
-Requires-Dist: tensorflow-macos<2.12.0,>=2.5.0; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tensorflow<2.12.0,>=2.5.0; platform_system != "Darwin" or platform_machine != "arm64"
+Requires-Dist: keras>=3.0.0
+Requires-Dist: torch>=2.1.0
 Requires-Dist: tifffile
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyinstrument; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `cellfinder-1.2.0/pyproject.toml` & `cellfinder-1.3.0rc0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,16 @@
     "dask[array]",
     "fancylog>=0.0.7",
     "natsort",
     "numba",
     "numpy",
     "scikit-image",
     "scikit-learn",
-    # See https://github.com/brainglobe/cellfinder-core/issues/103 for < 2.12.0 pin
-    "tensorflow-macos>=2.5.0,<2.12.0; platform_system=='Darwin' and platform_machine=='arm64'",
-    "tensorflow>=2.5.0,<2.12.0; platform_system!='Darwin' or platform_machine!='arm64'",
+    "keras>=3.0.0",
+    "torch>=2.1.0",
     "tifffile",
     "tqdm",
 ]
 dynamic = ["version"]
 
 [project.entry-points."napari.manifest"]
 cellfinder = "cellfinder.napari:napari.yaml"
@@ -75,15 +74,15 @@
 "User Support" = "https://forum.image.sc/tag/brainglobe"
 
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = 'setuptools.build_meta'
 
 [tool.black]
-target-version = ['py39', 'py310']
+target-version = ['py39', 'py310','py311']
 skip-string-normalization = false
 line-length = 79
 
 [tool.ruff]
 line-length = 79
 exclude = ["__init__.py", "build", ".eggs"]
 select = ["I", "E", "F"]
@@ -107,35 +106,38 @@
 addopts = "--cov=cellfinder"
 markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
 
 [tool.tox]
 legacy_tox_ini = """
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{39,310}
+envlist = py{39,310,311}
 isolated_build = true
 
 [gh-actions]
 python =
     3.9: py39
     3.10: py310
+    3.11: py311
 
 [testenv]
 commands = python -m pytest -v --color=yes --cov=cellfinder --cov-report=xml
 deps =
     pytest
     pytest-cov
     pytest-mock
     pytest-timeout
     # Even though napari is a requirement for cellfinder.napari, we have to
     # ensure it is installed with the default Qt backend here.
     napari[all]
     pytest-qt
 extras =
     napari
+setenv =
+    KERAS_BACKEND = torch
 passenv =
     NUMBA_DISABLE_JIT
     CI
     GITHUB_ACTIONS
     DISPLAY
     XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
```

