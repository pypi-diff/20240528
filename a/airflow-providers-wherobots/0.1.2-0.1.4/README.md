# Comparing `tmp/airflow_providers_wherobots-0.1.2.tar.gz` & `tmp/airflow_providers_wherobots-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_providers_wherobots-0.1.2.tar", max compression
+gzip compressed data, was "airflow_providers_wherobots-0.1.4.tar", max compression
```

## Comparing `airflow_providers_wherobots-0.1.2.tar` & `airflow_providers_wherobots-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/LICENSE
--rw-r--r--   0        0        0     2436 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/__init__.py
--rw-r--r--   0        0        0     1873 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/sql.py
--rw-r--r--   0        0        0       57 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/wherobots.py
--rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/__init__.py
--rw-r--r--   0        0        0     2000 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/sql.py
--rw-r--r--   0        0        0      492 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3006 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 13:47:25.620809 airflow_providers_wherobots-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2555 2024-05-28 13:47:25.620809 airflow_providers_wherobots-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 13:47:25.620809 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:47:25.620809 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/hooks/__init__.py
+-rw-r--r--   0        0        0     1873 2024-05-28 13:47:25.624810 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/hooks/sql.py
+-rw-r--r--   0        0        0       57 2024-05-28 13:47:25.624810 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/hooks/wherobots.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:47:25.624810 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/operators/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-28 13:47:25.624810 airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/operators/sql.py
+-rw-r--r--   0        0        0      492 2024-05-28 13:47:25.624810 airflow_providers_wherobots-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3125 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.4/PKG-INFO
```

### Comparing `airflow_providers_wherobots-0.1.2/LICENSE` & `airflow_providers_wherobots-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.2/README.md` & `airflow_providers_wherobots-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 ## Installation
 
 If you use [Poetry](https://python-poetry.org) in your project, add the
 dependency with `poetry add`:
 
 ```
-$ poetry add git+https://github.com/wherobots/airflow-providers-wherobots
+$ poetry add airflow-providers-wherobots
 ```
 
 Otherwise, just `pip install` it:
 
 ```
-$ pip install git+https://github.com/wherobots/airflow-providers-wherobots
+$ pip install airflow-providers-wherobots
 ```
 
 ## Usage
 
 ### Create a connection
 
 You first need to create a Connection in Airflow. This can be done from
@@ -30,46 +30,49 @@
 
 The only required fields for the connection are:
 - the Wherobots API endpoint in the `host` field;
 - your Wherobots API key in the `password` field.
 
 ```
 $ airflow connections add "wherobots_default" \
-    --conn-type "wherobots" \
+    --conn-type "generic" \
     --conn-host "api.cloud.wherobots.com" \
     --conn-password "$(< api.key)"
 ```
 
 ### Execute a SQL query
 
 The `WherobotsSqlOperator` allows you to run SQL queries on the
 Wherobots cloud, from which you can build your ETLs and data
 transformation workflows by querying, manipulating, and producing
 datasets with WherobotsDB.
 
 Refer to the [Wherobots Documentation](https://docs.wherobots.com) and
-this [guidance](https://docs.wherobots.com/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
+this [guidance](https://docs.wherobots.com/latest/tutorials/sedonadb/vector-data/vector-load/)
 to learn how to read data, transform data, and write results in Spatial
 SQL with WherobotsDB.
 
+Refer to the [Wherobots Apache Airflow Provider Documentation](https://docs.wherobots.com/latest/develop/airflow-provider)
+to get more detailed guidance about how to use the Wherobots Apache Airflow Provider.
+
 ## Example
 
 Below is an example Airflow DAG that executes a SQL query on Wherobots
 Cloud:
 
 ```python
 import datetime
 
 from airflow import DAG
 from airflow_providers_wherobots.operators.sql import WherobotsSqlOperator
 
 
 with DAG(
     dag_id="example_wherobots_sql_dag",
-    start_date=datetime.datetime.date(datetime.datetime.now()),
+    start_date=datetime.datetime.now(),
     schedule="@hourly",
     catchup=False
 ):
     # Create a `wherobots.test.airflow_example` table with 100 records
     # from the OMF `places_place` dataset.
     operator = WherobotsSqlOperator(
         task_id="execute_query",
```

### Comparing `airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/sql.py` & `airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/sql.py` & `airflow_providers_wherobots-0.1.4/airflow_providers_wherobots/operators/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Operator for firing sql queries and collect results to s3
 """
 
 from __future__ import annotations
 
+from typing import Sequence
+
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 from wherobots.db import Runtime
 from wherobots.db.constants import (
     DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS,
     DEFAULT_READ_TIMEOUT_SECONDS,
 )
@@ -26,14 +28,18 @@
             "handlers that are specifically designed for your database."
         )
     return cursor.fetchall()
 
 
 class WherobotsSqlOperator(SQLExecuteQueryOperator):  # type: ignore[misc]
 
+    template_fields: Sequence[str] = SQLExecuteQueryOperator.template_fields
+    template_fields_renderers = {"sql": "sql"}
+    conn_id_field = "wherobots_conn_id"
+
     def __init__(  # type: ignore[no-untyped-def]
         self,
         *,
         wherobots_conn_id: str = DEFAULT_CONN_ID,
         runtime_id: Runtime = Runtime.SEDONA,
         session_wait_timeout: int = DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS,
         read_timeout: int = DEFAULT_READ_TIMEOUT_SECONDS,
```

### Comparing `airflow_providers_wherobots-0.1.2/PKG-INFO` & `airflow_providers_wherobots-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-providers-wherobots
-Version: 0.1.2
+Version: 0.1.4
 Summary: Airflow extension for communicating with Wherobots Cloud
 Author: zongsi.zhang
 Author-email: zongsi@wherobots.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,21 +20,21 @@
 
 ## Installation
 
 If you use [Poetry](https://python-poetry.org) in your project, add the
 dependency with `poetry add`:
 
 ```
-$ poetry add git+https://github.com/wherobots/airflow-providers-wherobots
+$ poetry add airflow-providers-wherobots
 ```
 
 Otherwise, just `pip install` it:
 
 ```
-$ pip install git+https://github.com/wherobots/airflow-providers-wherobots
+$ pip install airflow-providers-wherobots
 ```
 
 ## Usage
 
 ### Create a connection
 
 You first need to create a Connection in Airflow. This can be done from
@@ -45,46 +45,49 @@
 
 The only required fields for the connection are:
 - the Wherobots API endpoint in the `host` field;
 - your Wherobots API key in the `password` field.
 
 ```
 $ airflow connections add "wherobots_default" \
-    --conn-type "wherobots" \
+    --conn-type "generic" \
     --conn-host "api.cloud.wherobots.com" \
     --conn-password "$(< api.key)"
 ```
 
 ### Execute a SQL query
 
 The `WherobotsSqlOperator` allows you to run SQL queries on the
 Wherobots cloud, from which you can build your ETLs and data
 transformation workflows by querying, manipulating, and producing
 datasets with WherobotsDB.
 
 Refer to the [Wherobots Documentation](https://docs.wherobots.com) and
-this [guidance](https://docs.wherobots.com/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
+this [guidance](https://docs.wherobots.com/latest/tutorials/sedonadb/vector-data/vector-load/)
 to learn how to read data, transform data, and write results in Spatial
 SQL with WherobotsDB.
 
+Refer to the [Wherobots Apache Airflow Provider Documentation](https://docs.wherobots.com/latest/develop/airflow-provider)
+to get more detailed guidance about how to use the Wherobots Apache Airflow Provider.
+
 ## Example
 
 Below is an example Airflow DAG that executes a SQL query on Wherobots
 Cloud:
 
 ```python
 import datetime
 
 from airflow import DAG
 from airflow_providers_wherobots.operators.sql import WherobotsSqlOperator
 
 
 with DAG(
     dag_id="example_wherobots_sql_dag",
-    start_date=datetime.datetime.date(datetime.datetime.now()),
+    start_date=datetime.datetime.now(),
     schedule="@hourly",
     catchup=False
 ):
     # Create a `wherobots.test.airflow_example` table with 100 records
     # from the OMF `places_place` dataset.
     operator = WherobotsSqlOperator(
         task_id="execute_query",
```

