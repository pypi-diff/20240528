# Comparing `tmp/mlops_ai-1.3.3.tar.gz` & `tmp/mlops_ai-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ai-1.3.3.tar", last modified: Mon May 27 18:08:51 2024, max compression
+gzip compressed data, was "mlops_ai-1.3.4.tar", last modified: Mon May 27 20:00:17 2024, max compression
```

## Comparing `mlops_ai-1.3.3.tar` & `mlops_ai-1.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.692061 mlops_ai-1.3.3/mlops/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/exceptions/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/mlops/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/src/monitored_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/mlops/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/mlops_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 18:08:51.000000 mlops_ai-1.3.3/mlops_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:08:51.696061 mlops_ai-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 18:08:42.000000 mlops_ai-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.450229 mlops_ai-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 20:00:17.450229 mlops_ai-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.446229 mlops_ai-1.3.4/mlops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.446229 mlops_ai-1.3.4/mlops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.446229 mlops_ai-1.3.4/mlops/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/exceptions/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/exceptions/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/exceptions/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/exceptions/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.450229 mlops_ai-1.3.4/mlops/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/src/monitored_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/mlops/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:17.450229 mlops_ai-1.3.4/mlops_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 20:00:17.000000 mlops_ai-1.3.4/mlops_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 20:00:17.000000 mlops_ai-1.3.4/mlops_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:00:17.000000 mlops_ai-1.3.4/mlops_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 20:00:17.000000 mlops_ai-1.3.4/mlops_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:00:17.000000 mlops_ai-1.3.4/mlops_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:00:17.450229 mlops_ai-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 20:00:07.000000 mlops_ai-1.3.4/setup.py
```

### Comparing `mlops_ai-1.3.3/PKG-INFO` & `mlops_ai-1.3.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.3.3
+Version: 1.3.4
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Home-page: https://mlops-ai.github.io/mlops/
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://mlops-ai.github.io/mlops/library_docs/library_overview.html
 Project-URL: Repository, https://github.com/mlops-ai/mlops
```

### Comparing `mlops_ai-1.3.3/README.md` & `mlops_ai-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/config/config.py` & `mlops_ai-1.3.4/mlops/config/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,16 +19,20 @@
         self.send_emails = False
 
     @staticmethod
     def get_username():
         # Check if the code is running in a GitHub Actions environment
         if os.getenv('GITHUB_ACTIONS') == 'true':
             return os.getenv('GITHUB_ACTOR')
+        elif os.getenv('USERNAME') is not None:
+            return os.getenv('USERNAME')
+        elif os.getenv('USER') is not None:
+            return os.getenv('USER')
         else:
-            return os.getlogin()
+            return 'root'
 
     def change_username(self, username: str):
         self.user_name = username
 
     def change_active_project(self, project_id: str):
         self.active_project_id = project_id
```

### Comparing `mlops_ai-1.3.3/mlops/exceptions/tracking.py` & `mlops_ai-1.3.4/mlops/exceptions/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/monitoring.py` & `mlops_ai-1.3.4/mlops/monitoring.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/src/chart.py` & `mlops_ai-1.3.4/mlops/src/chart.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/src/dataset.py` & `mlops_ai-1.3.4/mlops/src/dataset.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/src/iteration.py` & `mlops_ai-1.3.4/mlops/src/iteration.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/src/mailgun.py` & `mlops_ai-1.3.4/mlops/src/mailgun.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/src/monitored_model.py` & `mlops_ai-1.3.4/mlops/src/monitored_model.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops/tracking.py` & `mlops_ai-1.3.4/mlops/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/mlops_ai.egg-info/PKG-INFO` & `mlops_ai-1.3.4/mlops_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.3.3
+Version: 1.3.4
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Home-page: https://mlops-ai.github.io/mlops/
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 Author-email: kac.pekalski1@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://mlops-ai.github.io/mlops/library_docs/library_overview.html
 Project-URL: Repository, https://github.com/mlops-ai/mlops
```

### Comparing `mlops_ai-1.3.3/mlops_ai.egg-info/SOURCES.txt` & `mlops_ai-1.3.4/mlops_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlops_ai-1.3.3/setup.py` & `mlops_ai-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent.parent
 
 # The text of the README file
 README = (HERE/"README.md").read_text()
 
 setup(
    name="mlops-ai",
-   version="1.3.3",
+   version="1.3.4",
    description="Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.",
    long_description=README,
    long_description_content_type="text/markdown",
    url="https://mlops-ai.github.io/mlops/",
    author="Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński",
    author_email="kac.pekalski1@gmail.com",
    license="Apache License 2.0",
```

