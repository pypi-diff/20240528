# Comparing `tmp/easy_gui_prompt-2024.5.24.tar.gz` & `tmp/easy_gui_prompt-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gui_prompt-2024.5.24.tar", max compression
+gzip compressed data, was "easy_gui_prompt-2024.5.28.tar", max compression
```

## Comparing `easy_gui_prompt-2024.5.24.tar` & `easy_gui_prompt-2024.5.28.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1104 2024-05-24 12:17:21.219473 easy_gui_prompt-2024.5.24/LICENSE.txt
--rw-r--r--   0        0        0     1629 2024-05-24 12:51:02.146726 easy_gui_prompt-2024.5.24/README.md
--rw-r--r--   0        0        0      114 2024-05-24 12:45:42.594202 easy_gui_prompt-2024.5.24/easy_gui_prompt/__init__.py
--rw-r--r--   0        0        0     4159 2024-05-24 12:49:14.744717 easy_gui_prompt-2024.5.24/easy_gui_prompt/easy_gui_prompt.py
--rw-r--r--   0        0        0      723 2024-05-24 12:46:50.975345 easy_gui_prompt-2024.5.24/pyproject.toml
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 easy_gui_prompt-2024.5.24/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-24 12:17:21.219473 easy_gui_prompt-2024.5.28/LICENSE.txt
+-rw-r--r--   0        0        0     1757 2024-05-24 13:22:11.101035 easy_gui_prompt-2024.5.28/README.md
+-rw-r--r--   0        0        0      114 2024-05-24 12:45:42.594202 easy_gui_prompt-2024.5.28/easy_gui_prompt/__init__.py
+-rw-r--r--   0        0        0     7255 2024-05-28 11:13:28.760907 easy_gui_prompt-2024.5.28/easy_gui_prompt/easy_gui_prompt.py
+-rw-r--r--   0        0        0      779 2024-05-28 11:13:50.268736 easy_gui_prompt-2024.5.28/pyproject.toml
+-rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 easy_gui_prompt-2024.5.28/PKG-INFO
```

### Comparing `easy_gui_prompt-2024.5.24/LICENSE.txt` & `easy_gui_prompt-2024.5.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_gui_prompt-2024.5.24/README.md` & `easy_gui_prompt-2024.5.28/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-Here is a suggested README.md for the easy_gui_prompt project:
-
-```markdown
-# easy_gui_prompt
+# Easy GUI Prompt
 
+[![PyPI version](https://badge.fury.io/py/easy_gui_prompt.svg)](https://badge.fury.io/py/easy_gui_prompt)
+[![Python versions](https://img.shields.io/pypi/pyversions/easy_gui_prompt.svg)](https://pypi.org/project/easy_gui_prompt/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A Python library to simplify the creation of GUI elements in the terminal using prompt-toolkit.
 
 ## Installation
 
 Install easy_gui_prompt using pip:
@@ -52,23 +51,22 @@
 
 ```python
 gui.restore_default_settings()
 ```
 
 ## Configuration
 
-The library automatically saves user preferences to a configuration file located at `~/.easy_gui/easy_gui.yml`. This allows the GUI to remember the last entered values when `remember_value=True` is used.
+The library automatically saves user preferences to onfiguration files in `~/.easy_gui/`. This allows the GUI to remember the last entered values when `remember_value=True` is used.
 
 You can also access the configuration directly using the `get_config` and `save_config` functions:
 
 ```python
 from easy_gui_prompt import get_config, save_config
 
 config = get_config("My GUI")
 save_config("My GUI", config)
 ```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.
-```
```

### Comparing `easy_gui_prompt-2024.5.24/pyproject.toml` & `easy_gui_prompt-2024.5.28/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "easy_gui_prompt"
-version = "2024.05.24"
+version = "2024.05.28"
 description = "Simplify the creation of GUI elements in the terminal"
-authors = [ "Ricardo Henriques <ricardo@henriqueslab.org>", "Bruno Saraiva <bruno.msaraiva2@gmail.com>", "António Brito <antmsbrito95@gmail.com>",]
+license = "MIT"
+repository = "https://github.com/HenriquesLab/easy-gui-prompt"
+authors = [ "Ricardo Henriques <ricardo@henriqueslab.org>", "Bruno Saraiva <bruno.msaraiva2@gmail.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyyaml = "^6.0.1"
 toml = "^0.10.2"
 prompt-toolkit = "^3.0.43"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests",]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 ruff = "^0.4.3"
+lazydocs = "^0.4.8"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 pytest-xdist = "^3.6.1"
 gptrepo = "^1.0.3"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easy_gui_prompt-2024.5.24/PKG-INFO` & `easy_gui_prompt-2024.5.28/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: easy_gui_prompt
-Version: 2024.5.24
+Version: 2024.5.28
 Summary: Simplify the creation of GUI elements in the terminal
+Home-page: https://github.com/HenriquesLab/easy-gui-prompt
+License: MIT
 Author: Ricardo Henriques
 Author-email: ricardo@henriqueslab.org
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/HenriquesLab/easy-gui-prompt
 Description-Content-Type: text/markdown
 
-Here is a suggested README.md for the easy_gui_prompt project:
-
-```markdown
-# easy_gui_prompt
+# Easy GUI Prompt
 
+[![PyPI version](https://badge.fury.io/py/easy_gui_prompt.svg)](https://badge.fury.io/py/easy_gui_prompt)
+[![Python versions](https://img.shields.io/pypi/pyversions/easy_gui_prompt.svg)](https://pypi.org/project/easy_gui_prompt/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A Python library to simplify the creation of GUI elements in the terminal using prompt-toolkit.
 
 ## Installation
 
 Install easy_gui_prompt using pip:
@@ -68,24 +71,23 @@
 
 ```python
 gui.restore_default_settings()
 ```
 
 ## Configuration
 
-The library automatically saves user preferences to a configuration file located at `~/.easy_gui/easy_gui.yml`. This allows the GUI to remember the last entered values when `remember_value=True` is used.
+The library automatically saves user preferences to onfiguration files in `~/.easy_gui/`. This allows the GUI to remember the last entered values when `remember_value=True` is used.
 
 You can also access the configuration directly using the `get_config` and `save_config` functions:
 
 ```python
 from easy_gui_prompt import get_config, save_config
 
 config = get_config("My GUI")
 save_config("My GUI", config)
 ```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.
-```
```

