# Comparing `tmp/arvados-cwl-runner-2.7.2.tar.gz` & `tmp/arvados-cwl-runner-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.7.2.tar", last modified: Tue Apr  9 20:11:28 2024, max compression
+gzip compressed data, was "arvados-cwl-runner-2.7.3.tar", last modified: Tue May 28 15:09:52 2024, max compression
```

## Comparing `arvados-cwl-runner-2.7.2.tar` & `arvados-cwl-runner-2.7.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21372 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14533 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13027 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13514 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35935 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5794 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34462 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2260 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3935 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    45214 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18053 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    40584 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      213 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2140 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73538 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87248 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 15:09:52.567426 arvados-cwl-runner-2.7.3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-05-28 15:09:52.567426 arvados-cwl-runner-2.7.3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 15:09:52.515421 arvados-cwl-runner-2.7.3/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21372 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14533 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13027 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13514 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35935 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5794 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34462 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2260 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3935 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    45214 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18053 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    40584 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 15:09:52.515421 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2024-05-28 15:09:52.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 15:09:52.515421 arvados-cwl-runner-2.7.3/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 15:09:52.567426 arvados-cwl-runner-2.7.3/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 15:09:52.567426 arvados-cwl-runner-2.7.3/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73538 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87248 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2024-05-28 13:36:07.000000 arvados-cwl-runner-2.7.3/tests/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arvados-cwl-runner-2.7.2/LICENSE-2.0.txt` & `arvados-cwl-runner-2.7.3/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/PKG-INFO` & `arvados-cwl-runner-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.7.2
+Version: 2.7.3
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.7.3/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/arvcontainer.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/context.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/done.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/executor.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/executor.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/perf.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/runner.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl/util.py` & `arvados-cwl-runner-2.7.3/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.7.2
+Version: 2.7.3
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.7.3/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/arvados_version.py` & `arvados-cwl-runner-2.7.3/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/setup.py` & `arvados-cwl-runner-2.7.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,21 @@
           'ciso8601 >= 2.0.0',
           'networkx < 2.6',
           'msgpack==1.0.3',
           'importlib-metadata<5',
           'setuptools>=40.3.0',
 
           # zipp 3.16 dropped support for Python 3.7
-          'zipp<3.16.0; python_version<"3.8"'
+          'zipp<3.16.0; python_version<"3.8"',
+
+          # lxml 5.2 dropped support for Python 3.7
+          'lxml<5.2; python_version<"3.8"',
+
+          # pydot 2.0 requires pyparsing>=3 which creates a conflict
+          'pydot<2',
       ],
       data_files=[
           ('share/doc/arvados-cwl-runner', ['LICENSE-2.0.txt', 'README.rst']),
       ],
       python_requires=">=3.5, <4",
       classifiers=[
           'Programming Language :: Python :: 3',
```

### Comparing `arvados-cwl-runner-2.7.2/tests/matcher.py` & `arvados-cwl-runner-2.7.3/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_container.py` & `arvados-cwl-runner-2.7.3/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_copy_deps.py` & `arvados-cwl-runner-2.7.3/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_fsaccess.py` & `arvados-cwl-runner-2.7.3/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_make_output.py` & `arvados-cwl-runner-2.7.3/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_pathmapper.py` & `arvados-cwl-runner-2.7.3/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.7.3/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_submit.py` & `arvados-cwl-runner-2.7.3/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_tq.py` & `arvados-cwl-runner-2.7.3/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_urljoin.py` & `arvados-cwl-runner-2.7.3/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.2/tests/test_util.py` & `arvados-cwl-runner-2.7.3/tests/test_util.py`

 * *Files identical despite different names*

