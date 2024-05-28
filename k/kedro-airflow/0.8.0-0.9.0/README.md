# Comparing `tmp/kedro-airflow-0.8.0.tar.gz` & `tmp/kedro_airflow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-airflow-0.8.0.tar", last modified: Wed Dec 20 15:49:39 2023, max compression
+gzip compressed data, was "kedro_airflow-0.9.0.tar", last modified: Tue May 28 04:38:52 2024, max compression
```

## Comparing `kedro-airflow-0.8.0.tar` & `kedro_airflow-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:49:39.468908 kedro-airflow-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2023-12-20 15:49:39.468908 kedro-airflow-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:49:39.464908 kedro-airflow-0.8.0/kedro_airflow/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/kedro_airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/kedro_airflow/airflow_dag_template.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/kedro_airflow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:49:39.468908 kedro-airflow-0.8.0/kedro_airflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-20 15:49:39.000000 kedro-airflow-0.8.0/kedro_airflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 15:49:39.468908 kedro-airflow-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:49:39.468908 kedro-airflow-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2023-12-20 15:49:09.000000 kedro-airflow-0.8.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:38:52.710903 kedro_airflow-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-28 04:38:52.710903 kedro_airflow-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:38:52.706903 kedro_airflow-0.9.0/kedro_airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/kedro_airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/kedro_airflow/airflow_dag_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/kedro_airflow/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/kedro_airflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:38:52.706903 kedro_airflow-0.9.0/kedro_airflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 04:38:52.000000 kedro_airflow-0.9.0/kedro_airflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:38:52.710903 kedro_airflow-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:38:52.706903 kedro_airflow-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/tests/test_node_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-28 04:38:45.000000 kedro_airflow-0.9.0/tests/test_plugin.py
```

### Comparing `kedro-airflow-0.8.0/PKG-INFO` & `kedro_airflow-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: kedro-airflow
-Version: 0.8.0
+Version: 0.9.0
 Summary: Kedro-Airflow makes it easy to deploy Kedro projects to Airflow
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-airflow
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kedro>=0.17.5
+Requires-Dist: kedro>=0.19.0
 Requires-Dist: python-slugify>=4.0
 Requires-Dist: semver>=2.10
 Provides-Extra: test
-Requires-Dist: apache-airflow<2.7.0; extra == "test"
+Requires-Dist: apache-airflow<3.0; extra == "test"
 Requires-Dist: bandit; extra == "test"
 Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
-Requires-Dist: connexion<3.0.0; extra == "test"
+Requires-Dist: coverage>=7.2.0; extra == "test"
 Requires-Dist: kedro-datasets; extra == "test"
