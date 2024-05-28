# Comparing `tmp/fameio-2.1.0.tar.gz` & `tmp/fameio-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameio-2.1.0.tar", max compression
+gzip compressed data, was "fameio-2.2.0.tar", max compression
```

## Comparing `fameio-2.1.0.tar` & `fameio-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    10680 2024-05-11 12:41:36.554060 fameio-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/
--rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    19051 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0     7169 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1850 2024-05-11 12:41:36.554060 fameio-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    30377 2024-05-11 12:41:36.554060 fameio-2.1.0/README.md
--rw-r--r--   0        0        0      109 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/__init__.py
--rw-r--r--   0        0        0      741 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/scripts/__init__.py
--rw-r--r--   0        0        0      107 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/scripts/__init__.py.license
--rw-r--r--   0        0        0     3615 2024-05-11 12:41:36.555059 fameio-2.1.0/src/fameio/scripts/convert_results.py
--rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.1.0/src/fameio/scripts/convert_results.py.license
--rw-r--r--   0        0        0     1347 2024-05-11 12:41:36.555059 fameio-2.1.0/src/fameio/scripts/make_config.py
--rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.1.0/src/fameio/scripts/make_config.py.license
--rw-r--r--   0        0        0      278 2024-05-06 12:30:08.123528 fameio-2.1.0/src/fameio/source/__init__.py
--rw-r--r--   0        0        0      112 2024-05-06 12:30:08.123528 fameio-2.1.0/src/fameio/source/cli/__init__.py
--rw-r--r--   0        0        0     3412 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/convert_results.py
--rw-r--r--   0        0        0     2384 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/make_config.py
--rw-r--r--   0        0        0     1393 2024-05-11 12:35:35.384517 fameio-2.1.0/src/fameio/source/cli/options.py
--rw-r--r--   0        0        0     9423 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/parser.py
--rw-r--r--   0        0        0     7403 2024-05-11 12:41:36.557056 fameio-2.1.0/src/fameio/source/loader.py
--rw-r--r--   0        0        0     3684 2024-05-11 12:41:36.557056 fameio-2.1.0/src/fameio/source/logs.py
--rw-r--r--   0        0        0     1321 2024-05-06 12:30:08.125518 fameio-2.1.0/src/fameio/source/path_resolver.py
--rw-r--r--   0        0        0      109 2024-05-06 12:30:08.125518 fameio-2.1.0/src/fameio/source/results/__init__.py
--rw-r--r--   0        0        0     4321 2024-05-06 12:30:08.126499 fameio-2.1.0/src/fameio/source/results/agent_type.py
--rw-r--r--   0        0        0     3709 2024-05-11 12:41:36.558058 fameio-2.1.0/src/fameio/source/results/conversion.py
--rw-r--r--   0        0        0     4856 2024-05-11 12:41:36.558058 fameio-2.1.0/src/fameio/source/results/csv_writer.py
--rw-r--r--   0        0        0     5490 2024-05-11 12:35:35.385517 fameio-2.1.0/src/fameio/source/results/data_transformer.py
--rw-r--r--   0        0        0     6919 2024-05-11 12:41:36.559057 fameio-2.1.0/src/fameio/source/results/input_dao.py
--rw-r--r--   0        0        0     3960 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/results/output_dao.py
--rw-r--r--   0        0        0     5054 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/results/reader.py
--rw-r--r--   0        0        0      837 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/results/yaml_writer.py
--rw-r--r--   0        0        0      372 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/scenario/__init__.py
--rw-r--r--   0        0        0     4713 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/scenario/agent.py
--rw-r--r--   0        0        0     4834 2024-05-06 12:30:08.128497 fameio-2.1.0/src/fameio/source/scenario/attribute.py
--rw-r--r--   0        0        0     9442 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/scenario/contract.py
--rw-r--r--   0        0        0     1554 2024-05-11 12:41:36.561056 fameio-2.1.0/src/fameio/source/scenario/exception.py
--rw-r--r--   0        0        0     1376 2024-05-06 12:30:08.128497 fameio-2.1.0/src/fameio/source/scenario/fameiofactory.py
--rw-r--r--   0        0        0     4539 2024-05-11 12:41:36.561056 fameio-2.1.0/src/fameio/source/scenario/generalproperties.py
--rw-r--r--   0        0        0     3727 2024-05-06 12:30:08.129515 fameio-2.1.0/src/fameio/source/scenario/scenario.py
--rw-r--r--   0        0        0      270 2024-05-06 12:30:08.129515 fameio-2.1.0/src/fameio/source/schema/__init__.py
--rw-r--r--   0        0        0     5183 2024-05-11 12:41:36.562056 fameio-2.1.0/src/fameio/source/schema/agenttype.py
--rw-r--r--   0        0        0     8296 2024-05-11 12:41:36.562056 fameio-2.1.0/src/fameio/source/schema/attribute.py
--rw-r--r--   0        0        0      224 2024-05-06 12:30:08.130497 fameio-2.1.0/src/fameio/source/schema/exception.py
--rw-r--r--   0        0        0     2656 2024-05-11 12:41:36.563056 fameio-2.1.0/src/fameio/source/schema/java_packages.py
--rw-r--r--   0        0        0     2975 2024-05-11 12:41:36.563056 fameio-2.1.0/src/fameio/source/schema/schema.py
--rw-r--r--   0        0        0     8232 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/series.py
--rw-r--r--   0        0        0     6984 2024-05-06 12:30:08.132517 fameio-2.1.0/src/fameio/source/time.py
--rw-r--r--   0        0        0     1052 2024-05-06 12:30:08.132517 fameio-2.1.0/src/fameio/source/tools.py
--rw-r--r--   0        0        0    15719 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/validator.py
--rw-r--r--   0        0        0    11921 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/writer.py
--rw-r--r--   0        0        0    30847 1970-01-01 00:00:00.000000 fameio-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-28 06:47:52.866383 fameio-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.2.0/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2024-05-06 12:30:08.115006 fameio-2.2.0/LICENSES/
+-rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.2.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    19051 2024-05-06 12:30:08.115006 fameio-2.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7169 2024-05-06 12:30:08.115006 fameio-2.2.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1850 2024-05-28 06:45:30.688978 fameio-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    30764 2024-05-28 06:45:30.687980 fameio-2.2.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-06 12:30:08.121006 fameio-2.2.0/src/fameio/__init__.py
+-rw-r--r--   0        0        0      741 2024-05-06 12:30:08.121006 fameio-2.2.0/src/fameio/scripts/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.121006 fameio-2.2.0/src/fameio/scripts/__init__.py.license
+-rw-r--r--   0        0        0     3616 2024-05-28 06:45:30.689979 fameio-2.2.0/src/fameio/scripts/convert_results.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.2.0/src/fameio/scripts/convert_results.py.license
+-rw-r--r--   0        0        0     1388 2024-05-28 06:45:30.689979 fameio-2.2.0/src/fameio/scripts/make_config.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.2.0/src/fameio/scripts/make_config.py.license
+-rw-r--r--   0        0        0      278 2024-05-06 12:30:08.123528 fameio-2.2.0/src/fameio/source/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-06 12:30:08.123528 fameio-2.2.0/src/fameio/source/cli/__init__.py
+-rw-r--r--   0        0        0     3412 2024-05-11 12:41:36.556061 fameio-2.2.0/src/fameio/source/cli/convert_results.py
+-rw-r--r--   0        0        0     2738 2024-05-28 06:45:30.690979 fameio-2.2.0/src/fameio/source/cli/make_config.py
+-rw-r--r--   0        0        0     1422 2024-05-28 06:45:30.690979 fameio-2.2.0/src/fameio/source/cli/options.py
+-rw-r--r--   0        0        0     9726 2024-05-28 06:45:30.691978 fameio-2.2.0/src/fameio/source/cli/parser.py
+-rw-r--r--   0        0        0     7536 2024-05-28 06:45:30.691978 fameio-2.2.0/src/fameio/source/loader.py
+-rw-r--r--   0        0        0     3684 2024-05-11 12:41:36.557056 fameio-2.2.0/src/fameio/source/logs.py
+-rw-r--r--   0        0        0     1321 2024-05-06 12:30:08.125518 fameio-2.2.0/src/fameio/source/path_resolver.py
+-rw-r--r--   0        0        0      109 2024-05-06 12:30:08.125518 fameio-2.2.0/src/fameio/source/results/__init__.py
+-rw-r--r--   0        0        0     4321 2024-05-06 12:30:08.126499 fameio-2.2.0/src/fameio/source/results/agent_type.py
+-rw-r--r--   0        0        0     3709 2024-05-11 12:41:36.558058 fameio-2.2.0/src/fameio/source/results/conversion.py
+-rw-r--r--   0        0        0     4856 2024-05-11 12:41:36.558058 fameio-2.2.0/src/fameio/source/results/csv_writer.py
+-rw-r--r--   0        0        0     5490 2024-05-11 12:56:12.740446 fameio-2.2.0/src/fameio/source/results/data_transformer.py
+-rw-r--r--   0        0        0     6919 2024-05-11 12:41:36.559057 fameio-2.2.0/src/fameio/source/results/input_dao.py
+-rw-r--r--   0        0        0     4106 2024-05-28 06:46:31.657106 fameio-2.2.0/src/fameio/source/results/output_dao.py
+-rw-r--r--   0        0        0     5054 2024-05-11 12:41:36.560056 fameio-2.2.0/src/fameio/source/results/reader.py
+-rw-r--r--   0        0        0      837 2024-05-11 12:41:36.560056 fameio-2.2.0/src/fameio/source/results/yaml_writer.py
+-rw-r--r--   0        0        0      372 2024-05-06 12:30:08.127497 fameio-2.2.0/src/fameio/source/scenario/__init__.py
+-rw-r--r--   0        0        0     4713 2024-05-06 12:30:08.127497 fameio-2.2.0/src/fameio/source/scenario/agent.py
+-rw-r--r--   0        0        0     4834 2024-05-06 12:30:08.128497 fameio-2.2.0/src/fameio/source/scenario/attribute.py
+-rw-r--r--   0        0        0     9442 2024-05-11 12:41:36.560056 fameio-2.2.0/src/fameio/source/scenario/contract.py
+-rw-r--r--   0        0        0     1554 2024-05-11 12:41:36.561056 fameio-2.2.0/src/fameio/source/scenario/exception.py
+-rw-r--r--   0        0        0     1376 2024-05-06 12:30:08.128497 fameio-2.2.0/src/fameio/source/scenario/fameiofactory.py
+-rw-r--r--   0        0        0     4796 2024-05-28 06:45:30.692978 fameio-2.2.0/src/fameio/source/scenario/generalproperties.py
+-rw-r--r--   0        0        0     3727 2024-05-06 12:30:08.129515 fameio-2.2.0/src/fameio/source/scenario/scenario.py
+-rw-r--r--   0        0        0      270 2024-05-06 12:30:08.129515 fameio-2.2.0/src/fameio/source/schema/__init__.py
+-rw-r--r--   0        0        0     5183 2024-05-11 12:41:36.562056 fameio-2.2.0/src/fameio/source/schema/agenttype.py
+-rw-r--r--   0        0        0     8296 2024-05-11 12:41:36.562056 fameio-2.2.0/src/fameio/source/schema/attribute.py
+-rw-r--r--   0        0        0      224 2024-05-06 12:30:08.130497 fameio-2.2.0/src/fameio/source/schema/exception.py
+-rw-r--r--   0        0        0     2656 2024-05-11 12:41:36.563056 fameio-2.2.0/src/fameio/source/schema/java_packages.py
+-rw-r--r--   0        0        0     2975 2024-05-11 12:41:36.563056 fameio-2.2.0/src/fameio/source/schema/schema.py
+-rw-r--r--   0        0        0     8754 2024-05-28 06:45:30.693978 fameio-2.2.0/src/fameio/source/series.py
+-rw-r--r--   0        0        0     6984 2024-05-06 12:30:08.132517 fameio-2.2.0/src/fameio/source/time.py
+-rw-r--r--   0        0        0     1052 2024-05-06 12:30:08.132517 fameio-2.2.0/src/fameio/source/tools.py
+-rw-r--r--   0        0        0    15719 2024-05-12 07:51:04.303086 fameio-2.2.0/src/fameio/source/validator.py
+-rw-r--r--   0        0        0    12456 2024-05-28 06:45:30.693978 fameio-2.2.0/src/fameio/source/writer.py
+-rw-r--r--   0        0        0    31231 1970-01-01 00:00:00.000000 fameio-2.2.0/PKG-INFO
```

### Comparing `fameio-2.1.0/CHANGELOG.md` & `fameio-2.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 <!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: CC0-1.0 -->
 
 # Changelog
