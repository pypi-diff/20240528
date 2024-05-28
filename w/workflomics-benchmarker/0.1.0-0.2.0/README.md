# Comparing `tmp/workflomics_benchmarker-0.1.0.tar.gz` & `tmp/workflomics_benchmarker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workflomics_benchmarker-0.1.0.tar", max compression
+gzip compressed data, was "workflomics_benchmarker-0.2.0.tar", max compression
```

## Comparing `workflomics_benchmarker-0.1.0.tar` & `workflomics_benchmarker-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-01-29 16:10:00.222945 workflomics_benchmarker-0.1.0/LICENSE
--rw-r--r--   0        0        0     1404 2024-02-14 13:25:51.604818 workflomics_benchmarker-0.1.0/README.md
--rw-r--r--   0        0        0      987 2024-02-14 19:46:24.304613 workflomics_benchmarker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      191 2024-02-01 12:16:21.090935 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/__init__.py
--rw-r--r--   0        0        0     2371 2024-02-07 12:50:50.182414 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/cwltool_runner.py
--rw-r--r--   0        0        0    18284 2024-02-16 07:53:16.197994 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/cwltool_runtime_benchmark.py
--rw-r--r--   0        0        0     3347 2024-02-17 14:08:30.656691 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/cwltool_wrapper.py
--rw-r--r--   0        0        0     2281 2024-02-01 12:16:21.091972 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/loggingwrapper.py
--rw-r--r--   0        0        0      284 2024-02-15 15:00:07.433372 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/run.py
--rw-r--r--   0        0        0      200 2024-02-17 14:07:49.280575 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/utils.py
--rw-r--r--   0        0        0     2599 2024-02-07 12:50:50.188827 workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/workflomics.py
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 workflomics_benchmarker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-29 16:10:00.222945 workflomics_benchmarker-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4037 2024-05-28 10:14:43.068415 workflomics_benchmarker-0.2.0/README.md
+-rw-r--r--   0        0        0      971 2024-05-28 10:14:43.069355 workflomics_benchmarker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      191 2024-03-19 15:02:45.232860 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/__init__.py
+-rw-r--r--   0        0        0     8232 2024-05-28 10:14:43.069741 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/benchmark_utils.py
+-rw-r--r--   0        0        0      507 2024-05-28 10:14:43.069877 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwl_utils.py
+-rw-r--r--   0        0        0     3463 2024-05-28 10:14:43.070201 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwltool_runner.py
+-rw-r--r--   0        0        0    16605 2024-05-28 10:14:43.070435 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwltool_runtime_benchmark.py
+-rw-r--r--   0        0        0     2718 2024-05-28 10:14:43.070769 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwltool_wrapper.py
+-rw-r--r--   0        0        0     2281 2024-03-19 15:02:45.233911 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/loggingwrapper.py
+-rw-r--r--   0        0        0     3666 2024-05-28 10:14:43.070898 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/scientific_benchmarks.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:14:43.070932 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/technical_benchmarks.py
+-rw-r--r--   0        0        0      200 2024-05-01 08:27:48.954792 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/utils.py
+-rw-r--r--   0        0        0     3019 2024-05-28 10:14:43.071317 workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/workflomics.py
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 workflomics_benchmarker-0.2.0/PKG-INFO
```

### Comparing `workflomics_benchmarker-0.1.0/LICENSE` & `workflomics_benchmarker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workflomics_benchmarker-0.1.0/pyproject.toml` & `workflomics_benchmarker-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "workflomics-benchmarker"
-version = "0.1.0"
+version = "0.2.0"
 description = "Library used to execute workflows (in CWL) and benchmark them as part of the Workflomics ecosystem."
