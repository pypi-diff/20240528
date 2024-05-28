# Comparing `tmp/amirispy-2.0.0.tar.gz` & `tmp/amirispy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amirispy-2.0.0.tar", max compression
+gzip compressed data, was "amirispy-2.1.0.tar", max compression
```

## Comparing `amirispy-2.0.0.tar` & `amirispy-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3153 2024-04-04 11:55:47.392180 amirispy-2.0.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2024-01-08 09:00:55.404045 amirispy-2.0.0/LICENSES/
--rw-r--r--   0        0        0    10389 2024-01-08 09:00:55.405047 amirispy-2.0.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    13229 2023-04-21 13:23:31.581857 amirispy-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0     7167 2022-11-04 09:40:34.074112 amirispy-2.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1664 2024-04-04 11:55:47.392693 amirispy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8263 2024-04-04 11:55:47.392456 amirispy-2.0.0/README.md
--rw-r--r--   0        0        0      111 2022-11-04 09:40:34.076185 amirispy-2.0.0/src/amirispy/__init__.py
--rw-r--r--   0        0        0      182 2022-11-04 09:40:34.076185 amirispy-2.0.0/src/amirispy/scripts/__init__.py
--rw-r--r--   0        0        0     2065 2024-01-08 09:26:21.087000 amirispy-2.0.0/src/amirispy/scripts/amiris.py
--rw-r--r--   0        0        0      331 2024-04-04 09:45:19.492597 amirispy-2.0.0/src/amirispy/scripts/resources/fameSetup.yaml
--rw-r--r--   0        0        0        0 2022-11-04 09:38:53.186209 amirispy-2.0.0/src/amirispy/scripts/subcommands/__init__.py
--rw-r--r--   0        0        0     4667 2024-04-04 11:55:47.393018 amirispy-2.0.0/src/amirispy/scripts/subcommands/batch.py
--rw-r--r--   0        0        0     1711 2022-11-04 09:43:46.536502 amirispy-2.0.0/src/amirispy/scripts/subcommands/compare.py
--rw-r--r--   0        0        0     6149 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/scripts/subcommands/install.py
--rw-r--r--   0        0        0     1390 2024-04-04 10:27:55.347558 amirispy-2.0.0/src/amirispy/scripts/subcommands/run.py
--rw-r--r--   0        0        0      111 2022-11-04 09:40:34.078105 amirispy-2.0.0/src/amirispy/source/__init__.py
--rw-r--r--   0        0        0     6883 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/source/cli.py
--rw-r--r--   0        0        0     5510 2024-04-04 11:55:47.393139 amirispy-2.0.0/src/amirispy/source/fameio_calls.py
--rw-r--r--   0        0        0     5671 2022-11-04 09:43:46.537508 amirispy-2.0.0/src/amirispy/source/file_comparison.py
--rw-r--r--   0        0        0     2442 2024-04-04 10:27:55.348582 amirispy-2.0.0/src/amirispy/source/files.py
--rw-r--r--   0        0        0     2641 2023-02-07 15:32:49.998683 amirispy-2.0.0/src/amirispy/source/logs.py
--rw-r--r--   0        0        0      828 2023-02-07 15:47:53.342532 amirispy-2.0.0/src/amirispy/source/util.py
--rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 amirispy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3378 2024-05-28 11:50:58.205878 amirispy-2.1.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2024-04-17 12:34:23.599787 amirispy-2.1.0/LICENSES/
+-rw-r--r--   0        0        0    10389 2022-11-04 09:55:17.891458 amirispy-2.1.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    13229 2023-05-04 07:45:25.133674 amirispy-2.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7167 2022-11-04 09:55:17.891458 amirispy-2.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1668 2024-05-28 11:50:58.205878 amirispy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8263 2024-04-12 13:08:51.100756 amirispy-2.1.0/README.md
+-rw-r--r--   0        0        0      111 2022-11-04 09:55:17.894287 amirispy-2.1.0/src/amirispy/__init__.py
+-rw-r--r--   0        0        0      182 2022-11-04 09:55:17.894287 amirispy-2.1.0/src/amirispy/scripts/__init__.py
+-rw-r--r--   0        0        0     2065 2024-02-08 10:09:56.072596 amirispy-2.1.0/src/amirispy/scripts/amiris.py
+-rw-r--r--   0        0        0      377 2024-05-28 11:50:58.205878 amirispy-2.1.0/src/amirispy/scripts/resources/fameSetup.yaml
+-rw-r--r--   0        0        0        0 2022-11-04 09:19:34.176931 amirispy-2.1.0/src/amirispy/scripts/subcommands/__init__.py
+-rw-r--r--   0        0        0     4667 2024-05-28 07:38:04.662011 amirispy-2.1.0/src/amirispy/scripts/subcommands/batch.py
+-rw-r--r--   0        0        0     1711 2022-11-04 09:55:17.895289 amirispy-2.1.0/src/amirispy/scripts/subcommands/compare.py
+-rw-r--r--   0        0        0     6149 2024-04-12 13:08:51.101756 amirispy-2.1.0/src/amirispy/scripts/subcommands/install.py
+-rw-r--r--   0        0        0     1390 2024-04-12 13:08:51.101756 amirispy-2.1.0/src/amirispy/scripts/subcommands/run.py
+-rw-r--r--   0        0        0      111 2022-11-04 09:55:17.897287 amirispy-2.1.0/src/amirispy/source/__init__.py
+-rw-r--r--   0        0        0     6883 2024-04-12 13:08:51.102755 amirispy-2.1.0/src/amirispy/source/cli.py
+-rw-r--r--   0        0        0     5510 2024-05-28 07:42:01.672999 amirispy-2.1.0/src/amirispy/source/fameio_calls.py
+-rw-r--r--   0        0        0     5671 2022-11-04 09:55:17.897287 amirispy-2.1.0/src/amirispy/source/file_comparison.py
+-rw-r--r--   0        0        0     2442 2024-04-12 13:08:51.103774 amirispy-2.1.0/src/amirispy/source/files.py
+-rw-r--r--   0        0        0     2641 2022-11-04 09:55:17.898287 amirispy-2.1.0/src/amirispy/source/logs.py
+-rw-r--r--   0        0        0      828 2023-02-14 12:06:27.679022 amirispy-2.1.0/src/amirispy/source/util.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 amirispy-2.1.0/PKG-INFO
```

### Comparing `amirispy-2.0.0/CHANGELOG.md` & `amirispy-2.1.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 <!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: CC0-1.0 -->
+
 # Changelog
 
