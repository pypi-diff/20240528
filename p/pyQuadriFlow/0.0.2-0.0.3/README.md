# Comparing `tmp/pyQuadriFlow-0.0.2.tar.gz` & `tmp/pyquadriflow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyQuadriFlow-0.0.2.tar", last modified: Sat May 25 11:13:52 2024, max compression
+gzip compressed data, was "pyquadriflow-0.0.3.tar", last modified: Tue May 28 12:37:19 2024, max compression
```

## Comparing `pyQuadriFlow-0.0.2.tar` & `pyquadriflow-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 11:13:52.159319 pyQuadriFlow-0.0.2/
--rw-rw-rw-   0        0        0     1135 2024-05-25 11:13:52.160769 pyQuadriFlow-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      672 2024-05-25 11:03:46.000000 pyQuadriFlow-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 11:13:52.152916 pyQuadriFlow-0.0.2/pyQuadriFlow/
--rw-rw-rw-   0        0        0        0 2024-05-24 20:34:01.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 11:13:52.159319 pyQuadriFlow-0.0.2/pyQuadriFlow/clib/
--rw-rw-rw-   0        0        0        0 2024-05-24 20:34:01.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/clib/__init__.py
--rw-rw-rw-   0        0        0   540672 2024-05-24 20:58:05.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/clib/ctypes_QuadriFlow.dll
--rw-rw-rw-   0        0        0  1635432 2024-05-24 21:02:09.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/clib/ctypes_QuadriFlow.so
--rw-rw-rw-   0        0        0      576 2024-05-24 20:34:01.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/clib/load_library.py
--rw-rw-rw-   0        0        0     3249 2024-05-24 20:34:01.000000 pyQuadriFlow-0.0.2/pyQuadriFlow/pyQuadriFlow.py
-drwxrwxrwx   0        0        0        0 2024-05-25 11:13:52.156383 pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/
--rw-rw-rw-   0        0        0     1135 2024-05-25 11:13:52.000000 pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-25 11:13:52.000000 pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 11:13:52.000000 pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-25 11:13:52.000000 pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 11:13:52.161754 pyQuadriFlow-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1128 2024-05-25 11:12:34.000000 pyQuadriFlow-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:37:19.952654 pyquadriflow-0.0.3/
+-rw-rw-rw-   0        0        0        3 2024-05-28 12:16:58.000000 pyquadriflow-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1365 2024-05-28 12:37:19.952654 pyquadriflow-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2024-05-25 11:03:46.000000 pyquadriflow-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 12:37:19.942965 pyquadriflow-0.0.3/pyQuadriFlow.egg-info/
+-rw-rw-rw-   0        0        0     1365 2024-05-28 12:37:19.000000 pyquadriflow-0.0.3/pyQuadriFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-28 12:37:19.000000 pyquadriflow-0.0.3/pyQuadriFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:37:19.000000 pyquadriflow-0.0.3/pyQuadriFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:37:19.000000 pyquadriflow-0.0.3/pyQuadriFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      634 2024-05-28 12:37:13.000000 pyquadriflow-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:37:19.954203 pyquadriflow-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-05-25 11:12:34.000000 pyquadriflow-0.0.3/setup.py
```

### Comparing `pyQuadriFlow-0.0.2/PKG-INFO` & `pyquadriflow-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: pyQuadriFlow
-Version: 0.0.2
-Summary: Python QuadriFlow.
+Version: 0.0.3
+Summary: Python QuadriFlow wrapper
 Author: Satabol
+Author-email: Satabol <satabol@yandex.ru>
+Project-URL: Homepage, https://github.com/satabol/pyQuadriFlow
+Project-URL: Issues, https://github.com/satabol/pyQuadriFlow/issues
 Keywords: quadriflow,quad,remeshing,quadrangulation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This is a Python wrapper of quadriflow used in the Blender:
 
 ![image](https://github.com/satabol/QuadriFlow/assets/14288520/56dd4baf-284f-4cbb-b866-61b434e44b1b)
 
 See https://github.com/satabol/pyQuadriFlow
```

### Comparing `pyQuadriFlow-0.0.2/README.md` & `pyquadriflow-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/pyQuadriFlow.egg-info/PKG-INFO` & `pyquadriflow-0.0.3/pyQuadriFlow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: pyQuadriFlow
-Version: 0.0.2
-Summary: Python QuadriFlow.
+Version: 0.0.3
+Summary: Python QuadriFlow wrapper
 Author: Satabol
+Author-email: Satabol <satabol@yandex.ru>
+Project-URL: Homepage, https://github.com/satabol/pyQuadriFlow
+Project-URL: Issues, https://github.com/satabol/pyQuadriFlow/issues
 Keywords: quadriflow,quad,remeshing,quadrangulation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This is a Python wrapper of quadriflow used in the Blender:
 
 ![image](https://github.com/satabol/QuadriFlow/assets/14288520/56dd4baf-284f-4cbb-b866-61b434e44b1b)
 
 See https://github.com/satabol/pyQuadriFlow
```

### Comparing `pyQuadriFlow-0.0.2/setup.py` & `pyquadriflow-0.0.3/setup.py`

 * *Files identical despite different names*

