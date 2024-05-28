# Comparing `tmp/statistic_tool-0.0.2.tar.gz` & `tmp/statistic_tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistic_tool-0.0.2.tar", last modified: Mon May 13 13:03:30 2024, max compression
+gzip compressed data, was "statistic_tool-0.0.3.tar", last modified: Tue May 28 06:22:50 2024, max compression
```

## Comparing `statistic_tool-0.0.2.tar` & `statistic_tool-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/statistic_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/statistic_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:22:50.470421 statistic_tool-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-28 06:22:50.466421 statistic_tool-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:22:50.470421 statistic_tool-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:22:50.466421 statistic_tool-0.0.3/statistic_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/statistic_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/statistic_tool/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 06:22:42.000000 statistic_tool-0.0.3/statistic_tool/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:22:50.466421 statistic_tool-0.0.3/statistic_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-28 06:22:50.000000 statistic_tool-0.0.3/statistic_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 06:22:50.000000 statistic_tool-0.0.3/statistic_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:22:50.000000 statistic_tool-0.0.3/statistic_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 06:22:50.000000 statistic_tool-0.0.3/statistic_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 06:22:50.000000 statistic_tool-0.0.3/statistic_tool.egg-info/top_level.txt
```

### Comparing `statistic_tool-0.0.2/LICENSE` & `statistic_tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statistic_tool-0.0.2/PKG-INFO` & `statistic_tool-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistic-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple functions for statistic
 Home-page: https://github.com/cheerzhang/statistic_tool
 Author: ZhangLe
 Author-email: zhangle@gmail.com
 Project-URL: Bug Tracker, https://github.com/cheerzhang/statistic_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `statistic_tool-0.0.2/setup.py` & `statistic_tool-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='statistic-tool',
-    version='0.0.2',
+    version='0.0.3',
     author="ZhangLe",
     author_email="zhangle@gmail.com",
     description="simple functions for statistic",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cheerzhang/statistic_tool",
     project_urls={
```

### Comparing `statistic_tool-0.0.2/statistic_tool/feature.py` & `statistic_tool-0.0.3/statistic_tool/feature.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,7 +57,18 @@
     """
     iv_values = {}
     for column in dataframe.columns:
         if column != target:  # Exclude the target variable
             iv_values[column] = calculate_iv(dataframe, column, target)
     
     return pd.DataFrame.from_dict(iv_values, orient='index', columns=['IV']).sort_values(by='IV', ascending=False)
+
+def check_nan_inf(df):
+    result = {}
+    for col in df.columns:
+        nans = df[col].isna().sum()
+        infs = 0
+        if pd.api.types.is_numeric_dtype(df[col]):
+            infs = np.isinf(df[col]).sum()
+        if nans > 0 or infs > 0:
+            result[col] = {'NaN': nans, 'Inf': infs}
+    return result
```

### Comparing `statistic_tool-0.0.2/statistic_tool.egg-info/PKG-INFO` & `statistic_tool-0.0.3/statistic_tool.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistic-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple functions for statistic
 Home-page: https://github.com/cheerzhang/statistic_tool
 Author: ZhangLe
 Author-email: zhangle@gmail.com
 Project-URL: Bug Tracker, https://github.com/cheerzhang/statistic_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

