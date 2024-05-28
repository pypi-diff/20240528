# Comparing `tmp/magma_suite-3.2.2.tar.gz` & `tmp/magma_suite-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-3.2.2.tar", max compression
+gzip compressed data, was "magma_suite-3.2.3.tar", max compression
```

## Comparing `magma_suite-3.2.2.tar` & `magma_suite-3.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1083 2024-04-15 19:44:28.074703 magma_suite-3.2.2/LICENSE.txt
--rw-r--r--   0        0        0       96 2024-04-15 19:44:28.074703 magma_suite-3.2.2/README.md
--rw-r--r--   0        0        0        1 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/__init__.py
--rw-r--r--   0        0        0     3503 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/checkstatus.py
--rw-r--r--   0        0        0    13081 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/inputgenerator.py
--rw-r--r--   0        0        0    17831 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma/runupdate.py
--rw-r--r--   0        0        0        0 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/__init__.py
--rw-r--r--   0        0        0     2220 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/checkstatus.py
--rw-r--r--   0        0        0        0 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/commands/__init__.py
--rw-r--r--   0        0        0     1229 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/commands/create_meta_workflow_run.py
--rw-r--r--   0        0        0    63517 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/runupdate.py
--rw-r--r--   0        0        0     6153 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3866 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/utils.py
--rw-r--r--   0        0        0     4105 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_ff/wfrutils.py
--rw-r--r--   0        0        0        0 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/__init__.py
--rw-r--r--   0        0        0     2240 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/checkstatus.py
--rw-r--r--   0        0        0        0 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/commands/__init__.py
--rw-r--r--   0        0        0     3008 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/commands/create_meta_workflow_run.py
--rw-r--r--   0        0        0    11797 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/create_metawfr.py
--rw-r--r--   0        0        0      158 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/import_metawfr.py
--rw-r--r--   0        0        0     4744 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/inputgenerator.py
--rw-r--r--   0        0        0      781 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/metawfl.py
--rw-r--r--   0        0        0     3289 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/metawflrun.py
--rw-r--r--   0        0        0     5093 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/parser.py
--rw-r--r--   0        0        0     6924 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/reset_metawfr.py
--rw-r--r--   0        0        0     2473 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/run_metawfr.py
--rw-r--r--   0        0        0       30 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/runupdate.py
--rw-r--r--   0        0        0     6324 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/status_metawfr.py
--rw-r--r--   0        0        0     1401 2024-04-15 19:44:28.078703 magma_suite-3.2.2/magma_smaht/update_cost_metawfr.py
--rw-r--r--   0        0        0     6775 2024-04-15 19:44:28.082703 magma_suite-3.2.2/magma_smaht/utils.py
--rw-r--r--   0        0        0     4022 2024-04-15 19:44:28.082703 magma_suite-3.2.2/magma_smaht/wfrutils.py
--rw-r--r--   0        0        0     1494 2024-04-15 19:44:28.082703 magma_suite-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 magma_suite-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-28 21:52:00.416917 magma_suite-3.2.3/LICENSE.txt
+-rw-r--r--   0        0        0       96 2024-05-28 21:52:00.416917 magma_suite-3.2.3/README.md
+-rw-r--r--   0        0        0        1 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/__init__.py
+-rw-r--r--   0        0        0     3503 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/checkstatus.py
+-rw-r--r--   0        0        0    13081 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/inputgenerator.py
+-rw-r--r--   0        0        0    17831 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/commands/__init__.py
+-rw-r--r--   0        0        0     1229 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/commands/create_meta_workflow_run.py
+-rw-r--r--   0        0        0    63517 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     6153 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3866 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/utils.py
+-rw-r--r--   0        0        0     4105 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_smaht/__init__.py
+-rw-r--r--   0        0        0     2240 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_smaht/checkstatus.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:52:00.416917 magma_suite-3.2.3/magma_smaht/commands/__init__.py
+-rw-r--r--   0        0        0     3008 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/commands/create_meta_workflow_run.py
+-rw-r--r--   0        0        0    11797 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/create_metawfr.py
+-rw-r--r--   0        0        0      158 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/import_metawfr.py
+-rw-r--r--   0        0        0     4744 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/inputgenerator.py
+-rw-r--r--   0        0        0      781 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/metawfl.py
+-rw-r--r--   0        0        0     3289 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/metawflrun.py
+-rw-r--r--   0        0        0     5093 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/parser.py
+-rw-r--r--   0        0        0     6924 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/reset_metawfr.py
+-rw-r--r--   0        0        0     2473 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/run_metawfr.py
+-rw-r--r--   0        0        0       30 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/runupdate.py
+-rw-r--r--   0        0        0     6324 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/status_metawfr.py
+-rw-r--r--   0        0        0     1401 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/update_cost_metawfr.py
+-rw-r--r--   0        0        0     6888 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/utils.py
+-rw-r--r--   0        0        0     4022 2024-05-28 21:52:00.420917 magma_suite-3.2.3/magma_smaht/wfrutils.py
+-rw-r--r--   0        0        0     1494 2024-05-28 21:52:00.420917 magma_suite-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 magma_suite-3.2.3/PKG-INFO
```

### Comparing `magma_suite-3.2.2/LICENSE.txt` & `magma_suite-3.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma/checkstatus.py` & `magma_suite-3.2.3/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma/inputgenerator.py` & `magma_suite-3.2.3/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma/metawfl.py` & `magma_suite-3.2.3/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma/metawflrun.py` & `magma_suite-3.2.3/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma/runupdate.py` & `magma_suite-3.2.3/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/checkstatus.py` & `magma_suite-3.2.3/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/commands/create_meta_workflow_run.py` & `magma_suite-3.2.3/magma_ff/commands/create_meta_workflow_run.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/create_metawfr.py` & `magma_suite-3.2.3/magma_ff/create_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/import_metawfr.py` & `magma_suite-3.2.3/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/inputgenerator.py` & `magma_suite-3.2.3/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/metawfl.py` & `magma_suite-3.2.3/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/metawflrun.py` & `magma_suite-3.2.3/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/parser.py` & `magma_suite-3.2.3/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/reset_metawfr.py` & `magma_suite-3.2.3/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/run_metawfr.py` & `magma_suite-3.2.3/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/status_metawfr.py` & `magma_suite-3.2.3/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/update_cost_metawfr.py` & `magma_suite-3.2.3/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/utils.py` & `magma_suite-3.2.3/magma_ff/utils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_ff/wfrutils.py` & `magma_suite-3.2.3/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/checkstatus.py` & `magma_suite-3.2.3/magma_smaht/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/commands/create_meta_workflow_run.py` & `magma_suite-3.2.3/magma_smaht/commands/create_meta_workflow_run.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/create_metawfr.py` & `magma_suite-3.2.3/magma_smaht/create_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/inputgenerator.py` & `magma_suite-3.2.3/magma_smaht/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/metawfl.py` & `magma_suite-3.2.3/magma_smaht/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/metawflrun.py` & `magma_suite-3.2.3/magma_smaht/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/parser.py` & `magma_suite-3.2.3/magma_smaht/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/reset_metawfr.py` & `magma_suite-3.2.3/magma_smaht/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/run_metawfr.py` & `magma_suite-3.2.3/magma_smaht/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/status_metawfr.py` & `magma_suite-3.2.3/magma_smaht/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/update_cost_metawfr.py` & `magma_suite-3.2.3/magma_smaht/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/magma_smaht/utils.py` & `magma_suite-3.2.3/magma_smaht/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,21 +182,25 @@
 
     Raises:
         Exception: Raises an exception when there are multiple samples associated
 
     Returns:
         dict: Sample item from portal
     """
-    analyte = ff_utils.get_metadata(
-        library["analyte"], add_on="frame=raw&datastore=database", key=smaht_key
-    )
-    if len(analyte["samples"]) > 1:
+    samples = []
+    analytes = library.get("analytes", [])
+    for analyte in analytes:
+        item = ff_utils.get_metadata(
+            analyte, add_on="frame=raw&datastore=database", key=smaht_key
+        )
+        samples += item.get("samples", [])
+    if len(set(samples)) > 1:
         raise Exception(f"Multiple samples found for library {library['accession']}")
     sample = ff_utils.get_metadata(
-        analyte["samples"][0], add_on="frame=raw&datastore=database", key=smaht_key
+        samples[0], add_on="frame=raw&datastore=database", key=smaht_key
     )
     return sample
 
 
 def get_latest_mwf(mwf_name, smaht_key):
     """Get the latest version of the MWF with name `mwf_name`
```

### Comparing `magma_suite-3.2.2/magma_smaht/wfrutils.py` & `magma_suite-3.2.3/magma_smaht/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-3.2.2/pyproject.toml` & `magma_suite-3.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "3.2.2"
+version = "3.2.3"
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
```

### Comparing `magma_suite-3.2.2/PKG-INFO` & `magma_suite-3.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magma-suite
-Version: 3.2.2
+Version: 3.2.3
 Summary: Collection of tools to manage meta-workflows automation.
 Home-page: https://github.com/dbmi-bgm/magma
 License: MIT
 Author: Michele Berselli
 Author-email: berselli.michele@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