+## [2.2.0](https://gitlab.com/fame-framework/fame-io/-/tags/v2.2.0) - TBA
+### Changed
+- New command line option `-enc --encoding` to change encoding when reading yaml-files
+- Improve error message when timeseries is not found and is number string #178 (@dlr-cjs)
+
+### Added
+- Add writing of FAME-Io and FAME-Protobuf versions to created input protobuf #192 (@dlr-cjs)
+- Add deprecation warning for section `GeneralProperties.Output` in scenario #203 (@dlr-cjs)
+
+## [2.1.1](https://gitlab.com/fame-framework/fame-io/-/tags/v2.1.1) - 2024-05-28
+### Fixed
+- ConvertFameResults: Fix crash on complex column conversion if Agent has no simple columns #204 (@dlr_fn @dlr-cjs) 
 
 ## [2.1.0](https://gitlab.com/fame-framework/fame-io/-/tags/v2.1.0) - 2024-05-11
 ### Changed
-- Changed format of auto-created timeseries from constant values #196 (@dlr-cjs)
-- Changed default log level to "WARNING" #191 (@dlr_fn @dlr-cjs)
-- Adapted link-formatting in Changelog !155 (@dlr-cjs)
+- Change format of auto-created timeseries from constant values #196 (@dlr-cjs)
+- Change default log level to "WARNING" #191 (@dlr_fn @dlr-cjs)
+- Adapt link-formatting in Changelog !155 (@dlr-cjs)
 
 ### Added
 - Read java package names from Schema and write to input.pb #198 (@dlr-cjs)
 
 ### Fixed
 - Fix docstrings in CLI `handle_args()` #190 (@dlr-cjs @dlr_fn)
 - Fix potential duplicates in logging #191 (@dlr_fn @dlr-cjs)
