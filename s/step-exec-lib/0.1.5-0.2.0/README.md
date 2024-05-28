# Comparing `tmp/step-exec-lib-0.1.5.tar.gz` & `tmp/step_exec_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step-exec-lib-0.1.5.tar", max compression
+gzip compressed data, was "step_exec_lib-0.2.0.tar", max compression
```

## Comparing `step-exec-lib-0.1.5.tar` & `step_exec_lib-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      738 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1422 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/DCO
--rw-r--r--   0        0        0    11353 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/LICENSE
--rw-r--r--   0        0        0     3085 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/README.md
--rw-r--r--   0        0        0     1671 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       24 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/__init__.py
--rw-r--r--   0        0        0     1042 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/errors.py
--rw-r--r--   0        0        0    10077 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/steps.py
--rw-r--r--   0        0        0      128 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/types.py
--rw-r--r--   0        0        0       64 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/utils/__init__.py
--rw-r--r--   0        0        0     1878 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/utils/config.py
--rw-r--r--   0        0        0     1005 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/utils/files.py
--rw-r--r--   0        0        0     1985 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/utils/git.py
--rw-r--r--   0        0        0     1190 2021-10-28 08:25:37.370926 step-exec-lib-0.1.5/step_exec_lib/utils/processes.py
--rw-r--r--   0        0        0     3942 2021-10-28 08:25:50.031418 step-exec-lib-0.1.5/setup.py
--rw-r--r--   0        0        0     4231 2021-10-28 08:25:50.031996 step-exec-lib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      877 2024-05-28 08:32:35.276515 step_exec_lib-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1422 2024-05-28 08:32:35.276515 step_exec_lib-0.2.0/DCO
+-rw-r--r--   0        0        0    11353 2024-05-28 08:32:35.276515 step_exec_lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3085 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/README.md
+-rw-r--r--   0        0        0     1669 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/__init__.py
+-rw-r--r--   0        0        0     1042 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/errors.py
+-rw-r--r--   0        0        0    10089 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/steps.py
+-rw-r--r--   0        0        0      128 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/types.py
+-rw-r--r--   0        0        0       64 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/utils/__init__.py
+-rw-r--r--   0        0        0     1878 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/utils/config.py
+-rw-r--r--   0        0        0     1006 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/utils/files.py
+-rw-r--r--   0        0        0     1986 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/utils/git.py
+-rw-r--r--   0        0        0     1190 2024-05-28 08:32:35.280516 step_exec_lib-0.2.0/step_exec_lib/utils/processes.py
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 step_exec_lib-0.2.0/PKG-INFO
```

### Comparing `step-exec-lib-0.1.5/CHANGELOG.md` & `step_exec_lib-0.2.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 Based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), following [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [Unreleased]
+
+### Changed
+
+## [0.2.0] 2024-05-28
+
+- dependency updates
+- changed supported python versions to 3.9, 3.10, 3.11 and 3.12
+
 ## [0.1.5] 2021-10-22
 
 - fixed:
   - output capture in `run_and_handle_error`
 
 ## [0.1.4] 2021-10-20
```

### Comparing `step-exec-lib-0.1.5/DCO` & `step_exec_lib-0.2.0/DCO`

 * *Files identical despite different names*

### Comparing `step-exec-lib-0.1.5/LICENSE` & `step_exec_lib-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2016 - 2021 Giant Swarm GmbH
+   Copyright 2016 - 2024 Giant Swarm GmbH
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `step-exec-lib-0.1.5/README.md` & `step_exec_lib-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+# step-exec-lib
+
 [![build](https://github.com/giantswarm/step-exec-lib/actions/workflows/main.yml/badge.svg)](https://github.com/giantswarm/step-exec-lib/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/giantswarm/step-exec-lib/branch/master/graph/badge.svg)](https://codecov.io/gh/giantswarm/step-exec-lib)
 [![PyPI Version](https://img.shields.io/pypi/v/step-exec-lib.svg)](https://pypi.org/project/step-exec-lib/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/step-exec-lib.svg)](https://pypi.org/project/step-exec-lib/)
 [![Apache License](https://img.shields.io/badge/license-apache-blue.svg)](https://pypi.org/project/step-exec-lib/)
 
-# step-exec-lib
-
 A simple library to easily orchestrate a set of Steps into a filtrable pipeline.
 
 **Disclaimer**: docs are still work-in-progress!
 
 Each step provides a defined set of actions. When a pipeline is execute first all `pre` actions
 of all Steps are executed, then `run` actions and so on. Steps can provide labels, so
 you can easily disable/enable a subset of steps.
```

### Comparing `step-exec-lib-0.1.5/pyproject.toml` & `step_exec_lib-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "step-exec-lib"
-version = "0.1.5"
-description="A library that helps execute pipeline of tasks using filters and simple composition"
+version = "0.2.0"
+description = "A library that helps execute pipeline of tasks using filters and simple composition"
 authors = ["Łukasz Piątkowski <lukasz@giantswarm.io>"]
-license="Apache-2.0"
-repository="https://github.com/giantswarm/step-exec-lib"
-readme="README.md"
-keywords=["composition","steps"]
-include = ["CHANGELOG.md","DCO"]
-packages = [
-    { include = "step_exec_lib/**/*.py" },
-]
-classifiers=[
-    'Development Status :: 4 - Beta',
-    'Intended Audience :: Developers',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: Implementation :: CPython',
-    'Operating System :: POSIX :: Linux',
-    'License :: OSI Approved :: Apache Software License',
+license = "Apache-2.0"
+repository = "https://github.com/giantswarm/step-exec-lib"
+readme = "README.md"
+keywords = ["composition", "steps"]
+include = ["CHANGELOG.md", "DCO"]
+packages = [{ include = "step_exec_lib/**/*.py" }]
+classifiers = [
+  'Development Status :: 4 - Beta',
+  'Intended Audience :: Developers',
+  'Programming Language :: Python',
+  'Programming Language :: Python :: 3',
+  'Programming Language :: Python :: 3.9',
+  'Programming Language :: Python :: 3.10',
+  'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
+  'Programming Language :: Python :: Implementation :: CPython',
+  'Operating System :: POSIX :: Linux',
+  'License :: OSI Approved :: Apache Software License',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 configargparse = "^1.4.1"
-gitpython = "^3.1.17"
+gitpython = "^3.1.41"
 semver = "^2.13.0"
 # mkdocs = {version = "^1.1.2", optional = true }
 # mkapi = {version = "^1.0.10", optional = true}
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 pytest = "*"
@@ -46,15 +44,15 @@
 tox-pyenv = "^1.1.0"
 
 # [tool.poetry.extras]
 # docs = ["mkdocs", "mkapi"]
 
 [tool.black]
 line-length = 120
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `step-exec-lib-0.1.5/step_exec_lib/errors.py` & `step_exec_lib-0.2.0/step_exec_lib/errors.py`

 * *Files identical despite different names*

### Comparing `step-exec-lib-0.1.5/step_exec_lib/steps.py` & `step_exec_lib-0.2.0/step_exec_lib/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basic building block for implementing BuildSteps and Pipelines"""
+
 import argparse
 import logging
 import sys
 from abc import ABC, abstractmethod
 from typing import List, Callable, Set, cast, Optional
 
 import configargparse
@@ -204,15 +205,15 @@
     def __init__(self, config: configargparse.Namespace, steps: List[BuildStep]):
         self._config = config
         self._steps = steps
         self._context: Context = {}
         self._failed_build = False
 
     @property
-    def context(self):
+    def context(self) -> Context:
         return self._context
 
     def run(self) -> None:
         self.run_pre_steps()
         self.run_build_steps()
         self.run_cleanup()
         if self._failed_build is True:
```

### Comparing `step-exec-lib-0.1.5/step_exec_lib/utils/config.py` & `step_exec_lib-0.2.0/step_exec_lib/utils/config.py`

 * *Files identical despite different names*

### Comparing `step-exec-lib-0.1.5/step_exec_lib/utils/files.py` & `step_exec_lib-0.2.0/step_exec_lib/utils/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module with file utils"""
+
 import hashlib
 import shutil
 
 from step_exec_lib.errors import ValidationError
 
 
 def get_file_sha256(filename: str) -> str:
```

### Comparing `step-exec-lib-0.1.5/step_exec_lib/utils/git.py` & `step_exec_lib-0.2.0/step_exec_lib/utils/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module with git related utilities."""
+
 import git
 
 
 class GitRepoVersionInfo:
     """
     Provides application versions information based on the tags and commits in the repo
     """
```

### Comparing `step-exec-lib-0.1.5/step_exec_lib/utils/processes.py` & `step_exec_lib-0.2.0/step_exec_lib/utils/processes.py`

 * *Files identical despite different names*

### Comparing `step-exec-lib-0.1.5/PKG-INFO` & `step_exec_lib-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: step-exec-lib
-Version: 0.1.5
+Version: 0.2.0
 Summary: A library that helps execute pipeline of tasks using filters and simple composition
 Home-page: https://github.com/giantswarm/step-exec-lib
 License: Apache-2.0
 Keywords: composition,steps
 Author: Łukasz Piątkowski
 Author-email: lukasz@giantswarm.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: configargparse (>=1.4.1,<2.0.0)
-Requires-Dist: gitpython (>=3.1.17,<4.0.0)
+Requires-Dist: gitpython (>=3.1.41,<4.0.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0)
 Project-URL: Repository, https://github.com/giantswarm/step-exec-lib
 Description-Content-Type: text/markdown
 
+# step-exec-lib
+
 [![build](https://github.com/giantswarm/step-exec-lib/actions/workflows/main.yml/badge.svg)](https://github.com/giantswarm/step-exec-lib/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/giantswarm/step-exec-lib/branch/master/graph/badge.svg)](https://codecov.io/gh/giantswarm/step-exec-lib)
 [![PyPI Version](https://img.shields.io/pypi/v/step-exec-lib.svg)](https://pypi.org/project/step-exec-lib/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/step-exec-lib.svg)](https://pypi.org/project/step-exec-lib/)
 [![Apache License](https://img.shields.io/badge/license-apache-blue.svg)](https://pypi.org/project/step-exec-lib/)
 
-# step-exec-lib
-
 A simple library to easily orchestrate a set of Steps into a filtrable pipeline.
 
 **Disclaimer**: docs are still work-in-progress!
 
 Each step provides a defined set of actions. When a pipeline is execute first all `pre` actions
 of all Steps are executed, then `run` actions and so on. Steps can provide labels, so
 you can easily disable/enable a subset of steps.
```