-authors = ["Nauman Ahmed <n.ahmed@esciencecenter.nl>",
-            "Peter Kok <p.kok@esciencecenter.nl>",
-            "Vedran Kasalica <v.kaslica@esciencecenter.nl>"]
+authors = ["Vedran Kasalica <v.kaslica@esciencecenter.nl>",
+            "Nauman Ahmed <n.ahmed@esciencecenter.nl>",
+            "Peter Kok <p.kok@esciencecenter.nl>"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.13"
 pyyaml = "^6.0"
 cwltool= "^3.1"
-
-[tool.poetry.dev-dependencies]
-cwltool= "^3.1"
+jsonpath-ng = "^1.6.1"
+pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 pytest = "^7.4.3"
 pytest-datadir = "^1.5.0"
 pytest-cov = "^4.1.0"
-cwltool= "^3.1"
 
 [tool.poetry.scripts]
 workflomics = "workflomics_benchmarker.workflomics:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/cwltool_runtime_benchmark.py` & `workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwltool_runtime_benchmark.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import subprocess
 from pathlib import Path
 import os
-import re
-import datetime
 import json
-from typing import Dict, List, Literal
+from typing import List, Literal
 
 from workflomics_benchmarker.loggingwrapper import LoggingWrapper
 from workflomics_benchmarker.cwltool_wrapper import CWLToolWrapper
 
+from workflomics_benchmarker.cwl_utils import extract_steps_from_cwl
+from workflomics_benchmarker.benchmark_utils import (
+    is_line_useless,
+    create_output_dir,
+    setup_empty_benchmark_for_step,
+    step_success_pattern,
+    step_fail_pattern,
+    set_step_status_to_failed,
+    benchmark_successful_step_execution,
+    benchmark_failed_step_execution
+)
+
 
 class CWLToolRuntimeBenchmark(CWLToolWrapper):
     """Runtime benchmarking class  to gather information about the runtime of each step in a workflow."""
 
-    KNOWN_USELESS_WARNINGS_ERRORS = [
-        "WARNING: The requested image's platform",
-        " 0 errors",
-        "Calculating sensitivity...and error tables...",
-        " 0 warnings",
-    ]
     EXECUTION_TIME_DESIRABILITY_BINS = {
         "0-150": 1,
         "151-300": 0.75,
         "301-450": 0.5,
         "451-600": 0.25,
         "601+": 0,
     }
@@ -30,431 +34,408 @@
         "0-250": 1,
         "251-500": 0.75,
         "501-750": 0.5,
         "751-1000": 0.25,
         "1001+": 0,
     }
     WARNINGS_DESIRABILITY_BINS = {
-        "0-1": 0,
-        "2-3": -0.25,
+        "0-0": 0,
+        "1-3": -0.25,
         "4-5": -0.5,
         "6-7": -0.75,
         "8+": -1,
     }
 
     def __init__(self, args):
         super().__init__(args)
-        self.workflow_benchmark_result = {}
-
 
-    def is_line_useless(self, line):
-        """Check if a line is useless for the benchmarking.
-        
-        Parameters
-        ----------
-        line: str
-            The line to check.
-        
-        Returns
-        -------
-        bool
-            True if the line is useless, False otherwise.
-        
+    def execute_and_benchmark_workflow(self, workflow) -> dict:
         """
-        for useless in self.KNOWN_USELESS_WARNINGS_ERRORS:
-            if useless in line:
-                return True
-        return False
-
-    def run_workflow(self, workflow) -> None:
-        """Run a workflow and gather information about the runtime of each step.
-
+        Execute a single workflow, save the outputs and benchmark each step, i.e., tool, of the workflow.
+        TODO: Split into execute and benchmark functions.
         Parameters
         ----------
         workflow: str
             The path to the workflow file.
-        
+
         Returns
         -------
-        None
+        dict
+            A dictionary containing the benchmark results of the workflow.
         """
+        workflow_execution_information = {}
+        workflow_name = Path(workflow).name
+
         command = ["cwltool"]
 
         if self.container == "singularity":  # use singularity if the flag is set
             LoggingWrapper.warning(
                 "Using singularity container, memory usage will not be calculated."
             )
             command.append("--singularity")
 
