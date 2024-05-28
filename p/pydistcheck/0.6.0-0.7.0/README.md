# Comparing `tmp/pydistcheck-0.6.0.tar.gz` & `tmp/pydistcheck-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydistcheck-0.6.0.tar", last modified: Sun Feb 18 06:01:24 2024, max compression
+gzip compressed data, was "pydistcheck-0.7.0.tar", last modified: Tue May 28 05:02:48 2024, max compression
```

## Comparing `pydistcheck-0.6.0.tar` & `pydistcheck-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.751654 pydistcheck-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.743654 pydistcheck-0.6.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/LICENSES/DELOCATE_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-02-18 06:01:24.751654 pydistcheck-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 06:01:24.751654 pydistcheck-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.743654 pydistcheck-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.747655 pydistcheck-0.6.0/src/pydistcheck/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/shared_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/src/pydistcheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.751654 pydistcheck-0.6.0/src/pydistcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-18 06:01:24.000000 pydistcheck-0.6.0/src/pydistcheck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 06:01:24.747655 pydistcheck-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21365 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-18 06:01:18.000000 pydistcheck-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.239986 pydistcheck-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.235986 pydistcheck-0.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/LICENSES/DELOCATE_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-28 05:02:48.239986 pydistcheck-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:02:48.239986 pydistcheck-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.235986 pydistcheck-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.235986 pydistcheck-0.7.0/src/pydistcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/shared_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/src/pydistcheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.239986 pydistcheck-0.7.0/src/pydistcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 05:02:48.000000 pydistcheck-0.7.0/src/pydistcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:02:48.239986 pydistcheck-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-28 05:02:45.000000 pydistcheck-0.7.0/tests/test_utils.py
```

### Comparing `pydistcheck-0.6.0/LICENSE` & `pydistcheck-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.6.0/LICENSES/DELOCATE_LICENSE` & `pydistcheck-0.7.0/LICENSES/DELOCATE_LICENSE`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.6.0/PKG-INFO` & `pydistcheck-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydistcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Inspect Python package distributions and raise warnings on common problems.
 Author-email: James Lamb <jaylamb20@gmail.com>
 Maintainer-email: James Lamb <jaylamb20@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, James Lamb
         All rights reserved.
@@ -94,20 +94,28 @@
 
 See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
 
 For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
-Install with `pipx`.
+Install with `pip`.
 
 ```shell
-pipx install pydistcheck
+pip install pydistcheck
 ```
 
+Or `conda`.
+
+```shell
+conda install -c conda-forge pydistcheck
+```
+
+For more details, see "Installation" ([link](./docs/installation.rst)).
+
 ## Quickstart
 
 Try it out on the test data in this project ...
 
 ```shell
 pydistcheck tests/data/problematic-package-*
 ```
```

### Comparing `pydistcheck-0.6.0/README.md` & `pydistcheck-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,28 @@
 
 See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
 
 For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
-Install with `pipx`.
+Install with `pip`.
 
 ```shell
-pipx install pydistcheck
+pip install pydistcheck
 ```
 
+Or `conda`.
+
+```shell
+conda install -c conda-forge pydistcheck
+```
+
+For more details, see "Installation" ([link](./docs/installation.rst)).
+
 ## Quickstart
 
 Try it out on the test data in this project ...
 
 ```shell
 pydistcheck tests/data/problematic-package-*
 ```
```

### Comparing `pydistcheck-0.6.0/pyproject.toml` & `pydistcheck-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -63,24 +63,22 @@
 [build-system]
 
 requires = [
     "setuptools>=67",
 ]
 build-backend = "setuptools.build_meta"
 
-[tool.black]
-line-length = 100
-
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.mypy]
 exclude = 'docs/conf\.py$|build/*'
 ignore_missing_imports = true
+mypy_path = "./src:./tests/data"
 strict = true
 
 [tool.ruff]
 # this should be set to the oldest version of python the project supports
 target-version = "py38"
 
 [tool.ruff.lint]
@@ -103,14 +101,16 @@
     "C4",
     # pycodestyle
     "E",
     # eradicate
     "ERA",
     # pyflakes
     "F",
+    # flynt
+    "FLY",
     # perflint
     "PERF",
     # pygrep-hooks
     "PGH",
     # pylint
     "PL",
     # flake8-pyi
@@ -132,13 +132,17 @@
 ]
 "src/pydistcheck/cli.py" = [
     # Too many branches
     "PLR0912",
     # Too many statements
     "PLR0915"
 ]
