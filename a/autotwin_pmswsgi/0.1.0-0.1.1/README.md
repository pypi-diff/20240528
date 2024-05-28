# Comparing `tmp/autotwin_pmswsgi-0.1.0.tar.gz` & `tmp/autotwin_pmswsgi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotwin_pmswsgi-0.1.0.tar", max compression
+gzip compressed data, was "autotwin_pmswsgi-0.1.1.tar", max compression
```

## Comparing `autotwin_pmswsgi-0.1.0.tar` & `autotwin_pmswsgi-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1571 2024-05-14 09:56:06.566009 autotwin_pmswsgi-0.1.0/LICENSE
--rw-r--r--   0        0        0     7014 2024-05-14 09:56:06.566009 autotwin_pmswsgi-0.1.0/README.md
--rw-r--r--   0        0        0     3254 2024-05-14 09:56:06.566009 autotwin_pmswsgi-0.1.0/autotwin_pmswsgi.py
--rw-r--r--   0        0        0     1064 2024-05-14 09:56:06.566009 autotwin_pmswsgi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 autotwin_pmswsgi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1571 2024-05-28 09:22:22.920289 autotwin_pmswsgi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7241 2024-05-28 09:22:22.920289 autotwin_pmswsgi-0.1.1/README.md
+-rw-r--r--   0        0        0     3254 2024-05-28 09:22:22.920289 autotwin_pmswsgi-0.1.1/autotwin_pmswsgi.py
+-rw-r--r--   0        0        0     1064 2024-05-28 09:22:22.920289 autotwin_pmswsgi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8014 1970-01-01 00:00:00.000000 autotwin_pmswsgi-0.1.1/PKG-INFO
```

### Comparing `autotwin_pmswsgi-0.1.0/LICENSE` & `autotwin_pmswsgi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotwin_pmswsgi-0.1.0/README.md` & `autotwin_pmswsgi-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,32 +70,36 @@
 
 **Parameters**
 > None
 
 **Body**
 > Definition
 >
-> | Name                   | Type                    | Description                            |
-> |------------------------|-------------------------|----------------------------------------|
-> | `name`                 | `string`                | Name of the system to be discovered    |
-> | `version`              | `string`                | Version of the system to be discovered |
-> | `neo4j:interval`       | `array[number\|string]` | Interval of the event log to be used   |
-> | `model:delays:seize`   | `number\|string`        | Delay in seizing a queued part         |
-> | `model:delays:release` | `number\|string`        | Delay in releasing a blocked part      |
-> | `model:cdf:points`     | `number`                | Maximum number of points in CDFs       |
+> | Name                   | Type                    | Description                                   |
+> |------------------------|-------------------------|-----------------------------------------------|
+> | `name`                 | `string`                | Name of the system to be discovered           |
+> | `version`              | `string`                | Version of the system to be discovered        |
+> | `neo4j:interval`       | `array[number\|string]` | Interval of the event log to be used          |
+> | `model:formula:ratio`  | `number`                | Minimum ratio of a formula to the primary one |
+> | `model:delays:seize`   | `number\|string`        | Delay in seizing a queued part                |
+> | `model:delays:release` | `number\|string`        | Delay in releasing a blocked part             |
+> | `model:cdf:points`     | `number`                | Maximum number of points in a CDF             |
 
 > Example
 > ```json
 > {
 >     "name": "Pizza Line",
 >     "version": "V4",
 >     "neo4j": {
 >         "interval": [0, 500000000]
 >     },
 >     "model": {
+>         "formula": {
+>             "ratio": 0.06
+>         },
 >         "delays": {
 >             "seize": 30000,
 >             "release": 0
 >         },
 >         "cdf": {
 >             "points": 100
 >         }
```

### Comparing `autotwin_pmswsgi-0.1.0/autotwin_pmswsgi.py` & `autotwin_pmswsgi-0.1.1/autotwin_pmswsgi.py`

 * *Files identical despite different names*

