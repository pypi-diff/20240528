# Comparing `tmp/rra_tools-1.0.8.tar.gz` & `tmp/rra_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.8.tar", max compression
+gzip compressed data, was "rra_tools-1.0.9.tar", max compression
```

## Comparing `rra_tools-1.0.8.tar` & `rra_tools-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-22 04:20:07.505825 rra_tools-1.0.8/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-22 04:20:07.505825 rra_tools-1.0.8/README.md
--rw-r--r--   0        0        0     3770 2024-05-22 04:20:07.509825 rra_tools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      745 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     5439 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0    10244 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3082 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/translate.py
--rw-r--r--   0        0        0    14032 1970-01-01 00:00:00.000000 rra_tools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-27 23:05:14.885442 rra_tools-1.0.9/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-27 23:05:14.885442 rra_tools-1.0.9/README.md
+-rw-r--r--   0        0        0     3770 2024-05-27 23:05:14.885442 rra_tools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     5439 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0    10823 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-27 23:05:14.885442 rra_tools-1.0.9/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    14032 1970-01-01 00:00:00.000000 rra_tools-1.0.9/PKG-INFO
```

### Comparing `rra_tools-1.0.8/LICENSE` & `rra_tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/README.md` & `rra_tools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/pyproject.toml` & `rra_tools-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.8"
+version = "1.0.9"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rra_tools-1.0.8/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.9/src/rra_tools/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.9/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/cli_tools/options.py` & `rra_tools-1.0.9/src/rra_tools/cli_tools/options.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/jobmon.py` & `rra_tools-1.0.9/src/rra_tools/jobmon.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     task_name: str,
     task_resources: dict[str, str | int],
     *,
     node_args: dict[str, list[Any] | None] | None = None,
     flat_node_args: tuple[tuple[str, ...], list[tuple[Any, ...]]] | None = None,
     task_args: dict[str, Any] | None = None,
     op_args: dict[str, Any] | None = None,
+    max_attempts: int | None = None,
 ) -> list[Any]:
     """Build a parallel task graph for jobmon.
 
     Parameters
     ----------
     jobmon_tool
         The jobmon tool.
@@ -111,14 +112,16 @@
         The arguments to the task script that are the same for each task, but
         alter the behavior of the task (e.g. input and output root directories).
     op_args
         Arguments that are passed to the task script but do not alter the logical
         behavior of the task (e.g. number of cores, logging verbosity).
     task_resources
         The resources to allocate to the task.
+    max_attempts
+        The maximum number of attempts to make for each task.
 
     Returns
     -------
     list
         A list of tasks to run.
     """
     for arg in ["stdout", "stderr"]:
@@ -163,21 +166,25 @@
         arg_names, arg_values = flat_node_args
         for args in arg_values:
             task_args = {
                 **dict(zip(arg_names, args, strict=False)),
                 **clean_task_args,
                 **clean_op_args,
             }
-            task = task_template.create_task(**task_args)
+            task = task_template.create_task(
+                **task_args,
+                max_attempts=max_attempts,
+            )
             tasks.append(task)
     else:
         tasks = task_template.create_tasks(
             **clean_node_args,
             **clean_task_args,
             **clean_op_args,
+            max_attempts=max_attempts,
         )
     return tasks
 
 
 def run_workflow(  # type: ignore[no-untyped-def]
     workflow,
     log_method: Callable[[str], None] = print,
@@ -214,28 +221,34 @@
     task_name: str,
     task_resources: dict[str, str | int],
     *,
     node_args: dict[str, list[Any] | None] | None = None,
     flat_node_args: tuple[tuple[str, ...], list[tuple[Any, ...]]] | None = None,
     task_args: dict[str, Any] | None = None,
     op_args: dict[str, Any] | None = None,
+    concurrency_limit: int = 10000,
+    max_attempts: int | None = None,
     log_root: str | Path | None = None,
     log_method: Callable[[str], None] = print,
 ) -> None:
     """Run a parallel set of tasks using Jobmon.
 
     This helper function encapsulates one of the simpler workflow patterns in Jobmon:
     a set of tasks that run in parallel, each with the same command but
     different arguments. More complicated workflows should be implemented
     directly.
 
     Parameters
     ----------
+    runner
+        The runner to use for the task. Default is 'rptask'.
     task_name
-        pThe name of the task to run.  Will also be used as the tool and workflow name.
+        The name of the task to run.  Will also be used as the tool and workflow name.
+    task_resources
+        The resources to allocate to the task.
     node_args
         The arguments to the task script that are unique to each task. The keys of
         the dict are the names of the arguments and the values are lists of the
         values to use for each task. A dict with multiple keys will result in a
         cartesian product of the values. Mutually exclusive with
         flat_node_args.
     flat_node_args
@@ -246,18 +259,18 @@
         possible tasks. Mutually exclusive with node_args.
     task_args
         The arguments to the task script that are the same for each task, but
         alter the behavior of the task (e.g. input and output root directories).
     op_args
         Arguments that are passed to the task script but do not alter the logical
         behavior of the task (e.g. number of cores, logging verbosity).
-    task_resources
-        The resources to allocate to the task.
-    runner
-        The runner to use for the task. Default is 'rptask'.
+    concurrency_limit
+        The maximum number of tasks to run concurrently. Default is 10000.
+    max_attempts
+        The maximum number of attempts to make for each task.
     log_root
         The root directory for the logs. Default is None.
     log_method
         The method to use for logging. Default is print.
     """
     if node_args is not None and flat_node_args is not None:
         msg = "node_args and flat_node_args are mutually exclusive."
@@ -272,22 +285,26 @@
             raise KeyError(msg)
         log_root = Path(task_args["output-dir"])
     log_dir = make_log_dir(log_root)
     task_resources["stdout"] = str(log_dir / "output")
     task_resources["stderr"] = str(log_dir / "error")
 
     tool = get_jobmon_tool(workflow_name=task_name)
-    workflow = tool.create_workflow(name=f"{task_name}_{uuid.uuid4()}")
+    workflow = tool.create_workflow(
+        name=f"{task_name}_{uuid.uuid4()}",
+        max_concurrently_running=concurrency_limit,
+    )
 
     tasks = build_parallel_task_graph(
         jobmon_tool=tool,
         task_name=task_name,
         node_args=node_args,
         flat_node_args=flat_node_args,
         task_args=task_args,
         op_args=op_args,
         task_resources=task_resources,
         runner=runner,
+        max_attempts=max_attempts,
     )
 
     workflow.add_tasks(tasks)
     run_workflow(workflow, log_method)
```

### Comparing `rra_tools-1.0.8/src/rra_tools/logging/config.py` & `rra_tools-1.0.9/src/rra_tools/logging/config.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/logging/performance.py` & `rra_tools-1.0.9/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.9/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/parallel.py` & `rra_tools-1.0.9/src/rra_tools/parallel.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/shell_tools.py` & `rra_tools-1.0.9/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/src/rra_tools/translate.py` & `rra_tools-1.0.9/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.8/PKG-INFO` & `rra_tools-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