+"src/pydistcheck/distribution_summary.py" = [
+    # Too many branches
+    "PLR0912"
+]
 "tests/*" = [
     # (flake8-bugbear) Found useless expression
     "B018",
     # (flake8-bandit) use of assert detected
     "S101"
 ]
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/_compat.py` & `pydistcheck-0.7.0/src/pydistcheck/_compat.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.6.0/src/pydistcheck/checks.py` & `pydistcheck-0.7.0/src/pydistcheck/checks.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,50 +3,56 @@
 performs on distributions.
 """
 
 import os
 from collections import defaultdict
 from fnmatch import fnmatchcase
 from tempfile import TemporaryDirectory
-from typing import List, Protocol
+from typing import List, Protocol, Sequence
 
 from .distribution_summary import _DistributionSummary
 from .file_utils import _extract_subset_of_files_from_archive
 from .shared_lib_utils import _file_has_debug_symbols
 from .utils import _FileSize
 
 # ALL_CHECKS constant is used to validate configuration options like '--ignore' that reference
 # check names. It's a set literal so it doesn't need to be recomputed at runtime, and this project
 # relies on unit tests to ensure that it's updated as the list of checks changes.
 ALL_CHECKS = {
     "compiled-objects-have-debug-symbols",
     "distro-too-large-compressed",
     "distro-too-large-uncompressed",
+    "expected-files",
     "too-many-files",
     "files-only-differ-by-case",
     "mixed-file-extensions",
     "path-contains-non-ascii-characters",
     "path-contains-spaces",
+    "path-too-long",
     "unexpected-files",
 }
 
 
 class _CheckProtocol(Protocol):
     check_name: str
 
-    def __call__(self, distro_summary: _DistributionSummary) -> List[str]:  # pragma: no cover
+    def __call__(
+        self, distro_summary: _DistributionSummary
+    ) -> List[str]:  # pragma: no cover
         ...
 
 
 class _CompiledObjectsDebugSymbolCheck(_CheckProtocol):
     check_name = "compiled-objects-have-debug-symbols"
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
-        compiled_object_paths = [file_info.name for file_info in distro_summary.compiled_objects]
+        compiled_object_paths = [
+            file_info.name for file_info in distro_summary.compiled_objects
+        ]
         if not compiled_object_paths:
             return out
 
         with TemporaryDirectory() as tmp_dir:
             _extract_subset_of_files_from_archive(
                 archive_file=distro_summary.original_file,
                 archive_format=distro_summary.archive_format,
@@ -92,15 +98,17 @@
 
     def __init__(self, max_allowed_size_bytes: int):
         self.max_allowed_size_bytes = max_allowed_size_bytes
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
         max_size = _FileSize(num=self.max_allowed_size_bytes, unit_str="B")
-        actual_size = _FileSize(num=distro_summary.uncompressed_size_bytes, unit_str="B")
+        actual_size = _FileSize(
+            num=distro_summary.uncompressed_size_bytes, unit_str="B"
+        )
         if actual_size > max_size:
             msg = (
                 f"[{self.check_name}] Uncompressed size {actual_size} is larger "
                 f"than the allowed size ({max_size})."
             )
             out.append(msg)
         return out
@@ -151,15 +159,17 @@
 class _NonAsciiCharacterCheck(_CheckProtocol):
     check_name = "path-contains-non-ascii-characters"
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
         for file_path in distro_summary.all_paths:
             if not file_path.isascii():
-                ascii_converted_str = file_path.encode("ascii", "replace").decode("ascii")
+                ascii_converted_str = file_path.encode("ascii", "replace").decode(
+                    "ascii"
+                )
                 msg = (
                     f"[{self.check_name}] Found file path containing non-ASCII characters: "
                     f"'{ascii_converted_str}'"
                 )
                 out.append(msg)
         return out
 
@@ -190,45 +200,111 @@
                     f"[{self.check_name}] Found a mix of file extensions for "
                     f"the same file type: {count_str}"
                 )
                 out.append(msg)
         return out
 
 
+class _PathTooLongCheck(_CheckProtocol):
+    check_name = "path-too-long"
+
+    def __init__(self, max_path_length: int):
+        self.max_path_length = max_path_length
+
+    def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
+        out: List[str] = []
+        bad_paths = [
+            p for p in distro_summary.all_paths if len(p) > self.max_path_length
+        ]
+        for file_path in bad_paths:
+            msg = (
+                f"[{self.check_name}] Path too long ({len(file_path)} > {self.max_path_length}): "
+                f"'{file_path}'"
+            )
+            out.append(msg)
+        return out
+
+
 class _SpacesInPathCheck(_CheckProtocol):
     check_name = "path-contains-spaces"
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
         for file_path in distro_summary.all_paths:
             if file_path != file_path.replace(" ", ""):
                 msg = f"[{self.check_name}] Found path with spaces: '{file_path}'"
                 out.append(msg)
         return out
 
 
+class _ExpectedFilesCheck(_CheckProtocol):
+    check_name = "expected-files"
+
+    def __init__(
+        self,
+        directory_patterns: Sequence[str],
+        file_patterns: Sequence[str],
+    ):
+        self.directory_patterns = [
+            d for d in directory_patterns if not d.startswith("!")
+        ]
+        self.file_patterns = [f for f in file_patterns if not f.startswith("!")]
+
+    def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
+        out: List[str] = []
+        for pattern in self.file_patterns:
+            found_any = False
+            for file_path in distro_summary.file_paths:
+                if fnmatchcase(file_path, pattern):
+                    found_any = True
+                    break
+
+            if not found_any:
+                msg = f"[{self.check_name}] Did not find any files matching pattern '{pattern}'."
+                out.append(msg)
+
+        for pattern in self.directory_patterns:
+            found_any = False
+            for directory_path in distro_summary.directory_paths:
+                # NOTE: some archive formats have a trailing "/" on directory names,
+                #       some do not
+                if fnmatchcase(directory_path, pattern) or fnmatchcase(
+                    directory_path, pattern + "/"
+                ):
+                    found_any = True
+                    break
+            if not found_any:
+                msg = f"[{self.check_name}] Did not find any directories matching pattern '{pattern}'."
+                out.append(msg)
+        return out
+
+
 class _UnexpectedFilesCheck(_CheckProtocol):
     check_name = "unexpected-files"
 
     def __init__(
-        self, unexpected_directory_patterns: List[str], unexpected_file_patterns: List[str]
+        self,
+        directory_patterns: Sequence[str],
+        file_patterns: Sequence[str],
     ):
-        self.unexpected_directory_patterns = unexpected_directory_patterns
-        self.unexpected_file_patterns = unexpected_file_patterns
+        self.directory_patterns = [
+            d[1:] for d in directory_patterns if d.startswith("!")
+        ]
+        self.file_patterns = [f[1:] for f in file_patterns if f.startswith("!")]
 
     def __call__(self, distro_summary: _DistributionSummary) -> List[str]:
         out: List[str] = []
         for file_path in distro_summary.file_paths:
-            for pattern in self.unexpected_file_patterns:
+            for pattern in self.file_patterns:
                 if fnmatchcase(file_path, pattern):
                     msg = f"[{self.check_name}] Found unexpected file '{file_path}'."
                     out.append(msg)
 
         for directory_path in distro_summary.directory_paths:
-            for pattern in self.unexpected_directory_patterns:
+            for pattern in self.directory_patterns:
                 # NOTE: some archive formats have a trailing "/" on directory names,
                 #       some do not
                 if fnmatchcase(directory_path, pattern) or fnmatchcase(
                     directory_path, pattern + "/"
                 ):
                     msg = f"[{self.check_name}] Found unexpected directory '{directory_path}'."
                     out.append(msg)
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/cli.py` & `pydistcheck-0.7.0/src/pydistcheck/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 CLI entrypoints
 """
 
 import sys
-from typing import List
+from typing import List, Sequence
 
 import click
 
 from pydistcheck import __version__ as _VERSION
 
 from .checks import (
     ALL_CHECKS,
     _CompiledObjectsDebugSymbolCheck,
     _DistroTooLargeCompressedCheck,
     _DistroTooLargeUnCompressedCheck,
+    _ExpectedFilesCheck,
     _FileCountCheck,
     _FilesOnlyDifferByCaseCheck,
     _MixedFileExtensionCheck,
     _NonAsciiCharacterCheck,
+    _PathTooLongCheck,
     _SpacesInPathCheck,
     _UnexpectedFilesCheck,
 )
 from .config import _Config
 from .distribution_summary import _DistributionSummary
 from .inspect import inspect_distribution
 from .utils import _FileSize
@@ -29,121 +31,136 @@
 
 class ExitCodes:
     OK = 0
     CHECK_ERRORS = 1
     UNSUPPORTED_FILE_TYPE = 2
 
 
