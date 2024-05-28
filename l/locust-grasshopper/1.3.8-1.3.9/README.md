# Comparing `tmp/locust-grasshopper-1.3.8.tar.gz` & `tmp/locust-grasshopper-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-grasshopper-1.3.8.tar", last modified: Mon Sep 25 21:58:10 2023, max compression
+gzip compressed data, was "locust-grasshopper-1.3.9.tar", last modified: Tue Sep 26 22:48:01 2023, max compression
```

## Comparing `locust-grasshopper-1.3.8.tar` & `locust-grasshopper-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21193 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-09-25 21:57:56.000000 locust-grasshopper-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/grasshopper/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/grasshopper/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/grasshopper/lib/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/configuration/gh_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/grasshopper/lib/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    25172 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/fixtures/grasshopper_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/grasshopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.657603 locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/base_journey.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/temp_gh_composite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/er_basic_console_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/iextendedreporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/reporter_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/shared_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/src/grasshopper/lib/util/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/check_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-09-25 21:57:54.000000 locust-grasshopper-1.3.8/src/grasshopper/lib/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:58:10.661603 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-25 21:58:10.000000 locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.227045 locust-grasshopper-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2023-09-26 22:48:01.227045 locust-grasshopper-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-09-26 22:47:45.000000 locust-grasshopper-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 22:48:01.227045 locust-grasshopper-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/configuration/gh_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/fixtures/grasshopper_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/grasshopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/base_journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/temp_gh_composite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/iextendedreporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/reporter_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/shared_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.223045 locust-grasshopper-1.3.9/src/grasshopper/lib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/check_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-09-26 22:47:42.000000 locust-grasshopper-1.3.9/src/grasshopper/lib/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 22:48:01.227045 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-26 22:48:01.000000 locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/top_level.txt
```

### Comparing `locust-grasshopper-1.3.8/LICENSE` & `locust-grasshopper-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/PKG-INFO` & `locust-grasshopper-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.3.8
+Version: 1.3.9
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -219,15 +219,15 @@
 Classifier: Framework :: Pytest
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gevent~=21.12.0
 Requires-Dist: influxdb~=5.3.1
 Requires-Dist: locust~=2.12.2
-Requires-Dist: locust-influxdb-listener~=0.0.9
+Requires-Dist: locust-influxdb-listener~=1.0.2
 Requires-Dist: pytest~=6.2.5
 Requires-Dist: termcolor~=1.1.0
 Requires-Dist: pyyaml~=5.3.1
 Requires-Dist: tag-matcher~=0.0.5
 
 <div id="top"></div>
```

### Comparing `locust-grasshopper-1.3.8/README.md` & `locust-grasshopper-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/pyproject.toml` & `locust-grasshopper-1.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "cmake>=3.11.0,<4.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust-grasshopper"
-version = "1.3.8" # Managed by bump2version
+version = "1.3.9" # Managed by bump2version
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "a load testing tool extended from locust"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
@@ -29,15 +29,15 @@
 keywords = ["load testing", "performance", "locust", "grasshopper"]
 license = {file = "LICENSE"}
 requires-python = ">=3.9,<4"
 dependencies = [
     "gevent ~=21.12.0",
     "influxdb ~= 5.3.1",
     "locust ~= 2.12.2",
-    "locust-influxdb-listener ~= 0.0.9",
+    "locust-influxdb-listener ~= 1.0.2",
     "pytest ~= 6.2.5",
     "termcolor ~= 1.1.0",
     "pyyaml ~= 5.3.1",
     "tag-matcher ~= 0.0.5"
 ]
 
 [project.urls]
```

### Comparing `locust-grasshopper-1.3.8/setup.py` & `locust-grasshopper-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/configuration/gh_configuration.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/configuration/gh_configuration.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/fixtures/__init__.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/fixtures/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     for env_var_name, env_var_value in os.environ.items():
         if (
             env_var_name.lower() in ConfigurationConstants.COMPLETE_ATTRS.keys()
             or env_var_name.startswith(env_var_prefix_key)
             or env_var_name in extra_env_var_keys
         ):
             if env_var_name.startswith(env_var_prefix_key):
-                env_var_name = env_var_name.lstrip(env_var_prefix_key)
+                env_var_name = env_var_name.replace(env_var_prefix_key, "")
 
             if len(env_var_name) > 0:
                 config.update_single_key(env_var_name.lower(), env_var_value)
 
     logger.debug(f"CONFIG FIXTURE: env_var_args {config}")
 
     return config
