# Comparing `tmp/pytest_cleanslate-1.0.2.tar.gz` & `tmp/pytest_cleanslate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_cleanslate-1.0.2.tar", last modified: Mon May 20 01:29:40 2024, max compression
+gzip compressed data, was "pytest_cleanslate-1.0.3.tar", last modified: Tue May 28 19:49:40 2024, max compression
```

## Comparing `pytest_cleanslate-1.0.2.tar` & `pytest_cleanslate-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.610946 pytest_cleanslate-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/src/pytest_cleanslate/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/tests/test_cleanslate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.843793 pytest_cleanslate-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.843793 pytest_cleanslate-1.0.3/src/pytest_cleanslate/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/tests/test_cleanslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/tests/test_reduce.py
```

### Comparing `pytest_cleanslate-1.0.2/LICENSE` & `pytest_cleanslate-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.2/PKG-INFO` & `pytest_cleanslate-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
 Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
 
-# pytest-cleanslate: work around test state pollution
+# pytest-cleanslate: work around or find test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
 ![pyversions](https://img.shields.io/pypi/pyversions/pytest-cleanslate?logo=python&logoColor=FBE072)
 ![tests](https://github.com/plasma-umass/pytest-cleanslate/workflows/tests/badge.svg)
@@ -32,24 +32,29 @@
 ## About
 pytest-cleanslate is a small plugin for the [pytest](https://github.com/pytest-dev/pytest)
 test framework which, as the name implies, helps give each test module a "clean slate" to execute.
 Plugins such as [pytest-forked](https://github.com/pytest-dev/pytest-forked) and
 [pytest-isolate](https://github.com/gilfree/pytest-isolate) allow you to execute tests
 in separate processes, working around in-memory test "state pollution" resulting from
 their execution, but do not protect against pollution caused by top-level code in test
-modules. This is what pytest-CleanSlate remedies.
+modules; this is what pytest-cleanslate remedies.
+
+This module also includes `cleanslate-reduce`, a tool for finding where the state pollution
+is occurring.
+Invoked on a test suite with a failing test, `cleanslate-reduce` looks for a smaller
+set of test modules and functions that still lead to the test failure.
 
 ## How to use
-After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` invocation.
+After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` command line (or configuration options).
 
 ## Interaction with other plugins
-This plugin implies the use of `pytest-forked`, i.e., it is as though you installed that
+Running with `--cleanslate` also makes use of `pytest-forked`, i.e., it is as though you installed that
 plugin and passed in `--forked` to execute all tests in separate processes.
 
-This plugin subverts somewhat `pytest`'s mode of operation in that it postpones collecting
+It also subverts somewhat `pytest`'s mode of operation in that it postpones collecting
 test items within test modules (i.e., within Python test files) until the test execution phase.
 While we have attempted to stay as compatible with other plugins as possible, it is likely
 to not work in some combinations (such as, for example, [pytest-xdist](https://github.com/pytest-dev/pytest-xdist)).
 Feel free to [open an issue](https://github.com/plasma-umass/pytest-cleanslate/issues) if you come across a case where it doesn't work.
 
 ## Requirements
 Python 3.8+, Linux or MacOS.
```

### Comparing `pytest_cleanslate-1.0.2/README.md` & `pytest_cleanslate-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pytest-cleanslate: work around test state pollution
+# pytest-cleanslate: work around or find test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
 ![pyversions](https://img.shields.io/pypi/pyversions/pytest-cleanslate?logo=python&logoColor=FBE072)
 ![tests](https://github.com/plasma-umass/pytest-cleanslate/workflows/tests/badge.svg)
@@ -11,24 +11,29 @@
 ## About
 pytest-cleanslate is a small plugin for the [pytest](https://github.com/pytest-dev/pytest)
 test framework which, as the name implies, helps give each test module a "clean slate" to execute.
 Plugins such as [pytest-forked](https://github.com/pytest-dev/pytest-forked) and
 [pytest-isolate](https://github.com/gilfree/pytest-isolate) allow you to execute tests
 in separate processes, working around in-memory test "state pollution" resulting from
 their execution, but do not protect against pollution caused by top-level code in test
-modules. This is what pytest-CleanSlate remedies.
+modules; this is what pytest-cleanslate remedies.
+
+This module also includes `cleanslate-reduce`, a tool for finding where the state pollution
+is occurring.
+Invoked on a test suite with a failing test, `cleanslate-reduce` looks for a smaller
+set of test modules and functions that still lead to the test failure.
 
 ## How to use
-After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` invocation.
+After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` command line (or configuration options).
 
 ## Interaction with other plugins
-This plugin implies the use of `pytest-forked`, i.e., it is as though you installed that
+Running with `--cleanslate` also makes use of `pytest-forked`, i.e., it is as though you installed that
 plugin and passed in `--forked` to execute all tests in separate processes.
 
-This plugin subverts somewhat `pytest`'s mode of operation in that it postpones collecting
+It also subverts somewhat `pytest`'s mode of operation in that it postpones collecting
 test items within test modules (i.e., within Python test files) until the test execution phase.
 While we have attempted to stay as compatible with other plugins as possible, it is likely
 to not work in some combinations (such as, for example, [pytest-xdist](https://github.com/pytest-dev/pytest-xdist)).
 Feel free to [open an issue](https://github.com/plasma-umass/pytest-cleanslate/issues) if you come across a case where it doesn't work.
 
 ## Requirements
 Python 3.8+, Linux or MacOS.
```

### Comparing `pytest_cleanslate-1.0.2/pyproject.toml` & `pytest_cleanslate-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-cleanslate"
-version = "1.0.2"
+dynamic = ["version"]
 description = "Collects and executes pytest tests separately"
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -25,12 +25,26 @@
 
 [project.urls]
 "Repository" = "https://github.com/plasma-umass/pytest_cleanslate"
 
 [project.entry-points.pytest11]
 pytest_cleanslate = "pytest_cleanslate.plugin"
 
+[project.scripts]
+cleanslate-reduce = "pytest_cleanslate.reduce:main"
+
+[build-system]
+requires = [
+    "setuptools>=61",
+    "wheel",
+    "pytest",
+]
+
+build-backend = "setuptools.build_meta"
+[tool.setuptools.dynamic]
+version = {attr = "pytest_cleanslate.__version__"}
+
 [tool.pytest.ini_options]
 required_plugins = [
     'pytest-cleanslate',    # must be installed to test
     'pytest-asyncio',       # required by tests
 ]
```

### Comparing `pytest_cleanslate-1.0.2/src/pytest_cleanslate/plugin.py` & `pytest_cleanslate-1.0.3/src/pytest_cleanslate/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/PKG-INFO` & `pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
 Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
 
-# pytest-cleanslate: work around test state pollution
+# pytest-cleanslate: work around or find test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
 ![pyversions](https://img.shields.io/pypi/pyversions/pytest-cleanslate?logo=python&logoColor=FBE072)
 ![tests](https://github.com/plasma-umass/pytest-cleanslate/workflows/tests/badge.svg)
@@ -32,24 +32,29 @@
 ## About
 pytest-cleanslate is a small plugin for the [pytest](https://github.com/pytest-dev/pytest)
 test framework which, as the name implies, helps give each test module a "clean slate" to execute.
 Plugins such as [pytest-forked](https://github.com/pytest-dev/pytest-forked) and
 [pytest-isolate](https://github.com/gilfree/pytest-isolate) allow you to execute tests
 in separate processes, working around in-memory test "state pollution" resulting from
 their execution, but do not protect against pollution caused by top-level code in test
-modules. This is what pytest-CleanSlate remedies.
+modules; this is what pytest-cleanslate remedies.
+
+This module also includes `cleanslate-reduce`, a tool for finding where the state pollution
+is occurring.
+Invoked on a test suite with a failing test, `cleanslate-reduce` looks for a smaller
+set of test modules and functions that still lead to the test failure.
 
 ## How to use
-After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` invocation.
+After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` command line (or configuration options).
 
 ## Interaction with other plugins
-This plugin implies the use of `pytest-forked`, i.e., it is as though you installed that
+Running with `--cleanslate` also makes use of `pytest-forked`, i.e., it is as though you installed that
 plugin and passed in `--forked` to execute all tests in separate processes.
 
-This plugin subverts somewhat `pytest`'s mode of operation in that it postpones collecting
+It also subverts somewhat `pytest`'s mode of operation in that it postpones collecting
 test items within test modules (i.e., within Python test files) until the test execution phase.
 While we have attempted to stay as compatible with other plugins as possible, it is likely
 to not work in some combinations (such as, for example, [pytest-xdist](https://github.com/pytest-dev/pytest-xdist)).
 Feel free to [open an issue](https://github.com/plasma-umass/pytest-cleanslate/issues) if you come across a case where it doesn't work.
 
 ## Requirements
 Python 3.8+, Linux or MacOS.
```

### Comparing `pytest_cleanslate-1.0.2/tests/test_cleanslate.py` & `pytest_cleanslate-1.0.3/tests/test_cleanslate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,142 @@
 import pytest
 import sys
 import subprocess
 from pathlib import Path
 import json
+import random
+from textwrap import dedent
 
 pytestmark = pytest.mark.skipif(sys.platform == 'win32', reason='Unix-only')
 
 
 def seq2p(tests_dir, seq):
-    return tests_dir / f"test_{seq}.py"
+    return tests_dir / f"test_{seq:02}.py"
 
 
 FAILURES = {
     'assert': 'assert False',
     'exception': 'raise RuntimeError("test")',
     'kill': 'os.kill(os.getpid(), 9)',
     'exit': 'pytest.exit("goodbye")',
     'interrupt': 'raise KeyboardInterrupt()'
 }
 
-N_TESTS=10
-def make_polluted_suite(tests_dir: Path, fail_collect: bool, fail_kind: str):
-    """In a suite with 10 tests, test 6 fails; test 3 doesn't fail, but causes 6 to fail."""
-
-    for seq in range(N_TESTS):
-        seq2p(tests_dir, seq).write_text('def test_foo(): pass')
-
-    polluter = seq2p(tests_dir, 3)
-    polluter.write_text("import sys\n" + "sys.foobar = True\n" + "def test_foo(): pass")
-
-    failing = seq2p(tests_dir, 6)
-    failing.write_text(f"""\
-import sys
-import os
-import pytest
-
-def failure():
-    {FAILURES[fail_kind]}
+def make_polluted_suite(tests_dir: Path, *, pollute_in_collect: bool = True, fail_collect: bool = False,
+                        fail_kind: str = 'assert'):
+    """in a suite with 10 tests, 'polluter' doesn't fail, but causes 'failing' to fail."""
+    tests = list(range(10))
+
+    # note the polluter must run before the failing test
+
+    polluter_seq = tests.pop(random.choice(tests[:-1]))
+    polluter = seq2p(tests_dir, polluter_seq)
+    if pollute_in_collect:
+        polluter.write_text(dedent("""\
+            import sys
+            sys.foobar=True
+
+            def test_bar():
+                assert True
+            """))
+    else:
+        polluter.write_text(dedent("""\
+            import sys
 
-def test_foo():
-    if getattr(sys, 'foobar', False):
-        failure()
+            def test_polluter():
+                sys.foobar=True
+                assert True
+
+            def test_bar():
+                assert True
+            """))
+        polluter = f"{polluter}::test_polluter"
+
+    failing = seq2p(tests_dir, tests.pop(random.choice(range(polluter_seq, len(tests)))))
+    if fail_collect:
+        failing.write_text(dedent(f"""\
+            import sys
+            import os
+            import pytest
+
+            if getattr(sys, 'foobar', False):
+                {FAILURES[fail_kind]}
+
+            def test_ok():
+                assert True
+            """))
+    else:
+        failing.write_text(dedent(f"""\
+            import sys
+            import os
+            import pytest
+
+            def test_failing():
+                if getattr(sys, 'foobar', False):
+                    {FAILURES[fail_kind]}
+
+            def test_ok():
+                assert True
+            """))
+        failing = f"{failing}::test_failing"
 
-{'test_foo()' if fail_collect else ''}
-""")
+    for seq in tests:
+        seq2p(tests_dir, seq).write_text('def test_foo(): pass')
 
-    return failing, polluter
+    return str(failing), str(polluter), tests
 
 
 @pytest.fixture
 def tests_dir(tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
     tests_dir = Path('tests')
     tests_dir.mkdir()
     yield tests_dir
 
 
-@pytest.mark.parametrize("fail_collect", [True, False])
+@pytest.mark.parametrize("pollute_in_collect, fail_collect", [[False, False], [True, False], [True, True]])
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys() - {'kill'}))
-def test_check_suite_fails(tests_dir, fail_collect, fail_kind):
-    make_polluted_suite(tests_dir, fail_collect, fail_kind)
+def test_check_suite_fails(tests_dir, pollute_in_collect, fail_collect, fail_kind):
+    make_polluted_suite(tests_dir, pollute_in_collect=pollute_in_collect,
+                        fail_collect=fail_collect, fail_kind=fail_kind)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', tests_dir], check=False)
     if fail_collect or fail_kind in ('exit', 'interrupt'):
         assert p.returncode == pytest.ExitCode.INTERRUPTED
     else:
         assert p.returncode == pytest.ExitCode.TESTS_FAILED
 
 
 @pytest.mark.parametrize("plugin", ['asyncio', 'no:asyncio'])
-@pytest.mark.parametrize("fail_collect", [True, False])
+@pytest.mark.parametrize("pollute_in_collect, fail_collect", [[False, False], [True, False], [True, True]])
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
-def test_isolate_polluted(tests_dir, fail_collect, fail_kind, plugin):
-    make_polluted_suite(tests_dir, fail_collect, fail_kind)
+def test_isolate_polluted(tests_dir, pollute_in_collect, fail_collect, fail_kind, plugin):
+    make_polluted_suite(tests_dir, pollute_in_collect=pollute_in_collect,
+                        fail_collect=fail_collect, fail_kind=fail_kind)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', '-p', plugin, '--cleanslate', tests_dir], check=False)
     assert p.returncode == pytest.ExitCode.OK
 
 
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
 def test_pytest_discover_tests(tests_dir, fail_kind):
     make_polluted_suite(tests_dir, fail_collect=False, fail_kind=fail_kind)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate'], check=False) # no tests_dir here
     assert p.returncode == pytest.ExitCode.OK
 
 
-@pytest.mark.parametrize("fail_collect", [True, False])
+@pytest.mark.parametrize("pollute_in_collect, fail_collect", [[False, False], [True, False], [True, True]])
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
-def test_unconditionally_failing_test(tests_dir, fail_collect, fail_kind):
-    make_polluted_suite(tests_dir, fail_collect, fail_kind)
+def test_unconditionally_failing_test(tests_dir, pollute_in_collect, fail_collect, fail_kind):
+    _, _, tests = make_polluted_suite(tests_dir, pollute_in_collect=pollute_in_collect,
+                                      fail_collect=fail_collect, fail_kind=fail_kind)
 
     # _unconditionally_ failing test
-    failing = seq2p(tests_dir, 2)
+    failing = seq2p(tests_dir, random.choice(tests))
     failing.write_text(f"""\
 import sys
 import os
 import pytest
 
 def failure():
     {FAILURES[fail_kind]}
```