-@click.command()
-@click.argument(
+@click.command()  # type: ignore[misc]
+@click.argument(  # type: ignore[misc]
     "filepaths",
     type=click.Path(exists=True),
     nargs=-1,
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--version",
     is_flag=True,
     show_default=False,
     default=False,
     help="Print the version of pydistcheck and exit.",
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--config",
     type=click.Path(exists=True),
     default=None,
     help=(
         "Path to a TOML file containing a [tool.pydistcheck] table. "
         "If provided, pyproject.toml will be ignored."
     ),
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--ignore",
-    type=str,
+    multiple=True,
     default=_Config.ignore,
     help=(
-        "comma-separated list of checks to skip, e.g. "
-        "``distro-too-large-compressed,path-contains-spaces``."
+        "ID of a check to skip, e.g. 'compiled-objects-have-debug-symbols'. "
+        "See https://pydistcheck.readthedocs.io/en/docs-fix/check-reference.html for a "
+        "complete list of valid options. Can be passed multiple times."
     ),
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--inspect",
     is_flag=True,
     show_default=False,
     default=_Config.inspect,
-    help="print diagnostic information about the distribution",
+    help=(
+        "Print a summary of the distribution, like its total size and largest files."
+    ),
+)
+@click.option(  # type: ignore[misc]
+    "--expected-directories",
+    multiple=True,
+    default=_Config.expected_directories,
+    show_default=True,
+    help=(
+        "Pattern matching directories that are expected to be found in the distribution. "
+        "Prefix with '!' to indicate a pattern which should NOT match any of the distribution's "
+        "contents. Other than that possible leading '!', patterns should be in the format understood by "
+        "``fnmatch.fnmatchcase()`` (https://docs.python.org/3/library/fnmatch.html). "
+        "Can be passed multiple times."
+    ),
+)
+@click.option(  # type: ignore[misc]
+    "--expected-files",
+    multiple=True,
+    default=_Config.expected_files,
+    show_default=True,
+    help=(
+        "Pattern matching files that are expected to be found in the distribution. "
+        "Prefix with '!' to indicate a pattern which should NOT match any of the distribution's "
+        "contents. Other than that possible leading '!', patterns should be in the format understood by "
+        "``fnmatch.fnmatchcase()`` (https://docs.python.org/3/library/fnmatch.html). "
+        "Can be passed multiple times."
+    ),
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--max-allowed-files",
     default=_Config.max_allowed_files,
     show_default=True,
     type=int,
     help="maximum number of files allowed in the distribution",
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--max-allowed-size-compressed",
     default=_Config.max_allowed_size_compressed,
     show_default=True,
     type=str,
     help=(
         "maximum allowed compressed size, a string like '1.5M' indicating"
         " '1.5 megabytes'. Supported units:\n"
         "  - B = bytes\n"
         "  - K = kilobytes\n"
         "  - M = megabytes\n"
         "  - G = gigabytes"
     ),
 )
-@click.option(
+@click.option(  # type: ignore[misc]
     "--max-allowed-size-uncompressed",
     default=_Config.max_allowed_size_uncompressed,
     show_default=True,
     type=str,
     help=(
         "maximum allowed uncompressed size, a string like '1.5M' indicating"
         " '1.5 megabytes'. Supported units:\n"
         "  - B = bytes\n"
         "  - K = kilobytes\n"
         "  - M = megabytes\n"
         "  - G = gigabytes"
     ),
 )
-@click.option(
-    "--unexpected-directory-patterns",
-    default=_Config.unexpected_directory_patterns,
+@click.option(  # type: ignore[misc]
+    "--max-path-length",
+    default=_Config.max_path_length,
     show_default=True,
-    type=str,
-    help=(
-        "comma-delimited list of patterns matching directories that are not expected "
-        "to be found in the distribution. Patterns should be in the format understood "
-        "by ``fnmatch.fnmatchcase()``. See https://docs.python.org/3/library/fnmatch.html."
-    ),
-)
-@click.option(
-    "--unexpected-file-patterns",
-    default=_Config.unexpected_file_patterns,
-    show_default=True,
-    type=str,
-    help=(
-        "comma-delimited list of patterns matching files that are not expected "
-        "to be found in the distribution. Patterns should be in the format understood "
-        "by ``fnmatch.fnmatchcase()``. See https://docs.python.org/3/library/fnmatch.html."
-    ),
+    type=int,
+    help="Maximum allowed filepath length for files or directories in the distribution.",
 )
 def check(  # noqa: PLR0913
     *,
     filepaths: str,
     version: bool,
     config: str,
-    ignore: str,
+    expected_directories: Sequence[str],
+    expected_files: Sequence[str],
+    ignore: Sequence[str],
     inspect: bool,
     max_allowed_files: int,
     max_allowed_size_compressed: str,
     max_allowed_size_uncompressed: str,
-    unexpected_directory_patterns: str,
-    unexpected_file_patterns: str,
+    max_path_length: int,
 ) -> None:
     """
     Run the contents of a distribution through a set of checks, and warn about
     any problematic characteristics that are detected.
 
     Exit codes:
 
@@ -159,55 +176,63 @@
     conf = _Config()
     kwargs = {
         "ignore": ignore,
         "inspect": inspect,
         "max_allowed_files": max_allowed_files,
         "max_allowed_size_compressed": max_allowed_size_compressed,
         "max_allowed_size_uncompressed": max_allowed_size_uncompressed,
-        "unexpected_directory_patterns": unexpected_directory_patterns,
-        "unexpected_file_patterns": unexpected_file_patterns,
+        "max_path_length": max_path_length,
+        "expected_directories": expected_directories,
+        "expected_files": expected_files,
     }
     kwargs_that_differ_from_defaults = {}
     for k, v in kwargs.items():
         if v != getattr(conf, k):
             kwargs_that_differ_from_defaults[k] = v
     if config is not None:
         conf.update_from_toml(toml_file=click.format_filename(config))
     else:
         conf.update_from_toml(toml_file="pyproject.toml")
     conf.update_from_dict(input_dict=kwargs_that_differ_from_defaults)
 
-    checks_to_ignore = {x for x in conf.ignore.split(",") if x.strip()}
+    checks_to_ignore = {x for x in conf.ignore if x.strip()}
     unrecognized_checks = checks_to_ignore - ALL_CHECKS
     if unrecognized_checks:
         # converting to list + sorting here so outputs are deterministic
         # (since sets don't guarantee ordering)
         error_str = ",".join(sorted(unrecognized_checks))
-        print(f"ERROR: found the following unrecognized checks passed via '--ignore': {error_str}")
+        print(
+            f"ERROR: found the following unrecognized checks passed via '--ignore': {error_str}"
+        )
         sys.exit(1)
 
     checks = [
         _CompiledObjectsDebugSymbolCheck(),
         _DistroTooLargeCompressedCheck(
             max_allowed_size_bytes=_FileSize.from_string(
                 size_str=conf.max_allowed_size_compressed
             ).total_size_bytes
         ),
         _DistroTooLargeUnCompressedCheck(
             max_allowed_size_bytes=_FileSize.from_string(
                 size_str=conf.max_allowed_size_uncompressed
             ).total_size_bytes
         ),
+        _ExpectedFilesCheck(
+            directory_patterns=expected_directories,
+            file_patterns=expected_files,
+        ),
         _FileCountCheck(max_allowed_files=conf.max_allowed_files),
         _FilesOnlyDifferByCaseCheck(),
         _MixedFileExtensionCheck(),
+        _PathTooLongCheck(max_path_length=conf.max_path_length),
         _SpacesInPathCheck(),
         _UnexpectedFilesCheck(
-            unexpected_directory_patterns=unexpected_directory_patterns.split(","),
-            unexpected_file_patterns=unexpected_file_patterns.split(","),
+            directory_patterns=expected_directories,
+            file_patterns=expected_files,
         ),
         _NonAsciiCharacterCheck(),
     ]
 
     # filter out ignored checks
     checks = [c for c in checks if c.check_name not in checks_to_ignore]
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/config.py` & `pydistcheck-0.7.0/src/pydistcheck/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,81 +3,81 @@
 
   * validating configuration values
   * updating configuuration from files
 """
 
 import os
 from dataclasses import dataclass
-from typing import Any, Dict
+from typing import Any, Dict, Sequence
 
 from ._compat import tomllib
 
 # putting this in a module-level set to save on the cost of re-computing it inside methods
 # in `_Config` that validate configuration.
 #
 # unit tests confirm that it matches the `_Config` class, so it shouldn't ever drift from that class
 _ALLOWED_CONFIG_VALUES = {
+    "expected_directories",
+    "expected_files",
     "ignore",
     "inspect",
     "max_allowed_files",
     "max_allowed_size_compressed",
     "max_allowed_size_uncompressed",
-    "unexpected_directory_patterns",
-    "unexpected_file_patterns",
+    "max_path_length",
 }
 
-_UNEXPECTED_DIRECTORIES = ",".join(
-    [
-        "*/.appveyor",
-        "*/.binder",
-        "*/.circleci",
-        "*/.git",
-        "*/.github",
-        "*/.idea",
-        "*/.pytest_cache",
-        "*/.mypy_cache",
-    ]
+_EXPECTED_DIRECTORIES = (
+    "!*/.appveyor",
+    "!*/.binder",
+    "!*/.circleci",
+    "!*/.git",
+    "!*/.github",
+    "!*/.idea",
+    "!*/.pytest_cache",
+    "!*/.mypy_cache",
 )
 
-_UNEXPECTED_FILES = ",".join(
-    [
-        "*/appveyor.yml",
-        "*/.appveyor.yml",
-        "*/azure-pipelines.yml",
-        "*/.azure-pipelines.yml",
-        "*/.cirrus.star",
-        "*/.cirrus.yml",
-        "*/codecov.yml",
-        "*/.codecov.yml",
-        "*/.DS_Store",
-        "*/.gitignore",
-        "*/.gitpod.yml",
-        "*/.hadolint.yaml",
-        "*/.readthedocs.yaml",
-        "*/.travis.yml",
-        "*/vsts-ci.yml",
-        "*/.vsts-ci.yml",
-    ]
+_EXPECTED_FILES = (
+    "!*/appveyor.yml",
+    "!*/.appveyor.yml",
+    "!*/azure-pipelines.yml",
+    "!*/.azure-pipelines.yml",
+    "!*/.cirrus.star",
+    "!*/.cirrus.yml",
+    "!*/codecov.yml",
+    "!*/.codecov.yml",
+    "!*/.DS_Store",
+    "!*/.gitignore",
+    "!*/.gitpod.yml",
+    "!*/.hadolint.yaml",
+    "!*/.readthedocs.yaml",
+    "!*/.travis.yml",
+    "!*/vsts-ci.yml",
+    "!*/.vsts-ci.yml",
 )
 
 
 @dataclass
 class _Config:
-    ignore: str = ""
+    expected_directories: Sequence[str] = _EXPECTED_DIRECTORIES
+    expected_files: Sequence[str] = _EXPECTED_FILES
+    ignore: Sequence[str] = ()
     inspect: bool = False
     max_allowed_files: int = 2000
     max_allowed_size_compressed: str = "50M"
     max_allowed_size_uncompressed: str = "75M"
-    unexpected_directory_patterns: str = _UNEXPECTED_DIRECTORIES
-    unexpected_file_patterns: str = _UNEXPECTED_FILES
+    max_path_length: int = 200
 
     def __setattr__(self, name: str, value: Any) -> None:
         attr_name = name.replace("-", "_")
         if attr_name not in _ALLOWED_CONFIG_VALUES:
-            raise ValueError(f"Configuration value '{name}' is not recognized by pydistcheck")
+            raise ValueError(
+                f"Configuration value '{name}' is not recognized by pydistcheck"
+            )
         object.__setattr__(self, attr_name, value)
 
     def update_from_dict(self, input_dict: Dict[str, Any]) -> "_Config":
         for k, v in input_dict.items():
             setattr(self, k, v)
         return self
 
@@ -86,16 +86,9 @@
             return self
 
         tool_options: Dict[str, Any] = {}
         with open(toml_file, "rb") as f:
             config_dict = tomllib.load(f)
             tool_options = config_dict.get("tool", {}).get("pydistcheck", {})
 
-        # list-like stuff in TOML is expected to be a comma-delimited string when passed as
-        # a command-line argument
-        patch_dict: Dict[str, Any] = {}
-        for k, v in tool_options.items():
-            if isinstance(v, list):
-                patch_dict[k] = ",".join(v)
-        tool_options.update(patch_dict)
         self.update_from_dict(tool_options)
         return self
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/distribution_summary.py` & `pydistcheck-0.7.0/src/pydistcheck/distribution_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,78 +36,93 @@
         directories: List[_DirectoryInfo] = []
         files: List[_FileInfo] = []
         if archive_format == _ArchiveFormat.GZIP_TAR:
             with tarfile.open(filename, mode="r:gz") as tf:
                 for tar_info in tf.getmembers():
                     if tar_info.isfile():
                         files.append(
-                            _FileInfo.from_tarfile_member(archive_file=tf, tar_info=tar_info)
+                            _FileInfo.from_tarfile_member(
+                                archive_file=tf, tar_info=tar_info
+                            )
                         )
                     else:
                         directories.append(_DirectoryInfo(name=tar_info.name))
         elif archive_format == _ArchiveFormat.BZIP2_TAR:
             with tarfile.open(filename, mode="r:bz2") as tf:
                 for tar_info in tf.getmembers():
                     if tar_info.isfile():
                         files.append(
-                            _FileInfo.from_tarfile_member(archive_file=tf, tar_info=tar_info)
+                            _FileInfo.from_tarfile_member(
+                                archive_file=tf, tar_info=tar_info
+                            )
                         )
                     else:
                         directories.append(_DirectoryInfo(name=tar_info.name))
         elif archive_format == _ArchiveFormat.CONDA:
             # as of Jan 2023, .conda files are a zip archive containing:
             #   - an uncompresed file 'metadata.json' describing the contents
             #   - 2 zstd-compressed tarfiles with the package contents
             #      - 'info-*.tar.zst'
             #      - 'pkg-*.tar.zst'
             #
             # ref: https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/packages.html#conda-file-format
-            with zipfile.ZipFile(filename, mode="r") as f, TemporaryDirectory() as tmp_dir:
+            with zipfile.ZipFile(
+                filename, mode="r"
+            ) as f, TemporaryDirectory() as tmp_dir:
                 for zip_info in f.infolist():
                     # case 1 - is a directory
                     if zip_info.is_dir():
                         directories.append(_DirectoryInfo(name=zip_info.filename))
                     # case 2 - is a file but not one of the zstandard-compressed ones
                     elif not zip_info.filename.lower().endswith("tar.zst"):
                         files.append(
-                            _FileInfo.from_zipfile_member(archive_file=f, zip_info=zip_info)
+                            _FileInfo.from_zipfile_member(
+                                archive_file=f, zip_info=zip_info
+                            )
                         )
                     # case 3 - one of the zstandard-compressed archives
                     else:
                         full_path = os.path.join(tmp_dir, zip_info.filename)
                         # ref: https://stackoverflow.com/a/55260983/3986677
                         #
                         # decompress and write to a regular tarfile
                         with zipfile.ZipFile(filename, mode="r") as zf:
                             zf.extractall(path=tmp_dir, members=[zip_info.filename])
 
                             # decompress the .tar.zst to just .tar
-                            decompressed_tar_path = full_path.lower().replace(".tar.zst", ".tar")
+                            decompressed_tar_path = full_path.lower().replace(
+                                ".tar.zst", ".tar"
+                            )
                             _decompress_zstd_archive(
-                                tar_zst_file=full_path, decompressed_tar_path=decompressed_tar_path
+                                tar_zst_file=full_path,
+                                decompressed_tar_path=decompressed_tar_path,
                             )
 
                         # do tarfile things
                         with tarfile.open(decompressed_tar_path, mode="r") as tf:
                             for tar_info in tf.getmembers():
                                 if tar_info.isfile():
                                     files.append(
                                         _FileInfo.from_tarfile_member(
                                             archive_file=tf, tar_info=tar_info
                                         )
                                     )
                                 else:
-                                    directories.append(_DirectoryInfo(name=tar_info.name))
+                                    directories.append(
+                                        _DirectoryInfo(name=tar_info.name)
+                                    )
         elif archive_format == _ArchiveFormat.ZIP:
             # assume anything else can be opened with zipfile
             with zipfile.ZipFile(filename, mode="r") as f:
                 for zip_info in f.infolist():
                     if not zip_info.is_dir():
                         files.append(
-                            _FileInfo.from_zipfile_member(archive_file=f, zip_info=zip_info)
+                            _FileInfo.from_zipfile_member(
+                                archive_file=f, zip_info=zip_info
+                            )
                         )
                     else:
                         directories.append(_DirectoryInfo(name=zip_info.filename))
 
         return cls(
             archive_format=archive_format,
             compressed_size_bytes=compressed_size_bytes,
@@ -151,15 +166,17 @@
         return len(self.directories)
 
     @property
     def num_files(self) -> int:
         return len(self.files)
 
     def get_largest_files(self, n: int) -> List[_FileInfo]:
-        return sorted(self.files, key=lambda f: f.uncompressed_size_bytes, reverse=True)[:n]
+        return sorted(
+            self.files, key=lambda f: f.uncompressed_size_bytes, reverse=True
+        )[:n]
 
     @property
     def uncompressed_size_bytes(self) -> int:
         return sum(f.uncompressed_size_bytes for f in self.files)
 
     @property
     def size_by_file_extension(self) -> "OrderedDict[str, int]":
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/file_utils.py` & `pydistcheck-0.7.0/src/pydistcheck/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,16 @@
             _decompress_zstd_archive(
                 tar_zst_file=tar_zst_file, decompressed_tar_path=decompressed_tar_path
             )
 
             # do tarfile things
             with tarfile.open(decompressed_tar_path, mode="r") as tf:
                 files_to_extract = [
-                    tar_info for tar_info in tf.getmembers() if tar_info.name in relative_paths
+                    tar_info
+                    for tar_info in tf.getmembers()
+                    if tar_info.name in relative_paths
                 ]
                 tf.extractall(
                     path=out_dir,
                     members=files_to_extract,
                     filter="data",
                 )
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/inspect.py` & `pydistcheck-0.7.0/src/pydistcheck/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 
 def inspect_distribution(summary: "_DistributionSummary") -> None:
     print("file size")
     compressed_size = _FileSize(summary.compressed_size_bytes, "B")
     uncompressed_size = _FileSize(summary.uncompressed_size_bytes, "B")
     print(f"  * compressed size: {compressed_size}")
     print(f"  * uncompressed size: {uncompressed_size}")
-    space_saving = 1.0 - (compressed_size.total_size_bytes / uncompressed_size.total_size_bytes)
+    space_saving = 1.0 - (
+        compressed_size.total_size_bytes / uncompressed_size.total_size_bytes
+    )
     print(f"  * compression space saving: {round(100 * space_saving, 1)}%")
 
     print("contents")
     print(f"  * directories: {summary.num_directories}")
     print(f"  * files: {summary.num_files} ({len(summary.compiled_objects)} compiled)")
 
     print("size by extension")
     for extension, size in summary.size_by_file_extension.items():
         size_pct = size / summary.uncompressed_size_bytes
         print(f"  * {extension} - {_FileSize(size, 'B')} ({round(size_pct * 100, 1)}%)")
 
     largest_files = summary.get_largest_files(n=5)
     print("largest files")
     for file_info in largest_files:
-        print(f"  * ({_FileSize(file_info.uncompressed_size_bytes, 'B')}) {file_info.name}")
+        print(
+            f"  * ({_FileSize(file_info.uncompressed_size_bytes, 'B')}) {file_info.name}"
+        )
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/shared_lib_utils.py` & `pydistcheck-0.7.0/src/pydistcheck/shared_lib_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,34 +42,37 @@
 ]
 # fmt: on
 
 
 def _look_for_debug_symbols(lib_file: str) -> Tuple[bool, str]:
     for cmd_args, pattern in _COMMANDS_TO_PATTERNS:
         stdout = _run_command(args=[*cmd_args, lib_file])
-        contains_debug_symbols = any(bool(re.search(pattern, x)) for x in stdout.split("\n"))
+        contains_debug_symbols = any(
+            bool(re.search(pattern, x)) for x in stdout.split("\n")
+        )
         if contains_debug_symbols:
             return True, " ".join(cmd_args)
     # if you get here, no debug symbols were found by any tools
     return False, _NO_DEBUG_SYMBOLS
 
 
 def _get_symbols(cmd_args: List[str], lib_file: str) -> str:
     syms = _run_command(args=[*cmd_args, lib_file])
-    return "\n".join([line for line in syms.split("\n") if not (" a " in line or "\ta\t" in line)])
+    return "\n".join(
+        [line for line in syms.split("\n") if not (" a " in line or "\ta\t" in line)]
+    )
 
 
 def _nm_reports_debug_symbols(tool_name: str, lib_file: str) -> Tuple[bool, str]:
     exported_symbols = _get_symbols(cmd_args=[tool_name], lib_file=lib_file)
     all_symbols = _get_symbols(cmd_args=[tool_name, "-a"], lib_file=lib_file)
     return exported_symbols != all_symbols, f"{tool_name} -a"
 
 
 def _file_has_debug_symbols(file_absolute_path: str) -> Tuple[bool, str]:
-
     # test with tools that produce debug symbols that can be matched with a regex
     has_debug_symbols, cmd_str = _look_for_debug_symbols(lib_file=file_absolute_path)
     if has_debug_symbols:
         return True, cmd_str
 
     # "nm"'s test is like "check if the output is different when a flag is supplied",
     # instead of "test if this tool produces output matching this regex",
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck/utils.py` & `pydistcheck-0.7.0/src/pydistcheck/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,18 @@
         return cls(num=float(size_str[:-1]), unit_str=size_str[-1])
 
     @property
     def total_size_bytes(self) -> int:
         return int(self._num * _UNIT_TO_NUM_BYTES[self._unit_str])
 
     def __eq__(self, other: object) -> bool:
-        return isinstance(other, type(self)) and self.total_size_bytes == other.total_size_bytes
+        return (
+            isinstance(other, type(self))
+            and self.total_size_bytes == other.total_size_bytes
+        )
 
     def __ge__(self, other: "_FileSize") -> bool:
         return self.total_size_bytes >= other.total_size_bytes
 
     def __gt__(self, other: "_FileSize") -> bool:
         return self.total_size_bytes > other.total_size_bytes
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck.egg-info/PKG-INFO` & `pydistcheck-0.7.0/src/pydistcheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydistcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Inspect Python package distributions and raise warnings on common problems.
 Author-email: James Lamb <jaylamb20@gmail.com>
 Maintainer-email: James Lamb <jaylamb20@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, James Lamb
         All rights reserved.
@@ -94,20 +94,28 @@
 
 See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
 
 For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
-Install with `pipx`.
+Install with `pip`.
 
 ```shell
-pipx install pydistcheck
+pip install pydistcheck
 ```
 
+Or `conda`.
+
+```shell
+conda install -c conda-forge pydistcheck
+```
+
+For more details, see "Installation" ([link](./docs/installation.rst)).
+
 ## Quickstart
 
 Try it out on the test data in this project ...
 
 ```shell
 pydistcheck tests/data/problematic-package-*
 ```
```

### Comparing `pydistcheck-0.6.0/src/pydistcheck.egg-info/SOURCES.txt` & `pydistcheck-0.7.0/src/pydistcheck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.6.0/tests/test_checks.py` & `pydistcheck-0.7.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.6.0/tests/test_cli.py` & `pydistcheck-0.7.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,29 @@
 
 from pydistcheck.cli import check
 
 BASE_PACKAGES = [
     "base-package-0.1.0.tar.gz",
     "base-package-0.1.0.zip",
 ]
-PROBLEMATIC_PACKAGES = ["problematic-package-0.1.0.tar.gz", "problematic-package-0.1.0.zip"]
+PROBLEMATIC_PACKAGES = [
+    "problematic-package-0.1.0.tar.gz",
+    "problematic-package-0.1.0.zip",
+]
 MACOS_SUFFIX = "macosx_10_15_x86_64.macosx_11_6_x86_64.macosx_12_5_x86_64.whl"
 MANYLINUX_SUFFIX = "manylinux_2_28_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.whl"
-BASEBALL_PACKAGES = [
+BASEBALL_CONDA_PACKAGES = [
     "osx-64-baseballmetrics-0.1.0-0.conda",
     "osx-64-baseballmetrics-0.1.0-0.tar.bz2",
+]
+BASEBALL_WHEELS = [
     f"baseballmetrics-0.1.0-py3-none-{MACOS_SUFFIX}",
     f"baseballmetrics-0.1.0-py3-none-{MANYLINUX_SUFFIX}",
 ]
+BASEBALL_PACKAGES = BASEBALL_CONDA_PACKAGES + BASEBALL_WHEELS
 # NOTE: .bz2 and .tar.gz packages here are just unzipped
 #       and re-tarred Python wheels... to avoid pydistcheck
 #       implicitly assuming that, for example, '*.tar.gz' must
 #       be an sdist and therefore not have compiled objects
 PACKAGES_WITH_DEBUG_SYMBOLS = [
     "debug-baseballmetrics-0.1.0-macosx-wheel.tar.bz2",
     "debug-baseballmetrics-0.1.0-macosx-wheel.tar.gz",
@@ -31,15 +37,17 @@
     f"debug-baseballmetrics-py3-none-{MANYLINUX_SUFFIX}",
     "osx-64-debug-baseballmetrics-0.1.0-0.conda",
     "osx-64-debug-baseballmetrics-0.1.0-0.tar.bz2",
 ]
 TEST_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
 
 
-def _assert_log_matches_pattern(result: Result, pattern: str, num_times: int = 1) -> None:
+def _assert_log_matches_pattern(
+    result: Result, pattern: str, num_times: int = 1
+) -> None:
     log_lines = result.output.split("\n")
     match_results = [bool(re.search(pattern, log_line)) for log_line in log_lines]
     num_matches_found = sum(match_results)
     msg = (
         f"Expected to find 1 instance of '{pattern}' in logs, "
         f"found {num_matches_found} in {log_lines}."
     )
@@ -163,15 +171,16 @@
     assert result.exit_code == 1
 
     # fails with --ignore if all of the failing checks aren't mentioned in --ignore
     result = runner.invoke(
         check,
         [
             os.path.join(TEST_DATA_DIR, distro_file),
-            "--ignore=path-contains-spaces,too-many-files",
+            "--ignore=path-contains-spaces",
+            "--ignore=too-many-files",
             "--max-allowed-files=1",
             "--max-allowed-size-compressed=1B",
         ],
     )
     _assert_log_matches_pattern(
         result,
         (
@@ -182,45 +191,55 @@
     assert result.exit_code == 1
 
     # succeeds if the failing checks are mentioned in --ignore
     result = runner.invoke(
         check,
         [
             os.path.join(TEST_DATA_DIR, distro_file),
-            "--ignore=too-many-files,distro-too-large-compressed",
+            "--ignore=distro-too-large-compressed",
+            "--ignore=too-many-files",
             "--max-allowed-files=1",
         ],
     )
     assert result.exit_code == 0
     _assert_log_matches_pattern(result, "errors found while checking\\: 0")
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_check_fails_with_expected_error_if_one_check_is_unrecognized(distro_file):
     result = CliRunner().invoke(
         check,
-        [os.path.join(TEST_DATA_DIR, distro_file), "--ignore=too-many-files,random-nonsense"],
+        [
+            os.path.join(TEST_DATA_DIR, distro_file),
+            "--ignore=random-nonsense",
+            "--ignore=too-many-files",
+        ],
     )
     assert result.exit_code == 1
     _assert_log_matches_pattern(
         result,
         (
             r"ERROR\: found the following unrecognized checks passed via '\-\-ignore'\: "
             r"random\-nonsense"
         ),
     )
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
-def test_check_fails_with_expected_error_if_multiple_checks_are_unrecognized(distro_file):
+def test_check_fails_with_expected_error_if_multiple_checks_are_unrecognized(
+    distro_file,
+):
     result = CliRunner().invoke(
         check,
         [
             os.path.join(TEST_DATA_DIR, distro_file),
-            "--ignore=garbage,too-many-files,random-nonsense,other-trash",
+            "--ignore=garbage",
+            "--ignore=other-trash",
+            "--ignore=random-nonsense",
+            "--ignore=too-many-files",
         ],
     )
     assert result.exit_code == 1
     _assert_log_matches_pattern(
         result,
         (
             r"ERROR\: found the following unrecognized checks passed via '\-\-ignore'\: "
@@ -254,15 +273,18 @@
     ],
 )
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_check_respects_max_allowed_size_compressed(size_str, distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
-        [os.path.join(TEST_DATA_DIR, distro_file), f"--max-allowed-size-compressed={size_str}"],
+        [
+            os.path.join(TEST_DATA_DIR, distro_file),
+            f"--max-allowed-size-compressed={size_str}",
+        ],
     )
     assert result.exit_code == 1
 
     _assert_log_matches_pattern(
         result,
         (
             r"^1\. \[distro\-too\-large\-compressed\] Compressed size [0-9]+\.[0-9]+K is "
@@ -283,15 +305,18 @@
     ],
 )
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_check_respects_max_allowed_size_uncompressed(size_str, distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
-        [os.path.join(TEST_DATA_DIR, distro_file), f"--max-allowed-size-uncompressed={size_str}"],
+        [
+            os.path.join(TEST_DATA_DIR, distro_file),
+            f"--max-allowed-size-uncompressed={size_str}",
+        ],
     )
     assert result.exit_code == 1
 
     _assert_log_matches_pattern(
         result,
         (
             r"^1\. \[distro\-too\-large\-uncompressed\] Uncompressed size [0-9]+\.[0-9]+K is "
@@ -302,15 +327,17 @@
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_check_prefers_pyproject_toml_to_defaults(distro_file, tmp_path):
     runner = CliRunner()
     with runner.isolated_filesystem(temp_dir=tmp_path):
         with open("pyproject.toml", "w") as f:
-            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n")
+            f.write(
+                "[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n"
+            )
         result = runner.invoke(
             check,
             [os.path.join(TEST_DATA_DIR, distro_file)],
         )
 
     assert result.exit_code == 1
     _assert_log_matches_pattern(
@@ -345,22 +372,29 @@
             [os.path.join(TEST_DATA_DIR, distro_file), "--max-allowed-files=1"],
         )
         assert result.exit_code == 0
         _assert_log_matches_pattern(result, "errors found while checking\\: 0")
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
-def test_check_prefers_keyword_args_to_pyproject_toml_and_defaults(distro_file, tmp_path):
+def test_check_prefers_keyword_args_to_pyproject_toml_and_defaults(
+    distro_file, tmp_path
+):
     runner = CliRunner()
     with runner.isolated_filesystem(temp_dir=tmp_path):
         with open("pyproject.toml", "w") as f:
-            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n")
+            f.write(
+                "[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n"
+            )
         result = runner.invoke(
             check,
-            [os.path.join(TEST_DATA_DIR, distro_file), "--max-allowed-size-uncompressed=123B"],
+            [
+                os.path.join(TEST_DATA_DIR, distro_file),
+                "--max-allowed-size-uncompressed=123B",
+            ],
         )
 
     assert result.exit_code == 1
     _assert_log_matches_pattern(
         result,
         (
             r"^1\. \[distro\-too\-large\-uncompressed\] Uncompressed size [0-9]+\.[0-9]+K is "
@@ -371,20 +405,24 @@
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_check_prefers_custom_toml_file_to_root_pyproject_toml(distro_file, tmp_path):
     runner = CliRunner()
     with runner.isolated_filesystem(temp_dir=tmp_path):
         with open("pyproject.toml", "w") as f:
-            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '10GB'\n")
+            f.write(
+                "[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '10GB'\n"
+            )
         other_dir = os.path.join(tmp_path, "cool-files")
         other_config = os.path.join(other_dir, "stuff.toml")
         os.mkdir(other_dir)
         with open(other_config, "w") as f:
-            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n")
+            f.write(
+                "[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n"
+            )
         result = runner.invoke(
             check,
             [os.path.join(TEST_DATA_DIR, distro_file), f"--config={other_config}"],
         )
 
     assert result.exit_code == 1
     _assert_log_matches_pattern(
@@ -411,15 +449,17 @@
         pattern=(
             r"^1\. \[files\-only\-differ\-by\-case\] Found files which differ only by case\. "
             r"Files\: problematic\-package\-0\.1\.0/problematic_package/Question\.py"
             r",problematic\-package\-0\.1\.0/problematic_package/question\.PY"
             r",problematic\-package\-0\.1\.0/problematic_package/question\.py"
         ),
     )
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_mixed_file_extension_use_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
@@ -438,15 +478,17 @@
         result=result,
         pattern=(
             r"^3\. \[mixed\-file\-extensions\] Found a mix of file extensions for the "
             r"same file type\: \.yaml \(2\), \.yml \(1\)"
         ),
     )
 
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_path_contains_non_ascii_characters_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
@@ -461,15 +503,17 @@
         pattern=(
             r"^4\. \[path\-contains\-non\-ascii\-characters\] Found file path containing non-ASCII "
             r"characters\: "
             r"'problematic\-package\-0\.1\.0/problematic_package/\?+veryone-loves-python\.py'"
         ),
     )
 
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_path_contains_spaces_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
@@ -507,15 +551,17 @@
         result=result,
         pattern=(
             r"^8\. \[path\-contains\-spaces\] Found path with spaces\: "
             r"'problematic\-package\-0\.1\.0/problematic_package/bad code/ship\-it\.py"
         ),
     )
 
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_unexpected_files_check_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
@@ -553,26 +599,194 @@
         result=result,
         pattern=(
             r"^12\. \[unexpected\-files\] Found unexpected file "
             r"'problematic\-package\-0\.1\.0/problematic_package/\.gitignore'\."
         ),
     )
 
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: [0-9]{1}")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
-def test_cli_raises_exactly_the_expected_number_of_errors_for_the_problematic_package(distro_file):
+def test_unexpected_files_correctly_respects_multiple_cli_args(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            os.path.join(TEST_DATA_DIR, distro_file),
+            "--expected-files=!*.gitignore",
+            "--expected-files=!*.git/HEAD",
+            "--expected-directories=src/",
+        ],
+    )
+    assert result.exit_code == 1
+
+    # directories: should report that the expected directory was not found
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=r"\[expected\-files\] Did not find any directories matching pattern 'src/'",
+    )
+
+    # files: should find BOTH .gitignore files
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"\[unexpected\-files\] Found unexpected file 'problematic\-package\-0\.1\.0/\.gitignore"
+        ),
+    )
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"\[unexpected\-files\] Found unexpected file "
+            r"'problematic\-package\-0\.1\.0/problematic_package/\.gitignore"
+        ),
+    )
+
+    # files: should find the one .git/HEAD file
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"\[unexpected\-files\] Found unexpected file 'problematic\-package\-0\.1\.0/\.git/HEAD"
+        ),
+    )
+
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]{1}"
+    )
+
+
+@pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
+def test_expected_files_check_works(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            "--expected-files=*.R",
+            "--expected-directories=Movies/*",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
+    )
+    assert result.exit_code == 1
+
+    # directory
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"^1\. \[expected\-files\] Did not find any directories matching pattern 'Movies/\*'."
+        ),
+    )
+
+    # file
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"^2\. \[expected\-files\] Did not find any files matching pattern '\*\.R'."
+        ),
+    )
+
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: [0-9]+"
+    )
+
+
+@pytest.mark.parametrize("distro_file", BASEBALL_PACKAGES)
+def test_expected_files_does_not_raise_check_failure_if_all_patterns_match(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            # (wheel) lib/lib_baseball_metrics
+            # (conda) lib/python3.9/site-packages/lib/lib_baseballmetrics.dylib
+            "--expected-files=*/lib_baseballmetrics.*",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
+    )
+    assert result.exit_code == 0
+
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: 0"
+    )
+
+
+def test_expected_files_does_not_raise_check_failure_if_directory_pattern_matches():
+    # conda packages, macOS wheels do not preserve directory members...
+    # testing with a manylinux wheel to test that directory functionality works
+    distro_file = f"baseballmetrics-0.1.0-py3-none-{MANYLINUX_SUFFIX}"
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            "--expected-directories=lib/",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
+    )
+    assert result.exit_code == 0
+
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: 0"
+    )
+
+
+@pytest.mark.parametrize("distro_file", BASEBALL_CONDA_PACKAGES)
+def test_path_too_long_check_works_for_conda_packages(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            "--max-path-length=5",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
+    )
+    assert result.exit_code == 1
+
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"\[path\-too\-long\] Path too long \(78 > 5\)\: "
+            r"'lib/python3\.9/site\-packages/baseballmetrics/__pycache__/metrics\.cpython\-39\.pyc'"
+        ),
+    )
+
+
+@pytest.mark.parametrize("distro_file", BASEBALL_WHEELS)
+def test_path_too_long_check_works_for_wheels(distro_file):
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            "--max-path-length=5",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
+    )
+    assert result.exit_code == 1
+
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(
+            r"\[path\-too\-long\] Path too long \(30 > 5\)\: "
+            r"'baseballmetrics/_shared_lib\.py'"
+        ),
+    )
+
+
+@pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
+def test_cli_raises_exactly_the_expected_number_of_errors_for_the_problematic_package(
+    distro_file,
+):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
     assert result.exit_code == 1
