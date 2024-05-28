# Comparing `tmp/pytket_phir-0.7.1.tar.gz` & `tmp/pytket_phir-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket_phir-0.7.1.tar", last modified: Fri Apr 12 17:26:14 2024, max compression
+gzip compressed data, was "pytket_phir-0.7.2.tar", last modified: Tue May 28 12:17:10 2024, max compression
```

## Comparing `pytket_phir-0.7.1.tar` & `pytket_phir-0.7.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/pre-commit-au.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.rebasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.sharding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/pytket/phir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/phirgen_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/place_and_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/qtm_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/pytket/phir/rebasing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/rebasing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/rebasing/rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/pytket/phir/sharding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/shard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/shards2ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/pytket_phir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/tests/data/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/arbitrary_qreg_names.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/baby.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/baby_with_rollup.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/barrier_complex.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/big_gate.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/bv_n10.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/classical_hazards.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/classical_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_barrier.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_classical.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/exec_order_two_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/eztest.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/group_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/n10_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/oned_brickwork_circuit_n20.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/parallelization_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/qv20_0.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/rxrz.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/rz_exec_order_three_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/simple.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/simple_cond.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/single_qubit_parallel_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/sleep.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/tk2_diff_angles.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/tk2_same_angle.qasm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/tests/data/wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/wasm/add.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/wasm/testfile.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_parallel_tk2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_parallelization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_wasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.245024 pytket_phir-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.229024 pytket_phir-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.229024 pytket_phir-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.229024 pytket_phir-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/workflows/pre-commit-au.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-28 12:17:10.241024 pytket_phir-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.229024 pytket_phir-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.229024 pytket_phir-0.7.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/pytket.phir.rebasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/pytket.phir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/docs/source/pytket.phir.sharding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.225024 pytket_phir-0.7.2/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.233024 pytket_phir-0.7.2/pytket/phir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18886 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/phirgen_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/place_and_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/qtm_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.233024 pytket_phir-0.7.2/pytket/phir/rebasing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/rebasing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/rebasing/rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.233024 pytket_phir-0.7.2/pytket/phir/sharding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/sharding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/sharding/shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/sharding/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/pytket/phir/sharding/shards2ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.241024 pytket_phir-0.7.2/pytket_phir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 12:17:10.000000 pytket_phir-0.7.2/pytket_phir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:17:10.245024 pytket_phir-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.237024 pytket_phir-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.225024 pytket_phir-0.7.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.241024 pytket_phir-0.7.2/tests/data/qasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/arbitrary_qreg_names.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/baby.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/baby_with_rollup.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/barrier_complex.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/big_gate.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/bv_n10.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/classical_hazards.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/classical_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/cond_1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/cond_barrier.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/cond_classical.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/exec_order_two_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/eztest.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/group_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/n10_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/oned_brickwork_circuit_n20.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/parallelization_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/qv20_0.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/rxrz.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/rz_exec_order_three_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/simple.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/simple_cond.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/single_qubit_parallel_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/sleep.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/tk2_diff_angles.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/qasm/tk2_same_angle.qasm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:17:10.241024 pytket_phir-0.7.2/tests/data/wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/wasm/add.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/data/wasm/testfile.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_parallel_tk2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_parallelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-28 12:16:57.000000 pytket_phir-0.7.2/tests/test_wasm.py
```

### Comparing `pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pytket_phir-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/.github/pull_request_template.md` & `pytket_phir-0.7.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/.github/workflows/pre-commit-au.yml` & `pytket_phir-0.7.2/.github/workflows/pre-commit-au.yml`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/.github/workflows/python-app.yml` & `pytket_phir-0.7.2/.github/workflows/python-app.yml`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,14 @@
     - name: Run tests
       run: |
         python -m pytest
     - name: Sphinx documentation build
       run: |
         make docs
     - name: Deploy to GitHub Pages
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' && matrix.deploy-gh-pages }}
       with:
         publish_branch: gh-pages
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: docs/build/html/
         force_orphan: true
