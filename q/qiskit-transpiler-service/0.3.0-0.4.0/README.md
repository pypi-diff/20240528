# Comparing `tmp/qiskit-transpiler-service-0.3.0.tar.gz` & `tmp/qiskit_transpiler_service-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-transpiler-service-0.3.0.tar", last modified: Thu Feb 29 16:39:11 2024, max compression
+gzip compressed data, was "qiskit_transpiler_service-0.4.0.tar", last modified: Tue May 28 13:15:06 2024, max compression
```

## Comparing `qiskit-transpiler-service-0.3.0.tar` & `qiskit_transpiler_service-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-02-29 16:39:11.858183 qiskit-transpiler-service-0.3.0/
--rw-r--r--   0 juancb     (501) staff       (20)    10314 2024-02-29 16:39:11.857446 qiskit-transpiler-service-0.3.0/PKG-INFO
--rw-r--r--   0 juancb     (501) staff       (20)     8840 2024-02-29 16:37:47.000000 qiskit-transpiler-service-0.3.0/README.md
-drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-02-29 16:39:11.847160 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/
--rw-r--r--   0 juancb     (501) staff       (20)      629 2023-12-11 12:59:15.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/__init__.py
-drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-02-29 16:39:11.854763 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/
--rw-r--r--   0 juancb     (501) staff       (20)      522 2023-12-11 12:59:15.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/__init__.py
--rw-r--r--   0 juancb     (501) staff       (20)     9452 2024-02-22 10:49:32.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/collection.py
--rw-r--r--   0 juancb     (501) staff       (20)     6247 2024-02-22 10:49:32.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/routing.py
--rw-r--r--   0 juancb     (501) staff       (20)     1789 2024-02-12 15:49:06.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/routing_service_wrapper.py
--rw-r--r--   0 juancb     (501) staff       (20)     5222 2023-12-04 00:25:15.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/service_wrapper.py
--rw-r--r--   0 juancb     (501) staff       (20)     5200 2024-02-22 10:49:32.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/synthesis.py
--rw-r--r--   0 juancb     (501) staff       (20)     3810 2024-02-12 15:49:06.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/synthesis_service_wrappers.py
--rw-r--r--   0 juancb     (501) staff       (20)     2522 2024-02-29 16:18:25.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/transpiler_service.py
--rw-r--r--   0 juancb     (501) staff       (20)     4892 2024-02-12 15:49:06.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/transpiler_service_api.py
--rw-r--r--   0 juancb     (501) staff       (20)     1277 2023-12-04 00:25:15.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/utils.py
-drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-02-29 16:39:11.856558 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/
--rw-r--r--   0 juancb     (501) staff       (20)    10314 2024-02-29 16:39:11.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/PKG-INFO
--rw-r--r--   0 juancb     (501) staff       (20)      797 2024-02-29 16:39:11.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/SOURCES.txt
--rw-r--r--   0 juancb     (501) staff       (20)        1 2024-02-29 16:39:11.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/dependency_links.txt
--rw-r--r--   0 juancb     (501) staff       (20)       73 2024-02-29 16:39:11.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/requires.txt
--rw-r--r--   0 juancb     (501) staff       (20)       26 2024-02-29 16:39:11.000000 qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/top_level.txt
--rw-r--r--   0 juancb     (501) staff       (20)       38 2024-02-29 16:39:11.858301 qiskit-transpiler-service-0.3.0/setup.cfg
--rw-r--r--   0 juancb     (501) staff       (20)     2616 2024-02-29 16:37:47.000000 qiskit-transpiler-service-0.3.0/setup.py
-drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-02-29 16:39:11.855466 qiskit-transpiler-service-0.3.0/tests/
--rw-r--r--   0 juancb     (501) staff       (20)     4503 2024-02-29 16:18:25.000000 qiskit-transpiler-service-0.3.0/tests/test_transpiler_service.py
+drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-05-28 13:15:06.044882 qiskit_transpiler_service-0.4.0/
+-rw-r--r--   0 juancb     (501) staff       (20)    11937 2024-05-28 13:15:06.044028 qiskit_transpiler_service-0.4.0/PKG-INFO
+-rw-r--r--   0 juancb     (501) staff       (20)    10467 2024-05-16 23:41:53.000000 qiskit_transpiler_service-0.4.0/README.md
+drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-05-28 13:15:06.034987 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/
+-rw-r--r--   0 juancb     (501) staff       (20)      629 2023-12-11 12:59:15.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/__init__.py
+drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-05-28 13:15:06.041556 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/
+-rw-r--r--   0 juancb     (501) staff       (20)     1194 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/__init__.py
+-rw-r--r--   0 juancb     (501) staff       (20)    12401 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/collection.py
+-rw-r--r--   0 juancb     (501) staff       (20)     7336 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/routing.py
+-rw-r--r--   0 juancb     (501) staff       (20)     1813 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/routing_service_wrapper.py
+-rw-r--r--   0 juancb     (501) staff       (20)     5294 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/service_wrapper.py
+-rw-r--r--   0 juancb     (501) staff       (20)     7623 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/synthesis.py
+-rw-r--r--   0 juancb     (501) staff       (20)     4536 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/synthesis_service_wrappers.py
+-rw-r--r--   0 juancb     (501) staff       (20)     4370 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/transpiler_service.py
+-rw-r--r--   0 juancb     (501) staff       (20)     4899 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/transpiler_service_api.py
+-rw-r--r--   0 juancb     (501) staff       (20)     1686 2024-05-16 23:41:53.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/utils.py
+drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-05-28 13:15:06.042970 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/
+-rw-r--r--   0 juancb     (501) staff       (20)    11937 2024-05-28 13:15:06.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/PKG-INFO
+-rw-r--r--   0 juancb     (501) staff       (20)      797 2024-05-28 13:15:06.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/SOURCES.txt
+-rw-r--r--   0 juancb     (501) staff       (20)        1 2024-05-28 13:15:06.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/dependency_links.txt
+-rw-r--r--   0 juancb     (501) staff       (20)       69 2024-05-28 13:15:06.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/requires.txt
+-rw-r--r--   0 juancb     (501) staff       (20)       26 2024-05-28 13:15:06.000000 qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/top_level.txt
+-rw-r--r--   0 juancb     (501) staff       (20)       38 2024-05-28 13:15:06.044992 qiskit_transpiler_service-0.4.0/setup.cfg
+-rw-r--r--   0 juancb     (501) staff       (20)     2612 2024-05-28 13:11:51.000000 qiskit_transpiler_service-0.4.0/setup.py
+drwxr-xr-x   0 juancb     (501) staff       (20)        0 2024-05-28 13:15:06.042065 qiskit_transpiler_service-0.4.0/tests/
+-rw-r--r--   0 juancb     (501) staff       (20)     4515 2024-05-28 09:59:20.000000 qiskit_transpiler_service-0.4.0/tests/test_transpiler_service.py
```

### Comparing `qiskit-transpiler-service-0.3.0/PKG-INFO` & `qiskit_transpiler_service-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-transpiler-service
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library to use Qiskit Transpiler service(https://docs.quantum.ibm.com/transpile/qiskit-transpiler-service) and the AI transpiler passes(https://docs.quantum.ibm.com/transpile/ai-transpiler-passes)
 Home-page: https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service
 Author: Data & Intelligence team, IBM Quantum
 Author-email: 
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service/issues
 Project-URL: Documentation, https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service
@@ -19,17 +19,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: qiskit==1.0.0
+Requires-Dist: qiskit~=1.0
 Requires-Dist: backoff==2.2.1
-Requires-Dist: qiskit-qasm3-import==0.4.1
+Requires-Dist: qiskit-qasm3-import~=0.4
 Requires-Dist: requests==2.31.0
 
 # qiskit_transpiler_service
 
 A library to use [Qiskit Transpiler service](https://docs.quantum.ibm.com/transpile/qiskit-transpiler-service) and the [AI transpiler passes](https://docs.quantum.ibm.com/transpile/ai-transpiler-passes).
 
 **Note** The Qiskit transpiler service and the AI transpiler passes use different experimental services that are only available for IBM Quantum Premium Plan users. This library and the releated services are an alpha release, subject to change.
@@ -157,7 +157,50 @@
 To complement the synthesis passes we also provide custom collection passes for Cliffords, Linear Functions and Permutations that can be imported from `qiskit_transpiler_service.ai.collection`:
 
 - *CollectCliffords*: Collects Clifford blocks as `Instruction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectLinearFunctions*: Collects blocks of `SWAP` and `CX` as `LinearFunction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectPermutations*: Collects blocks of `SWAP` circuits as `Permutations`.
 
 These custom collection passes limit the sizes of the collected sub-circuits so that they are supported by the AI synthesis passes, so it is recommended to use them after the routing passes and before the synthesis passes to get a better optimization overall.
+
+## Contributing
+
+### Documentation
+
+**Write**
+
+We use Sphinx to compile docstrings into API documentation. The docstrings are written in reStructuredText. See our [Sphinx guide](https://qiskit.github.io/qiskit_sphinx_theme/sphinx_guide/index.html) for more information on writing Sphinx documentation.
+
+If you want an object to appear in the API documentation, you'll need to add it to the autosummary of the appropriate module-level docstring. For example, the [`qiskit_transpiler_service.ai`](./qiskit_transpiler_service/ai/__init__.py) module contains the following autosummary.
+
+```rst
+Classes
+=======
+.. autosummary::
+   :toctree: ../stubs/
+
+   AIRouting
+```
+
+Functions should be inlined in the module's file, e.g. `utils.py`:
+
+```rst
+.. currentmodule:: qiskit_transpiler_service.utils
+
+Functions
+=========
+
+.. autofunction:: create_random_linear_function
+.. autofunction:: get_metrics
+```
+
+When adding a new module, you'll also need to add a new file to `docs/apidocs`. The file name should match the module's name, e.g. `my_module.submodule.rst`. You'll probably find it easiest to copy one of the existing files. You also need to update `apidocs/index.rst` with the new file name.
+
+**Build**
+
+To build the documentation, install Sphinx and the `qiskit-sphinx-theme` (both included in `requirements-dev.txt`) then run the following command.
+
+```
+make docs
+```
+
+To view the documentation open `docs/_build/html/index.html`. Note that this is just a preview, the final documentation content is pulled into [Qiskit/documentation](https://github.com/qiskit/documentation) and re-rendered into https://docs.quantum.ibm.com.
```

### Comparing `qiskit-transpiler-service-0.3.0/README.md` & `qiskit_transpiler_service-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -127,7 +127,50 @@
 To complement the synthesis passes we also provide custom collection passes for Cliffords, Linear Functions and Permutations that can be imported from `qiskit_transpiler_service.ai.collection`:
 
 - *CollectCliffords*: Collects Clifford blocks as `Instruction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectLinearFunctions*: Collects blocks of `SWAP` and `CX` as `LinearFunction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectPermutations*: Collects blocks of `SWAP` circuits as `Permutations`.
 
 These custom collection passes limit the sizes of the collected sub-circuits so that they are supported by the AI synthesis passes, so it is recommended to use them after the routing passes and before the synthesis passes to get a better optimization overall.
+
+## Contributing
+
+### Documentation
+
+**Write**
+
+We use Sphinx to compile docstrings into API documentation. The docstrings are written in reStructuredText. See our [Sphinx guide](https://qiskit.github.io/qiskit_sphinx_theme/sphinx_guide/index.html) for more information on writing Sphinx documentation.
+
+If you want an object to appear in the API documentation, you'll need to add it to the autosummary of the appropriate module-level docstring. For example, the [`qiskit_transpiler_service.ai`](./qiskit_transpiler_service/ai/__init__.py) module contains the following autosummary.
+
+```rst
+Classes
+=======
+.. autosummary::
+   :toctree: ../stubs/
+
+   AIRouting
+```
+
+Functions should be inlined in the module's file, e.g. `utils.py`:
+
+```rst
+.. currentmodule:: qiskit_transpiler_service.utils
+
+Functions
+=========
+
+.. autofunction:: create_random_linear_function
+.. autofunction:: get_metrics
+```
+
+When adding a new module, you'll also need to add a new file to `docs/apidocs`. The file name should match the module's name, e.g. `my_module.submodule.rst`. You'll probably find it easiest to copy one of the existing files. You also need to update `apidocs/index.rst` with the new file name.
+
+**Build**
+
+To build the documentation, install Sphinx and the `qiskit-sphinx-theme` (both included in `requirements-dev.txt`) then run the following command.
+
+```
+make docs
+```
+
+To view the documentation open `docs/_build/html/index.html`. Note that this is just a preview, the final documentation content is pulled into [Qiskit/documentation](https://github.com/qiskit/documentation) and re-rendered into https://docs.quantum.ibm.com.
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/__init__.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/collection.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 # that they have been altered from the originals.
 
 
 """Replace each sequence of Clifford gates by a single Clifford gate."""
 
 from functools import partial
 
+from qiskit import QuantumCircuit
 from qiskit.circuit import Instruction
 from qiskit.circuit.library import LinearFunction, PermutationGate
+from qiskit.converters import circuit_to_dag, dag_to_dagdependency, dagdependency_to_dag
+from qiskit.dagcircuit.dagcircuit import DAGCircuit
 from qiskit.quantum_info.operators import Clifford
+from qiskit.transpiler.basepasses import TransformationPass
 from qiskit.transpiler.passes.optimization.collect_and_collapse import (
     CollectAndCollapse,
     collapse_to_operation,
 )
 from qiskit.transpiler.passes.utils import control_flow
-from qiskit.converters import dag_to_dagdependency, dagdependency_to_dag
-from qiskit.transpiler.basepasses import TransformationPass
-from qiskit.dagcircuit.dagcircuit import DAGCircuit
-from qiskit.converters import circuit_to_dag
-from qiskit import QuantumCircuit
 
 CLIFFORD_MAX_BLOCK_SIZE = 9
 LINEAR_MAX_BLOCK_SIZE = 9
 PERMUTATION_MAX_BLOCK_SIZE = 12
 
 
 clifford_gate_names = [
@@ -216,15 +215,29 @@
         if self.do_commutative_analysis:
             dag = dagdependency_to_dag(dag)
 
         return dag
 
 
 class CollectCliffords(RepeatedCollectAndCollapse):
-    """Collects blocks of Clifford gates"""
+    """CollectCliffords(do_commutative_analysis: bool = True, min_block_size: int = 2, max_block_size: int = CLIFFORD_MAX_BLOCK_SIZE, collect_from_back: bool = False, num_reps: int = 10)
+
+    Collects Clifford blocks as `Instruction` objects and stores the original sub-circuit to compare against it after synthesis.
+
+    :param do_commutative_analysis: Enable or disable commutative analysis, defaults to True
+    :type do_commutative_analysis: bool, optional
+    :param min_block_size: Set the minimum size for blocks generated during the collect Cliffords pass, defaults to 2.
+    :type min_block_size: int, optional
+    :param max_block_size: Set the maximum size for blocks generated during the collect Cliffords pass, defaults to 9.
+    :type max_block_size: int, optional
+    :param collect_from_back: Specify if collect blocks in reverse order or not, defaults to False.
+    :type collect_from_back: bool, optional
+    :param num_reps: Specify how many times to repeat the optimization process, defaults to 10.
+    :type num_reps: int, optional
+    """
 
     def __init__(
         self,
         do_commutative_analysis=True,
         min_block_size=2,
         max_block_size=CLIFFORD_MAX_BLOCK_SIZE,
         collect_from_back=False,
@@ -242,15 +255,29 @@
             split_layers=False,
             collect_from_back=collect_from_back,
             num_reps=num_reps,
         )
 
 
 class CollectLinearFunctions(RepeatedCollectAndCollapse):
-    """Collects Linear Function blocks, containing Cnot and Swap gates"""
+    """CollectLinearFunctions(do_commutative_analysis: bool = True, min_block_size: int = 4, max_block_size: int = LINEAR_MAX_BLOCK_SIZE, collect_from_back: bool = False, num_reps: int = 10)
+
+    Collects blocks of `SWAP` and `CX` as `LinearFunction` objects and stores the original sub-circuit to compare against it after synthesis.
+
+    :param do_commutative_analysis: Enable or disable commutative analysis, defaults to True
+    :type do_commutative_analysis: bool, optional
+    :param min_block_size: Set the minimum size for blocks generated during the collect linear functions pass, defaults to 4.
+    :type min_block_size: int, optional
+    :param max_block_size: Set the maximum size for blocks generated during the collect linear functions pass, defaults to 9.
+    :type max_block_size: int, optional
+    :param collect_from_back: Specify if collect blocks in reverse order or not, defaults to False.
+    :type collect_from_back: bool, optional
+    :param num_reps: Specify how many times to repeat the optimization process, defaults to 10.
+    :type num_reps: int, optional
+    """
 
     def __init__(
         self,
         do_commutative_analysis=True,
         min_block_size=4,
         max_block_size=LINEAR_MAX_BLOCK_SIZE,
         collect_from_back=False,
@@ -268,15 +295,29 @@
             split_layers=False,
             collect_from_back=collect_from_back,
             num_reps=num_reps,
         )
 
 
 class CollectPermutations(RepeatedCollectAndCollapse):
-    """Collects Permutation blocks containing Swap gates"""
+    """CollectPermutations(do_commutative_analysis: bool = True, min_block_size: int = 4, max_block_size: int = PERMUTATION_MAX_BLOCK_SIZE, collect_from_back: bool = False, num_reps: int = 10)
+
+    Collects blocks of `SWAP` circuits as `Permutations`.
+
+    :param do_commutative_analysis: Enable or disable commutative analysis, defaults to True
+    :type do_commutative_analysis: bool, optional
+    :param min_block_size: Set the minimum size for blocks generated during the collect permutations pass, defaults to 4.
+    :type min_block_size: int, optional
+    :param max_block_size: Set the maximum size for blocks generated during the collect permutations pass, defaults to 12.
+    :type max_block_size: int, optional
+    :param collect_from_back: Specify if collect blocks in reverse order or not, defaults to False.
+    :type collect_from_back: bool, optional
+    :param num_reps: Specify how many times to repeat the optimization process, defaults to 10.
+    :type num_reps: int, optional
+    """
 
     def __init__(
         self,
         do_commutative_analysis=True,
         min_block_size=4,
         max_block_size=PERMUTATION_MAX_BLOCK_SIZE,
         collect_from_back=False,
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/routing.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/routing.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,25 +16,40 @@
 # torch.set_num_threads(1)
 
 import logging
 
 import numpy as np
 from qiskit import ClassicalRegister, QuantumCircuit
 from qiskit.converters import circuit_to_dag, dag_to_circuit
-from qiskit.transpiler import TranspilerError, CouplingMap
+from qiskit.transpiler import CouplingMap, TranspilerError
 from qiskit.transpiler.basepasses import TransformationPass
 from qiskit.transpiler.layout import Layout
 
 from .routing_service_wrapper import AIRoutingService
 
 logging.basicConfig()
-logging.getLogger().setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 class AIRouting(TransformationPass):
+    """AIRouting(backend_name: str | None = None, coupling_map: list[list[int]] | None = None, optimization_level: int = 2, layout_mode: str = "OPTIMIZE")
+
+    The `AIRouting` pass acts both as a layout stage and a routing stage.
+
+    :param backend_name: Name of the backend used for doing the transpilation.
+    :type backend_name: str, optional
+    :param coupling_map: A list of pairs that represents physical links between qubits.
+    :type coupling_map: list[list[int]], optional
+    :param optimization_level: With a range from 1 to 3, determines the computational effort to spend in the process (higher usually gives better results but takes longer), defaults to 2.
+    :type optimization_level: int
+    :param layout_mode: Specifies how to handle the layout selection. There are 3 layout modes: keep (respects the layout set by the previous transpiler passes), improve (uses the layout set by the previous transpiler passes as a starting point) and optimize (ignores previous layout selections), defaults to `OPTIMIZE`.
+    :type layout_mode: str
+    """
+
     def __init__(
         self,
         backend_name=None,
         coupling_map=None,
         optimization_level: int = 2,
         layout_mode: str = "OPTIMIZE",
     ):
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/routing_service_wrapper.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/routing_service_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from qiskit import QuantumCircuit, qasm2, qasm3
 from qiskit.qasm2 import QASM2ExportError
 
 from .service_wrapper import AIService
 
 logging.basicConfig()
-logging.getLogger().setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 class AIRoutingService(AIService):
     """A helper class that covers some basic funcionality from the AIRouting plugin"""
 
     def __init__(self, url: str = None, token: str = None):
         if url is None:
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/service_wrapper.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/service_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from pathlib import Path
 
 import backoff
 import requests
 from qiskit.transpiler.exceptions import TranspilerError
 
 logging.basicConfig()
-logging.getLogger().setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 class BackendTaskError(Exception):
     def __init__(self, status: str, msg: str):
         self.status = status
         self.msg = msg
 
@@ -23,15 +24,15 @@
     token = os.environ.get("QISKIT_IBM_TOKEN")
 
     if not token:
         with open(Path.home() / ".qiskit" / "qiskit-ibm.json", "r") as _sc:
             creds = json.loads(_sc.read())
         token = creds.get("default-ibm-quantum", {}).get("token")
         if token is None:
-            logging.warning("The token is undefined")
+            logger.warning("The token is undefined")
     return token
 
 
 class AIService:
     """A helper class that covers some common basic funcionality AIServices"""
 
     def __init__(self, url: str = None, token: str = None):
@@ -41,17 +42,18 @@
         # If it couldn't find it, it fails
 
         self.url = url.rstrip("/")
 
         token = token if token else _get_token_from_system()
 
         self.headers = {
-            "accept": "application/json",
+            "Accept": "application/json",
             "Authorization": f"Bearer {token}",
             "Content-Type": "application/json",
+            "X-Caller": "qiskit-transpiler-service",
         }
 
     def get_versions(self):
         url = f"{self.url}/version"
         resp = requests.get(
             url,
             headers=self.headers,
@@ -81,15 +83,15 @@
             requests.exceptions.Timeout,
             requests.exceptions.ConnectionError,
             requests.exceptions.JSONDecodeError,
         ),
         max_time=120,  # TODO: Define by config or circuit?
     )
     def request_status(self, endpoint, task_id):
-        logging.info(f"Getting status of task {task_id} ...")
+        logger.info(f"Getting status of task {task_id} ...")
         res = requests.get(url=f"{self.url}/{endpoint}/{task_id}", headers=self.headers)
         res.raise_for_status()
         return res.json()
 
     def request_and_wait(self, endpoint: str, body: dict, params: dict):
         try:
             return self._request_and_wait(endpoint, body, params)
@@ -116,29 +118,29 @@
             status="PENDING", msg=f"The background task {task_id} timed out"
         )
 
         resp = self.request_status(endpoint, task_id)
         if resp.get("state") == "SUCCESS":
             result = resp.get("result")
         elif resp.get("state") == "FAILURE":
-            logging.error("The request FAILED")
+            logger.error("The request FAILED")
             result = BackendTaskError(
                 status="FAILURE", msg=f"The background task {task_id} FAILED"
             )
 
         if isinstance(result, BackendTaskError):
             # TODO: Shall we show this  "The background task 99cf52d2-3942-4ae5-b2a7-d672af7f1216 FAILED" to the user?
-            logging.error(f"Failed to get a result for {endpoint}: {result.msg}")
+            logger.error(f"Failed to get a result for {endpoint}: {result.msg}")
             raise result
         else:
             return result
 
 
 def _raise_transpiler_error_and_log(msg: str):
-    logging.error(msg)
+    logger.error(msg)
     raise TranspilerError(msg)
 
 
 def _get_error_msg_from_response(exc: requests.exceptions.HTTPError):
     if exc.response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY.value:
         # Default message
         msg = "Internal error."
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/ai/synthesis_service_wrappers.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/ai/synthesis_service_wrappers.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,45 +18,56 @@
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import LinearFunction
 from qiskit.quantum_info import Clifford
 
 from .service_wrapper import AIService
 
 logging.basicConfig()
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger(__name__).setLevel(logging.INFO)
 
 
 class CliffordAIService(AIService):
     """A helper class that covers some basic funcionality from the Clifford AI Synthesis service"""
 
     def __init__(self, url: str = None, token: str = None):
         # If it does not recive URL or token, the function tries to find your Qiskit
         # token from the QISKIT_IBM_TOKEN env var
         # If it couldn't find it, it will try to get it from your ~/.qiskit/qiskit-ibm.json file
         # If it couldn't find it, it fails
 
         if url is None:
             url = os.environ.get(
                 "CLIFFORDAI_URL",
-                "https://clifford-ai.quantum.ibm.com",
+                "https://cloud-transpiler.quantum.ibm.com/clifford/",
             )
 
         super().__init__(url, token)
 
     def transpile(
-        self, circuit: Union[QuantumCircuit, Clifford], backend: str, qargs: list[int]
+        self,
+        circuits: list[Union[QuantumCircuit, Clifford]],
+        backend: str,
+        qargs: list[list[int]],
     ):
-        transpile_resp = self.request_and_wait(
+        transpile_resps = self.request_and_wait(
             endpoint="transpile",
-            body={"clifford_dict": Clifford(circuit).to_dict(), "qargs": qargs},
+            body={
+                "clifford_dict": [Clifford(circuit).to_dict() for circuit in circuits],
+                "qargs": qargs,
+            },
             params={"backend": backend},
         )
 
-        if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
-            return QuantumCircuit.from_qasm_str(transpile_resp.get("qasm"))
+        results = []
+        for transpile_resp in transpile_resps:
+            if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
+                results.append(QuantumCircuit.from_qasm_str(transpile_resp.get("qasm")))
+            else:
+                results.append(None)
+        return results
 
 
 class LinearFunctionAIService(AIService):
     """A helper class that covers some basic funcionality from the Linear Function AI Synthesis service"""
 
     def __init__(self, url: str = None, token: str = None):
         if url is None:
@@ -64,26 +75,34 @@
                 "LINEARFUNCTIONAI_URL",
                 "https://cloud-transpiler.quantum.ibm.com/linear_functions/",
             )
         super().__init__(url, token)
 
     def transpile(
         self,
-        circuit: Union[QuantumCircuit, LinearFunction],
+        circuits: list[Union[QuantumCircuit, LinearFunction]],
         backend: str,
-        qargs: list[int],
+        qargs: list[list[int]],
     ):
-        transpile_resp = self.request_and_wait(
+        transpile_resps = self.request_and_wait(
             endpoint="transpile",
-            body={"clifford_dict": Clifford(circuit).to_dict(), "qargs": qargs},
+            body={
+                "clifford_dict": [Clifford(circuit).to_dict() for circuit in circuits],
+                "qargs": qargs,
+            },
             params={"backend": backend},
         )
 
-        if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
-            return QuantumCircuit.from_qasm_str(transpile_resp.get("qasm"))
+        results = []
+        for transpile_resp in transpile_resps:
+            if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
+                results.append(QuantumCircuit.from_qasm_str(transpile_resp.get("qasm")))
+            else:
+                results.append(None)
+        return results
 
 
 class PermutationAIService(AIService):
     """A helper class that covers some basic funcionality from the Permutation AI Synthesis service"""
 
     def __init__(self, url: str = None, token: str = None):
         if url is None:
@@ -92,19 +111,24 @@
                 "https://cloud-transpiler.quantum.ibm.com/permutations/",
             )
 
         super().__init__(url, token)
 
     def transpile(
         self,
-        pattern: list[int],
+        patterns: list[list[int]],
         backend: str,
-        qargs: list[int],
+        qargs: list[list[int]],
     ):
-        transpile_resp = self.request_and_wait(
+        transpile_resps = self.request_and_wait(
             endpoint="transpile",
-            body={"permutation": pattern, "qargs": qargs},
+            body={"permutation": patterns, "qargs": qargs},
             params={"backend": backend},
         )
 
-        if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
-            return QuantumCircuit.from_qasm_str(transpile_resp.get("qasm"))
+        results = []
+        for transpile_resp in transpile_resps:
+            if transpile_resp.get("success") and transpile_resp.get("qasm") is not None:
+                results.append(QuantumCircuit.from_qasm_str(transpile_resp.get("qasm")))
+            else:
+                results.append(None)
+        return results
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/transpiler_service_api.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/transpiler_service_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from qiskit.qasm2 import QASM2ExportError, QASM2ParseError
 from qiskit.transpiler import TranspileLayout
 from qiskit.transpiler.layout import Layout
 
 from qiskit_transpiler_service.ai.service_wrapper import AIService
 
 logging.basicConfig()
-logging.getLogger().setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 class BackendTaskError(Exception):
     def __init__(self, status: str, msg: str):
         self.status = status
         self.msg = msg
 
@@ -63,29 +64,29 @@
             json_args["qiskit_transpile_options"] = qiskit_transpile_options
         if coupling_map is not None:
             json_args["backend_coupling_map"] = coupling_map
 
         params = {
             "backend": backend,
             "optimization_level": optimization_level,
-            "use_ai": ai,
+            "ai": ai,
         }
 
         if ai_layout_mode is not None:
             params["ai_layout_mode"] = ai_layout_mode
 
         transpile_resp = self.request_and_wait(
             endpoint="transpile", body=json_args, params=params
         )
 
-        logging.info(f"transpile_resp={transpile_resp}")
+        logger.info(f"transpile_resp={transpile_resp}")
 
         transpiled_circuits = []
         for res in transpile_resp:
-            transpiled_circuits.append(_get_circuit_from_result(res, params["use_ai"]))
+            transpiled_circuits.append(_get_circuit_from_result(res, params["ai"]))
         return (
             transpiled_circuits
             if len(transpiled_circuits) > 1
             else transpiled_circuits[0]
         )
 
     def benchmark(
@@ -109,29 +110,29 @@
     elif isinstance(input_circ, str):
         qasm = input_circ.replace("\n", " ")
     else:
         raise TypeError("Input circuits must be QuantumCircuit or qasm string.")
     return qasm
 
 
-def _get_circuit_from_result(transpile_resp, use_ai):
+def _get_circuit_from_result(transpile_resp, ai):
     try:
         transpiled_circuit = QuantumCircuit.from_qasm_str(transpile_resp["qasm"])
     except QASM2ParseError:
         transpiled_circuit = qasm3.loads(transpile_resp["qasm"])
 
     qubits = transpiled_circuit.qubits
     init_layout = transpile_resp["layout"]["initial"]
     final_layout = transpile_resp["layout"]["final"]
 
     full_initial_layout = init_layout + sorted(
         set(range(len(qubits))) - set(init_layout)
     )
     full_final_layout = final_layout + list(range(len(final_layout), len(init_layout)))
-    if use_ai:
+    if ai:
         full_final_layout = [
             full_final_layout[i] for i in np.argsort(full_initial_layout)
         ]
 
     initial_layout_qiskit = Layout(dict(zip(full_initial_layout, qubits)))
     final_layout_qiskit = Layout(dict(zip(full_final_layout, qubits)))
     input_qubit_mapping = {q: i for i, q in enumerate(qubits)}
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service/utils.py` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,30 @@
+"""
+===============================================================================
+Utilities (:mod:`qiskit_transpiler_service.utils`)
+===============================================================================
+
+.. currentmodule:: qiskit_transpiler_service.utils
+
+Functions
+=========
+
+.. autofunction:: create_random_linear_function
+.. autofunction:: get_metrics
+
+"""
+
 import numpy as np
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import LinearFunction
 from qiskit.quantum_info import Clifford
 from qiskit.synthesis.linear.linear_matrix_utils import random_invertible_binary_matrix
 
 
-def get_metrics(qc: QuantumCircuit):
+def get_metrics(qc: QuantumCircuit) -> dict[str, int]:
     """Returns a dict with metrics from a QuantumCircuit"""
     qcd = qc.decompose(reps=3)
     return {
         "n_gates": qcd.size(),
         "n_layers": qcd.depth(),
         "n_cnots": qcd.num_nonlocal_gates(),
         "n_layers_cnots": qcd.depth(lambda x: x[0].name == "cx"),
@@ -17,15 +32,15 @@
 
 
 def random_permutation(n_qubits):
     """Generate a random permutation of n_qubits qubits."""
     return np.random.permutation(n_qubits)
 
 
-def create_random_linear_function(n_qubits: int, seed: int = 123):
+def create_random_linear_function(n_qubits: int, seed: int = 123) -> LinearFunction:
     rand_lin = lambda seed: LinearFunction(
         random_invertible_binary_matrix(n_qubits, seed=seed)
     )
 
     return LinearFunction(rand_lin(seed))
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/PKG-INFO` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-transpiler-service
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library to use Qiskit Transpiler service(https://docs.quantum.ibm.com/transpile/qiskit-transpiler-service) and the AI transpiler passes(https://docs.quantum.ibm.com/transpile/ai-transpiler-passes)
 Home-page: https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service
 Author: Data & Intelligence team, IBM Quantum
 Author-email: 
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service/issues
 Project-URL: Documentation, https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service
@@ -19,17 +19,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: qiskit==1.0.0
+Requires-Dist: qiskit~=1.0
 Requires-Dist: backoff==2.2.1
-Requires-Dist: qiskit-qasm3-import==0.4.1
+Requires-Dist: qiskit-qasm3-import~=0.4
 Requires-Dist: requests==2.31.0
 
 # qiskit_transpiler_service
 
 A library to use [Qiskit Transpiler service](https://docs.quantum.ibm.com/transpile/qiskit-transpiler-service) and the [AI transpiler passes](https://docs.quantum.ibm.com/transpile/ai-transpiler-passes).
 
 **Note** The Qiskit transpiler service and the AI transpiler passes use different experimental services that are only available for IBM Quantum Premium Plan users. This library and the releated services are an alpha release, subject to change.
@@ -157,7 +157,50 @@
 To complement the synthesis passes we also provide custom collection passes for Cliffords, Linear Functions and Permutations that can be imported from `qiskit_transpiler_service.ai.collection`:
 
 - *CollectCliffords*: Collects Clifford blocks as `Instruction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectLinearFunctions*: Collects blocks of `SWAP` and `CX` as `LinearFunction` objects and stores the original sub-circuit to compare against it after synthesis.
 - *CollectPermutations*: Collects blocks of `SWAP` circuits as `Permutations`.
 
 These custom collection passes limit the sizes of the collected sub-circuits so that they are supported by the AI synthesis passes, so it is recommended to use them after the routing passes and before the synthesis passes to get a better optimization overall.
+
+## Contributing
+
+### Documentation
+
+**Write**
+
+We use Sphinx to compile docstrings into API documentation. The docstrings are written in reStructuredText. See our [Sphinx guide](https://qiskit.github.io/qiskit_sphinx_theme/sphinx_guide/index.html) for more information on writing Sphinx documentation.
+
+If you want an object to appear in the API documentation, you'll need to add it to the autosummary of the appropriate module-level docstring. For example, the [`qiskit_transpiler_service.ai`](./qiskit_transpiler_service/ai/__init__.py) module contains the following autosummary.
+
+```rst
+Classes
+=======
+.. autosummary::
+   :toctree: ../stubs/
+
+   AIRouting
+```
+
+Functions should be inlined in the module's file, e.g. `utils.py`:
+
+```rst
+.. currentmodule:: qiskit_transpiler_service.utils
+
+Functions
+=========
+
+.. autofunction:: create_random_linear_function
+.. autofunction:: get_metrics
+```
+
+When adding a new module, you'll also need to add a new file to `docs/apidocs`. The file name should match the module's name, e.g. `my_module.submodule.rst`. You'll probably find it easiest to copy one of the existing files. You also need to update `apidocs/index.rst` with the new file name.
+
+**Build**
+
+To build the documentation, install Sphinx and the `qiskit-sphinx-theme` (both included in `requirements-dev.txt`) then run the following command.
+
+```
+make docs
+```
+
+To view the documentation open `docs/_build/html/index.html`. Note that this is just a preview, the final documentation content is pulled into [Qiskit/documentation](https://github.com/qiskit/documentation) and re-rendered into https://docs.quantum.ibm.com.
```

### Comparing `qiskit-transpiler-service-0.3.0/qiskit_transpiler_service.egg-info/SOURCES.txt` & `qiskit_transpiler_service-0.4.0/qiskit_transpiler_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-transpiler-service-0.3.0/setup.py` & `qiskit_transpiler_service-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 # NOTE: The lists below require each requirement on a separate line,
 # putting multiple requirements on the same line will prevent qiskit-bot
 # from correctly updating the versions for the qiskit packages.
 requirements = [
-    "qiskit==1.0.0",
+    "qiskit~=1.0",
     "backoff==2.2.1",
-    "qiskit-qasm3-import==0.4.1",
+    "qiskit-qasm3-import~=0.4",
     "requests==2.31.0",
 ]
 
 setup(
     name="qiskit-transpiler-service",
-    version="0.3.0",
+    version="0.4.0",
     description="A library to use Qiskit Transpiler service(https://docs.quantum.ibm.com/transpile/qiskit-transpiler-service) and the AI transpiler passes(https://docs.quantum.ibm.com/transpile/ai-transpiler-passes)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.ibm.com/IBM-Q-Software/qiskit-transpiler-service",
     author="Data & Intelligence team, IBM Quantum",
     author_email="",
     license="Apache 2.0",
```

### Comparing `qiskit-transpiler-service-0.3.0/tests/test_transpiler_service.py` & `qiskit_transpiler_service-0.4.0/tests/test_transpiler_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 import pytest
 from qiskit import QuantumCircuit, qasm2
 from qiskit.circuit.library import QuantumVolume
 from qiskit.circuit.random import random_circuit
 
 from qiskit_transpiler_service.transpiler_service import TranspilerService
 
-logging.getLogger().setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 @pytest.mark.parametrize(
     "optimization_level", [1, 2, 3], ids=["opt_level_1", "opt_level_2", "opt_level_3"]
 )
-@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "use_ai"])
+@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "ai"])
 @pytest.mark.parametrize(
     "qiskit_transpile_options",
     [None, {"seed_transpiler": 0}],
     ids=["no opt", "one option"],
 )
 def test_rand_circ_backend_routing(optimization_level, ai, qiskit_transpile_options):
     backend_name = "ibm_brisbane"
@@ -47,15 +48,15 @@
 
     assert isinstance(transpiled_circuit, QuantumCircuit)
 
 
 @pytest.mark.parametrize(
     "optimization_level", [1, 2, 3], ids=["opt_level_1", "opt_level_2", "opt_level_3"]
 )
-@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "use_ai"])
+@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "ai"])
 @pytest.mark.parametrize(
     "qiskit_transpile_options",
     [None, {"seed_transpiler": 0}],
     ids=["no opt", "one option"],
 )
 def test_qv_backend_routing(optimization_level, ai, qiskit_transpile_options):
     backend_name = "ibm_brisbane"
@@ -76,15 +77,15 @@
     "coupling_map",
     [
         [[0, 1], [1, 2], [2, 3], [3, 4], [4, 5]],
         [[0, 1], [1, 2], [2, 3], [3, 4], [4, 5], [5, 6], [6, 7]],
     ],
 )
 @pytest.mark.parametrize("optimization_level", [1, 2, 3])
-@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "use_ai"])
+@pytest.mark.parametrize("ai", [False, True], ids=["no_ai", "ai"])
 @pytest.mark.parametrize("qiskit_transpile_options", [None, {"seed_transpiler": 0}])
 def test_rand_circ_cmap_routing(
     coupling_map, optimization_level, ai, qiskit_transpile_options
 ):
     random_circ = random_circuit(5, depth=3, seed=42).decompose(reps=3)
 
     cloud_transpiler_service = TranspilerService(
```