-    _assert_log_matches_pattern(result=result, pattern=r"errors found while checking\: 12$")
+    _assert_log_matches_pattern(
+        result=result, pattern=r"errors found while checking\: 12$"
+    )
 
 
 @pytest.mark.parametrize("distro_file", PACKAGES_WITH_DEBUG_SYMBOLS)
 def test_debug_symbols_check_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
@@ -613,15 +827,20 @@
 # --------------------- #
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
 def test_inspect_runs_before_checks(distro_file):
     runner = CliRunner()
     result = runner.invoke(
-        check, ["--inspect", "--max-allowed-files=1", os.path.join(TEST_DATA_DIR, distro_file)]
+        check,
+        [
+            "--inspect",
+            "--max-allowed-files=1",
+            os.path.join(TEST_DATA_DIR, distro_file),
+        ],
     )
     assert result.exit_code == 1
 
     _assert_log_matches_pattern(
         result, r"^1\. \[too\-many\-files\] Found 11 files\. Only 1 allowed\.$"
     )
     _assert_log_matches_pattern(result, "errors found while checking\\: 1")
```

### Comparing `pydistcheck-0.6.0/tests/test_config.py` & `pydistcheck-0.7.0/tests/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,111 +41,118 @@
 def test_update_from_dict_raises_exception_for_first_bad_value_encountered(base_config):
     with pytest.raises(
         ValueError, match=r"Configuration value 'a' is not recognized by pydistcheck"
     ):
         base_config.update_from_dict({"a": 7, "b": 8, "inspect": False})
 
 
