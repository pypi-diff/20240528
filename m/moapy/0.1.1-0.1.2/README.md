# Comparing `tmp/moapy-0.1.1.tar.gz` & `tmp/moapy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moapy-0.1.1.tar", last modified: Tue May 28 08:25:38 2024, max compression
+gzip compressed data, was "moapy-0.1.2.tar", last modified: Tue May 28 08:46:03 2024, max compression
```

## Comparing `moapy-0.1.1.tar` & `moapy-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.816928 moapy-0.1.1/
--rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 moapy-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7186 2024-05-28 08:25:38.815385 moapy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 moapy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.793678 moapy-0.1.1/moapy/
--rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/__init__.py
--rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 moapy-0.1.1/moapy/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 moapy-0.1.1/moapy/calculator_asd.py
--rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 moapy-0.1.1/moapy/dgncodeutil.py
--rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/engineers.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 moapy-0.1.1/moapy/geometry.py
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 moapy-0.1.1/moapy/meshutil.py
--rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasapi.py
--rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasapi.pyi
--rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/midasutil.py
--rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 moapy-0.1.1/moapy/midasutil_server.py
--rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/midasutil_web.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.802186 moapy-0.1.1/moapy/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.806187 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
--rw-rw-rw-   0        0        0     1330 2024-05-27 08:15:52.000000 moapy-0.1.1/moapy/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.807487 moapy-0.1.1/moapy/steel/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.1/moapy/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 moapy-0.1.1/moapy/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 moapy-0.1.1/moapy/symbol.py
--rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 moapy-0.1.1/moapy/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 moapy-0.1.1/moapy/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 moapy-0.1.1/moapy/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 moapy-0.1.1/moapy/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.813384 moapy-0.1.1/moapy.egg-info/
--rw-rw-rw-   0        0        0     7186 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 08:25:38.000000 moapy-0.1.1/moapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 08:25:38.816928 moapy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-05-28 08:25:09.000000 moapy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:38.807487 moapy-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 moapy-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-05-27 03:36:50.000000 moapy-0.1.1/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.820902 moapy-0.1.2/
+-rw-rw-rw-   0        0        0       56 2024-05-28 08:45:47.000000 moapy-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7186 2024-05-28 08:46:03.819899 moapy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 moapy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.796640 moapy-0.1.2/moapy/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 moapy-0.1.2/moapy/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.2/moapy/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 moapy-0.1.2/moapy/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 moapy-0.1.2/moapy/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 moapy-0.1.2/moapy/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 moapy-0.1.2/moapy/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 moapy-0.1.2/moapy/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 moapy-0.1.2/moapy/hello.html
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 moapy-0.1.2/moapy/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 moapy-0.1.2/moapy/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 moapy-0.1.2/moapy/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 moapy-0.1.2/moapy/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 moapy-0.1.2/moapy/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 moapy-0.1.2/moapy/midasutil_web.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.804281 moapy-0.1.2/moapy/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.2/moapy/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.809510 moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.811639 moapy-0.1.2/moapy/project/sectionproperty/
+-rw-rw-rw-   0        0        0      504 2024-05-27 08:38:03.000000 moapy-0.1.2/moapy/project/sectionproperty/report_sectionproperty.py
+-rw-rw-rw-   0        0        0     1312 2024-05-28 08:44:34.000000 moapy-0.1.2/moapy/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.813863 moapy-0.1.2/moapy/steel/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 moapy-0.1.2/moapy/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 moapy-0.1.2/moapy/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 moapy-0.1.2/moapy/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 moapy-0.1.2/moapy/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 moapy-0.1.2/moapy/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 moapy-0.1.2/moapy/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 moapy-0.1.2/moapy/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.817899 moapy-0.1.2/moapy.egg-info/
+-rw-rw-rw-   0        0        0     7186 2024-05-28 08:46:03.000000 moapy-0.1.2/moapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      942 2024-05-28 08:46:03.000000 moapy-0.1.2/moapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:46:03.000000 moapy-0.1.2/moapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-28 08:46:03.000000 moapy-0.1.2/moapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 08:46:03.000000 moapy-0.1.2/moapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:46:03.820902 moapy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-05-28 08:45:57.000000 moapy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:46:03.816899 moapy-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 moapy-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-27 03:36:50.000000 moapy-0.1.2/tests/test_baseplate_kds.py
```

### Comparing `moapy-0.1.1/PKG-INFO` & `moapy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moapy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Midas Open API for Python
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `moapy-0.1.1/README.md` & `moapy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/ReportUtil.py` & `moapy-0.1.2/moapy/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/baseformidasapi.py` & `moapy-0.1.2/moapy/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/calculator_asd.py` & `moapy-0.1.2/moapy/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/dgncodeutil.py` & `moapy-0.1.2/moapy/dgncodeutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/geometry.py` & `moapy-0.1.2/moapy/geometry.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/meshutil.py` & `moapy-0.1.2/moapy/meshutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/midasapi.py` & `moapy-0.1.2/moapy/midasapi.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/midasapi.pyi` & `moapy-0.1.2/moapy/midasapi.pyi`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/midasutil.py` & `moapy-0.1.2/moapy/midasutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/midasutil_server.py` & `moapy-0.1.2/moapy/midasutil_server.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/midasutil_web.py` & `moapy-0.1.2/moapy/midasutil_web.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `moapy-0.1.2/moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/section_property.py` & `moapy-0.1.2/moapy/section_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sectionproperties.analysis.section import Section
 from sectionproperties.pre.geometry import Polygon, Geometry
 import json
 import base.ReportUtil as rptutil
-import project.sectionproperty.report_sectionproperty
+import moapy.section_property as sp
 
 def calc(dictvertices):
     polygon = Polygon(dictvertices)
     geom = Geometry(polygon)
     geom.create_mesh(mesh_sizes=100.0)
 
     section = Section(geom)
```

