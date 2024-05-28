# Comparing `tmp/pyQuadriFlow-0.0.2.tar.gz` & `tmp/pyquadriflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyQuadriFlow-0.0.2.tar", last modified: Sat May 25 11:13:52 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyQuadriFlow-0.0.2.tar` & `pyquadriflow-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,13 @@
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
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/setup.cfg
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/__init__.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/pyQuadriFlow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/clib/__init__.py
+-rw-r--r--   0        0        0   540672 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/clib/ctypes_QuadriFlow.dll
+-rw-r--r--   0        0        0  1635432 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/clib/ctypes_QuadriFlow.so
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/src/pyQuadriFlow/clib/load_library.py
+-rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/.gitignore
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pyquadriflow-0.0.4/PKG-INFO
```

### Comparing `pyQuadriFlow-0.0.2/README.md` & `pyquadriflow-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/pyQuadriFlow/clib/ctypes_QuadriFlow.dll` & `pyquadriflow-0.0.4/src/pyQuadriFlow/clib/ctypes_QuadriFlow.dll`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/pyQuadriFlow/clib/ctypes_QuadriFlow.so` & `pyquadriflow-0.0.4/src/pyQuadriFlow/clib/ctypes_QuadriFlow.so`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/pyQuadriFlow/clib/load_library.py` & `pyquadriflow-0.0.4/src/pyQuadriFlow/clib/load_library.py`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/pyQuadriFlow/pyQuadriFlow.py` & `pyquadriflow-0.0.4/src/pyQuadriFlow/pyQuadriFlow.py`

 * *Files identical despite different names*

### Comparing `pyQuadriFlow-0.0.2/setup.py` & `pyquadriflow-0.0.4/setup.py`

 * *Files identical despite different names*