-def test_update_from_dict_works_even_if_dict_does_not_include_all_config_values(base_config):
+def test_update_from_dict_works_even_if_dict_does_not_include_all_config_values(
+    base_config,
+):
     assert base_config.inspect is False
     base_config.update_from_dict({"inspect": True})
     assert base_config.inspect is True
 
 
 def test_update_from_dict_works_when_changing_all_values(base_config):
     assert base_config.inspect is False
     assert base_config.max_allowed_files == 7
     assert base_config.max_allowed_size_compressed == "1G"
     assert base_config.max_allowed_size_uncompressed == "18K"
     patch_dict = {
+        "expected_directories": "!*/tests",
+        "expected_files": "!*.xlsx,!data/*.csv",
         "ignore": "path-contains-spaces,too-many-files",
         "inspect": True,
         "max_allowed_files": 8,
         "max_allowed_size_compressed": "2G",
         "max_allowed_size_uncompressed": "141K",
-        "unexpected_directory_patterns": "*/tests",
-        "unexpected_file_patterns": "*.xlsx,data/*.csv",
+        "max_path_length": 600,
     }
-    assert set(patch_dict.keys()) == _ALLOWED_CONFIG_VALUES, "this test needs to be updated"
+    assert (
+        set(patch_dict.keys()) == _ALLOWED_CONFIG_VALUES
+    ), "this test needs to be updated"
     base_config.update_from_dict(patch_dict)