```

### Comparing `pytket_phir-0.7.1/.github/workflows/python-publish.yml` & `pytket_phir-0.7.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/.gitignore` & `pytket_phir-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/CHANGELOG.md` & `pytket_phir-0.7.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/LICENSE` & `pytket_phir-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/PKG-INFO` & `pytket_phir-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.7.1
+Version: 0.7.2
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket_phir-0.7.1/README.md` & `pytket_phir-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/docs/Makefile` & `pytket_phir-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/docs/source/conf.py` & `pytket_phir-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/docs/source/index.rst` & `pytket_phir-0.7.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/docs/source/pytket.phir.rst` & `pytket_phir-0.7.2/docs/source/pytket.phir.rst`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/docs/source/pytket.phir.sharding.rst` & `pytket_phir-0.7.2/docs/source/pytket.phir.sharding.rst`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pyproject.toml` & `pytket_phir-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/api.py` & `pytket_phir-0.7.2/pytket/phir/api.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/cli.py` & `pytket_phir-0.7.2/pytket/phir/cli.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/machine.py` & `pytket_phir-0.7.2/pytket/phir/machine.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/phirgen.py` & `pytket_phir-0.7.2/pytket/phir/phirgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,22 @@
     return {
         "cop": "=",
         "returns": lhs,
         "args": rhs,
     }
 
 
-def classical_op(exp: LogicExp, *, bitwise: bool = False) -> JsonDict:
+def classical_op(exp: LogicExp, *, bitwise: bool = False) -> JsonDict | int:
     """PHIR for classical register operations."""
     match exp.op:
+        # Nullary
+        case BitWiseOp.ZERO:
+            return 0
+        case BitWiseOp.ONE:
+            return 1
         # Bitwise
         case RegWiseOp.AND | BitWiseOp.AND:
             cop = "&"
         case RegWiseOp.OR | BitWiseOp.OR:
             cop = "|"
         case RegWiseOp.XOR | BitWiseOp.XOR:
             cop = "^"
```

### Comparing `pytket_phir-0.7.1/pytket/phir/phirgen_parallel.py` & `pytket_phir-0.7.2/pytket/phir/phirgen_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     # group numbers for each gate are incremented by 3 so they don't overlap
     # and different gate types don't go in the same group
     # RZ gates go in (mod 3)=0 groups, R1XY gates go in (mod 3)=1 groups,
     # and all other gates will go in (mod 3)=2 groups
     rz_group_number = -3  # set to 0 when first RZ gate is assigned (-3 + 3 = 0)
     r1xy_group_number = -2  # set to 1 when first R1XY gate is assigned (-2 + 3 = 1)
     other_group_number = -1  # set to 2 when first other gate is assigned (-1 + 3 = 2)
-    num_scs_per_qubit: dict["UnitID", int] = {}
+    num_scs_per_qubit: dict[UnitID, int] = {}
     group_exec_order: list[int] = []
 
     for qubit, cmds in sub_commands.items():
         num_scs_per_qubit[qubit] = len(cmds)
 
     max_len = max(num_scs_per_qubit.values())
 
@@ -127,22 +127,22 @@
 
     return dict(groups.items())
 
 
 def groups2qops(groups: dict[int, list[tk.Command]], ops: list["JsonDict"]) -> None:  # noqa: PLR0912
     """Convert the groups of parallel ops to properly formatted PHIR."""
     for group in groups.values():
-        angles2qops: dict[tuple[sympy.Expr | float, ...], "JsonDict"] = {}
+        angles2qops: dict[tuple[sympy.Expr | float, ...], JsonDict] = {}
         for qop in group:
             if not qop.op.is_gate():
                 append_cmd(qop, ops)
             else:
                 angles = qop.op.params
                 if tuple(angles) not in angles2qops:
-                    fmt_qop: "JsonDict" = {
+                    fmt_qop: JsonDict = {
                         "qop": tket_gate_to_phir[qop.op.type],
                         "angles": [angles, "pi"],
                     }
                     if len(qop.qubits) == 1:
                         fmt_qop["args"] = [arg_to_bit(qop.qubits[0])]
                     else:
                         arg = [arg_to_bit(a) for a in qop.qubits]
@@ -155,15 +155,15 @@
                     else:
                         arg = [arg_to_bit(a) for a in qop.qubits]
                         fmt_qop["args"].append(arg)
         # in the case where the qop is not a gate (a conditional for example)
         # this branch is skipped because non-gate sub-commands
         # are always the only member of their group (see process_sub_commands)
         if len(angles2qops) > 1:
-            pll_block: "JsonDict" = {"block": "qparallel", "ops": []}
+            pll_block: JsonDict = {"block": "qparallel", "ops": []}
             for phir_qop in angles2qops.values():
                 pll_block["ops"].append(phir_qop)
             comment = {"//": f"Parallel {tket_gate_to_phir[qop.op.type]}"}
             ops.extend((comment, pll_block))
         else:
             for phir_qop in angles2qops.values():
                 if len(phir_qop["args"]) > 1:
@@ -252,27 +252,27 @@
             gate_type = tket_gate_to_phir[group[0].primary_command.op.type]
             # for init, just append normally
             if gate_type == "Init":
                 for shard in group:
                     append_cmd(shard.primary_command, ops)
             # for measure, format and include "returns"
             elif gate_type == "Measure":
-                fmt_measure: "JsonDict" = {
+                fmt_measure: JsonDict = {
                     "qop": "Measure",
                     "args": [],
                     "returns": [],
                 }
                 for shard in group:
                     pc = shard.primary_command
                     fmt_measure["args"].append(arg_to_bit(pc.args[0]))
                     fmt_measure["returns"].append(arg_to_bit(pc.bits[0]))
                 ops.append(fmt_measure)
             # all other gates, treat as standard qops
             else:
-                fmt_qop: "JsonDict" = {"qop": gate_type, "args": []}
+                fmt_qop: JsonDict = {"qop": gate_type, "args": []}
                 for shard in group:
                     pc = shard.primary_command
                     fmt_qop["args"].append(arg_to_bit(pc.args[0]))
                 ops.append(fmt_qop)
         else:
             fmt_g2q: dict[int, list[tk.Command]] = {0: []}
             for shard in group:
@@ -321,15 +321,15 @@
         machine: a QTM machine on which to simulate the circuit
     """
     max_parallel_tq_gates = len(machine.tq_options) // 2
     max_parallel_sq_gates = len(machine.sq_options) // 2
 
     phir = PHIR_HEADER
     phir["metadata"]["strict_parallelism"] = True
-    ops: list["JsonDict"] = []
+    ops: list[JsonDict] = []
 
     qbits = set()
     cbits = set()
     for _orders, shard_layer, layer_cost in inp:
         # within each shard layer, create groups of parallelizable shards
         # squash all the sub-commands into the first shard in the group
         shard_groups = process_shards(
```

### Comparing `pytket_phir-0.7.1/pytket/phir/place_and_route.py` & `pytket_phir-0.7.2/pytket/phir/place_and_route.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/placement.py` & `pytket_phir-0.7.2/pytket/phir/placement.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/qtm_machine.py` & `pytket_phir-0.7.2/pytket/phir/qtm_machine.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/rebasing/rebaser.py` & `pytket_phir-0.7.2/pytket/phir/rebasing/rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/routing.py` & `pytket_phir-0.7.2/pytket/phir/routing.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/sharding/shard.py` & `pytket_phir-0.7.2/pytket/phir/sharding/shard.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/sharding/sharder.py` & `pytket_phir-0.7.2/pytket/phir/sharding/sharder.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/pytket/phir/sharding/shards2ops.py` & `pytket_phir-0.7.2/pytket/phir/sharding/shards2ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ) -> tuple[list[Layer], list["ShardLayer"]]:
     """Parse a set of shards and return a circuit representation for placement."""
     layers: list[Layer] = []
     shards_in_layer: list[ShardLayer] = []
     scheduled: set[int] = set()
     num_shards: int = len(shards)
     qid_count: int = 0
-    qubits2ids: dict["UnitID", int] = {}
+    qubits2ids: dict[UnitID, int] = {}
 
     while len(scheduled) < num_shards:
         layer: Layer = []
 
         # Iterate the shards, looking for shards whose dependencies have been
         # satisfied, or initially, shards with no dependencies
         to_schedule: ShardLayer = [
```

### Comparing `pytket_phir-0.7.1/pytket_phir.egg-info/PKG-INFO` & `pytket_phir-0.7.2/pytket_phir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.7.1
+Version: 0.7.2
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket_phir-0.7.1/pytket_phir.egg-info/SOURCES.txt` & `pytket_phir-0.7.2/pytket_phir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/qasm/arbitrary_qreg_names.qasm` & `pytket_phir-0.7.2/tests/data/qasm/arbitrary_qreg_names.qasm`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/qasm/bv_n10.qasm` & `pytket_phir-0.7.2/tests/data/qasm/bv_n10.qasm`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/qasm/oned_brickwork_circuit_n20.qasm` & `pytket_phir-0.7.2/tests/data/qasm/oned_brickwork_circuit_n20.qasm`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/qasm/qv20_0.qasm` & `pytket_phir-0.7.2/tests/data/qasm/qv20_0.qasm`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/wasm/add.wat` & `pytket_phir-0.7.2/tests/data/wasm/add.wat`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/data/wasm/testfile.wat` & `pytket_phir-0.7.2/tests/data/wasm/testfile.wat`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/e2e_test.py` & `pytket_phir-0.7.2/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_api.py` & `pytket_phir-0.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_parallel_tk2.py` & `pytket_phir-0.7.2/tests/test_parallel_tk2.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_parallelization.py` & `pytket_phir-0.7.2/tests/test_parallelization.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_phirgen.py` & `pytket_phir-0.7.2/tests/test_phirgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ##############################################################################
 
 # mypy: disable-error-code="misc"
 
 import json
 
 from pytket.circuit import Bit, Circuit
+from pytket.circuit.logic_exp import BitWiseOp, create_bit_logic_exp
 from pytket.phir.api import pytket_to_phir
 from pytket.qasm.qasm import circuit_from_qasm_str
 from pytket.unit_id import BitRegister
 
 from .test_utils import QasmFile, get_qasm_as_circuit
 
 
@@ -427,7 +428,37 @@
             {
                 "cop": "=",
                 "returns": [["c", 1]],
                 "args": [{"cop": "&", "args": [["b", 1], ["c", 0]]}],
             },
         ],
     }
+
+
+def test_nullary_ops() -> None:
+    """From https://github.com/CQCL/pytket-phir/issues/178 ."""
+    c = Circuit(1, 1)
+    exp1 = create_bit_logic_exp(BitWiseOp.ONE, [])
+    c.H(0, condition=exp1)
+    exp0 = create_bit_logic_exp(BitWiseOp.ZERO, [])
+    c.H(0, condition=exp0)
+    c.measure_all()
+    phir = json.loads(pytket_to_phir(c))
+
+    assert phir["ops"][4] == {
+        "cop": "=",
+        "returns": [["tk_SCRATCH_BIT", 0]],
+        "args": [1],
+    }
+    assert phir["ops"][6] == {
+        "cop": "=",
+        "returns": [["tk_SCRATCH_BIT", 1]],
+        "args": [0],
+    }
+    assert phir["ops"][8]["condition"] == {
+        "cop": "==",
+        "args": [["tk_SCRATCH_BIT", 0], 1],
+    }
+    assert phir["ops"][10]["condition"] == {
+        "cop": "==",
+        "args": [["tk_SCRATCH_BIT", 1], 1],  # evals to False
+    }
```

### Comparing `pytket_phir-0.7.1/tests/test_placement.py` & `pytket_phir-0.7.2/tests/test_placement.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_rebaser.py` & `pytket_phir-0.7.2/tests/test_rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_sharder.py` & `pytket_phir-0.7.2/tests/test_sharder.py`

 * *Files identical despite different names*

### Comparing `pytket_phir-0.7.1/tests/test_utils.py` & `pytket_phir-0.7.2/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,8 +84,10 @@
     placed = place_and_route(shards, machine)
     return json.loads(genphir_parallel(placed, machine))  # type: ignore[misc, no-any-return]
 
 
 def get_wat_as_wasm_bytes(wat_file: WatFile) -> bytes:
     """Gets a given wat file, converted to WASM bytes by wasmtime."""
     this_dir = Path(Path(__file__).resolve()).parent
-    return wat2wasm(Path(f"{this_dir}/data/wasm/{wat_file.name}.wat").read_text())
+    return wat2wasm(
+        Path(f"{this_dir}/data/wasm/{wat_file.name}.wat").read_text(encoding="utf-8")
+    )
```

### Comparing `pytket_phir-0.7.1/tests/test_wasm.py` & `pytket_phir-0.7.2/tests/test_wasm.py`

 * *Files identical despite different names*