### Comparing `moapy-0.1.1/moapy/steel/steelutil.py` & `moapy-0.1.2/moapy/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/symbol.py` & `moapy-0.1.2/moapy/symbol.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/unit_converter.py` & `moapy-0.1.2/moapy/unit_converter.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy/vector.py` & `moapy-0.1.2/moapy/vector.py`

 * *Files identical despite different names*

### Comparing `moapy-0.1.1/moapy.egg-info/PKG-INFO` & `moapy-0.1.2/moapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moapy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Midas Open API for Python
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `moapy-0.1.1/moapy.egg-info/SOURCES.txt` & `moapy-0.1.2/moapy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 moapy/ReportUtil.py
 moapy/__init__.py
 moapy/baseformidasapi.py
 moapy/calculator_asd.py
 moapy/dgncodeutil.py
 moapy/engineers.py
 moapy/geometry.py
+moapy/hello.html
 moapy/meshutil.py
 moapy/midasapi.py
 moapy/midasapi.pyi
 moapy/midasutil.py
 moapy/midasutil_server.py
 moapy/midasutil_web.py
 moapy/section_property.py
@@ -25,11 +26,12 @@
 moapy.egg-info/dependency_links.txt
 moapy.egg-info/requires.txt
 moapy.egg-info/top_level.txt
 moapy/project/__init__.py
 moapy/project/baseplate_KDS41_30_2022/__init__.py
 moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
 moapy/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+moapy/project/sectionproperty/report_sectionproperty.py
 moapy/steel/__init__.py
 moapy/steel/steelutil.py
 tests/__init__.py
 tests/test_baseplate_kds.py
```

### Comparing `moapy-0.1.1/setup.py` & `moapy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README_en.md', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='moapy',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     description='Midas Open API for Python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
```

### Comparing `moapy-0.1.1/tests/test_baseplate_kds.py` & `moapy-0.1.2/tests/test_baseplate_kds.py`

 * *Files identical despite different names*