+    assert base_config.expected_directories == "!*/tests"
+    assert base_config.expected_files == "!*.xlsx,!data/*.csv"
     assert base_config.inspect is True
     assert base_config.max_allowed_files == 8
     assert base_config.max_allowed_size_compressed == "2G"
     assert base_config.max_allowed_size_uncompressed == "141K"
-    assert base_config.unexpected_directory_patterns == "*/tests"
-    assert base_config.unexpected_file_patterns == "*.xlsx,data/*.csv"
+    assert base_config.max_path_length == 600
 
 
 def test_update_from_toml_silently_returns_self_if_file_does_not_exist(base_config):
     original_config = deepcopy(base_config)
     out = base_config.update_from_toml(toml_file=f"{uuid.uuid4().hex}.toml")
     assert out == original_config
 
 
-def test_update_from_toml_works_for_files_with_no_pydistcheck_configuration(base_config, tmpdir):
+def test_update_from_toml_works_for_files_with_no_pydistcheck_configuration(
+    base_config, tmpdir
+):
     original_config = deepcopy(base_config)
     temp_file = os.path.join(tmpdir, f"{uuid.uuid4().hex}.toml")
     with open(temp_file, "w") as f:
         f.write("""[tool.pylint]\n""")
     base_config.update_from_toml(toml_file=temp_file)
     assert base_config == original_config
 
 