-Requires-Dist: pendulum<3.0.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: trufflehog<3.0,>=2.1.0; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-cachetools; extra == "test"
+Requires-Dist: types-toml; extra == "test"
 
 # Kedro-Airflow
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-airflow/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro-airflow/)
 [![PyPI Version](https://badge.fury.io/py/kedro-airflow.svg)](https://pypi.org/project/kedro-airflow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 
 [Apache Airflow](https://github.com/apache/airflow) is a tool for orchestrating complex workflows and data processing pipelines. The Kedro-Airflow plugin can be used for:
 - Rapid pipeline creation in the prototyping phase. You can write Python functions in Kedro without worrying about schedulers, daemons, services or having to recreate the Airflow DAG file.
 - Automatic dependency resolution in Kedro. This allows you to bypass Airflow's need to specify the order of your tasks.
 - Distributing Kedro tasks across many workers. You can also enable monitoring and scheduling of the tasks' runtimes.
@@ -69,15 +72,15 @@
 
 For more information about the DAGs folder, please visit [Airflow documentation](https://airflow.apache.org/docs/stable/concepts.html#dags).
 The Airflow DAG configuration can be customized by editing this file.
 
 ### Step 3: Package and install the Kedro pipeline in the Airflow executor's environment
 
 After generating and deploying the DAG file, you will then need to package and install the Kedro pipeline into the Airflow executor's environment.
-Please visit the guide to [deploy Kedro as a Python package](https://docs.kedro.org/en/stable/deployment/single_machine.html#package-based) for more details.
+Please visit the guide to [Apache Airflow deployment](https://docs.kedro.org/en/stable/deployment/airflow.html) for more details.
 
 ### FAQ
 
 #### What if my DAG file is in a different directory to my project folder?
 
 By default, the generated DAG file is configured to live in the same directory as your project as per this [template](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/kedro_airflow/airflow_dag_template.j2#L44). If your DAG file is located in a different directory to your project, you will need to tweak this  manually after running the `kedro airflow create` command.
 
@@ -181,14 +184,27 @@
 
 Which Airflow Operator to use depends on the environment your project is running in.
 You can set the operator to use by providing a custom template.
 See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
 The [rich offering](https://airflow.apache.org/docs/apache-airflow-providers/operators-and-hooks-ref/index.html) of operators means that the `kedro-airflow` plugin is providing templates for specific operators.
 The default template provided by `kedro-airflow` uses the `BaseOperator`.
 
+### Can I group nodes together?
+
+When running Kedro nodes using Airflow, MemoryDatasets are often not shared across operators.
+This will cause the DAG run to fail.
+
+MemoryDatasets may be used to provide logical separation between nodes in Kedro, without the overhead of needing to write to disk (and in the case of distributed running needing multiple executors).
+
+Nodes that are connected through MemoryDatasets are grouped together via the `--group-in-memory` flag.
+This preserves the option to have logical separation in Kedro, with little computational overhead.
+
+It is possible to use [task groups](https://docs.astronomer.io/learn/task-groups) by changing the template.
+See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
+
 ## Can I contribute?
 
 Yes! Want to help build Kedro-Airflow? Check out our guide to [contributing](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/CONTRIBUTING.md).
 
 ## What licence do you use?
 
 Kedro-Airflow is licensed under the [Apache 2.0](https://github.com/kedro-org/kedro-plugins/blob/main/LICENSE.md) License.
```

### Comparing `kedro-airflow-0.8.0/README.md` & `kedro_airflow-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Kedro-Airflow
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-airflow/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro-airflow/)
 [![PyPI Version](https://badge.fury.io/py/kedro-airflow.svg)](https://pypi.org/project/kedro-airflow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 
 [Apache Airflow](https://github.com/apache/airflow) is a tool for orchestrating complex workflows and data processing pipelines. The Kedro-Airflow plugin can be used for:
 - Rapid pipeline creation in the prototyping phase. You can write Python functions in Kedro without worrying about schedulers, daemons, services or having to recreate the Airflow DAG file.
 - Automatic dependency resolution in Kedro. This allows you to bypass Airflow's need to specify the order of your tasks.
 - Distributing Kedro tasks across many workers. You can also enable monitoring and scheduling of the tasks' runtimes.
@@ -38,15 +38,15 @@
 
 For more information about the DAGs folder, please visit [Airflow documentation](https://airflow.apache.org/docs/stable/concepts.html#dags).
 The Airflow DAG configuration can be customized by editing this file.
 
 ### Step 3: Package and install the Kedro pipeline in the Airflow executor's environment
 
 After generating and deploying the DAG file, you will then need to package and install the Kedro pipeline into the Airflow executor's environment.
-Please visit the guide to [deploy Kedro as a Python package](https://docs.kedro.org/en/stable/deployment/single_machine.html#package-based) for more details.
+Please visit the guide to [Apache Airflow deployment](https://docs.kedro.org/en/stable/deployment/airflow.html) for more details.
 
 ### FAQ
 
 #### What if my DAG file is in a different directory to my project folder?
 
 By default, the generated DAG file is configured to live in the same directory as your project as per this [template](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/kedro_airflow/airflow_dag_template.j2#L44). If your DAG file is located in a different directory to your project, you will need to tweak this  manually after running the `kedro airflow create` command.
 
@@ -150,14 +150,27 @@
 
 Which Airflow Operator to use depends on the environment your project is running in.
 You can set the operator to use by providing a custom template.
 See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
 The [rich offering](https://airflow.apache.org/docs/apache-airflow-providers/operators-and-hooks-ref/index.html) of operators means that the `kedro-airflow` plugin is providing templates for specific operators.
 The default template provided by `kedro-airflow` uses the `BaseOperator`.
 
+### Can I group nodes together?
+
+When running Kedro nodes using Airflow, MemoryDatasets are often not shared across operators.
+This will cause the DAG run to fail.
+
+MemoryDatasets may be used to provide logical separation between nodes in Kedro, without the overhead of needing to write to disk (and in the case of distributed running needing multiple executors).
+
+Nodes that are connected through MemoryDatasets are grouped together via the `--group-in-memory` flag.
+This preserves the option to have logical separation in Kedro, with little computational overhead.
+
+It is possible to use [task groups](https://docs.astronomer.io/learn/task-groups) by changing the template.
+See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
+
 ## Can I contribute?
 
 Yes! Want to help build Kedro-Airflow? Check out our guide to [contributing](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/CONTRIBUTING.md).
 
 ## What licence do you use?
 
 Kedro-Airflow is licensed under the [Apache 2.0](https://github.com/kedro-org/kedro-plugins/blob/main/LICENSE.md) License.
```

### Comparing `kedro-airflow-0.8.0/kedro_airflow/airflow_dag_template.j2` & `kedro_airflow-0.9.0/kedro_airflow/airflow_dag_template.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from datetime import datetime, timedelta
 from pathlib import Path
 
 from airflow import DAG
 from airflow.models import BaseOperator
 from airflow.utils.decorators import apply_defaults
 
@@ -12,32 +13,32 @@
 
 class KedroOperator(BaseOperator):
     @apply_defaults
     def __init__(
         self,
         package_name: str,
         pipeline_name: str,
-        node_name: str,
+        node_name: str | list[str],
         project_path: str | Path,
         env: str,
         *args, **kwargs
     ) -> None:
         super().__init__(*args, **kwargs)
         self.package_name = package_name
         self.pipeline_name = pipeline_name
         self.node_name = node_name
         self.project_path = project_path
         self.env = env
 
     def execute(self, context):
         configure_project(self.package_name)
-        with KedroSession.create(project_path=self.project_path,
-                                 env=self.env) as session:
-            session.run(self.pipeline_name, node_names=[self.node_name])
-
+        with KedroSession.create(self.project_path, env=self.env) as session:
+            if isinstance(self.node_name, str):
+                self.node_name = [self.node_name]
+            session.run(self.pipeline_name, node_names=self.node_name)
 
 # Kedro settings required to run your pipeline
 env = "{{ env }}"
 pipeline_name = "{{ pipeline_name }}"
 project_path = Path.cwd()
 package_name = "{{ package_name }}"
 
@@ -56,21 +57,21 @@
         email_on_failure={{ email_on_failure | default(False) }},
         email_on_retry={{ email_on_retry | default(False) }},
         retries={{ retries | default(1) }},
         retry_delay=timedelta(minutes={{ retry_delay | default(5) }})
     )
 ) as dag:
     tasks = {
-    {% for node in pipeline.nodes %}        "{{ node.name | safe | slugify }}": KedroOperator(
-            task_id="{{ node.name | safe | slugify  }}",
+    {% for node_name, node_list in nodes.items() %}        "{{ node_name | safe | slugify }}": KedroOperator(
+            task_id="{{ node_name | safe | slugify  }}",
             package_name=package_name,
             pipeline_name=pipeline_name,
-            node_name="{{ node.name | safe }}",
+            node_name={% if node_list | length > 1 %}[{% endif %}{% for node in node_list %}"{{ node.name | safe }}"{% if not loop.last %}, {% endif %}{% endfor %}{% if node_list | length > 1 %}]{% endif %},
             project_path=project_path,
             env=env,
         ),
 {% endfor %}    }
 
     {% for parent_node, child_nodes in dependencies.items() -%}
-    {% for child in child_nodes %}    tasks["{{ parent_node.name | safe | slugify }}"] >> tasks["{{ child.name | safe | slugify }}"]
+    {% for child in child_nodes %}    tasks["{{ parent_node | safe | slugify }}"] >> tasks["{{ child | safe | slugify }}"]
     {% endfor %}
     {%- endfor %}
```

### Comparing `kedro-airflow-0.8.0/kedro_airflow.egg-info/PKG-INFO` & `kedro_airflow-0.9.0/kedro_airflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: kedro-airflow
-Version: 0.8.0
+Version: 0.9.0
 Summary: Kedro-Airflow makes it easy to deploy Kedro projects to Airflow
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-airflow
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kedro>=0.17.5
+Requires-Dist: kedro>=0.19.0
 Requires-Dist: python-slugify>=4.0
 Requires-Dist: semver>=2.10
 Provides-Extra: test
-Requires-Dist: apache-airflow<2.7.0; extra == "test"
+Requires-Dist: apache-airflow<3.0; extra == "test"
 Requires-Dist: bandit; extra == "test"
 Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
-Requires-Dist: connexion<3.0.0; extra == "test"
+Requires-Dist: coverage>=7.2.0; extra == "test"
 Requires-Dist: kedro-datasets; extra == "test"
-Requires-Dist: pendulum<3.0.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: trufflehog<3.0,>=2.1.0; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-cachetools; extra == "test"
+Requires-Dist: types-toml; extra == "test"
 
 # Kedro-Airflow
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-airflow/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro-airflow/)
 [![PyPI Version](https://badge.fury.io/py/kedro-airflow.svg)](https://pypi.org/project/kedro-airflow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 
 [Apache Airflow](https://github.com/apache/airflow) is a tool for orchestrating complex workflows and data processing pipelines. The Kedro-Airflow plugin can be used for:
 - Rapid pipeline creation in the prototyping phase. You can write Python functions in Kedro without worrying about schedulers, daemons, services or having to recreate the Airflow DAG file.
 - Automatic dependency resolution in Kedro. This allows you to bypass Airflow's need to specify the order of your tasks.
 - Distributing Kedro tasks across many workers. You can also enable monitoring and scheduling of the tasks' runtimes.
@@ -69,15 +72,15 @@
 
 For more information about the DAGs folder, please visit [Airflow documentation](https://airflow.apache.org/docs/stable/concepts.html#dags).
 The Airflow DAG configuration can be customized by editing this file.
 
 ### Step 3: Package and install the Kedro pipeline in the Airflow executor's environment
 
 After generating and deploying the DAG file, you will then need to package and install the Kedro pipeline into the Airflow executor's environment.
-Please visit the guide to [deploy Kedro as a Python package](https://docs.kedro.org/en/stable/deployment/single_machine.html#package-based) for more details.
+Please visit the guide to [Apache Airflow deployment](https://docs.kedro.org/en/stable/deployment/airflow.html) for more details.
 
 ### FAQ
 
 #### What if my DAG file is in a different directory to my project folder?
 
 By default, the generated DAG file is configured to live in the same directory as your project as per this [template](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/kedro_airflow/airflow_dag_template.j2#L44). If your DAG file is located in a different directory to your project, you will need to tweak this  manually after running the `kedro airflow create` command.
 
@@ -181,14 +184,27 @@
 
 Which Airflow Operator to use depends on the environment your project is running in.
 You can set the operator to use by providing a custom template.
 See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
 The [rich offering](https://airflow.apache.org/docs/apache-airflow-providers/operators-and-hooks-ref/index.html) of operators means that the `kedro-airflow` plugin is providing templates for specific operators.
 The default template provided by `kedro-airflow` uses the `BaseOperator`.
 
+### Can I group nodes together?
+
+When running Kedro nodes using Airflow, MemoryDatasets are often not shared across operators.
+This will cause the DAG run to fail.
+
+MemoryDatasets may be used to provide logical separation between nodes in Kedro, without the overhead of needing to write to disk (and in the case of distributed running needing multiple executors).
+
+Nodes that are connected through MemoryDatasets are grouped together via the `--group-in-memory` flag.
+This preserves the option to have logical separation in Kedro, with little computational overhead.
+
+It is possible to use [task groups](https://docs.astronomer.io/learn/task-groups) by changing the template.
+See ["What if I want to use a different Jinja2 template?"](#what-if-i-want-to-use-a-different-jinja2-template) for instructions on using custom templates.
+
 ## Can I contribute?
 
 Yes! Want to help build Kedro-Airflow? Check out our guide to [contributing](https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/CONTRIBUTING.md).
 
 ## What licence do you use?
 
 Kedro-Airflow is licensed under the [Apache 2.0](https://github.com/kedro-org/kedro-plugins/blob/main/LICENSE.md) License.
```

### Comparing `kedro-airflow-0.8.0/pyproject.toml` & `kedro_airflow-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,42 +7,46 @@
 authors = [
     {name = "Kedro"}
 ]
 description = "Kedro-Airflow makes it easy to deploy Kedro projects to Airflow"
 requires-python = ">=3.8"
 license = {text = "Apache Software License (Apache 2.0)"}
 dependencies = [
-    "kedro>=0.17.5",
+    "kedro>=0.19.0",
     "python-slugify>=4.0",
     "semver>=2.10",  # Needs to be at least 2.10.0 to make use of `VersionInfo.match`.
 ]
 dynamic = ["readme", "version"]
 
 [project.urls]
 Source = "https://github.com/kedro-org/kedro-plugins/tree/main/kedro-airflow"
 Documentation = "https://github.com/kedro-org/kedro-plugins/blob/main/kedro-airflow/README.md"
 Tracker = "https://github.com/kedro-org/kedro-plugins/issues"
 
 [project.optional-dependencies]
 test = [
-    "apache-airflow<2.7.0", # TODO: Temporary fix, to be reverted
+    "apache-airflow<3.0",
     "bandit",
     "behave",
     "black~=22.0",
-    "connexion<3.0.0", # TODO: Temporary fix, connexion has changed their API, but airflow hasn't caught up yet
+    "coverage>=7.2.0",
     "kedro-datasets",
-    "pendulum<3.0.0", # TODO: Also to be removed
+    "mypy~=1.0",
     "pre-commit>=2.9.2",
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pytest-xdist",
     "trufflehog>=2.1.0, <3.0",
     "ruff~=0.0.290",
-    "wheel"
+    "wheel",
+    # mypy requirements
+    "types-PyYAML",
+    "types-cachetools",
+    "types-toml",
 ]
 
 [project.entry-points."kedro.project_commands"]
 airflow = "kedro_airflow.plugin:commands"
 
 [tool.setuptools]
 include-package-data = true
@@ -68,15 +72,15 @@
 [tool.black]
 exclude=".*template.py"
 
 [tool.coverage.report]
 fail_under = 100
 show_missing = true
 omit = ["tests/*"]
-exclude_lines = ["pragma: no cover", "raise NotImplementedError"]
+exclude_also = ["raise NotImplementedError"]
 
 [tool.ruff]
 line-length = 88
 show-fixes = true
 select = [
     "F",   # Pyflakes
     "W",   # pycodestyle
```

