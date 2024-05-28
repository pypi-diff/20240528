# Comparing `tmp/eflips_depot-3.0.5.tar.gz` & `tmp/eflips_depot-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_depot-3.0.5.tar", max compression
+gzip compressed data, was "eflips_depot-3.1.5.tar", max compression
```

## Comparing `eflips_depot-3.0.5.tar` & `eflips_depot-3.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    34143 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/LICENSE.md
--rw-r--r--   0        0        0     4899 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/README.md
--rw-r--r--   0        0        0     1556 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/__init__.py
--rw-r--r--   0        0        0    51939 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/__init__.py
--rw-r--r--   0        0        0     5375 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/defaults/default_settings.json
--rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/__init__.py
--rw-r--r--   0        0        0    17136 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/depot.py
--rw-r--r--   0        0        0    15362 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/util.py
--rw-r--r--   0        0        0    35678 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/configuration.py
--rw-r--r--   0        0        0   105566 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/depot.py
--rw-r--r--   0        0        0   140842 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/evaluation.py
--rw-r--r--   0        0        0    16131 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/filters.py
--rw-r--r--   0        0        0     5569 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/input_epex_power_price.py
--rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/doc/__init__.py
--rw-r--r--   0        0        0    22330 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/doc/direct_details.pdf
--rw-r--r--   0        0        0    24855 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/evaluation.py
--rw-r--r--   0        0        0      594 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/__init__.py
--rw-r--r--   0        0        0     1057 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/crossover.py
--rw-r--r--   0        0        0     8230 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
--rw-r--r--   0        0        0     7027 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_util.py
--rw-r--r--   0        0        0    14707 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/init.py
--rw-r--r--   0        0        0    12238 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/mutation.py
--rw-r--r--   0        0        0     9821 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/optimize_c_urfd.py
--rw-r--r--   0        0        0    56989 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/packing.py
--rw-r--r--   0        0        0      810 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/settings.py
--rw-r--r--   0        0        0     9736 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/template_creation.py
--rw-r--r--   0        0        0     3780 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/util.py
--rw-r--r--   0        0        0     2509 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/plots.py
--rw-r--r--   0        0        0    58757 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/processes.py
--rw-r--r--   0        0        0    16648 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/rating.py
--rw-r--r--   0        0        0    13568 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/resources.py
--rw-r--r--   0        0        0     2527 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/settings_config.py
--rw-r--r--   0        0        0     9375 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/simple_vehicle.py
--rw-r--r--   0        0        0    10676 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/simulation.py
--rw-r--r--   0        0        0    54311 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/smart_charging.py
--rw-r--r--   0        0        0    22338 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/standalone.py
--rw-r--r--   0        0        0     7097 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/validation.py
--rw-r--r--   0        0        0     1215 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     5809 1970-01-01 00:00:00.000000 eflips_depot-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-05-28 09:46:16.087822 eflips_depot-3.1.5/LICENSE.md
+-rw-r--r--   0        0        0     4899 2024-05-28 09:46:16.087822 eflips_depot-3.1.5/README.md
+-rw-r--r--   0        0        0     1556 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/__init__.py
+-rw-r--r--   0        0        0    51939 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/__init__.py
+-rw-r--r--   0        0        0     5375 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/defaults/default_settings.json
+-rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/__init__.py
+-rw-r--r--   0        0        0    17136 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/depot.py
+-rw-r--r--   0        0        0    15362 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/util.py
+-rw-r--r--   0        0        0    35678 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/configuration.py
+-rw-r--r--   0        0        0   105566 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/depot.py
+-rw-r--r--   0        0        0   140842 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/evaluation.py
+-rw-r--r--   0        0        0    16131 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/filters.py
+-rw-r--r--   0        0        0     5569 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/input_epex_power_price.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/doc/__init__.py
+-rw-r--r--   0        0        0    22330 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/doc/direct_details.pdf
+-rw-r--r--   0        0        0    24855 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/evaluation.py
+-rw-r--r--   0        0        0      594 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/__init__.py
+-rw-r--r--   0        0        0     1057 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/crossover.py
+-rw-r--r--   0        0        0     8230 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
+-rw-r--r--   0        0        0     7027 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_util.py
+-rw-r--r--   0        0        0    14707 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/init.py
+-rw-r--r--   0        0        0    12238 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/mutation.py
+-rw-r--r--   0        0        0     9821 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/optimize_c_urfd.py
+-rw-r--r--   0        0        0    56989 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/packing.py
+-rw-r--r--   0        0        0      810 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/settings.py
+-rw-r--r--   0        0        0     9736 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/template_creation.py
+-rw-r--r--   0        0        0     3780 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/util.py
+-rw-r--r--   0        0        0     2509 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/plots.py
+-rw-r--r--   0        0        0    58757 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/processes.py
+-rw-r--r--   0        0        0    16648 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/rating.py
+-rw-r--r--   0        0        0    13568 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/resources.py
+-rw-r--r--   0        0        0     2527 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/settings_config.py
+-rw-r--r--   0        0        0     9375 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/simple_vehicle.py
+-rw-r--r--   0        0        0    10676 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/simulation.py
+-rw-r--r--   0        0        0    54311 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/smart_charging.py
+-rw-r--r--   0        0        0    22338 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/standalone.py
+-rw-r--r--   0        0        0     7097 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/validation.py
+-rw-r--r--   0        0        0     1215 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5809 1970-01-01 00:00:00.000000 eflips_depot-3.1.5/PKG-INFO
```

### Comparing `eflips_depot-3.0.5/LICENSE.md` & `eflips_depot-3.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/README.md` & `eflips_depot-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/__init__.py` & `eflips_depot-3.1.5/eflips/depot/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/api/__init__.py` & `eflips_depot-3.1.5/eflips/depot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/api/defaults/default_settings.json` & `eflips_depot-3.1.5/eflips/depot/api/defaults/default_settings.json`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/api/private/depot.py` & `eflips_depot-3.1.5/eflips/depot/api/private/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/api/private/util.py` & `eflips_depot-3.1.5/eflips/depot/api/private/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/configuration.py` & `eflips_depot-3.1.5/eflips/depot/configuration.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/depot.py` & `eflips_depot-3.1.5/eflips/depot/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/evaluation.py` & `eflips_depot-3.1.5/eflips/depot/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/filters.py` & `eflips_depot-3.1.5/eflips/depot/filters.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/input_epex_power_price.py` & `eflips_depot-3.1.5/eflips/depot/input_epex_power_price.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/doc/direct_details.pdf` & `eflips_depot-3.1.5/eflips/depot/layout_opt/doc/direct_details.pdf`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/evaluation.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/__init__.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/crossover.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/crossover.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_util.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/init.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/init.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/mutation.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/mutation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/optimize_c_urfd.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/optimize_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/packing.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/packing.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/settings.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/settings.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/template_creation.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/template_creation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/layout_opt/util.py` & `eflips_depot-3.1.5/eflips/depot/layout_opt/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/plots.py` & `eflips_depot-3.1.5/eflips/depot/plots.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/processes.py` & `eflips_depot-3.1.5/eflips/depot/processes.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/rating.py` & `eflips_depot-3.1.5/eflips/depot/rating.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/resources.py` & `eflips_depot-3.1.5/eflips/depot/resources.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/settings_config.py` & `eflips_depot-3.1.5/eflips/depot/settings_config.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/simple_vehicle.py` & `eflips_depot-3.1.5/eflips/depot/simple_vehicle.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/simulation.py` & `eflips_depot-3.1.5/eflips/depot/simulation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/smart_charging.py` & `eflips_depot-3.1.5/eflips/depot/smart_charging.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/standalone.py` & `eflips_depot-3.1.5/eflips/depot/standalone.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/eflips/depot/validation.py` & `eflips_depot-3.1.5/eflips/depot/validation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.5/pyproject.toml` & `eflips_depot-3.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-depot"
-version = "3.0.5"
+version = "3.1.5"
 description = "Depot Simulation for eFLIPS"
 authors = ["Enrico Lauth <enrico.lauth@tu-berlin.de>",
     "Ludger Heide <ludger.heide@tu-berlin.de",
     "Shuyao Guo <shuyao.guo@tu-berlin.de"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/mpm-tu-berlin/eflips-depot"
```

### Comparing `eflips_depot-3.0.5/PKG-INFO` & `eflips_depot-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-depot
-Version: 3.0.5
+Version: 3.1.5
 Summary: Depot Simulation for eFLIPS
 Home-page: https://github.com/mpm-tu-berlin/eflips-depot
 License: AGPL-3.0-or-later
 Author: Enrico Lauth
 Author-email: enrico.lauth@tu-berlin.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

