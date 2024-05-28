# Comparing `tmp/truenaspy-0.6.3.tar.gz` & `tmp/truenaspy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truenaspy-0.6.3.tar", last modified: Mon May 27 12:37:48 2024, max compression
+gzip compressed data, was "truenaspy-0.6.4.tar", last modified: Mon May 27 16:47:26 2024, max compression
```

## Comparing `truenaspy-0.6.3.tar` & `truenaspy-0.6.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.643072 truenaspy-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.643072 truenaspy-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 12:37:38.000000 truenaspy-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 12:37:38.000000 truenaspy-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 12:37:38.000000 truenaspy-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 12:37:48.647072 truenaspy-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 12:37:38.000000 truenaspy-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-27 12:37:38.000000 truenaspy-0.6.3/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-27 12:37:38.000000 truenaspy-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 12:37:38.000000 truenaspy-0.6.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 12:37:38.000000 truenaspy-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:37:48.647072 truenaspy-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/truenaspy/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/collects.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 12:37:38.000000 truenaspy-0.6.3/truenaspy/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:37:48.647072 truenaspy-0.6.3/truenaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 12:37:48.000000 truenaspy-0.6.3/truenaspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.742401 truenaspy-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:47:11.000000 truenaspy-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 16:47:11.000000 truenaspy-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 16:47:26.742401 truenaspy-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:47:11.000000 truenaspy-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-27 16:47:11.000000 truenaspy-0.6.4/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 16:47:11.000000 truenaspy-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 16:47:11.000000 truenaspy-0.6.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 16:47:11.000000 truenaspy-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:47:26.742401 truenaspy-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/truenaspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/collects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.742401 truenaspy-0.6.4/truenaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/top_level.txt
```

### Comparing `truenaspy-0.6.3/.github/dependabot.yml` & `truenaspy-0.6.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/.github/workflows/auto-approve.yml` & `truenaspy-0.6.4/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/.github/workflows/lint.yml` & `truenaspy-0.6.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/.github/workflows/pythonpublish.yml` & `truenaspy-0.6.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/.github/workflows/release.yml` & `truenaspy-0.6.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/.gitignore` & `truenaspy-0.6.4/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -104,9 +104,9 @@
 
 # mypy
 .mypy_cache/
 
 #pyannotate
 type_info.json
 
-#perso
-test_home.py
+# Secret files
+secrets.yaml
```

### Comparing `truenaspy-0.6.3/.pre-commit-config.yaml` & `truenaspy-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/LICENSE` & `truenaspy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/PKG-INFO` & `truenaspy-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.3
+Version: 0.6.4
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truenaspy-0.6.3/README.md` & `truenaspy-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/example.py` & `truenaspy-0.6.4/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 #!/usr/bin/env python3
 """Example code."""
 
 import asyncio
 import logging
 
+import yaml
+
 from truenaspy import Events, TruenasClient
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 # create console handler and set level to debug
 ch = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
-# Please , fill good values...
-HOST = "my.nas.local:8080"
-TOKEN = "xxxxxxxxxxxxxxxxxxxxxxxxx"
+# Fill out the secrets in secrets.yaml, you can find an example
+# _secrets.yaml file, which has to be renamed after filling out the secrets.
+with open("./secrets.yaml", encoding="UTF-8") as file:
+    secrets = yaml.safe_load(file)
+
+TOKEN = secrets["TOKEN"]
+HOST = secrets["HOST"]
 
 
-async def main() -> None:
+async def async_main() -> None:
     """Main function."""
 
     api = TruenasClient(token=TOKEN, host=HOST, use_ssl=True, verify_ssl=True)
     rlst = await api.async_get_system()
     logger.info(rlst)
 
     # Fetch all data
@@ -66,10 +72,10 @@
         if i == 5:
             api.unsubscribe(Events.DISKS.value, log_disk)
             polling = False
 
     await api.async_close()
 
 
-loop = asyncio.new_event_loop()
-asyncio.set_event_loop(loop)
-loop.run_until_complete(main())
+if __name__ == "__main__":
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(async_main())
```

### Comparing `truenaspy-0.6.3/pyproject.toml` & `truenaspy-0.6.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.lint.flake8-tidy-imports.banned-api]
-"async_timeout".msg = "use asyncio.timeout instead"
-"pytz".msg = "use zoneinfo instead"
-
 [tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
+
+[[tool.mypy.overrides]]
+module = "yaml"
+ignore_missing_imports = true
```

### Comparing `truenaspy-0.6.3/truenaspy/api.py` & `truenaspy-0.6.4/truenaspy/api.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/truenaspy/auth.py` & `truenaspy-0.6.4/truenaspy/auth.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/truenaspy/collects.py` & `truenaspy-0.6.4/truenaspy/collects.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/truenaspy/helper.py` & `truenaspy-0.6.4/truenaspy/helper.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/truenaspy/subscription.py` & `truenaspy-0.6.4/truenaspy/subscription.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.3/truenaspy.egg-info/PKG-INFO` & `truenaspy-0.6.4/truenaspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.3
+Version: 0.6.4
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truenaspy-0.6.3/truenaspy.egg-info/SOURCES.txt` & `truenaspy-0.6.4/truenaspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