### Comparing `autotwin_pmswsgi-0.1.0/pyproject.toml` & `autotwin_pmswsgi-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autotwin_pmswsgi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Process Mining Service WSGI for Auto-Twin"
 license = "BSD-3-Clause"
 authors = [
     "Lulai Zhu <lulai.zhu@gmail.com>",
     "Wei Cheng <wei.cheng.me@gmail.com>",
     "Livia Lestingi <livia.lestingi@polimi.it>",
     "Matteo Giovanni Rossi <matteo.rossi@polimi.it>"
@@ -21,15 +21,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^3.0.2"
 Paste = "^3.7.1"
 waitress = "^3.0.0"
-autotwin_gmglib = "^0.1.0"
+autotwin_gmglib = "^0.1.1"
 
 [tool.poetry.group.test.dependencies]
 black = "^24.2.0"
 flake8 = "^7.0.0"
 pytest = "^8.0.0"
 
 [build-system]
```

### Comparing `autotwin_pmswsgi-0.1.0/PKG-INFO` & `autotwin_pmswsgi-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotwin_pmswsgi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Process Mining Service WSGI for Auto-Twin
 Home-page: https://github.com/AutotwinEU/proc-mining-serv
 License: BSD-3-Clause
 Keywords: auto-twin,system discovery,restful service
 Author: Lulai Zhu
 Author-email: lulai.zhu@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: Flask (>=3.0.2,<4.0.0)
 Requires-Dist: Paste (>=3.7.1,<4.0.0)
-Requires-Dist: autotwin_gmglib (>=0.1.0,<0.2.0)
+Requires-Dist: autotwin_gmglib (>=0.1.1,<0.2.0)
 Requires-Dist: waitress (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![PyPI - License](https://img.shields.io/pypi/l/autotwin_pmswsgi)](https://github.com/AutotwinEU/proc-mining-serv/blob/main/LICENSE)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/autotwin_pmswsgi)](https://www.python.org/downloads/)
 [![PyPI - Version](https://img.shields.io/pypi/v/autotwin_pmswsgi)](https://pypi.org/project/autotwin_pmswsgi/)
 
@@ -95,32 +95,36 @@
 
 **Parameters**
 > None
 
 **Body**
 > Definition
 >
-> | Name                   | Type                    | Description                            |
-> |------------------------|-------------------------|----------------------------------------|
-> | `name`                 | `string`                | Name of the system to be discovered    |
-> | `version`              | `string`                | Version of the system to be discovered |
-> | `neo4j:interval`       | `array[number\|string]` | Interval of the event log to be used   |
-> | `model:delays:seize`   | `number\|string`        | Delay in seizing a queued part         |
-> | `model:delays:release` | `number\|string`        | Delay in releasing a blocked part      |
-> | `model:cdf:points`     | `number`                | Maximum number of points in CDFs       |
+> | Name                   | Type                    | Description                                   |
+> |------------------------|-------------------------|-----------------------------------------------|
+> | `name`                 | `string`                | Name of the system to be discovered           |
+> | `version`              | `string`                | Version of the system to be discovered        |
+> | `neo4j:interval`       | `array[number\|string]` | Interval of the event log to be used          |
+> | `model:formula:ratio`  | `number`                | Minimum ratio of a formula to the primary one |
+> | `model:delays:seize`   | `number\|string`        | Delay in seizing a queued part                |
+> | `model:delays:release` | `number\|string`        | Delay in releasing a blocked part             |
+> | `model:cdf:points`     | `number`                | Maximum number of points in a CDF             |
 
 > Example
 > ```json
 > {
 >     "name": "Pizza Line",
 >     "version": "V4",
 >     "neo4j": {
 >         "interval": [0, 500000000]
 >     },
 >     "model": {
+>         "formula": {
+>             "ratio": 0.06
+>         },
 >         "delays": {
 >             "seize": 30000,
 >             "release": 0
 >         },
 >         "cdf": {
 >             "points": 100
 >         }
```

