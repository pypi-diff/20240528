# Comparing `tmp/adam_assist-0.1.0.tar.gz` & `tmp/adam_assist-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_assist-0.1.0.tar", last modified: Tue May 28 18:25:57 2024, max compression
+gzip compressed data, was "adam_assist-0.1.1a1.tar", last modified: Tue May 28 19:45:22 2024, max compression
```

## Comparing `adam_assist-0.1.0.tar` & `adam_assist-0.1.1a1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     9721 2024-05-28 18:20:35.619053 adam_assist-0.1.0/LICENSE
--rw-r--r--   0        0        0      384 2024-05-28 18:21:23.001059 adam_assist-0.1.0/README.md
--rw-r--r--   0        0        0     2027 2024-05-28 18:25:57.524507 adam_assist-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    21730 2024-05-28 18:20:35.613218 adam_assist-0.1.0/src/adam_core/propagator/adam_assist.py
--rw-r--r--   0        0        0      108 2023-10-30 16:49:04.234853 adam_assist-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5471 2024-05-15 14:10:31.374416 adam_assist-0.1.0/tests/data/I00007_orbit.parquet
--rw-r--r--   0        0        0      983 2024-05-15 14:10:33.961975 adam_assist-0.1.0/tests/test_impacts.py
--rw-r--r--   0        0        0     1052 2024-05-15 14:10:33.962138 adam_assist-0.1.0/tests/test_propagate.py
--rw-r--r--   0        0        0    13020 1970-01-01 00:00:00.000000 adam_assist-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9721 2024-05-28 18:20:35.619053 adam_assist-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0      384 2024-05-28 18:21:23.001059 adam_assist-0.1.1a1/README.md
+-rw-r--r--   0        0        0     2172 2024-05-28 19:45:22.641230 adam_assist-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0    21851 2024-05-28 18:29:43.863344 adam_assist-0.1.1a1/src/adam_core/propagator/adam_assist.py
+-rw-r--r--   0        0        0       23 2024-05-28 19:45:22.640081 adam_assist-0.1.1a1/src/adam_core/propagator/adam_assist_version.py
+-rw-r--r--   0        0        0      108 2023-10-30 16:49:04.234853 adam_assist-0.1.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     5471 2024-05-15 14:10:31.374416 adam_assist-0.1.1a1/tests/data/I00007_orbit.parquet
+-rw-r--r--   0        0        0      983 2024-05-15 14:10:33.961975 adam_assist-0.1.1a1/tests/test_impacts.py
+-rw-r--r--   0        0        0     1052 2024-05-15 14:10:33.962138 adam_assist-0.1.1a1/tests/test_propagate.py
+-rw-r--r--   0        0        0    13022 1970-01-01 00:00:00.000000 adam_assist-0.1.1a1/PKG-INFO
```

### Comparing `adam_assist-0.1.0/LICENSE` & `adam_assist-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `adam_assist-0.1.0/pyproject.toml` & `adam_assist-0.1.1a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "adam-assist"
-version = "0.1.0"
+dynamic = []
 description = "ADAM Core Propagator class using ASSIST"
 authors = [
     { name = "Alec Koumjian", email = "akoumjian@gmail.com" },
     { name = "Kathleen Kiker" },
 ]
 readme = "README.md"
 keywords = [
@@ -25,14 +25,15 @@
     "adam-core>=0.2.0a1",
     "assist",
     "naif-de440",
     "numpy",
     "ray",
     "spiceypy>=6.0.0",
 ]
+version = "0.1.1a1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Documentation = "https://github.com/unknown/adam-assist#readme"
 Issues = "https://github.com/unknown/adam-assist/issues"
@@ -58,14 +59,19 @@
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
 includes = [
     "src/adam_core/",
 ]
 
+[tool.pdm.version]
+source = "scm"
+write_to = "adam_core/propagator/adam_assist_version.py"
+write_template = "__version__ = '{}'"
+
 [tool.pdm.scripts]
 fix = "ruff ./src/adam_core --fix"
 typecheck = "mypy --strict ./src/adam_core"
 test = "pytest --benchmark-disable {args}"
 doctest = "pytest --doctest-plus --doctest-only"
 benchmark = "pytest --benchmark-only"
 coverage = "pytest --cov=src --cov-report=xml"
```

### Comparing `adam_assist-0.1.0/src/adam_core/propagator/adam_assist.py` & `adam_assist-0.1.1a1/src/adam_core/propagator/adam_assist.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     EphemerisType,
     ObserverType,
     OrbitType,
     Propagator,
     TimestampType,
 )
 
+try:
+    from adam_core.propagator.adam_assist_version import __version__
+except ImportError:
+    __version__ = "0.0.0"
+
 DATA_DIR = os.getenv("ASSIST_DATA_DIR", "~/.adam_assist_data")
 
 # Use the Earth's equatorial radius as used in DE4XX ephemerides
 # adam_core defines it in au but we need it in km
 EARTH_RADIUS_KM = Constants.R_EARTH * KM_P_AU
```

### Comparing `adam_assist-0.1.0/tests/data/I00007_orbit.parquet` & `adam_assist-0.1.1a1/tests/data/I00007_orbit.parquet`

 * *Files identical despite different names*

### Comparing `adam_assist-0.1.0/tests/test_impacts.py` & `adam_assist-0.1.1a1/tests/test_impacts.py`

 * *Files identical despite different names*

### Comparing `adam_assist-0.1.0/tests/test_propagate.py` & `adam_assist-0.1.1a1/tests/test_propagate.py`

 * *Files identical despite different names*

### Comparing `adam_assist-0.1.0/PKG-INFO` & `adam_assist-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-assist
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: ADAM Core Propagator class using ASSIST
 Keywords: astronomy,orbital mechanics,propagation
 Author: Kathleen Kiker
 Author-Email: Alec Koumjian <akoumjian@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
```