-        self.workflow_outdir = os.path.join(
-            self.outdir, Path(workflow).name + "_output"
-        )  # create the output directory for the workflow
-        Path(self.workflow_outdir).mkdir(
-            exist_ok=True
-        )  # create the output directory for the workflow
+        workflow_outdir = create_output_dir(self.outdir, workflow_name)
+
         command.extend(
             [
+                "--on-error",
+                "continue",
                 "--disable-color",
                 "--timestamps",
                 "--outdir",
-                self.workflow_outdir,
+                workflow_outdir,
                 workflow,
                 self.input_yaml_path,
             ]
         )  # add the required option in cwltool to disable color and timestamps to enable benchmarking
-        steps = self.extract_steps_from_cwl(workflow)
+        steps = extract_steps_from_cwl(workflow)
+
         result = subprocess.run(
             command,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             text=True,
             encoding="utf-8",
         )  # run the workflow
         if self.verbose:
             print(result.stdout)
-        output_lines = result.stdout.split("\n")
-        success_pattern = re.compile(
-            r"\[job (.+)\] completed success"
-        )  # pattern to match the success of a step
-        fail_pattern = re.compile(
-            r"\[job (.+)\] completed permanentFail|ERROR Exception on step '([^']+)'"
-        )  # pattern to match the failure of a step
-        success_steps = set()  #Set of step names that were executed successfully.
-        step_results = [
-            {
-                "step": step,
-                "status": "-",
-                "time": "N/A",
-                "memory": "N/A",
-                "warnings": "N/A",
-                "errors": "N/A",
-            }
-            for step in steps
-        ]
+        cwltool_output_lines = result.stdout.split("\n")
 
