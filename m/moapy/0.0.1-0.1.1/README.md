# Comparing `tmp/moapy-0.0.1.tar.gz` & `tmp/moapy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moapy-0.0.1.tar", last modified: Tue May 28 06:02:55 2024, max compression
+gzip compressed data, was "moapy-0.1.1.tar", last modified: Tue May 28 08:25:38 2024, max compression
```

## Comparing `moapy-0.0.1.tar` & `moapy-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.085570 moapy-0.0.1/
--rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 moapy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7186 2024-05-28 06:02:55.083569 moapy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 moapy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.034291 moapy-0.0.1/moapy/
--rw-rw-rw-   0        0        0        0 2024-05-28 05:54:14.000000 moapy-0.0.1/moapy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.066830 moapy-0.0.1/moapy/base/
--rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 moapy-0.0.1/moapy/base/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.0.1/moapy/base/__init__.py
--rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 moapy-0.0.1/moapy/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 moapy-0.0.1/moapy/base/calculator_asd.py
--rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 moapy-0.0.1/moapy/base/dgncodeutil.py
--rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 moapy-0.0.1/moapy/base/engineers.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 moapy-0.0.1/moapy/base/geometry.py
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 moapy-0.0.1/moapy/base/meshutil.py
--rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 moapy-0.0.1/moapy/base/midasapi.py
--rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 moapy-0.0.1/moapy/base/midasapi.pyi
--rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 moapy-0.0.1/moapy/base/midasutil.py
--rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 moapy-0.0.1/moapy/base/midasutil_server.py
--rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 moapy-0.0.1/moapy/base/midasutil_web.py
--rw-rw-rw-   0        0        0     1330 2024-05-27 08:15:52.000000 moapy-0.0.1/moapy/base/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.066830 moapy-0.0.1/moapy/base/steel/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.0.1/moapy/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 moapy-0.0.1/moapy/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 moapy-0.0.1/moapy/base/symbol.py
--rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 moapy-0.0.1/moapy/base/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 moapy-0.0.1/moapy/base/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 moapy-0.0.1/moapy/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 moapy-0.0.1/moapy/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.073342 moapy-0.0.1/moapy/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.0.1/moapy/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.077573 moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.082564 moapy-0.0.1/moapy.egg-info/
--rw-rw-rw-   0        0        0     7186 2024-05-28 06:02:54.000000 moapy-0.0.1/moapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      992 2024-05-28 06:02:54.000000 moapy-0.0.1/moapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 06:02:54.000000 moapy-0.0.1/moapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-28 06:02:54.000000 moapy-0.0.1/moapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 06:02:54.000000 moapy-0.0.1/moapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 06:02:55.085570 moapy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-28 06:02:43.000000 moapy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:55.078908 moapy-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 moapy-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-05-27 03:36:50.000000 moapy-0.0.1/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.816928 moapy-0.1.1/
+-rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 moapy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7186 2024-05-28 08:25:38.815385 moapy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 moapy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.793678 moapy-0.1.1/moapy/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 moapy-0.1.1/moapy/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 moapy-0.1.1/moapy/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 moapy-0.1.1/moapy/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 moapy-0.1.1/moapy/geometry.py
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 moapy-0.1.1/moapy/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/midasutil_web.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.802186 moapy-0.1.1/moapy/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.806187 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+-rw-rw-rw-   0        0        0     1330 2024-05-27 08:15:52.000000 moapy-0.1.1/moapy/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.807487 moapy-0.1.1/moapy/steel/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 moapy-0.1.1/moapy/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 moapy-0.1.1/moapy/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 moapy-0.1.1/moapy/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 moapy-0.1.1/moapy/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 moapy-0.1.1/moapy/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.813384 moapy-0.1.1/moapy.egg-info/
+-rw-rw-rw-   0        0        0     7186 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:25:38.816928 moapy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-05-28 08:25:09.000000 moapy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.807487 moapy-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 moapy-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-27 03:36:50.000000 moapy-0.1.1/tests/test_baseplate_kds.py
```

### Comparing `moapy-0.0.1/PKG-INFO` & `moapy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moapy
-Version: 0.0.1
+Version: 0.1.1
 Summary: Midas Open API for Python
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `moapy-0.0.1/README.md` & `moapy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/ReportUtil.py` & `moapy-0.1.1/moapy/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/baseformidasapi.py` & `moapy-0.1.1/moapy/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/calculator_asd.py` & `moapy-0.1.1/moapy/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/dgncodeutil.py` & `moapy-0.1.1/moapy/dgncodeutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/geometry.py` & `moapy-0.1.1/moapy/geometry.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/meshutil.py` & `moapy-0.1.1/moapy/meshutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/midasapi.py` & `moapy-0.1.1/moapy/midasapi.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/midasapi.pyi` & `moapy-0.1.1/moapy/midasapi.pyi`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/midasutil.py` & `moapy-0.1.1/moapy/midasutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/midasutil_server.py` & `moapy-0.1.1/moapy/midasutil_server.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/midasutil_web.py` & `moapy-0.1.1/moapy/midasutil_web.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/section_property.py` & `moapy-0.1.1/moapy/section_property.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/steel/steelutil.py` & `moapy-0.1.1/moapy/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/symbol.py` & `moapy-0.1.1/moapy/symbol.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/unit_converter.py` & `moapy-0.1.1/moapy/unit_converter.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/base/vector.py` & `moapy-0.1.1/moapy/vector.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `moapy-0.0.1/moapy.egg-info/PKG-INFO` & `moapy-0.1.1/moapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moapy
-Version: 0.0.1
+Version: 0.1.1
 Summary: Midas Open API for Python
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `moapy-0.0.1/setup.py` & `moapy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 def readme():
     with open('README_en.md', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='moapy',
-    version='0.0.1',
+    version='0.1.1',
     packages=find_packages(),
     include_package_data=True,
     description='Midas Open API for Python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
     url='https://github.com/MIDASIT-Co-Ltd/engineers-api-python',
     install_requires=['mdutils', "numpy", "matplotlib"],
     extras_require={
         'full': ["concreteproperties", "sectionproperties"],
     },
 )
+
```

### Comparing `moapy-0.0.1/tests/test_baseplate_kds.py` & `moapy-0.1.1/tests/test_baseplate_kds.py`

 * *Files identical despite different names*

