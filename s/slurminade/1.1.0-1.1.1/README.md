# Comparing `tmp/slurminade-1.1.0.tar.gz` & `tmp/slurminade-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurminade-1.1.0.tar", last modified: Tue Feb 27 15:41:52 2024, max compression
+gzip compressed data, was "slurminade-1.1.1.tar", last modified: Tue May 28 13:33:52 2024, max compression
```

## Comparing `slurminade-1.1.0.tar` & `slurminade-1.1.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.533044 slurminade-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.521044 slurminade-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.525044 slurminade-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-27 15:41:44.000000 slurminade-1.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-27 15:41:44.000000 slurminade-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-27 15:41:44.000000 slurminade-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-02-27 15:41:44.000000 slurminade-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-27 15:41:44.000000 slurminade-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-27 15:41:44.000000 slurminade-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16044 2024-02-27 15:41:52.533044 slurminade-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15425 2024-02-27 15:41:44.000000 slurminade-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.525044 slurminade-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-27 15:41:44.000000 slurminade-1.1.0/docs/slurminade.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.525044 slurminade-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-27 15:41:44.000000 slurminade-1.1.0/examples/example_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-27 15:41:44.000000 slurminade-1.1.0/examples/example_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-27 15:41:44.000000 slurminade-1.1.0/examples/example_2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-27 15:41:44.000000 slurminade-1.1.0/examples/example_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-02-27 15:41:44.000000 slurminade-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-27 15:41:44.000000 slurminade-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 15:41:52.533044 slurminade-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.525044 slurminade-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.529044 slurminade-1.1.0/src/slurminade/
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/bundling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/execute_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/function_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/guard.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/job_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/node_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-27 15:41:44.000000 slurminade-1.1.0/src/slurminade/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.529044 slurminade-1.1.0/src/slurminade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16044 2024-02-27 15:41:52.000000 slurminade-1.1.0/src/slurminade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-27 15:41:52.000000 slurminade-1.1.0/src/slurminade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 15:41:52.000000 slurminade-1.1.0/src/slurminade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-27 15:41:52.000000 slurminade-1.1.0/src/slurminade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 15:41:52.000000 slurminade-1.1.0/src/slurminade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:52.529044 slurminade-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_create_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_dispatch_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_local_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_node_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-27 15:41:44.000000 slurminade-1.1.0/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.335905 slurminade-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.323905 slurminade-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.327905 slurminade-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-28 13:33:44.000000 slurminade-1.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 13:33:44.000000 slurminade-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-28 13:33:44.000000 slurminade-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-28 13:33:44.000000 slurminade-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 13:33:44.000000 slurminade-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 13:33:44.000000 slurminade-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16153 2024-05-28 13:33:52.335905 slurminade-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15534 2024-05-28 13:33:44.000000 slurminade-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.327905 slurminade-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-28 13:33:44.000000 slurminade-1.1.1/docs/slurminade.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.327905 slurminade-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-28 13:33:44.000000 slurminade-1.1.1/examples/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-28 13:33:44.000000 slurminade-1.1.1/examples/example_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 13:33:44.000000 slurminade-1.1.1/examples/example_2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-28 13:33:44.000000 slurminade-1.1.1/examples/example_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-28 13:33:44.000000 slurminade-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 13:33:44.000000 slurminade-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:33:52.335905 slurminade-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.327905 slurminade-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.331905 slurminade-1.1.1/src/slurminade/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/bundling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/execute_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/function_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/job_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/node_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-28 13:33:44.000000 slurminade-1.1.1/src/slurminade/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.331905 slurminade-1.1.1/src/slurminade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16153 2024-05-28 13:33:52.000000 slurminade-1.1.1/src/slurminade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-28 13:33:52.000000 slurminade-1.1.1/src/slurminade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:33:52.000000 slurminade-1.1.1/src/slurminade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 13:33:52.000000 slurminade-1.1.1/src/slurminade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 13:33:52.000000 slurminade-1.1.1/src/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:52.331905 slurminade-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_create_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_create_command_with_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_dispatch_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_local_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_node_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-28 13:33:44.000000 slurminade-1.1.1/tests/test_subprocess.py
```

### Comparing `slurminade-1.1.0/.github/workflows/pytest.yml` & `slurminade-1.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/.github/workflows/release.yml` & `slurminade-1.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/.gitignore` & `slurminade-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/.pre-commit-config.yaml` & `slurminade-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/.readthedocs.yaml` & `slurminade-1.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/LICENSE` & `slurminade-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/PKG-INFO` & `slurminade-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 1.1.0
+Version: 1.1.1
 Summary: A decorator-based slurm runner.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/slurminade
 Project-URL: Issues, https://github.com/d-krupke/slurminade/issues
 Keywords: slurm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -372,14 +372,15 @@
 -  guard.py: Contains code to prevent you accidentally DDoSing your
    infrastructure.
 -  options.py: Contains a simple data structure to save slurm options.
 
 Changes
 -------
 
