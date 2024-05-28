# Comparing `tmp/lariat_python_sdk-0.1.5.tar.gz` & `tmp/lariat_python_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lariat_python_sdk-0.1.5.tar", last modified: Mon May 22 19:49:25 2023, max compression
+gzip compressed data, was "lariat_python_sdk-0.1.6.tar", last modified: Tue May 28 15:13:30 2024, max compression
```

## Comparing `lariat_python_sdk-0.1.5.tar` & `lariat_python_sdk-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.382398 lariat_python_sdk-0.1.5/
--rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.5/LICENSE
--rw-r--r--   0 vikas      (501) staff       (20)     3290 2023-05-22 19:49:25.382254 lariat_python_sdk-0.1.5/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)     2310 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/README.md
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.380870 lariat_python_sdk-0.1.5/lariat_client/
--rw-r--r--   0 vikas      (501) staff       (20)      346 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/lariat_client/__init__.py
--rw-r--r--   0 vikas      (501) staff       (20)    23214 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/lariat_client/lariat_client.py
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.381808 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/
--rw-r--r--   0 vikas      (501) staff       (20)     3290 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/requires.txt
--rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-22 19:49:03.000000 lariat_python_sdk-0.1.5/pyproject.toml
--rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-22 19:49:25.382440 lariat_python_sdk-0.1.5/setup.cfg
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.381959 lariat_python_sdk-0.1.5/tests/
--rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.5/tests/test_lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2024-05-28 15:13:30.381339 lariat_python_sdk-0.1.6/
+-rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.6/LICENSE
+-rw-r--r--   0 vikas      (501) staff       (20)     3393 2024-05-28 15:13:30.381141 lariat_python_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)     2310 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.6/README.md
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2024-05-28 15:13:30.379456 lariat_python_sdk-0.1.6/lariat_client/
+-rw-r--r--   0 vikas      (501) staff       (20)      367 2024-05-28 12:34:28.000000 lariat_python_sdk-0.1.6/lariat_client/__init__.py
+-rw-r--r--   0 vikas      (501) staff       (20)    25504 2024-05-28 14:53:47.000000 lariat_python_sdk-0.1.6/lariat_client/lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2024-05-28 15:13:30.380936 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/
+-rw-r--r--   0 vikas      (501) staff       (20)     3393 2024-05-28 15:13:30.000000 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)      321 2024-05-28 15:13:30.000000 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vikas      (501) staff       (20)        1 2024-05-28 15:13:30.000000 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       43 2024-05-28 15:13:30.000000 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       14 2024-05-28 15:13:30.000000 lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vikas      (501) staff       (20)     1102 2024-05-28 14:54:06.000000 lariat_python_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0 vikas      (501) staff       (20)       38 2024-05-28 15:13:30.381379 lariat_python_sdk-0.1.6/setup.cfg
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2024-05-28 15:13:30.380626 lariat_python_sdk-0.1.6/tests/
+-rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.6/tests/test_lariat_client.py
```

### Comparing `lariat_python_sdk-0.1.5/LICENSE` & `lariat_python_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.5/PKG-INFO` & `lariat_python_sdk-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lariat_python_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: flatten-json
 
 # Lariat Python SDK
 
 A Python module to interact with Lariat API and perform various operations like querying indicators, fetching datasets, etc.
 
 ## Installation
```

### Comparing `lariat_python_sdk-0.1.5/README.md` & `lariat_python_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.5/lariat_client/lariat_client.py` & `lariat_python_sdk-0.1.6/lariat_client/lariat_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -686,7 +686,70 @@
     except requests.exceptions.ConnectionError as errc:
         logging.error(f"Error Connecting: {errc}")
     except requests.exceptions.Timeout as errt:
         logging.error(f"Timeout Error: {errt}")
     except requests.exceptions.RequestException as err:
         logging.error(f"Something went wrong: {err}")
         sys.exit(1)
+
+
+def query_streaming(
+    indicator_id: str,
+    from_ts: datetime.datetime,
+    to_ts: datetime.datetime = None,
+    group_by: List[str] = None,
+    aggregate: str = None,
+    query_filter: Filter = None,
+) -> MetricRecordList:
+    """
+    Queries a provided indicator for its metric data,.
+
+    Args:
+        indicator (indicator_id): Indicator id to query.
+        from_ts (datetime.datetime): The start time for the indicator evaluation.
+        to_ts (datetime.datetime): The end time for the indicator evaluation.
+        group_by (list): A list of strings to group the metrics data by.
+        aggregate (str): An optional aggregation function to apply to the metric.
+        query_filter (filter): A filter function to apply to the metric.
+
+    Returns:
+        MetricRecordList: An object that contains the list of records output by the query.
+    """
+    if to_ts is None:
+        to_ts = datetime.datetime.now()
+    data_filter = {"operator": "or", "filters": []}
+    if group_by:
+        data_filter["group_by_clauses"] = group_by
+    else:
+        group_by = []
+    if query_filter:
+        data_filter["operator"] = query_filter.operator
+        data_filter["filters"] = [
+            {"field": clause.field, "operator": clause.operator, "value": clause.values}
+            for clause in query_filter.clauses
+        ]
+    data = {
+        "indicator_id": indicator_id,
+        "filter": data_filter,
+        "time_range": {
+            "from_ts": int(from_ts.timestamp() * 1000),
+            "to_ts": int(to_ts.timestamp() * 1000),
+        },
+    }
+    if aggregate:
+        data["aggregation"] = aggregate
+    try:
+        r = s.get(
+            url=f"{LARIAT_PUBLIC_API_ENDPOINT}/streaming-query-metrics", json=data
+        )
+        r.raise_for_status()
+        records = r.json()["records"]
+        return MetricRecordList(group_by, records)
+    except requests.exceptions.HTTPError as errh:
+        logging.error(f"Http Error: {errh}")
+    except requests.exceptions.ConnectionError as errc:
+        logging.error(f"Error Connecting: {errc}")
+    except requests.exceptions.Timeout as errt:
+        logging.error(f"Timeout Error: {errt}")
+    except requests.exceptions.RequestException as err:
+        logging.error(f"Something went wrong: {err}")
+        sys.exit(1)
```

### Comparing `lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/PKG-INFO` & `lariat_python_sdk-0.1.6/lariat_python_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lariat-python-sdk
-Version: 0.1.5
+Name: lariat_python_sdk
+Version: 0.1.6
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: flatten-json
 
 # Lariat Python SDK
 
 A Python module to interact with Lariat API and perform various operations like querying indicators, fetching datasets, etc.
 
 ## Installation
```

### Comparing `lariat_python_sdk-0.1.5/pyproject.toml` & `lariat_python_sdk-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lariat_python_sdk"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python module to interact with Lariat API to access data quality metrics and diagnostics"
 readme = "README.md"
 authors = [
     { name = "Lariat Data Team", email = "info@lariatdata.com"}
 ]
 license = {text = "BSD-3-Clause"}
 dependencies = [
```

### Comparing `lariat_python_sdk-0.1.5/tests/test_lariat_client.py` & `lariat_python_sdk-0.1.6/tests/test_lariat_client.py`

 * *Files identical despite different names*

