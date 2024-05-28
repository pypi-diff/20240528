# Comparing `tmp/symmetria-0.0.3.tar.gz` & `tmp/symmetria-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmetria-0.0.3.tar", last modified: Sat May 25 16:15:15 2024, max compression
+gzip compressed data, was "symmetria-0.0.4.tar", last modified: Tue May 28 21:34:32 2024, max compression
```

## Comparing `symmetria-0.0.3.tar` & `symmetria-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.400738 symmetria-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 16:15:05.000000 symmetria-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-25 16:15:15.400738 symmetria-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-25 16:15:05.000000 symmetria-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-25 16:15:05.000000 symmetria-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:15:15.400738 symmetria-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/elements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    27101 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/cycle_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/groups/symmetric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-25 16:15:05.000000 symmetria-0.0.3/tests/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.334811 symmetria-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 21:34:20.000000 symmetria-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-28 21:34:32.334811 symmetria-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-05-28 21:34:20.000000 symmetria-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-28 21:34:20.000000 symmetria-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:34:32.334811 symmetria-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29943 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/cycle_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/permutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/groups/symmetric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-28 21:34:20.000000 symmetria-0.0.4/tests/test_factory.py
```

### Comparing `symmetria-0.0.3/LICENSE.txt` & `symmetria-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symmetria-0.0.3/PKG-INFO` & `symmetria-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.3
+Version: 0.0.4
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
@@ -43,15 +43,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-<span style="font-size:1.9em;">**Welcome to symmetria**</span>
+<span style="font-size:4em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -136,15 +136,16 @@
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
 | **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 |-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Size**          | ![GitHub repo file or directory count](https://img.shields.io/github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://img.shields.io/github/repo-size/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
-| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-⚖️-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)                                                                                                                                                                                                                                               |
 | **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
 | **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
 | **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
 | **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.3 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.4 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