-        for (
-            line
-        ) in (
-            output_lines
-        ):  # iterate over the output of the workflow and find which steps were executed successfully
-            successfull_match = success_pattern.search(line)
-            failed_match = fail_pattern.search(line)
-            if successfull_match:
-                success_steps.add(successfull_match.group(1))
-            elif failed_match:
-                failed_tool_name = failed_match.group(1) if failed_match.group(1) is not None else failed_match.group(2)
-                for entry in step_results:
-                    # set the benchmark values for the failed steps to N/A
-                    if entry["step"] == failed_tool_name:
-                        entry["status"] = "✗"
-                        entry["time"] = "N/A"
-                        entry["memory"] = "N/A"
-                        entry["warnings"] = "N/A"
-                        entry["errors"] = "N/A"
-        for (
-            step
-        ) in (
-            success_steps
-        ):  # iterate over the output of the workflow and find the benchmark values for each step
-            max_memory_step = "N/A"
-            step_start = False
-            warnings_step = []
-            errors_step = []
-            for line in output_lines:
-                if f"[step {step}] start" in line:
-                    start_time_step = datetime.datetime.strptime(
-                        line[:21], "[%Y-%m-%d %H:%M:%S]"
-                    )
-                    step_start = True
-                elif f"[job {step}] completed success" in line:
-                    end_time_step = datetime.datetime.strptime(
-                        line[:21], "[%Y-%m-%d %H:%M:%S]"
+        # Set of step names that were executed successfully.
+        successfully_executed_steps = set()
+        failed_steps = set()
+
+        step_results = [setup_empty_benchmark_for_step(tool) for tool in steps]
+        # iterate over the output of the workflow and find which steps were executed successfully
+        for line in cwltool_output_lines:
+            successful_match = step_success_pattern(line)
+            if successful_match:
+                successfully_executed_steps.add(successful_match.group(1))
+            else:
+                failed_match = step_fail_pattern(line)
+                if failed_match:
+                    failed_tool_name = (
+                        failed_match.group(1)
+                        if failed_match.group(1) is not None
+                        else failed_match.group(2)
                     )
-                    break
-                elif step_start:
-                    if f"[job {step}] Max memory used" in line:
-                        max_memory_step = int(
-                            line.split()[-1].rstrip(line.split()[-1][-3:])
-                        )
-                        if line.split()[-1].endswith("GiB"):
-                            max_memory_step = max_memory_step * 1024
-                        if max_memory_step == 0:
-                            max_memory_step = 1
-                    elif "warning" in line.lower():
-                        if not self.is_line_useless(line):
-                            warnings_step.append(line)
-                    elif "error" in line.lower():
-                        if not self.is_line_useless(line):
-                            errors_step.append(line)
-
-            execution_time_step = int((end_time_step - start_time_step).total_seconds())
-            if execution_time_step == 0:
-                execution_time_step = 1 # set the minimum execution time to 1 second. Decimal values cannot be retrieved from the cwltool output, so the number of seconds is rounded up.
-            for (
-                entry
-            ) in (
-                step_results
-            ):  # store the benchmark values for each successfully executed step
-                if entry["step"] == step:
-                    entry["status"] = "✓"
-                    entry["time"] = execution_time_step
-                    entry["memory"] = max_memory_step
-                    entry["warnings"] = warnings_step
-                    entry["errors"] = errors_step
+                    failed_steps.add(failed_tool_name)
 
+        # iterate over the output of the workflow and find the benchmark values for each step
+        step_results = benchmark_successful_step_execution(successfully_executed_steps, cwltool_output_lines, step_results, workflow_outdir)
+        step_results = benchmark_failed_step_execution(failed_steps, cwltool_output_lines, step_results)
         workflow_status = "✓"
         for entry in step_results:  # check if the workflow was executed successfully
             if entry["status"] == "✗" or entry["status"] == "-":
                 workflow_status = "✗"
                 break
 
-        self.workflow_benchmark_result = {
+        workflow_execution_information = {
             "n_steps": len(steps),
             "status": workflow_status,
             "steps": step_results,
         }
 
-    def aggregate_workflow_benchmark_value(self, benchmark_name) -> int | Literal["✗", "N/A"]:
+        LoggingWrapper.info(
+                "Benchmarking " + workflow_name + " completed.", color="green"
+            )
+
+        return workflow_execution_information
+
+    def count_successful_steps(self, all_tools_exe) -> int:
+        """Count the number of steps that were executed successfully.
+
+        Parameters
+        ----------
+        step_results: List[dict]
+            The list of step results.
+
+        Returns
+        -------
+        int
+            The number of steps that were executed successfully.
+        """
+        return len([tool_execution for tool_execution in all_tools_exe if tool_execution["status"] == "✓"])
+    
+
+    def aggregate_workflow_benchmark_value(
+        self, benchmark_name, workflow_execution_information
+    ) -> int | Literal["✗", "N/A"]:
         """Calculate the aggregate benchmark value for the given workflow.
 
         Parameters
         ----------
         benchmark_name: str
             The name of the benchmark to calculate.
-        
+
         Returns
         -------
         value: int | Literal["✗", "N/A"]
             The value of the benchmark.
         """
         value: int = 0
-        for entry in self.workflow_benchmark_result["steps"]:
+        for tool_execution in workflow_execution_information["steps"]:
             match benchmark_name:
                 case "status":
-                    if entry[benchmark_name] != "✗" and entry[benchmark_name] != "-":
+                    if tool_execution[benchmark_name] != "✗" and tool_execution[benchmark_name] != "-":
                         value = "✓"
                     else:
-                        return "✗"
+                        return f"({self.count_successful_steps(workflow_execution_information['steps'])}/{len(workflow_execution_information['steps'])}) ✗"
                 case "time":
-                    if entry[benchmark_name] != "N/A":
-                        value = value + entry["time"]
-                    else:
-                        return "N/A"
+                    if tool_execution[benchmark_name] != "-":
+                        value = value + tool_execution[benchmark_name]
                 case "memory":
-                    if entry[benchmark_name] != "N/A":
+                    if tool_execution["memory"] not in ["-", "N/A"]:
                         # remove last 3 characters from string (MiB, GiB, etc.)
-                        value = max(value, entry["memory"])
-                    else:
-                        return "N/A"
+                        value = max(value, tool_execution["memory"])
                 case "warnings":
-                    value = value + len(entry["warnings"])
+                    value = value + len(tool_execution["warnings"])
                 case "errors":
-                    value = value + len(entry["errors"])
+                    value = value + len(tool_execution["errors"])
+                case "go_terms":
+                    if tool_execution[benchmark_name] != "-":
+                        value = value + tool_execution[benchmark_name]
+                case "identified_proteins":
+                    if tool_execution[benchmark_name] != "-":
+                        value = value + tool_execution[benchmark_name]
         return value
 
-    def calc_desirability(self, benchmark_name, value):
+    def calc_desirability(self, benchmark_name, value, status="✓"):
         """Calculate the desirability for the given benchmark value.
-        
+
         Parameters
         ----------
         benchmark_name: str
             The name of the benchmark.
         value: int
             The value of the benchmark.
-        
+
         Returns
         -------
         float
             The desirability of the benchmark value.
         """
         match benchmark_name:
             case "status":
                 if value == "✓":
                     return 1
-                elif value == "✗":
-                    return -1
-                else:
+                elif value == "-":
                     return 0
+                else:
+                    return -1
             case "errors":
                 if isinstance(value, list):
                     value = len(value)
                 return 0 if value == 0 else -1
             case "time":
-                if value == "N/A":
+                if value == "-":
                     return 0
+                elif status == "✗":
+                    return -1
                 bins = self.EXECUTION_TIME_DESIRABILITY_BINS
             case "memory":
-                if value == "N/A":
+                if value == "-":
                     return 0
+                elif status == "✗":
+                    return -1
                 bins = self.MAX_MEMORY_DESIRABILITY_BINS
             case "warnings":
                 bins = self.WARNINGS_DESIRABILITY_BINS
                 if isinstance(value, list):
                     value = len(value)
+            case "go_terms":
+                if value == "-":
+                    return 0
+                if value == 0 or value > 1000:
+                    return -1
+                return 1
+            case "identified_proteins":
+                if value == "-":
+                    return 0
+                if value == 0 or value > 1000:
+                    return -1
+                return 1
+
         for key, value in bins.items():
             if "-" in key:
                 if value <= int(key.split("-")[1]):
                     return bins[key]
             else:
                 return bins[key]
         return 0
 
-    def get_step_benchmarks(self, name) -> List[dict]:
+    def get_step_benchmarks(self, name, workflow_execution_information) -> List[dict]:
         """Get benchmark data for all the steps of the workflow for the given benchmark.
-        
+
         Parameters
         ----------
         name: str
             The name of the benchmark.
-        
+
         Returns
         -------
         List[dict]
             The list of benchmark data for all the steps of the workflow.
         """
         benchmark = []
         # iterate over the steps and store the benchmark values for each step
-        for entry in self.workflow_benchmark_result["steps"]:
+        for entry in workflow_execution_information["steps"]:
             # each step 'entry' is either having a numeric value, or is "N/A" in case it was not executed. Special case are the status entries, which are either "✓", "✗" or "-" (when not reached).
-            val = (entry[name])
+            val = entry[name]
             tooltip = {}
             if name == "errors" or name == "warnings":
                 if (val) != "N/A" and len(entry[name]) > 0:
                     tooltip = {"tooltip": entry[name]}
                     val = len(entry[name])
                 else:
                     val = 0
-                
+
             step_benchmark = {
                 "label": entry["step"].rstrip(
                     "_0123456789"
                 ),  # Label the step without the number at the end
                 "value": val,
                 "desirability": (
-                    -1
-                    if entry["status"] == "✗"
-                    else self.calc_desirability(name, val)
+                    -1 if entry["status"] == "✗" else self.calc_desirability(name, val)
                 ),
             }
             step_benchmark.update(tooltip)
             benchmark.append(step_benchmark)
         return benchmark
 
+    def create_benchmark(self, description, title, unit, key, workflow_execution_information) -> dict:
+        """
+        Create a benchmark json entry.
+
+        Parameters
+        ----------
+        benchmarks : list
+            A list to which the benchmark data will be appended.
+        description : str
+            A description of the benchmark.
+        title : str
+            The title of the benchmark.
+        unit : str
+            The unit of measurement for the benchmark data.
+        key : str
+            The key used to fetch and calculate benchmark values from the workflow.
+        
+        Returns
+        -------
+        dict
+            A dictionary containing the benchmark data.
+
+        """
+        return {
+                "description": description,
+                "title": title,
+                "unit": unit,
+                "aggregate_value": {
+                    "value": self.aggregate_workflow_benchmark_value(key, workflow_execution_information),
+                    "desirability": self.calc_desirability(
+                        key, self.aggregate_workflow_benchmark_value(key, workflow_execution_information), workflow_execution_information["status"]
+                    ),
+                },
+                "steps": self.get_step_benchmarks(key, workflow_execution_information),
+            }
+        
+
+    def compute_technical_benchmarks(self,workflow_execution_information) -> List[dict]:
+        """
+        Compute the technical benchmarks for the workflow.
+
+        Returns:
+        - List[dict]: A list of technical benchmarks.
+        """
+        technical_benchmarks = []  # Define the "benchmarks" variable
+        technical_benchmarks.append(self.create_benchmark(
+            "Status for each step in the workflow",
+            "Status",
+            "✓ or ✗",
+            "status",
+        workflow_execution_information))
+
+        technical_benchmarks.append(self.create_benchmark(
+            "Execution time for each step in the workflow",
+            "Execution time",
+            "seconds",
+            "time",
+        workflow_execution_information))
+        
+        technical_benchmarks.append(self.create_benchmark(
+            "Memory usage for each step in the workflow",
+            "Memory usage",
+            "MB",
+            "memory",
+        workflow_execution_information))
+
+        technical_benchmarks.append(self.create_benchmark(
+            "Warnings for each step in the workflow",
+            "Warnings",
+            "count",
+            "warnings",
+        workflow_execution_information))
+
+        technical_benchmarks.append(self.create_benchmark(
+            "Errors for each step in the workflow",
+            "Errors",
+            "count",
+            "errors",
+        workflow_execution_information))
+
+        technical_benchmarks.append(self.create_benchmark(
+            "The number of identified proteins.",
+            "Proteins",
+            "count",
+            "identified_proteins",
+        workflow_execution_information))
+
+        technical_benchmarks.append(self.create_benchmark(
+            "The number of identified significantly enriched unique GO-terms.",
+            "GO-terms",
+            "count",
+            "go_terms",
+        workflow_execution_information))
+
+        return technical_benchmarks
+
+
     def run_workflows(self) -> None:
         """Run the workflows in the given directory and store the results in a json file."""
         success_workflows = []
         failed_workflows = []
         workflows_benchmarks = []
 
         for (
             workflow_path
         ) in self.workflows:  # iterate over the workflows and execute them
             workflow_name = Path(workflow_path).name
             LoggingWrapper.info("Benchmarking " + workflow_name + "...", color="green")
-            self.run_workflow(workflow_path)
-            if (
-                self.workflow_benchmark_result["status"] == "✗"
-            ):  # check if the workflow was executed successfully
+            workflow_execution_information = self.execute_and_benchmark_workflow(workflow_path)
+            
+            if (workflow_execution_information["status"] == "✗"): 
                 LoggingWrapper.error(workflow_name + " failed")
                 failed_workflows.append(workflow_name)
             else:
                 LoggingWrapper.info(
                     workflow_name + " finished successfully.", color="green"
                 )
                 success_workflows.append(workflow_name)
-            LoggingWrapper.info(
-                f"Output of {workflow_name} is stored in {self.workflow_outdir}. It may be empty if the workflow failed."
-            )
-            LoggingWrapper.info(
-                "Benchmarking " + workflow_name + " completed.", color="green"
-            )
+            
             # store the benchmark results for each workflow in a json file
             all_workflow_data = {
-                "workflowName": "",
+                "workflowName": workflow_name,
                 "executor": "cwltool " + self.version,
                 "runID": "39eddf71ea1700672984653",
                 "inputs": {
                     key: {"filename": self.input[key]["filename"]} for key in self.input
                 },
-                "benchmarks": [],
+                "benchmarks": self.compute_technical_benchmarks(workflow_execution_information),
             }
 
-            all_workflow_data["workflowName"] = workflow_name
-
-            all_workflow_data["benchmarks"].append(
-                {
-                    "description": "Status for each step in the workflow",
-                    "title": "Status",
-                    "unit": "✓ or ✗",
-                    "aggregate_value": {
-                        "value": str(self.aggregate_workflow_benchmark_value("status")),
-                        "desirability": self.calc_desirability(
-                            "status", self.aggregate_workflow_benchmark_value("status")
-                        ),
-                    },
-                    "steps": self.get_step_benchmarks("status"),
-                }
-            )
-            all_workflow_data["benchmarks"].append(
-                {
-                    "description": "Execution time for each step in the workflow",
-                    "title": "Execution time",
-                    "unit": "seconds",
-                    "aggregate_value": {
-                        "value": self.aggregate_workflow_benchmark_value("time"),
-                        "desirability": self.calc_desirability(
-                            "time", self.aggregate_workflow_benchmark_value("time")
-                        ),
-                    },
-                    "steps": self.get_step_benchmarks("time"),
-                }
-            )
-            all_workflow_data["benchmarks"].append(
-                {
-                    "description": "Memory usage for each step in the workflow",
-                    "title": "Memory usage",
-                    "unit": "MB",
-                    "aggregate_value": {
-                        "value": self.aggregate_workflow_benchmark_value("memory"),
-                        "desirability": self.calc_desirability(
-                            "memory", self.aggregate_workflow_benchmark_value("memory")
-                        ),
-                    },
-                    "steps": self.get_step_benchmarks("memory"),
-                }
-            )
-            all_workflow_data["benchmarks"].append(
-                {
-                    "description": "Warnings for each step in the workflow",
-                    "title": "Warnings",
-                    "unit": "count",
-                    "aggregate_value": {
-                        "value": self.aggregate_workflow_benchmark_value("warnings"),
-                        "desirability": self.calc_desirability(
-                            "warnings", self.aggregate_workflow_benchmark_value("warnings")
-                        ),
-                    },
-                    "steps": self.get_step_benchmarks("warnings"),
-                }
-            )
-            all_workflow_data["benchmarks"].append(
-                {
-                    "description": "Errors for each step in the workflow",
-                    "title": "Errors",
-                    "unit": "count",
-                    "aggregate_value": {
-                        "value": self.aggregate_workflow_benchmark_value("errors"),
-                        "desirability": self.calc_desirability(
-                            "errors", self.aggregate_workflow_benchmark_value("errors")
-                        ),
-                    },
-                    "steps": self.get_step_benchmarks("errors"),
-                }
-            )
-
             workflows_benchmarks.append(all_workflow_data)
 
         with open(os.path.join(self.outdir, "benchmarks.json"), "w") as f:
             json.dump(workflows_benchmarks, f, indent=3)
             LoggingWrapper.info(
                 "Benchmark results stored in "
                 + os.path.join(self.outdir, "benchmarks.json"),
```

### Comparing `workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/cwltool_wrapper.py` & `workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/cwltool_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from typing import List
 import yaml
 import subprocess
 import sys
 
 from workflomics_benchmarker.loggingwrapper import LoggingWrapper
 from workflomics_benchmarker.utils import natural_keys
 class CWLToolWrapper():
@@ -64,28 +63,9 @@
                     inputs[key] = {"filename": Path(value['path']).name}
                 else:
                     inputs[key] = {"filename": Path(value['path']).name}
         with open(input_yaml_path, 'w') as file:
             documents = yaml.dump(input_data, file)
         return inputs
 
-    def extract_steps_from_cwl(self, workflow_file) -> List[str]:
-        """Extract the step (tool) names from the cwl workflow file in the order they are defined.
-        
-        Parameters
-        ----------
-        workflow_file : str
-            The path to the cwl workflow file.
-            
-        Returns
-        -------
-        List[str]
-            The list of step names.
-        """
-        with open(workflow_file, 'r') as file:
-            data = yaml.safe_load(file)
-        steps = []
-        for step_name in data.get('steps', {}):
-            steps.append(step_name)
-        return steps
-
+
```

### Comparing `workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/loggingwrapper.py` & `workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/loggingwrapper.py`

 * *Files identical despite different names*

### Comparing `workflomics_benchmarker-0.1.0/src/workflomics_benchmarker/workflomics.py` & `workflomics_benchmarker-0.2.0/src/workflomics_benchmarker/workflomics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 
+from sys import platform
 from workflomics_benchmarker.loggingwrapper import LoggingWrapper
 from workflomics_benchmarker.cwltool_runtime_benchmark import CWLToolRuntimeBenchmark
 from workflomics_benchmarker.cwltool_runner import CWLToolRunner
 
 
 def add_benchmark_args(parser):
     """Add the arguments for the benchmark command."""
@@ -19,19 +20,23 @@
     parser.add_argument('-o','--outdir', help='Path to the output directory to store the results (default: workflows directory).', default= None)
     parser.add_argument('-v', '--verbose', action='store_true', help='Print the output of the cwltool command.')
     parser.add_argument('-i','--input', help='Path to the input yaml file (default: input.yml in the workflows directory).', default= None)
     parser.add_argument('workflows', help='Path to the workflows directory.')
    
 
 def main():
-    """Main entry point for the workflomics_runner application."""
+    """Main entry point for the workflomics-benchmarker application."""
 
-    LoggingWrapper.info("Starting workflomics_runner...", color="green", bold=True)
+    LoggingWrapper.info("Starting workflomics-benchmarker...", color="green", bold=True)
 
-    parser = argparse.ArgumentParser(description='Wrapper for cwltool command.')
+    if platform == "win32":
+        LoggingWrapper.error("This application uses tools that are not supported on Windows natively. To run on Windows, use WSL.", color="red", bold=True)
+        return
+
+    parser = argparse.ArgumentParser(description='Wrapper for cwltool command.', epilog='See \'workflomics <subcommand> --help\' for additional information about a specific subcommand.')
     # Adding subparsers for the benchmark and run commands
     subparsers = parser.add_subparsers(dest='subcommand', help='Subcommands.')
     parser_benchmark = subparsers.add_parser('benchmark', help='Run the benchmark.')
     parser_run = subparsers.add_parser('run', help='Run the workflow.')
 
     add_benchmark_args(parser_benchmark)
     add_run_args(parser_run)
@@ -39,14 +44,17 @@
 
     
     if (args.subcommand == "benchmark"):
         LoggingWrapper.info("Benchmarking Workflows...", color="green", bold=True)
         op = CWLToolRuntimeBenchmark(args)
     elif (args.subcommand == "run"):
         LoggingWrapper.info("Running Workflows...", color="green", bold=True)
-        op = CWLToolRunner(args)    
+        op = CWLToolRunner(args)
+    elif (args.subcommand == None):
+        parser.print_help()
+        return    
 
     op.run_workflows()
 
 
 if __name__ == "__main__":
     main()
```