+## [2.1.0](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v2.1.0) - 2024-05-28
+### Changed
+- Update to fameio version 2 #48 (@dlr-cjs)
+- Improve CI config with more stages to reduce runner times #46 (@dlr-cjs)
+
 ## [2.0.0](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v2.0.0) - 2024-04-04
 ### Changed
 - **Breaking**: Removed support for `python==3.8` #42 (@dlr_fn)
 - **Breaking**: Removed support for `fameio<2.0.0` #42 (@dlr_fn)
 - Upgrade to `pytest>=8.1` #42 (@dlr-cjs @dlr_fn)
-- If output folder is specified, no subfolder with the name of the scenario will be created (#44 @dlr-cjs)  
-- Loosen dependency restrictions for fameio (#39 @dlr-cjs)
-- Replace setup.py with pyproject.toml (#13 @dlr-cjs)
+- If output folder is specified, no subfolder with the name of the scenario will be created #44 (@dlr-cjs)
+- Loosen dependency restrictions for fameio #39 (@dlr-cjs)
+- Replace setup.py with pyproject.toml #13 (@dlr-cjs)
 
 ### Added
-- Option to use CLI commands as list of strings directly within a script (!35 @maurerle @dlr-cjs @dlr_fn)
-- Acknowledgement section in Readme (#41 @dlr-cjs)
-- Option to pass through FAME-Io output conversion options (#42 @dlr-cjs)
+- Option to use CLI commands as list of strings directly within a script !35 (@maurerle @dlr-cjs @dlr_fn)
+- Acknowledgement section in Readme #41 (@dlr-cjs)
+- Option to pass through FAME-Io output conversion options #42 (@dlr-cjs)
 - PyTests for `python==3.12` #42 (@dlr_fn)
 
 ### Fixed
 - Fix deprecated `pkg_resources.resource_filename` in `_conduct_model_installation` #42 (@dlr-cjs @dlr_fn)
 
 ## [1.3](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.3) - 2023-06-13
 ### Changed
-- Updated dependency to latest fameio version (#36 @dlr-cjs)
+- Updated dependency to latest fameio version #36 (@dlr-cjs)
 
 ### Removed
-- Removed JDK8 support and updated AMIRIS artifact downloading during install (#38 @dlr-cjs)
+- Removed JDK8 support and updated AMIRIS artifact downloading during install #38 (@dlr-cjs)
 
 ## [1.2](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.2) - 2023-04-21
 ### Changed
-- When writing outputs during `amiris run`, TimeStep is now converted from Fame TimeStep to datetime by default (#30 @dlr_fn)
-- When writing outputs during `amiris run`, results are merged to hourly values using `fameio merge-time` (#31 (@dlr_fn)
+- When writing outputs during `amiris run`, TimeStep is now converted from Fame TimeStep to datetime by default #30
+  (@dlr_fn)
+- When writing outputs during `amiris run`, results are merged to hourly values using `fameio merge-time` #31 (@dlr_fn)
 
-### Added 
-- Added `amiris batch` for running multiple scenarios (#32 @dlr_elghazi, @dlr_fn)
+### Added
+- Added `amiris batch` for running multiple scenarios #32 (@dlr_elghazi @dlr_fn)
 
 ## [1.1.4](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.1.4) - 2023-02-24
 ### Added
-- Added `-m/--mode` option to `amiris install` for model only `-m/--mode model` or [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) only with `-m/--mode examples` (#27 @dlr_fn)
+- Added `-m/--mode` option to `amiris install` for model only `-m/--mode model`
+  or [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) only with `-m/--mode examples` #27 (@dlr_fn)
 
 ## [1.1.3](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.1.3) - 2023-02-20
 ### Added
-- Added option to `-f/--force` install overwriting existing AMIRIS installation (#26 @dlr_fn)
+- Added option to `-f/--force` install overwriting existing AMIRIS installation #26 (@dlr_fn)
 
 ### Fixed
-- `amiris run` not working on linux due to improper check of access rights (#29 @dlr_fn, @dlr-cjs)
+- `amiris run` not working on linux due to improper check of access rights #29 (@dlr_fn @dlr-cjs)
 
 ## [1.1.2](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.1.2) - 2023-02-07
 ### Added
-- Added check for required Java installation (#25 @dlr_fn)
-- Added check for sufficient writing access in directories (#18 @dlr_fn)
+- Added check for required Java installation #25 (@dlr_fn)
+- Added check for sufficient writing access in directories #18 (@dlr_fn)
 - Added `" "` to paths to improve identification of paths in logs
 
 ## [1.1.1](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.1.1) - 2023-01-27
 ### Fixed
-- `amiris run` not working on Mac OS X (#24 @dlr_fn)
+- `amiris run` not working on Mac OS X #24 (@dlr_fn)
 
 ## [1.1](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.1) - 2022-12-07
 ### Changed
 - **Breaking**: Compatibility with AMIRIS >= v1.2.3.4
 - Moved to new AMIRIS packaging with executable Jar and prepackaged log4j.properties
 
 ## [1.0](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/-/tags/v1.0) - 2022-11-02
```

### Comparing `amirispy-2.0.0/LICENSES/Apache-2.0.txt` & `amirispy-2.1.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/LICENSES/CC-BY-4.0.txt` & `amirispy-2.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/LICENSES/CC0-1.0.txt` & `amirispy-2.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/pyproject.toml` & `amirispy-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "amirispy"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python tools for the electricity market model AMIRIS"
 license = "Apache-2.0"
 authors = [
     "Christoph Schimeczek <amiris@dlr.de>",
     "Felix Nitsch <amiris@dlr.de>",
 ]
 maintainers = [
@@ -24,28 +24,28 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
 ]
-packages = [{include = "amirispy", from = "src"}]
+packages = [{ include = "amirispy", from = "src" }]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fameio = "^2.0.0"
+fameio = "^2.1.0"
 wget = "^3.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1"
-coverage = {version = "^7.3", extras = ["toml"]}
+coverage = { version = "^7.3", extras = ["toml"] }
 black = "^23.10"
 
 [tool.poetry.scripts]
 amiris = "amirispy.scripts.amiris:amiris_cli"
 
 [tool.black]
 line-length = 120
```

### Comparing `amirispy-2.0.0/README.md` & `amirispy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/scripts/amiris.py` & `amirispy-2.1.0/src/amirispy/scripts/amiris.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/scripts/subcommands/batch.py` & `amirispy-2.1.0/src/amirispy/scripts/subcommands/batch.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/scripts/subcommands/compare.py` & `amirispy-2.1.0/src/amirispy/scripts/subcommands/compare.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/scripts/subcommands/install.py` & `amirispy-2.1.0/src/amirispy/scripts/subcommands/install.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/scripts/subcommands/run.py` & `amirispy-2.1.0/src/amirispy/scripts/subcommands/run.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/cli.py` & `amirispy-2.1.0/src/amirispy/source/cli.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/fameio_calls.py` & `amirispy-2.1.0/src/amirispy/source/fameio_calls.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/file_comparison.py` & `amirispy-2.1.0/src/amirispy/source/file_comparison.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/files.py` & `amirispy-2.1.0/src/amirispy/source/files.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/logs.py` & `amirispy-2.1.0/src/amirispy/source/logs.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/src/amirispy/source/util.py` & `amirispy-2.1.0/src/amirispy/source/util.py`

 * *Files identical despite different names*

### Comparing `amirispy-2.0.0/PKG-INFO` & `amirispy-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amirispy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python tools for the electricity market model AMIRIS
 Home-page: https://dlr-ve.gitlab.io/esy/amiris/home/
 License: Apache-2.0
 Keywords: AMIRIS,agent-based modelling,electricity market
 Author: Christoph Schimeczek
 Author-email: amiris@dlr.de
 Maintainer: Christoph Schimeczek
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: fameio (>=2.0.0,<3.0.0)
+Requires-Dist: fameio (>=2.1.0,<3.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://gitlab.com/dlr-ve/esy/amiris/amiris-py/
 Description-Content-Type: text/markdown
 
 <!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
```