-def test_update_from_toml_works_for_files_with_empty_pydistcheck_configuration(base_config, tmpdir):
+def test_update_from_toml_works_for_files_with_empty_pydistcheck_configuration(
+    base_config, tmpdir
+):
     original_config = deepcopy(base_config)
     temp_file = os.path.join(tmpdir, f"{uuid.uuid4().hex}.toml")
     with open(temp_file, "w") as f:
         f.write("""\n[tool.pylint]\n[tool.pydistcheck]\n""")
     base_config.update_from_toml(toml_file=temp_file)
     assert base_config == original_config
 
 
 @pytest.mark.parametrize(
     "config_key", ["max_allowed_size_compressed", "max-allowed-size_compressed"]
 )
-def test_update_from_toml_works_with_underscores_and_hyphens(base_config, tmpdir, config_key):
+def test_update_from_toml_works_with_underscores_and_hyphens(
+    base_config, tmpdir, config_key
+):
     temp_file = os.path.join(tmpdir, f"{uuid.uuid4().hex}.toml")
     with open(temp_file, "w") as f:
         f.write(f"[tool.pylint]\n[tool.pydistcheck]\n{config_key} = '2.5G'\n")
     base_config.update_from_toml(toml_file=temp_file)
     assert base_config.max_allowed_size_compressed == "2.5G"
 
 
 @pytest.mark.parametrize("use_hyphens", [True, False])