@@ -70,32 +70,38 @@
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------| | **Repository** | ![GitHub
 Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
-forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
-| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
-VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
-Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub
+watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria) | |
+**Size** | ![GitHub repo file or directory count](https://img.shields.io/
+github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://
+img.shields.io/github/repo-size/VascoSch92/symmetria) | | **Issues** | ![GitHub
+Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
 Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
 symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
 img.shields.io/github/issues-pr-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
 img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
 symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
 ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
-CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
-readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
-github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
-(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
-badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
-release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-âï¸-
+blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)
+| | **DOCS** | ![Read the Docs](https://img.shields.io/readthedocs/
+symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://github.com/
+VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) !
+[tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/
+badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
 8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
 [Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
```

### Comparing `symmetria-0.0.3/README.md` & `symmetria-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-<span style="font-size:1.9em;">**Welcome to symmetria**</span>
+<span style="font-size:4em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -89,15 +89,16 @@
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
 | **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 |-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Size**          | ![GitHub repo file or directory count](https://img.shields.io/github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://img.shields.io/github/repo-size/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
-| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-⚖️-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)                                                                                                                                                                                                                                               |
 | **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
 | **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
 | **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
 | **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -43,32 +43,38 @@
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------| | **Repository** | ![GitHub
 Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
-forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
-| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
-VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
-Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub
+watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria) | |
+**Size** | ![GitHub repo file or directory count](https://img.shields.io/
+github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://
+img.shields.io/github/repo-size/VascoSch92/symmetria) | | **Issues** | ![GitHub
+Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
 Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
 symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
 img.shields.io/github/issues-pr-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
 img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
 symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
 ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
-CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
-readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
-github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
-(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
-badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
-release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-âï¸-
+blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)
+| | **DOCS** | ![Read the Docs](https://img.shields.io/readthedocs/
+symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://github.com/
+VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) !
+[tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/
+badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
 8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
 [Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
```

### Comparing `symmetria-0.0.3/pyproject.toml` & `symmetria-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "symmetria"
-version = "0.0.3"
+version = "0.0.4"
 description = "Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements."
 authors = [
     {name = "Vasco Schiavo"},
 ]
 maintainers = [
     {name = "Vasco Schiavo"},
 ]
```

### Comparing `symmetria-0.0.3/symmetria/__init__.py` & `symmetria-0.0.4/symmetria/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from symmetria.elements.cycle import Cycle
 from symmetria.elements.permutation import Permutation
 from symmetria.elements.cycle_decomposition import CycleDecomposition
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __all__ = ["__version__", "Permutation", "Cycle", "CycleDecomposition"]
 
 
 def _log_version() -> None:
     """Private method which take a command line argument and log the version of `symmetria`."""
     if len(sys.argv) == 0 or len(sys.argv) == 1:
         raise Exception("No command provided.")
```

### Comparing `symmetria-0.0.3/symmetria/elements/_interface.py` & `symmetria-0.0.4/symmetria/elements/_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 
     @abstractmethod
     def __mul__(self, other):
         """Implement multiplication between two object."""
         raise NotImplementedError
 
     @abstractmethod
+    def __pow__(self, power: int) -> "_Element":
+        """Implement method `__pow__()`."""
+        raise NotImplementedError
+
+    @abstractmethod
     def __repr__(self) -> str:
         """Implement method `__repr__( )`."""
         raise NotImplementedError
 
     @abstractmethod
     def __str__(self) -> str:
         """Implement method `__str__( )`."""
@@ -74,14 +79,19 @@
 
     @abstractmethod
     def inverse(self) -> "_Element":
         """Return the inverse of the permutation object."""
         raise NotImplementedError
 
     @abstractmethod
+    def inversions(self) -> List[Tuple[int, int]]:
+        """Return the inversions of the permutation object."""
+        raise NotImplementedError
+
+    @abstractmethod
     def is_conjugate(self, other: "_Element") -> bool:
         """Return True if self and other are conjugate."""
 
     @abstractmethod
     def is_derangement(self) -> bool:
         """Return if the element is a derangement or not."""
         raise NotImplementedError
@@ -92,14 +102,19 @@
         raise NotImplementedError
 
     @abstractmethod
     def is_odd(self) -> bool:
         """Return if the element is odd or not."""
         raise NotImplementedError
 
+    @abstractmethod
+    def is_regular(self) -> bool:
+        """Return if the element is regular or not."""
+        raise NotImplementedError
+
     @property
     @abstractmethod
     def map(self) -> Dict[int, int]:
         """Return a dictionary representing the map defining the element."""
         raise NotImplementedError
 
     def name(self) -> str:
```

### Comparing `symmetria-0.0.3/symmetria/elements/cycle.py` & `symmetria-0.0.4/symmetria/elements/cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,44 @@
 
     def __mul__(self, other: "Cycle") -> "Cycle":
         raise NotImplementedError(
             "Multiplication between cycles is not supported. However, composition is supported. \n"
             "Try to call your cycle on the cycle you would like to compose."
         )
 
+    def __pow__(self, power: int) -> "Cycle":
+        """Return the cycle object to the chosen power.
+
+        :param power: the exponent for the power operation.
+        :type power: int
+
+        :return: the power of the cycle.
+        :rtype: Cycle
+
+        :example:
+            >>> from symmetria import Cycle
+            ...
+            >>> Cycle(1, 3, 2) ** 0
+            Cycle(1, 2, 3)
+            >>> Cycle(1, 3, 2) ** 1
+            Cycle(1, 3, 2)
+            >>> Cycle(1, 3, 2) ** -1
+            Cycle(1, 2, 3)
+        """
+        if isinstance(power, int) is False:
+            raise TypeError(f"Power operation for type {type(power)} not supported.")
+        elif self is False or power == 0:
+            return Cycle(*list(self.domain))
+        elif power == 1:
+            return self
+        elif power <= -1:
+            return self.inverse() ** abs(power)
+        else:
+            return self(self ** (power - 1))
+
     def __repr__(self) -> str:
         r"""Return a string representation of the cycle in the format "Cycle(x, y, z, ...)",
         where :math:`x, y, z, ... \in \mathbb{N}` are the elements of the cycle.
 
         :return: A string representation of the cycle.
         :rtype: str
 
@@ -453,14 +483,48 @@
             >>> Cycle(1, 3, 4, 2).inverse()
             Cycle(1, 2, 4, 3)
             >>> Cycle(2, 3, 1, 5, 4).inverse()
             Cycle(1, 3, 2, 4, 5)
         """
         return Cycle(*self.elements[::-1])
 
+    def inversions(self) -> List[Tuple[int, int]]:
+        r"""Return the inversions of the cycle.
+
+        Recall that an inversion of a permutation :math:`\sigma \in S_n`, for :math:`n \in \mathbb{N}`, is a pair
+        :math:`(i, j)` of positions (indexes), where the entries of the permutation are in the opposite order, i.e.,
+        :math:`i<j` but :math:`\sigma(i)>\sigma(j)`.
+
+        .. note:: The inversions of the cycle are computed after the cycle is standardized in its normal form, i.e.,
+            :math:`c_1 < c_j` for every :math:`c_j \neq c_1` in the cycle :math:`c = (c_1, ..., c_n)`.
+
+        :return: The inversions of the cycle.
+        :rtype: List[Tuple[int, int]]
+
+        :example:
+            >>> from symmetria import Cycle
+            ...
+            >>> Cycle(1, 2, 3).inversions()
+            []
+            >>> Cycle(1, 3, 4, 2).inversions()
+            [(2, 4), (3, 4)]
+            >>> Cycle(1, 2, 5, 4, 3).inversions()
+            [(3, 4), (3, 5), (4, 5)]
+        """
+        inversions, elements = [], list(self.elements)
+        min_element = 1
+        for i, p in enumerate(elements, 1):
+            if p == min_element:
+                min_element += 1
+            else:
+                for j, q in enumerate(elements[i:], 1):
+                    if p > q:
+                        inversions.append((i, i + j))
+        return inversions
+
     def is_conjugate(self, other: "Cycle") -> bool:
         """
         :raise NotImplementedError: The method `is_conjugate` is not implemented for cycles.
             This is because cycles are just building blocks for permutations.
         """
         raise NotImplementedError(
             "Method `is_conjugate` is not implemented for cycles. \n"
@@ -532,14 +596,24 @@
             >>> Cycle(1, 2, 3, 4, 5, 6).is_odd()
             True
             >>> Cycle(1, 2, 3, 4, 5, 6, 7).is_odd()
             False
         """
         return self.sgn() == -1
 
+    def is_regular(self) -> bool:
+        """
+        :raise NotImplementedError: The method `is_regular` is not implemented for cycles.
+            This is because cycles are just building blocks for permutations, and don't have a cycle decomposition.
+        """
+        raise NotImplementedError(
+            "Method `is_regular` is not implemented for cycles. \n"
+            "Convert the cycle into a `Permutation` or a `CycleDecomposition`."
+        )
+
     @property
     def map(self) -> Dict[int, int]:
         """Return a dictionary representing the mapping of the cycle,
         where keys are indices and values are the corresponding elements after the permutation.
 
         :return: The mapping of the cycle.
         :rtype: Dict[int, int]
```

### Comparing `symmetria-0.0.3/symmetria/elements/cycle_decomposition.py` & `symmetria-0.0.4/symmetria/elements/cycle_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,44 @@
                     " because they don't live in the same Symmetric group."
                 )
             return symmetria.elements.permutation.Permutation.from_dict(
                 p={idx: self.map[other.map[idx]] for idx in self.domain}
             ).cycle_decomposition()
         raise TypeError(f"Product between types `CycleDecomposition` and {type(other)} is not implemented.")
 
+    def __pow__(self, power: int) -> "CycleDecomposition":
+        """Return the permutation object to the chosen power.
+
+        :param power: the exponent for the power operation.
+        :type power: int
+
+        :return: the power of the cycle decomposition.
+        :rtype: Permutation
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(3), Cycle(1), Cycle(2)) ** 0
+            CycleDecomposition(Cycle(1), Cycle(2), Cycle(3))
+            >>> CycleDecomposition(Cycle(1, 2), Cycle(3)) ** 1
+            CycleDecomposition(Cycle(1, 2), Cycle(3))
+            >>> CycleDecomposition(Cycle(1, 2), Cycle(3)) ** -1
+            CycleDecomposition(Cycle(1, 2), Cycle(3))
+        """
+        if isinstance(power, int) is False:
+            raise TypeError(f"Power operation for type {type(power)} not supported.")
+        elif self is False or power == 0:
+            return CycleDecomposition(*[symmetria.elements.cycle.Cycle(i) for i in self.domain])
+        elif power == 1:
+            return self
+        elif power <= -1:
+            return self.inverse() ** abs(power)
+        else:
+            return self * (self ** (power - 1))
+
     def __repr__(self) -> str:
         r"""Return a string representation of the cycle decomposition in the format
         'CycleDecomposition(Cycle(x, ...), Cycle(y, ...), ...)', where :math:`x, y, ... \in \mathbb{N}` are
         the elements of the cycles.
 
         :return: A string representation of the cycle decomposition.
         :rtype: str
@@ -450,14 +480,34 @@
             >>> CycleDecomposition(Cycle(1, 2, 3)).inverse()
             CycleDecomposition(Cycle(1, 3, 2))
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3, 4)).inverse()
             CycleDecomposition(Cycle(1, 2), Cycle(3, 4))
         """
         return CycleDecomposition(*[cycle.inverse() for cycle in self])
 
+    def inversions(self) -> List[Tuple[int, int]]:
+        r"""Return the inversions of the cycle decomposition.
+
+        Recall that an inversion of a permutation :math:`\sigma \in S_n`, for :math:`n \in \mathbb{N}`, is a pair
+        :math:`(i, j)` of positions (indexes), where the entries of the permutation are in the opposite order, i.e.,
+        :math:`i<j` but :math:`\sigma(i)>\sigma(j)`.
+
+        :return: The inversions of the ycle decomposition.
+        :rtype: List[Tuple[int, int]]
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1), Cycle(2), Cycle(3)).inversions()
+            []
+            >>> CycleDecomposition(Cycle(1, 2, 3)).inversions()
+            [(1, 3), (2, 3)]
+        """
+        return symmetria.elements.permutation.Permutation.from_cycle_decomposition(self).inversions()
+
     def is_conjugate(self, other: "CycleDecomposition") -> bool:
         r"""Check if two cycle decompositions are conjugated.
 
         Recall that two permutations :math:`\sigma, \quad \tau \in S_n`, for some :math:`n \in \mathbb{N}`, are said to
         be conjugated if there is :math:`\gamma \in S_n` such that :math:`\gamma\sigma\gamma^{-1} = \tau`.
 
         :param other: a cycle decomposition
@@ -547,14 +597,34 @@
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3)).is_odd()
             True
             >>> CycleDecomposition(Cycle(1), Cycle(2, 4, 7, 6), Cycle(3, 5)).is_odd()
             False
         """
         return self.sgn() == -1
 
+    def is_regular(self) -> bool:
+        """Check if the cycle decomposition is regular.
+
+        Recall that a permutation is said regular if all cycles in its cycle decomposition have the same length.
+
+        :return: True if the cycle decomposition is regular, False otherwise.
+        :rtype: bool
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1)).is_regular()
+            True
+            >>> CycleDecomposition(Cycle(2, 1)).is_regular()
+            True
+            >>> CycleDecomposition(Cycle(2, 1), Cycle(3)).is_regular()
+            False
+        """
+        return all(len(cycle) == len(self[0]) for cycle in self)
+
     @property
     def map(self) -> Dict[int, int]:
         """Return a dictionary representing the mapping of the cycle decomposition,
         where keys are indices and values are the corresponding elements after permutation.
 
         :return: The mapping of the cycle decompostiion.
         :rtype: Dict[int, int]
```

### Comparing `symmetria-0.0.3/symmetria/elements/permutation.py` & `symmetria-0.0.4/symmetria/elements/permutation.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,20 @@
         >>> from symmetria import Permutation
         ...
         >>> permutation = Permutation(3, 1, 2)
         >>> permutation = Permutation(*[3, 1, 2])
         >>> permutation = Permutation(*(3, 1, 2))
     """
 
-    __slots__ = ["_map", "_domain"]
+    __slots__ = ["_map", "_domain", "_image"]
 
     def __init__(self, *image: int) -> None:
         self._map: Dict[int, int] = self._validate_image(image)
         self._domain: Iterable[int] = range(1, len(self._map) + 1)
+        self._image: Tuple[int] = tuple(image)
 
     @staticmethod
     def _validate_image(image: Tuple[int, ...]) -> Dict[int, int]:
         """Private method to check if a set of integers is eligible as image for a permutation.
 
         Recall that, a tuple of integers represent the image of a permutation if the following conditions hold:
             - all the integers are strictly positive;
@@ -258,14 +259,44 @@
                 raise ValueError(
                     f"Cannot compose permutation {self} with permutation {other},"
                     " because they don't live in the same Symmetric group."
                 )
             return Permutation.from_dict(p={idx: self._map[other._map[idx]] for idx in self.domain})
         raise TypeError(f"Product between types `Permutation` and {type(other)} is not implemented.")
 
+    def __pow__(self, power: int) -> "Permutation":
+        """Return the permutation object to the chosen power.
+
+        :param power: the exponent for the power operation.
+        :type power: int
+
+        :return: the power of the permutation.
+        :rtype: Permutation
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(3, 1, 2) ** 0
+            Permutation(1, 2, 3)
+            >>> Permutation(3, 1, 2) ** 1
+            Permutation(3, 1, 2)
+            >>> Permutation(3, 1, 2) ** -1
+            Permutation(2, 3, 1)
+        """
+        if isinstance(power, int) is False:
+            raise TypeError(f"Power operation for type {type(power)} not supported.")
+        elif self is False or power == 0:
+            return Permutation(*list(self.domain))
+        elif power == 1:
+            return self
+        elif power <= -1:
+            return self.inverse() ** abs(power)
+        else:
+            return self * (self ** (power - 1))
+
     def __repr__(self) -> str:
         r"""Return a string representation of the permutation in the format "Permutation(x, y, z, ...)",
         where :math:`x, y, z, ... \in \mathbb{N}` are the elements of the permutation.
 
         :return: A string representation of the permutation.
         :rtype: str
 
@@ -483,14 +514,36 @@
             >>> from symmetria import Permutation
             ...
             >>> Permutation.from_dict({1: 3, 2: 1, 3: 2})
             Permutation(3, 1, 2)
         """
         return Permutation(*[p[idx] for idx in range(1, len(p) + 1)])
 
+    @property
+    def image(self) -> Tuple[int]:
+        r"""Return the image of the permutation.
+
+        For example, to define the permutation :math:`\sigma \in S_3` given by :math:`\sigma(1)=3, \sigma(2)=1`, and
+        :math:`\sigma (3)=2`, then the image of :math:`\sigma` is :math:`(3, 1, 2)` .
+
+        :return: The image of the permutation.
+        :rtype: Tuple[int]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).image
+            (1, 2, 3)
+            >>> Permutation(1, 3, 4, 2).image
+            (1, 3, 4, 2)
+            >>> Permutation(2, 3, 1, 5, 4).image
+            (2, 3, 1, 5, 4)
+        """
+        return self._image
+
     def inverse(self) -> "Permutation":
         r"""Return the inverse of the permutation.
 
         Recall that the inverse of a permutation :math:`\sigma \in S_n`, for some :math:`n \in \mathbb{N}`, is the
         the only permutation :math:`\tau \in S_n` such that :math:`\sigma * \tau = \tau * \sigma = id`,
         where :math:`id` is the identity permutation.
 
@@ -505,14 +558,45 @@
             >>> Permutation(1, 3, 4, 2).inverse()
             Permutation(1, 4, 2, 3)
             >>> Permutation(2, 3, 1, 5, 4).inverse()
             Permutation(3, 1, 2, 5, 4)
         """
         return Permutation.from_dict({item: key for key, item in self.map.items()})
 
+    def inversions(self) -> List[Tuple[int, int]]:
+        r"""Return the inversions of the permutation.
+
+        Recall that an inversion of a permutation :math:`\sigma \in S_n`, for :math:`n \in \mathbb{N}`, is a pair
+        :math:`(i, j)` of positions (indexes), where the entries of the permutation are in the opposite order, i.e.,
+        :math:`i<j` but :math:`\sigma(i)>\sigma(j)`.
+
+        :return: The inversions of the permutation
+        :rtype: List[Tuple[int, int]]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).inversions()
+            []
+            >>> Permutation(1, 3, 4, 2).inversions()
+            [(2, 4), (3, 4)]
+            >>> Permutation(3, 1, 2, 5, 4).inversions()
+            [(1, 2), (1, 3), (4, 5)]
+        """
+        inversions, image = [], list(self.image)
+        min_element = 1
+        for i, p in enumerate(image, 1):
+            if p == min_element:
+                min_element += 1
+            else:
+                for j, q in enumerate(image[i:], 1):
+                    if p > q:
+                        inversions.append((i, i + j))
+        return inversions
+
     def is_conjugate(self, other: "Permutation") -> bool:
         r"""Check if two permutations are conjugated.
 
         Recall that two permutations :math:`\sigma, \quad \tau \in S_n`, for some :math:`n \in \mathbb{N}`, are said to
         be conjugated if there is :math:`\gamma \in S_n` such that :math:`\gamma\sigma\gamma^{-1} = \tau`.
 
         :param other: a permutation
@@ -603,14 +687,35 @@
             >>> Permutation(2, 1, 3).is_odd()
             True
             >>> Permutation(2, 3, 4, 5, 6, 1).is_odd()
             True
         """
         return self.sgn() == -1
 
+    def is_regular(self) -> bool:
+        """Check if the permutation is regular.
+
+        Recall that a permutation is said regular if all cycles in its cycle decomposition have the same length.
+
+        :return: True if the permutation is regular, False otherwise.
+        :rtype: bool
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).is_regular()
+            True
+            >>> Permutation(2, 1).is_regular()
+            True
+            >>> Permutation(2, 1, 3).is_regular()
+            False
+        """
+        cycle_decomposition = self.cycle_decomposition()
+        return all(len(cycle) == len(cycle_decomposition[0]) for cycle in cycle_decomposition)
+
     @property
     def map(self) -> Dict[int, int]:
         """Return a dictionary representing the mapping of the permutation.
 
         The keys of the dictionary are indices, while the values are the corresponding elements after permutation.
 
         :return: The mapping of the permutation.
```

### Comparing `symmetria-0.0.3/symmetria.egg-info/PKG-INFO` & `symmetria-0.0.4/symmetria.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.3
+Version: 0.0.4
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
@@ -43,15 +43,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-<span style="font-size:1.9em;">**Welcome to symmetria**</span>
+<span style="font-size:4em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -136,15 +136,16 @@
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
 | **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 |-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Size**          | ![GitHub repo file or directory count](https://img.shields.io/github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://img.shields.io/github/repo-size/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
 | **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
-| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-⚖️-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)                                                                                                                                                                                                                                               |
 | **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
 | **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
 | **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
 | **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.3 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.4 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
@@ -70,32 +70,38 @@
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------| | **Repository** | ![GitHub
 Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
-forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
-| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
-VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
-Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) ![GitHub
+watchers](https://img.shields.io/github/watchers/VascoSch92/symmetria) | |
+**Size** | ![GitHub repo file or directory count](https://img.shields.io/
+github/directory-file-count/VascoSch92/symmetria) ![GitHub repo size](https://
+img.shields.io/github/repo-size/VascoSch92/symmetria) | | **Issues** | ![GitHub
+Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
 Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
 symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
 img.shields.io/github/issues-pr-closed/VascoSch92/
 symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
 img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
 symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
 ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
-CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
-readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
-github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
-(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
-badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
-release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+CONTRIBUTING.md) [![MIT](https://img.shields.io/badge/Code_of_conduct-âï¸-
+blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CODE_OF_CONDUCT.md)
+| | **DOCS** | ![Read the Docs](https://img.shields.io/readthedocs/
+symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://github.com/
+VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) !
+[tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/
+badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
 8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
 [Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
```

### Comparing `symmetria-0.0.3/tests/test_factory.py` & `symmetria-0.0.4/tests/test_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-from typing import Any, Set, Dict, Type, Tuple
+from typing import (
+    Any,
+    Set,
+    Dict,
+    List,
+    Type,
+    Tuple,
+)
 
 import pytest
 
 from symmetria import CycleDecomposition
 
 ##########################
 # CONSTRUCTOR VALIDATORS #
@@ -64,14 +71,21 @@
 def validate_inverse(item: Any, expected_value: Any) -> None:
     if item.inverse() != expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.inverse()` must evaluate {expected_value}, but got {item.inverse()}."
         )
 
 
+def validate_inversions(item: Any, expected_value: List[Tuple[int, int]]) -> None:
+    if item.inversions() != expected_value:
+        raise ValueError(
+            f"The expression `{item.rep()}.inversions()` must evaluate {expected_value}, but got {item.inversions()}."
+        )
+
+
 def validate_is_conjugate(item: Any, other: Any, expected_value: bool) -> None:
     if item.is_conjugate(other) is not expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.is_conjugate({other.rep()})` must evaluate {expected_value}, "
             f"but got {item.is_conjugate(other)}."
         )
 
@@ -94,14 +108,21 @@
 def validate_is_odd(item: Any, expected_value: bool) -> None:
     if item.is_odd() is not expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.is_odd()` must evaluate {expected_value}, but got {item.is_odd()}."
         )
 
 
+def validate_is_regular(item: Any, expected_value: bool) -> None:
+    if item.is_regular() is not expected_value:
+        raise ValueError(
+            f"The expression `{item.rep()}.is_regular()` must evaluate {expected_value}, but got {item.is_regular()}."
+        )
+
+
 def validate_equivalent(lhs: Any, rhs: Any, expected_value: bool) -> None:
     if lhs.equivalent(other=rhs) != expected_value:
         raise ValueError(
             f"The expression `{lhs.rep()}.equivalent({rhs.rep()})` must evaluate {expected_value}, "
             f"but got {lhs.equivalent(other=rhs)}."
         )
 
@@ -196,14 +217,26 @@
 
 
 def validate_mul_error(lhs: Any, rhs: Any, error: Type[Exception], msg: str) -> None:
     with pytest.raises(error, match=msg):
         _ = lhs * rhs
 
 
+def validate_pow(item: Any, power: int, expected_value: Any) -> None:
+    if item**power != expected_value:
+        raise ValueError(
+            f"The expression `{item.rep()} ** {power}` must evaluate {expected_value}, but got {item ** power}."
+        )
+
+
+def validate_pow_error(item: Any, power: Any, error: Type[Exception], msg: str) -> None:
+    with pytest.raises(error, match=msg):
+        _ = item**power
+
+
 def validate_repr(item: Any, expected_value: str) -> None:
     if item.__repr__() != expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.__repr__()` must evaluate {expected_value}, but got {item.__repr__()}."
         )
```