```

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/fixtures/grasshopper_constants.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/fixtures/grasshopper_constants.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/grasshopper.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/grasshopper.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/base_journey.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/base_journey.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     """The base journey class for all other journey classes."""
 
     VUS_DICT = {}
     host = ""
     _incoming_test_parameters = {}
     abstract = True
     base_torn_down = False
-    defaults = {"tags": {}, "thresholds": {}}
+    tags = {}
+    defaults = {"tags": tags, "thresholds": {}}
 
     @classmethod
     @property
     def incoming_scenario_args(cls):
         return cls._incoming_test_parameters
 
     @property
@@ -47,28 +48,36 @@
     @classmethod
     def merge_incoming_scenario_args(cls, lower_precedence_args):
         """Add more values to scenario_args with lower precedence."""
         new_args = lower_precedence_args.copy()
         new_args.update(cls._incoming_test_parameters)
         cls.replace_incoming_scenario_args(new_args)
 
+    def update_tags(self, new_tags: dict):
+        """Update the tags for the influxdb listener."""
+        self.tags.update(new_tags)
+        db_listener = self.environment.grasshopper_listeners.influxdb_listener
+        if db_listener is not None:
+            db_listener.additional_tags.update(new_tags)
+
     @classmethod
     def reset_class_attributes(cls):
         """Reset the class level attributes to their starting state.
 
         We are using class level attributes because most of the time we want the state
         to be shared across all the instances of the class, since these values *should*
         always be the same across the instances and performance should be better without
         storing a copy for every instance.
 
         But in order to support unit testing and possibly other scenarios, this method
         is provided as a way to reset to the starting state.
         """
         cls._incoming_test_parameters = {}
-        cls.defaults = {"tags": {}}
+        cls.tags = {}
+        cls.defaults = {"tags": cls.tags}
         cls.host = ""
         cls.abstract = True
         cls.base_torn_down = False
         BaseJourney.VUS_DICT = {}
 
     @classmethod
     def get_journey_object_given_vu_number(cls, vu_number):
@@ -81,14 +90,15 @@
         self._merge_incoming_defaults_and_params()
         self._test_parameters = self._incoming_test_parameters.copy()
         self._set_base_teardown_listeners()
         self.client_id = str(uuid4())
         self._register_new_vu()
         self._set_thresholds()
         self.environment.host = self.scenario_args.get("target_url", "") or self.host
+        self.update_tags({"environment": self.environment.host})
 
         # TODO: currently global iterations is stored in the environment stats object
         # TODO: poke around to see if we can move it to a class attribute here
         self.vu_iteration = 0
 
     def _register_new_vu(self):
         """Increment the user count and return the new vu's number."""
```

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/journeys/temp_gh_composite.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/journeys/temp_gh_composite.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/er_basic_console_reporter.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/iextendedreporter.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/iextendedreporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/reporter_extensions.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/reporter_extensions.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/reporting/shared_reporting.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/reporting/shared_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/decorators.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/decorators.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/launch.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/launch.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/listeners.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,20 @@
         environment_base_url = self.locust_environment.host
         tags = {"check_name": check_name, "environment": environment_base_url}
         if hasattr(self.locust_environment, "extra_context"):
             tags.update(self.locust_environment.extra_context)
         tags.update(extra_tags)
         fields = {"check_passed": int(check_passed)}
         time = datetime.utcnow()
-        points = [
-            {
-                "measurement": "locust_checks",
-                "tags": tags,
-                "time": time,
-                "fields": fields,
-            }
-        ]
 
         if getattr(self, "influxdb_listener") is not None:
-            self.influxdb_listener.influxdb_client.write_points(points)
+            point = self.influxdb_listener._InfluxDBListener__make_data_point(
+                "locust_checks", fields, time, tags=tags
+            )
+            self.influxdb_listener.cache.append(point)
 
     @staticmethod
     def _append_trend_data(environment):
         if (
             hasattr(environment.stats, "trends")
             and type(environment.stats.trends) is dict
         ):
```

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/metrics.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/metrics.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/shapes.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/shapes.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/grasshopper/lib/util/utils.py` & `locust-grasshopper-1.3.9/src/grasshopper/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/PKG-INFO` & `locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.3.8
+Version: 1.3.9
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -219,15 +219,15 @@
 Classifier: Framework :: Pytest
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gevent~=21.12.0
 Requires-Dist: influxdb~=5.3.1
 Requires-Dist: locust~=2.12.2
-Requires-Dist: locust-influxdb-listener~=0.0.9
+Requires-Dist: locust-influxdb-listener~=1.0.2
 Requires-Dist: pytest~=6.2.5
 Requires-Dist: termcolor~=1.1.0
 Requires-Dist: pyyaml~=5.3.1
 Requires-Dist: tag-matcher~=0.0.5
 
 <div id="top"></div>
```

### Comparing `locust-grasshopper-1.3.8/src/locust_grasshopper.egg-info/SOURCES.txt` & `locust-grasshopper-1.3.9/src/locust_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