-def test_update_from_toml_works_with_all_config_values(base_config, tmpdir, use_hyphens):
+def test_update_from_toml_works_with_all_config_values(
+    base_config, tmpdir, use_hyphens
+):
     temp_file = os.path.join(tmpdir, f"{uuid.uuid4().hex}.toml")
     patch_dict = {
+        "expected_directories": "[\n'!tests/*'\n]",
+        "expected_files": "[\n'!*.pq',\n'!*/tests/data/*.csv']",
         "ignore": "[\n'path-contains-spaces',\n'too-many-files'\n]",
         "inspect": "true",
         "max_allowed_files": 8,
         "max_allowed_size_compressed": "'3G'",
         "max_allowed_size_uncompressed": "'4.12G'",
-        "unexpected_directory_patterns": "[\n'tests/*'\n]",
-        "unexpected_file_patterns": "[\n'*.pq',\n'*/tests/data/*.csv']",
+        "max_path_length": 25,
     }
-    assert set(patch_dict.keys()) == _ALLOWED_CONFIG_VALUES, "this test needs to be updated"
+    assert (
+        set(patch_dict.keys()) == _ALLOWED_CONFIG_VALUES
+    ), "this test needs to be updated"
     if use_hyphens:
         patch_dict = {k.replace("_", "-"): v for k, v in patch_dict.items()}
     with open(temp_file, "w") as f:
         lines = ["[tool.pylint]", "[tool.pydistcheck]"] + [
             f"{k} = {v}" for k, v in patch_dict.items()
         ]
         f.write("\n".join(lines))
     base_config.update_from_toml(toml_file=temp_file)
-    assert base_config.ignore == "path-contains-spaces,too-many-files"
+    assert base_config.expected_directories == ["!tests/*"]
+    assert base_config.expected_files == ["!*.pq", "!*/tests/data/*.csv"]
+    assert base_config.ignore == ["path-contains-spaces", "too-many-files"]
     assert base_config.inspect is True
     assert base_config.max_allowed_files == 8
     assert base_config.max_allowed_size_compressed == "3G"
     assert base_config.max_allowed_size_uncompressed == "4.12G"
-    assert base_config.unexpected_directory_patterns == "tests/*"
-    assert base_config.unexpected_file_patterns == "*.pq,*/tests/data/*.csv"
-
-
-def test_update_from_toml_converts_lists_to_comma_delimited_string(base_config, tmpdir):
-    temp_file = os.path.join(tmpdir, f"{uuid.uuid4().hex}.toml")
-    with open(temp_file, "w") as f:
-        f.write(
-            "[tool.pylint]\n[tool.pydistcheck]\n"
-            "max_allowed_size_compressed = [\n'2.5G',\n'1.56K',\n'4.236B'\n]\n"
-        )
-    base_config.update_from_toml(toml_file=temp_file)
-    assert base_config.max_allowed_size_compressed == "2.5G,1.56K,4.236B"
+    assert base_config.max_path_length == 25
```

### Comparing `pydistcheck-0.6.0/tests/test_distribution_summary.py` & `pydistcheck-0.7.0/tests/test_distribution_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,18 @@
         "no-extension": 382,
         ".py": 70,
         ".txt": 11603,
     }
 
     # files_by_extension makes sense
     assert ds.files_by_extension.keys() == ds.size_by_file_extension.keys()
-    assert sum(len(file_list) for file_list in ds.files_by_extension.values()) == ds.num_files
+    assert (
+        sum(len(file_list) for file_list in ds.files_by_extension.values())
+        == ds.num_files
+    )
 
     # size_by_file_extension should return results sorted from largest to smallest by file size
     last_size_seen = float("inf")
     for size_in_bytes in ds.size_by_file_extension.values():
         assert size_in_bytes < last_size_seen
         last_size_seen = size_in_bytes
 
@@ -96,15 +99,17 @@
 
     # should actually choose the 2 largest files
     assert largest_files[0].name == "base-package-0.1.0/LICENSE.txt"
     assert largest_files[1].name == "base-package-0.1.0/setup.cfg"
 
 
 def test_distribution_summary_get_largest_files_works():
-    ds = _DistributionSummary.from_file(os.path.join(TEST_DATA_DIR, BASE_PACKAGE_SDISTS[0]))
+    ds = _DistributionSummary.from_file(
+        os.path.join(TEST_DATA_DIR, BASE_PACKAGE_SDISTS[0])
+    )
 
     # get_largest_files() should return a non-empty list of _FileInfo objects
     num_files = ds.num_files
 
     # if you ask for more files than there are, you get however many there are
     assert len(ds.get_largest_files(n=num_files + 1)) == num_files
```

### Comparing `pydistcheck-0.6.0/tests/test_docs.py` & `pydistcheck-0.7.0/tests/test_docs.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     missing_opts = _ALLOWED_CONFIG_VALUES - opts_in_docs
     assert len(missing_opts) == 0, f"missing options: {','.join(missing_opts)}"
     extra_opts = opts_in_docs - _ALLOWED_CONFIG_VALUES
     assert len(extra_opts) == 0, f"unrecognized options: {','.join(extra_opts)}"
 
     # values should exactly match the defaults
     config = _Config().update_from_toml(defaults_example_file)
+
+    # The default in _Config class is a tuple because 'dataclasses' requires something immutable,
+    # but it's read in as a list from pyproject.toml.
+    #
+    # This allows for that deviation.
+    config.expected_directories = tuple(config.expected_directories)
+    config.expected_files = tuple(config.expected_files)
+    config.ignore = ()
+
     assert (
         config == _Config()
     ), "values in 'docs/_static/defaults.toml' do not match actual defaults used by pydistcheck"
 
 
 def test_all_checks_are_documented_in_check_reference():
     check_ref_file = DOCS_ROOT.joinpath("check-reference.rst")
```

### Comparing `pydistcheck-0.6.0/tests/test_utils.py` & `pydistcheck-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