+- 1.1.1: Fixing bug when there is some output to stdout when loading the code, such as deprecation warnings.
 - 1.1.0: Slurminade can now be called from iPython, too! `exec` has been renamed `shell` to prevent confusion with the Python call `exec` which will evaluate a string as Python code.
 - 1.0.1: Dispatcher now return jobs references instead of job ids. This allows to do some fancier stuff in the future, when the jobs infos are only available a short time after the job has been submitted.
 - 0.10.1: FIX: Listing functions will no longer execute setup functions.
 -  0.10.0: `Batch` is now named `JobBundling`. There is a method `join` for easier synchronization. `exec` allows to executed commands just like `srun` and `sbatch`, but uniform syntax with other slurmified functions. Functions can now also be called with `distribute_and_wait`. If you call `python3 -m slurminade.check --partition YOUR_PARTITION --constraint YOUR_CONSTRAINT` you can check if your slurm configuration is running correctly.
 -  0.9.0: Lots of improvements.
 -  0.8.1: Bugfix and automatic detection of wrong usage when using ``Batch`` with ``wait_for``.
 -  0.8.0: Added extensive logging and improved typing.
```

### Comparing `slurminade-1.1.0/README.rst` & `slurminade-1.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,15 @@
 -  guard.py: Contains code to prevent you accidentally DDoSing your
    infrastructure.
 -  options.py: Contains a simple data structure to save slurm options.
 
 Changes
 -------
 
+- 1.1.1: Fixing bug when there is some output to stdout when loading the code, such as deprecation warnings.
 - 1.1.0: Slurminade can now be called from iPython, too! `exec` has been renamed `shell` to prevent confusion with the Python call `exec` which will evaluate a string as Python code.
 - 1.0.1: Dispatcher now return jobs references instead of job ids. This allows to do some fancier stuff in the future, when the jobs infos are only available a short time after the job has been submitted.
 - 0.10.1: FIX: Listing functions will no longer execute setup functions.
 -  0.10.0: `Batch` is now named `JobBundling`. There is a method `join` for easier synchronization. `exec` allows to executed commands just like `srun` and `sbatch`, but uniform syntax with other slurmified functions. Functions can now also be called with `distribute_and_wait`. If you call `python3 -m slurminade.check --partition YOUR_PARTITION --constraint YOUR_CONSTRAINT` you can check if your slurm configuration is running correctly.
 -  0.9.0: Lots of improvements.
 -  0.8.1: Bugfix and automatic detection of wrong usage when using ``Batch`` with ``wait_for``.
 -  0.8.0: Added extensive logging and improved typing.
```

### Comparing `slurminade-1.1.0/docs/Makefile` & `slurminade-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/docs/conf.py` & `slurminade-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/docs/make.bat` & `slurminade-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/docs/slurminade.rst` & `slurminade-1.1.1/docs/slurminade.rst`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/examples/example_1.py` & `slurminade-1.1.1/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/examples/example_2.py` & `slurminade-1.1.1/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/examples/example_3.py` & `slurminade-1.1.1/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/pyproject.toml` & `slurminade-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "slurminade"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)", email = "krupke@ibr.cs.tu-bs.de" },
 ]
 description = "A decorator-based slurm runner."
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `slurminade-1.1.0/src/slurminade/__init__.py` & `slurminade-1.1.1/src/slurminade/__init__.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/bundling.py` & `slurminade-1.1.1/src/slurminade/bundling.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/check.py` & `slurminade-1.1.1/src/slurminade/check.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/conf.py` & `slurminade-1.1.1/src/slurminade/conf.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/dispatcher.py` & `slurminade-1.1.1/src/slurminade/dispatcher.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/execute.py` & `slurminade-1.1.1/src/slurminade/execute.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/execute_cmds.py` & `slurminade-1.1.1/src/slurminade/execute_cmds.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,9 +59,10 @@
         "-m",
         "slurminade.execute",
         "--root",
         str(entry_point),
         "--listfuncs",
     ]
     out = subprocess.check_output(cmd).decode()
+    out = out.strip().split("\n")[-1].strip()
     ids = json.loads(out)
     return set(ids)
```

### Comparing `slurminade-1.1.0/src/slurminade/function.py` & `slurminade-1.1.1/src/slurminade/function.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/function_call.py` & `slurminade-1.1.1/src/slurminade/function_call.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/function_map.py` & `slurminade-1.1.1/src/slurminade/function_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Not relevant for endusers.
 """
 
 import inspect
 import logging
 import pathlib
 import typing
+from typing import Optional
 from pathlib import Path
 
 from .execute_cmds import call_slurminade_to_get_function_ids
 
 
 class FunctionMap:
     """