```

### Comparing `fameio-2.1.0/LICENSE.txt` & `fameio-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/LICENSES/Apache-2.0.txt` & `fameio-2.2.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/LICENSES/CC-BY-4.0.txt` & `fameio-2.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/LICENSES/CC0-1.0.txt` & `fameio-2.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/pyproject.toml` & `fameio-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fameio"
-version = "2.1.0"
+version = "2.2.0"
 description = "Python scripts for operation of FAME models"
 license = "Apache-2.0"
 authors = [
     "Felix Nitsch <fame@dlr.de>",
     "Christoph Schimeczek <fame@dlr.de>",
     "Ulrich Frey <fame@dlr.de>",
     "Benjamin Fuchs <fame@dlr.de>",
```

### Comparing `fameio-2.1.0/README.md` & `fameio-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,19 +42,20 @@
 Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
 Call structure:
 
     makeFameRunConfig -f <path/to/scenario.yaml>
 
 You may also specify any of the following arguments:
 
-| Command              | Action                                                                                                          |
-|----------------------|-----------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log`      | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
-| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.      |
-| `-o` or `--output`   | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                     |
+| Command                | Action                                                                                                                                   |
+|------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log`        | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                          |
+| `-lf` or `--logfile`   | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                               |
+| `-o` or `--output`     | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                                              |
+| `-enc` or `--encoding` | Sets the encoding of all yaml files to the given one (e.g. 'utf8' or 'cp1252'. Default is `None`, i.e. your operating system's standard. |
 
 This could look as follows:
 
     makeFameRunConfig -f <path/to/scenario.yaml> -l debug -lf <path/to/scenario.log> -o <path/to/config.pb>
 
 You may also call the configuration builder from any Python script with
 
@@ -226,14 +227,16 @@
 
 Parameters:
 * `RunId` an ID that can be given to the simulation; use at your discretion
 * `StartTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; first moment of the simulation.
 * `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates
   after passing that time stamp
 * `RandomSeed` seed to initialise random number generation; each value leads to a unique series of random numbers.
+
+Parameters in section `Output` are deprecated and will be removed in FAME-Io v3.0
 * `Interval` number of simulation ticks in between write-to-disk events; may be used for performance optimisations;
 * `Process` id of process that performs write-to-disk operations; leave at 0 to be compatible with single-processes;
 
 #### Agents
 Specifies all Agents to be created in the simulation in a list. Each Agent has its own entry.
 Structure:
```

### Comparing `fameio-2.1.0/src/fameio/scripts/__init__.py` & `fameio-2.2.0/src/fameio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/scripts/convert_results.py` & `fameio-2.2.0/src/fameio/scripts/convert_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fameio.source.results.data_transformer import DataTransformer
 from fameio.source.results.input_dao import InputDao
 from fameio.source.results.output_dao import OutputDAO
 from fameio.source.results.reader import Reader
 from fameio.source.results.yaml_writer import data_to_yaml_file
 
 ERR_MEMORY_ERROR = "Out of memory. Try using `-m` or `--memory-saving` option."
-ERR_MEMORY_SEVERE = "Out of memory despite memory-saving mode. Reduce output interval in `FAME-Core` and rerun model"
+ERR_MEMORY_SEVERE = "Out of memory despite memory-saving mode. Reduce output interval in `FAME-Core` and rerun model."
 
 
 def run(config: dict = None) -> None:
     """Reads file in protobuf format for configures FILE and extracts its content to .csv file(s)"""
     config = update_default_config(config, DEFAULT_CONFIG)
     fameio_logger(log_level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
```

### Comparing `fameio-2.1.0/src/fameio/scripts/make_config.py` & `fameio-2.2.0/src/fameio/scripts/make_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def run(config: dict = None) -> None:
     """Executes the main workflow for the building of a FAME configuration file"""
     config = update_default_config(config, DEFAULT_CONFIG)
     fameio_logger(log_level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
 
     file = config[Options.FILE]
     check_for_yaml_file_type(Path(file))
-    scenario = Scenario.from_dict(load_yaml(Path(file)))
+    scenario = Scenario.from_dict(load_yaml(Path(file), encoding=config[Options.INPUT_ENCODING]))
     SchemaValidator.check_agents_have_contracts(scenario)
 
     timeseries_manager = SchemaValidator.validate_scenario_and_timeseries(scenario)
     writer = ProtoWriter(config[Options.OUTPUT], timeseries_manager)
     writer.write_validated_scenario(scenario)
 
     log().info("Configuration completed.")
```

### Comparing `fameio-2.1.0/src/fameio/source/cli/convert_results.py` & `fameio-2.2.0/src/fameio/source/cli/convert_results.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/cli/make_config.py` & `fameio-2.2.0/src/fameio/source/cli/make_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,31 @@
 from fameio.source.cli.options import Options
 from fameio.source.cli.parser import (
     add_file_argument,
     add_log_level_argument,
     add_logfile_argument,
     add_output_argument,
     map_namespace_to_options_dict,
+    add_encoding_argument,
 )
 
 CLI_DEFAULTS = {
     Options.FILE: None,
     Options.LOG_LEVEL: "WARN",
     Options.LOG_FILE: None,
     Options.OUTPUT: Path("config.pb"),
+    Options.INPUT_ENCODING: None,
 }
 
 _INFILE_PATH_HELP = "provide path to configuration file"
 _OUTFILE_PATH_HELP = "provide file-path for the file to generate"
+_ENCODING_HELP = (
+    "provide encoding; will be applied to all input yaml files, "
+    "for available encodings see https://docs.python.org/3.9/library/codecs.html#standard-encodings"
+)
 
 
 def handle_args(args: List[str], defaults: Optional[Dict[Options, Any]] = None) -> Dict[Options, Any]:
     """
     Converts given `arguments` and returns a configuration for the make_config script
 
     Args:
@@ -50,13 +56,14 @@
     """
     defaults = defaults if (defaults is not None) else {}
     parser = argparse.ArgumentParser()
     add_file_argument(parser, _get_default(defaults, Options.FILE), _INFILE_PATH_HELP)
     add_log_level_argument(parser, _get_default(defaults, Options.LOG_LEVEL))
     add_logfile_argument(parser, _get_default(defaults, Options.LOG_FILE))
     add_output_argument(parser, _get_default(defaults, Options.OUTPUT), _OUTFILE_PATH_HELP)
+    add_encoding_argument(parser, _get_default(defaults, Options.INPUT_ENCODING), _ENCODING_HELP)
     return parser
 
 
 def _get_default(defaults: dict, option: Options) -> Any:
     """Returns default for given `option` or, if missing, its cli default"""
     return defaults.get(option, CLI_DEFAULTS[option])
```

### Comparing `fameio-2.1.0/src/fameio/source/cli/options.py` & `fameio-2.2.0/src/fameio/source/cli/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     AGENT_LIST = auto()
     SINGLE_AGENT_EXPORT = auto()
     MEMORY_SAVING = auto()
     RESOLVE_COMPLEX_FIELD = auto()
     TIME = auto()
     TIME_MERGING = auto()
     INPUT_RECOVERY = auto()
+    INPUT_ENCODING = auto()
 
 
 class TimeOptions(ParsableEnum, Enum):
     """Specifies options for conversion of time in output"""
 
     INT = auto()
     UTC = auto()
```

### Comparing `fameio-2.1.0/src/fameio/source/cli/parser.py` & `fameio-2.2.0/src/fameio/source/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 _ERR_NEGATIVE_INT = "Given value `{}` is not a non-negative int."
 
 _OPTION_ARGUMENT_NAME: Dict[str, Union[Options, Dict]] = {
     "file": Options.FILE,
     "log": Options.LOG_LEVEL,
     "logfile": Options.LOG_FILE,
     "output": Options.OUTPUT,
+    "encoding": Options.INPUT_ENCODING,
     "agents": Options.AGENT_LIST,
     "single_export": Options.SINGLE_AGENT_EXPORT,
     "memory_saving": Options.MEMORY_SAVING,
     "time": Options.TIME,
     "input_recovery": Options.INPUT_RECOVERY,
     "complex_column": Options.RESOLVE_COMPLEX_FIELD,
     "time_merging": {
@@ -76,14 +77,19 @@
         default=default_value,
         choices=[level.name for level in LogLevel if level not in [LogLevel.PRINT, LogLevel.WARN]],
         type=str.upper,
         help=help_text,
     )
 
 
+def add_encoding_argument(parser: ArgumentParser, default_value: Optional[str], help_text: str) -> None:
+    """Adds optional argument `enc` to given parser"""
+    parser.add_argument("-enc", "--encoding", type=str, default=default_value, help=help_text)
+
+
 def add_single_export_argument(parser: ArgumentParser, default_value: bool) -> None:
     """Adds optional repeatable string argument 'agent' to given `parser`"""
     help_text = "Enable export of single agents (default=False)"
     parser.add_argument(
         "-se",
         "--single-export",
         default=default_value,
```

### Comparing `fameio-2.1.0/src/fameio/source/loader.py` & `fameio-2.2.0/src/fameio/source/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from pathlib import Path
 from fnmatch import fnmatch
 from typing import IO, Any, Callable
 
 import yaml
 from fameio.source.logs import log_and_raise_critical, log
 from fameio.source.path_resolver import PathResolver
 
 DISABLING_YAML_FILE_PREFIX = "IGNORE_"
 
-CRIT_ERR_NO_YAML_GIVEN = "Please provide a valid YAML file. Received `-f/--file {}` instead."
+CRIT_NO_YAML_SUFFIX = "File must have a `.yaml` or `.yml` suffix. Received `-f/--file {}` instead."
+
+FILE_ENCODINGS = [None]
 
 
 class Args:
     def __init__(self, file_string, node_string):
         self.file_string = file_string
         self.node_string = node_string
 
@@ -149,30 +151,31 @@
     """
     args = read_args(loader, args)
     nodes = split_nodes(args.node_string)
     files = resolve_imported_path(loader, args.file_string)
 
     joined_data = None
     for file_name in files:
-        with open(file_name, "r") as open_file:
+        with open(file_name, "r", encoding=FILE_ENCODINGS[0]) as open_file:
             data = read_data_from_file(open_file, nodes, loader.path_resolver)
             joined_data = join_data(data, joined_data)
     log().debug("Joined all files `{}` to joined data `{}`".format(files, joined_data))
     return joined_data
 
 
 FameYamlLoader.add_constructor("!include", construct_include)
 
 
-def load_yaml(yaml_file_path: Path, path_resolver=PathResolver()):
+def load_yaml(yaml_file_path: Path, path_resolver=PathResolver(), encoding: str = None) -> dict:
     """Loads the yaml file from given `yaml_file_path` and returns its content"""
     log().info("Loading yaml from {}".format(yaml_file_path))
-    with open(yaml_file_path, "r") as configfile:
+    FILE_ENCODINGS[0] = encoding
+    with open(yaml_file_path, "r", encoding=encoding) as configfile:
         data = yaml.load(configfile, make_yaml_loader_builder(path_resolver))
+    FILE_ENCODINGS[0] = None
     return data
 
 
-def check_for_yaml_file_type(yaml_file_path: Path) -> None:
-    """Raises Exception if given `yaml_file_path` is not a valid YAML file"""
-    suffix = yaml_file_path.suffix.lower()
-    if suffix != ".yaml" and suffix != ".yml":
-        log_and_raise_critical(CRIT_ERR_NO_YAML_GIVEN.format(yaml_file_path))
+def check_for_yaml_file_type(yaml_file: Path) -> None:
+    """Raises Exception if given `yaml_file` has no YAML-associated file suffix"""
+    if yaml_file.suffix.lower() not in [".yaml", ".yml"]:
+        log_and_raise_critical(CRIT_NO_YAML_SUFFIX.format(yaml_file))
```

### Comparing `fameio-2.1.0/src/fameio/source/logs.py` & `fameio-2.2.0/src/fameio/source/logs.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/path_resolver.py` & `fameio-2.2.0/src/fameio/source/path_resolver.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/agent_type.py` & `fameio-2.2.0/src/fameio/source/results/agent_type.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/conversion.py` & `fameio-2.2.0/src/fameio/source/results/conversion.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/csv_writer.py` & `fameio-2.2.0/src/fameio/source/results/csv_writer.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/data_transformer.py` & `fameio-2.2.0/src/fameio/source/results/data_transformer.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/input_dao.py` & `fameio-2.2.0/src/fameio/source/results/input_dao.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/output_dao.py` & `fameio-2.2.0/src/fameio/source/results/output_dao.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,11 @@
         """
         Returns DataFrame(s) containing all data of given `agent` - data is removed after the first call
         Depending on the chosen ResolveOption the dict contains one DataFrame for the simple (and merged columns),
         or, in `SPLIT` mode, additional DataFrames mapped to each complex column's name.
         """
         agent_series = self._all_series.pop(agent_name) if agent_name in self._all_series else []
         agent_type = self._agent_type_log.get_agent_type(agent_name)
-        return data_transformer.extract_agent_data(agent_series, agent_type)
+        extracted_data = data_transformer.extract_agent_data(agent_series, agent_type)
+        if None in extracted_data and extracted_data[None].empty:
+            extracted_data.pop(None)
+        return extracted_data
```

### Comparing `fameio-2.1.0/src/fameio/source/results/reader.py` & `fameio-2.2.0/src/fameio/source/results/reader.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/results/yaml_writer.py` & `fameio-2.2.0/src/fameio/source/results/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/agent.py` & `fameio-2.2.0/src/fameio/source/scenario/agent.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/attribute.py` & `fameio-2.2.0/src/fameio/source/scenario/attribute.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/contract.py` & `fameio-2.2.0/src/fameio/source/scenario/contract.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/exception.py` & `fameio-2.2.0/src/fameio/source/scenario/exception.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/fameiofactory.py` & `fameio-2.2.0/src/fameio/source/scenario/fameiofactory.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/scenario/generalproperties.py` & `fameio-2.2.0/src/fameio/source/scenario/generalproperties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from fameio.source.logs import log
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.time import FameTime
@@ -17,28 +17,29 @@
     _KEY_START = "StartTime".lower()
     _KEY_STOP = "StopTime".lower()
     _KEY_SEED = "RandomSeed".lower()
     _KEY_OUTPUT = "Output".lower()
     _KEY_INTERVAL = "Interval".lower()
     _KEY_PROCESS = "Process".lower()
 
-    _MISSING_KEY = "General Properties requires key '{}' but it is missing."
-    _SIMULATION_DURATION = "Simulation starts after its end time - check start and stop times."
+    _ERR_MISSING_KEY = "General Properties requires key '{}' but it is missing."
+    _ERR_SIMULATION_DURATION = "Simulation starts after its end time - check start and stop times."
+    _WARN_OUTPUT_DEPRECATED = "Deprecation warning: GeneralProperties.Output will be removed with FAME-Io version > 3.0"
 
     def __init__(
         self,
         run_id: int,
         simulation_start_time: int,
         simulation_stop_time: int,
         simulation_random_seed: int,
         output_interval: int,
         output_process: int,
     ) -> None:
         if simulation_stop_time < simulation_start_time:
-            log().warning(GeneralProperties._SIMULATION_DURATION)
+            log().warning(GeneralProperties._ERR_SIMULATION_DURATION)
         self._run_id = run_id
         self._simulation_start_time = simulation_start_time
         self._simulation_stop_time = simulation_stop_time
         self._simulation_random_seed = simulation_random_seed
         self._output_interval = output_interval
         self._output_process = output_process
 
@@ -48,34 +49,36 @@
         definitions = keys_to_lower(definitions)
         run_id = get_or_default(definitions, GeneralProperties._KEY_RUN, 1)
 
         simulation_definition = keys_to_lower(
             get_or_raise(
                 definitions,
                 GeneralProperties._KEY_SIMULATION,
-                GeneralProperties._MISSING_KEY,
+                GeneralProperties._ERR_MISSING_KEY,
             )
         )
         start_time = FameTime.convert_string_if_is_datetime(
             get_or_raise(
                 simulation_definition,
                 GeneralProperties._KEY_START,
-                GeneralProperties._MISSING_KEY,
+                GeneralProperties._ERR_MISSING_KEY,
             )
         )
         stop_time = FameTime.convert_string_if_is_datetime(
             get_or_raise(
                 simulation_definition,
                 GeneralProperties._KEY_STOP,
-                GeneralProperties._MISSING_KEY,
+                GeneralProperties._ERR_MISSING_KEY,
             )
         )
         random_seed = get_or_default(simulation_definition, GeneralProperties._KEY_SEED, 1)
 
         output_definitions = keys_to_lower(get_or_default(definitions, GeneralProperties._KEY_OUTPUT, dict()))
+        if len(output_definitions) > 1:
+            log().warning(GeneralProperties._WARN_OUTPUT_DEPRECATED)
         output_interval = get_or_default(output_definitions, GeneralProperties._KEY_INTERVAL, 100)
         output_process = get_or_default(output_definitions, GeneralProperties._KEY_PROCESS, 0)
 
         return cls(run_id, start_time, stop_time, random_seed, output_interval, output_process)
 
     def to_dict(self) -> dict:
         """Serializes the general properties to a dict"""
```

### Comparing `fameio-2.1.0/src/fameio/source/scenario/scenario.py` & `fameio-2.2.0/src/fameio/source/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/schema/agenttype.py` & `fameio-2.2.0/src/fameio/source/schema/agenttype.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/schema/attribute.py` & `fameio-2.2.0/src/fameio/source/schema/attribute.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/schema/java_packages.py` & `fameio-2.2.0/src/fameio/source/schema/java_packages.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/schema/schema.py` & `fameio-2.2.0/src/fameio/source/schema/schema.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/series.py` & `fameio-2.2.0/src/fameio/source/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     """Manages matching of files to time series ids and their protobuf representation"""
 
     _TIMESERIES_RECONSTRUCTION_PATH = "./timeseries/"
     _CONSTANT_IDENTIFIER = "Constant value: {}"
     _KEY_ROW_TIME = "timeStep"
     _KEY_ROW_VALUE = "value"
 
-    _ERR_FILE_NOT_FOUND = "Cannot find Timeseries file '{}'"
+    _ERR_FILE_NOT_FOUND = "Cannot find Timeseries file '{}'."
+    _ERR_NUMERIC_STRING = " Remove quotes to use a constant numeric value instead of a timeseries file."
     _ERR_CORRUPT_TIME_SERIES_KEY = "TimeSeries file '{}' corrupt: At least one entry in first column isn't a timestamp."
     _ERR_CORRUPT_TIME_SERIES_VALUE = "TimeSeries file '{}' corrupt: At least one entry in value column isn't numeric."
     _ERR_NON_NUMERIC = "Values in TimeSeries must be numeric but was: '{}'"
     _ERR_NAN_VALUE = "Values in TimeSeries must not be missing or NaN."
     _ERR_UNREGISTERED_SERIES = "No timeseries registered with identifier '{}' - was the Scenario validated?"
     _WARN_NO_DATA = "No timeseries stored in timeseries manager. Double check if you expected timeseries."
 
@@ -82,15 +83,18 @@
                 try:
                     return identifier, self._check_and_convert_series(data)
                 except TypeError as e:
                     log_error_and_raise(TimeSeriesException(self._ERR_CORRUPT_TIME_SERIES_VALUE.format(identifier), e))
                 except ConversionException:
                     log_error_and_raise(TimeSeriesException(self._ERR_CORRUPT_TIME_SERIES_KEY.format(identifier)))
             else:
-                log_error_and_raise(TimeSeriesException(self._ERR_FILE_NOT_FOUND.format(identifier)))
+                message = self._ERR_FILE_NOT_FOUND.format(identifier)
+                if self._is_number_string(identifier):
+                    message += self._ERR_NUMERIC_STRING
+                log_error_and_raise(TimeSeriesException(message))
         else:
             return self._create_timeseries_from_value(identifier)
 
     def _check_and_convert_series(self, data: pd.DataFrame) -> pd.DataFrame:
         """Ensures validity of time series and convert to required format for writing to disk"""
         data = data.apply(
             lambda r: [FameTime.convert_string_if_is_datetime(r[0]), self._assert_valid(r[1])],
@@ -107,14 +111,23 @@
         except ValueError:
             log_error_and_raise(TypeError(TimeSeriesManager._ERR_NON_NUMERIC.format(value)))
         if math.isnan(value):
             log_error_and_raise(TypeError(TimeSeriesManager._ERR_NAN_VALUE))
         return value
 
     @staticmethod
+    def _is_number_string(identifier: str) -> bool:
+        """Returns True if given identifier can be cast to float"""
+        try:
+            float(identifier)
+            return True
+        except ValueError:
+            return False
+
+    @staticmethod
     def _create_timeseries_from_value(value: Union[int, float]) -> Tuple[str, pd.DataFrame]:
         """Returns name and dataframe for a new static timeseries created from the given `value`"""
         if math.isnan(value):
             log_error_and_raise(TimeSeriesException(TimeSeriesManager._ERR_NAN_VALUE))
         data = pd.DataFrame({0: [INT64_MIN, INT64_MAX], 1: [value, value]})
         return TimeSeriesManager._CONSTANT_IDENTIFIER.format(value), data
```

### Comparing `fameio-2.1.0/src/fameio/source/time.py` & `fameio-2.2.0/src/fameio/source/time.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/tools.py` & `fameio-2.2.0/src/fameio/source/tools.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/validator.py` & `fameio-2.2.0/src/fameio/source/validator.py`

 * *Files identical despite different names*

### Comparing `fameio-2.1.0/src/fameio/source/writer.py` & `fameio-2.2.0/src/fameio/source/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
-
+import sys
+from importlib.metadata import version
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
+from fameprotobuf.Contract_pb2 import ProtoContract
 from fameprotobuf.DataStorage_pb2 import DataStorage
-from fameprotobuf.InputFile_pb2 import InputData
+from fameprotobuf.ExecutionData_pb2 import ExecutionData
 from fameprotobuf.Field_pb2 import NestedField
-from fameprotobuf.Contract_pb2 import ProtoContract
+from fameprotobuf.InputFile_pb2 import InputData
 from fameprotobuf.Model_pb2 import ModelData
 
 from fameio.source.logs import log_error_and_raise, log
 from fameio.source.results.reader import Reader
 from fameio.source.scenario import (
     Agent,
     Attribute,
@@ -68,14 +70,15 @@
         self._set_general_properties(pb_input, scenario.general_properties)
         self._add_agents(pb_input, scenario.agents, scenario.schema)
         self._add_contracts(pb_input, scenario.contracts)
         self._set_time_series(pb_input)
         self._set_schema(pb_input, scenario.schema)
 
         self._set_java_package_names(pb_data_storage.model, scenario.schema.packages)
+        self._set_execution_versions(pb_data_storage.execution.versions)
         return pb_data_storage
 
     @staticmethod
     def _set_general_properties(pb_input: InputData, general_properties: GeneralProperties) -> None:
         """Saves a scenario's general properties to specified protobuf `pb_input` container"""
         log().info("Adding General Properties")
         pb_input.runId = general_properties.run_id
@@ -235,7 +238,14 @@
                 serialised_data_storage = pb_data_storage.SerializeToString()
                 file.write(self._FAME_PROTOBUF_STREAM_HEADER.encode(Reader.HEADER_ENCODING))
                 file.write(len(serialised_data_storage).to_bytes(Reader.BYTES_DEFINING_MESSAGE_LENGTH, byteorder="big"))
                 file.write(serialised_data_storage)
         except OSError as e:
             log_error_and_raise(ProtoWriterException(ProtoWriter._NO_FILE_SPECIFIED.format(self.file_path), e))
         log().info(self._INFO_WRITING_COMPLETED.format(self.file_path))
+
+    @staticmethod
+    def _set_execution_versions(pb_versions: ExecutionData.Versions) -> None:
+        """Adds version strings for fameio, fameprotobuf, and python to the given Versions message"""
+        pb_versions.fameProtobuf = version("fameprotobuf")
+        pb_versions.fameIo = version("fameio")
+        pb_versions.python = sys.version
```

### Comparing `fameio-2.1.0/PKG-INFO` & `fameio-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fameio
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python scripts for operation of FAME models
 Home-page: https://gitlab.com/fame-framework/wiki/-/wikis/home
 License: Apache-2.0
 Keywords: FAME,fameio,agent-based modelling,energy systems
 Author: Felix Nitsch
 Author-email: fame@dlr.de
 Maintainer: Felix Nitsch
@@ -71,19 +71,20 @@
 Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
 Call structure:
 
     makeFameRunConfig -f <path/to/scenario.yaml>
 
 You may also specify any of the following arguments:
 
-| Command              | Action                                                                                                          |
-|----------------------|-----------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log`      | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`. |
-| `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.      |
-| `-o` or `--output`   | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                     |
+| Command                | Action                                                                                                                                   |
+|------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log`        | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                          |
+| `-lf` or `--logfile`   | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                               |
+| `-o` or `--output`     | Sets the path of the compiled protobuf output file. Default is `config.pb`.                                                              |
+| `-enc` or `--encoding` | Sets the encoding of all yaml files to the given one (e.g. 'utf8' or 'cp1252'. Default is `None`, i.e. your operating system's standard. |
 
 This could look as follows:
 
     makeFameRunConfig -f <path/to/scenario.yaml> -l debug -lf <path/to/scenario.log> -o <path/to/config.pb>
 
 You may also call the configuration builder from any Python script with
 
@@ -255,14 +256,16 @@
 
 Parameters:
 * `RunId` an ID that can be given to the simulation; use at your discretion
 * `StartTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; first moment of the simulation.
 * `StopTime` time stamp in the format YYYY-MM-DD_hh:mm:ss; last moment of the simulation - i.e. simulation terminates
   after passing that time stamp
 * `RandomSeed` seed to initialise random number generation; each value leads to a unique series of random numbers.
+
+Parameters in section `Output` are deprecated and will be removed in FAME-Io v3.0
 * `Interval` number of simulation ticks in between write-to-disk events; may be used for performance optimisations;
 * `Process` id of process that performs write-to-disk operations; leave at 0 to be compatible with single-processes;
 
 #### Agents
 Specifies all Agents to be created in the simulation in a list. Each Agent has its own entry.
 Structure:
```