@@ -20,15 +21,15 @@
     """
 
     # Needed to save the entry point at the slurm node.
     # The slurm node just executes the file content of a script, so the file name is lost.
     # slurminade will set this value in the beginning to reconstruct it.
     entry_point: typing.Optional[str] = None
     _data = {}
-    _ids = set()
+    _ids: Optional[set] = set()
 
     @staticmethod
     def get_id(func: typing.Callable) -> str:
         """
         Returns the unique id of a function. Necessary to slurmify it.
         Probably not needed by the enduser.
         It uses the function name and its file, which should be sufficient unless you
@@ -98,17 +99,28 @@
         if func_id not in FunctionMap._data:
             msg = f"Function '{func_id}' unknown!"
             raise KeyError(msg)
         return FunctionMap._data[func_id](*args, **kwargs)
 
     @staticmethod
     def check_id(func_id: str, entry_point: Path) -> bool:
+        if FunctionMap._ids is None:
+            return True
         if func_id in FunctionMap._ids:
             return True
-        FunctionMap._ids = call_slurminade_to_get_function_ids(entry_point)
+        try:
+            # Try to identify the available function ids when the entry point is known.
+            # This can help detect some bugs early on.
+            FunctionMap._ids = call_slurminade_to_get_function_ids(entry_point)
+        except Exception as e:
+            logging.getLogger("slurminade").warning(
+                "Cannot verify function ids before submitting to slurm: %s. This is not critical, things will just be more difficult to debug in case you make an error.", e
+            )
+            FunctionMap._ids = None
+            return True
         logging.getLogger("slurminade").info(
             "Entry point '%s' has functions %s",
             entry_point,
             list(FunctionMap._ids),
         )
         return func_id in FunctionMap._ids
```

### Comparing `slurminade-1.1.0/src/slurminade/guard.py` & `slurminade-1.1.1/src/slurminade/guard.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/node_setup.py` & `slurminade-1.1.1/src/slurminade/node_setup.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade/options.py` & `slurminade-1.1.1/src/slurminade/options.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/src/slurminade.egg-info/PKG-INFO` & `slurminade-1.1.1/src/slurminade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 1.1.0
+Version: 1.1.1
 Summary: A decorator-based slurm runner.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/slurminade
 Project-URL: Issues, https://github.com/d-krupke/slurminade/issues
 Keywords: slurm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -372,14 +372,15 @@
 -  guard.py: Contains code to prevent you accidentally DDoSing your
    infrastructure.
 -  options.py: Contains a simple data structure to save slurm options.
 
 Changes
 -------
 
+- 1.1.1: Fixing bug when there is some output to stdout when loading the code, such as deprecation warnings.
 - 1.1.0: Slurminade can now be called from iPython, too! `exec` has been renamed `shell` to prevent confusion with the Python call `exec` which will evaluate a string as Python code.
 - 1.0.1: Dispatcher now return jobs references instead of job ids. This allows to do some fancier stuff in the future, when the jobs infos are only available a short time after the job has been submitted.
 - 0.10.1: FIX: Listing functions will no longer execute setup functions.
 -  0.10.0: `Batch` is now named `JobBundling`. There is a method `join` for easier synchronization. `exec` allows to executed commands just like `srun` and `sbatch`, but uniform syntax with other slurmified functions. Functions can now also be called with `distribute_and_wait`. If you call `python3 -m slurminade.check --partition YOUR_PARTITION --constraint YOUR_CONSTRAINT` you can check if your slurm configuration is running correctly.
 -  0.9.0: Lots of improvements.
 -  0.8.1: Bugfix and automatic detection of wrong usage when using ``Batch`` with ``wait_for``.
 -  0.8.0: Added extensive logging and improved typing.
```

### Comparing `slurminade-1.1.0/src/slurminade.egg-info/SOURCES.txt` & `slurminade-1.1.1/src/slurminade.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 src/slurminade.egg-info/PKG-INFO
 src/slurminade.egg-info/SOURCES.txt
 src/slurminade.egg-info/dependency_links.txt
 src/slurminade.egg-info/requires.txt
 src/slurminade.egg-info/top_level.txt
 tests/__init__.py
 tests/test_create_command.py
+tests/test_create_command_with_noise.py
 tests/test_dispatch_guard.py
 tests/test_local.py
 tests/test_local_function.py
 tests/test_node_setup.py
 tests/test_subprocess.py
```

### Comparing `slurminade-1.1.0/tests/test_create_command.py` & `slurminade-1.1.1/tests/test_create_command.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/tests/test_dispatch_guard.py` & `slurminade-1.1.1/tests/test_dispatch_guard.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/tests/test_local.py` & `slurminade-1.1.1/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/tests/test_node_setup.py` & `slurminade-1.1.1/tests/test_node_setup.py`

 * *Files identical despite different names*

### Comparing `slurminade-1.1.0/tests/test_subprocess.py` & `slurminade-1.1.1/tests/test_subprocess.py`

 * *Files identical despite different names*

