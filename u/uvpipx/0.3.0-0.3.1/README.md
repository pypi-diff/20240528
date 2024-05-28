# Comparing `tmp/uvpipx-0.3.0.tar.gz` & `tmp/uvpipx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvpipx-0.3.0.tar", max compression
+gzip compressed data, was "uvpipx-0.3.1.tar", max compression
```

## Comparing `uvpipx-0.3.0.tar` & `uvpipx-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35143 2024-05-20 20:45:02.783271 uvpipx-0.3.0/LICENSE
--rw-r--r--   0        0        0     1085 2024-05-20 20:45:02.783271 uvpipx-0.3.0/README.md
--rw-r--r--   0        0        0     1570 2024-05-28 17:10:30.522939 uvpipx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3729 2024-05-26 19:26:28.236343 uvpipx-0.3.0/uvpipx/UvPipxEnv.py
--rw-r--r--   0        0        0        0 2024-05-28 17:10:30.542939 uvpipx-0.3.0/uvpipx/__init__.py
--rw-r--r--   0        0        0     2020 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/__main__.py
--rw-r--r--   0        0        0     3539 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/cmd_launcher.py
--rw-r--r--   0        0        0     1163 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/config.py
--rw-r--r--   0        0        0        0 2024-05-28 17:10:30.542939 uvpipx-0.3.0/uvpipx/internal_libs/__init__.py
--rw-r--r--   0        0        0     7852 2024-05-27 20:27:55.155655 uvpipx-0.3.0/uvpipx/internal_libs/args.py
--rw-r--r--   0        0        0     3550 2024-05-20 20:45:02.783271 uvpipx-0.3.0/uvpipx/internal_libs/colors.py
--rw-r--r--   0        0        0      979 2024-05-20 20:45:02.783271 uvpipx-0.3.0/uvpipx/internal_libs/http_utils.py
--rw-r--r--   0        0        0     7920 2024-05-26 19:26:28.236343 uvpipx-0.3.0/uvpipx/internal_libs/misc.py
--rw-r--r--   0        0        0     3326 2024-05-20 20:45:02.783271 uvpipx-0.3.0/uvpipx/internal_libs/print.py
--rw-r--r--   0        0        0     1933 2024-05-26 19:26:28.236343 uvpipx-0.3.0/uvpipx/req_spec.py
--rw-r--r--   0        0        0      824 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_all.py
--rw-r--r--   0        0        0     4136 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_args.py
--rw-r--r--   0        0        0     2764 2024-05-20 20:45:02.783271 uvpipx-0.3.0/uvpipx/uvpipx_bins.py
--rw-r--r--   0        0        0     3002 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_infos.py
--rw-r--r--   0        0        0     4151 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_inject.py
--rw-r--r--   0        0        0     4433 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_install.py
--rw-r--r--   0        0        0     1756 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/uvpipx_upgrade.py
--rw-r--r--   0        0        0      499 2024-05-28 17:10:30.522939 uvpipx-0.3.0/uvpipx/version.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 uvpipx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35143 2024-05-20 20:45:02.783271 uvpipx-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1216 2024-05-28 17:59:36.032234 uvpipx-0.3.1/README.md
+-rw-r--r--   0        0        0     1570 2024-05-28 20:28:58.881593 uvpipx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3721 2024-05-28 20:18:24.941741 uvpipx-0.3.1/uvpipx/UvPipxEnv.py
+-rw-r--r--   0        0        0        0 2024-05-28 20:29:31.051597 uvpipx-0.3.1/uvpipx/__init__.py
+-rw-r--r--   0        0        0     2020 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/__main__.py
+-rw-r--r--   0        0        0     3539 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/cmd_launcher.py
+-rw-r--r--   0        0        0     1163 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/config.py
+-rw-r--r--   0        0        0        0 2024-05-28 20:29:31.051597 uvpipx-0.3.1/uvpipx/internal_libs/__init__.py
+-rw-r--r--   0        0        0     7852 2024-05-27 20:27:55.155655 uvpipx-0.3.1/uvpipx/internal_libs/args.py
+-rw-r--r--   0        0        0     3550 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/colors.py
+-rw-r--r--   0        0        0      979 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/http_utils.py
+-rw-r--r--   0        0        0     7920 2024-05-26 19:26:28.236343 uvpipx-0.3.1/uvpipx/internal_libs/misc.py
+-rw-r--r--   0        0        0     3326 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/print.py
+-rw-r--r--   0        0        0     1933 2024-05-26 19:26:28.236343 uvpipx-0.3.1/uvpipx/req_spec.py
+-rw-r--r--   0        0        0      824 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_all.py
+-rw-r--r--   0        0        0     4136 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_args.py
+-rw-r--r--   0        0        0     2764 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/uvpipx_bins.py
+-rw-r--r--   0        0        0     3002 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_infos.py
+-rw-r--r--   0        0        0     4151 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_inject.py
+-rw-r--r--   0        0        0     4424 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_install.py
+-rw-r--r--   0        0        0     1756 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_upgrade.py
+-rw-r--r--   0        0        0      499 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/version.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 uvpipx-0.3.1/PKG-INFO
```

### Comparing `uvpipx-0.3.0/LICENSE` & `uvpipx-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/README.md` & `uvpipx-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # uvpipx
 
 ![unpipx logo](https://gitlab.com/pytgaen-group/uvpipx/-/raw/main/uvpipx_logo.jpg)  
-_A small tool like **pipx** using **uv** behind the scene._ ___Fast, Small ...___
+_A small tool like **pipx** using **uv** behind the scene._ _**Fast, Small ...**_
 
 The first intention is to use it in a container or CI, (so with unix) and ⭕ dependency except uv
 
 ## Install the tool (himself 🎉)
 
 ```bash
 pip install uvpipx
@@ -60,8 +60,13 @@
 uvpipx info jc --get-venv
 ```
 
 ## Run a package in venv
 
 ```bash
 wc README.md | uvpipx venv jc -- jc --wc 
-```
+```
+
+## More documentation
+
+[https://uvpipx-pytgaen-group-cc4651f865d7ce5bdaea510cdc656d736634827532.gitlab.io
+](Gitlab pages uvpipx)
```

### Comparing `uvpipx-0.3.0/pyproject.toml` & `uvpipx-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uvpipx"
 description = "A small tool like pipx using uv behind the scene. Fast, Small ..."
-version = "0.3.0" # to bump
+version = "0.3.1" # to bump
 authors = ["Pytgaen <32298455+pytgaen@users.noreply.github.com>"]
 readme = "README.md"
 license = "GPL"
 
 homepage = "https://gitlab.com/pytgaen-group/uvpipx"
 repository = "https://gitlab.com/pytgaen-group/uvpipx"
 # documentation = "https://gitlab.com/pytgaen-group/uvpipx" # gitlab page
```

### Comparing `uvpipx-0.3.0/uvpipx/UvPipxEnv.py` & `uvpipx-0.3.1/uvpipx/UvPipxEnv.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def exists(self) -> bool:
         return self.pck_venv.exists()
 
     def saved_bin_exposed(self) -> List[ExposeBin]:
         return [
             ExposeBin(
-                venv_path=self.pck_venv / "bin",
+                venv_path=self.pck_venv,
                 venv_bin_name=Path(exposed_bin[0]).name,
                 local_bin_path=Path(exposed_bin[1]),
             )
             for exposed_bin in self.uvpipx_dict.get("exposed_bins", [])
         ]
 
     def load(self) -> None:
```

### Comparing `uvpipx-0.3.0/uvpipx/__main__.py` & `uvpipx-0.3.1/uvpipx/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from uvpipx.internal_libs.colors import Painter
 from uvpipx.version import show_version
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import uvpipx.cmd_launcher as cmd_launcher
 
 # import (
```

### Comparing `uvpipx-0.3.0/uvpipx/cmd_launcher.py` & `uvpipx-0.3.1/uvpipx/cmd_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import os
 import sys
```

### Comparing `uvpipx-0.3.0/uvpipx/config.py` & `uvpipx-0.3.1/uvpipx/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import os
 from pathlib import Path
```

### Comparing `uvpipx-0.3.0/uvpipx/internal_libs/args.py` & `uvpipx-0.3.1/uvpipx/internal_libs/args.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/internal_libs/colors.py` & `uvpipx-0.3.1/uvpipx/internal_libs/colors.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/internal_libs/http_utils.py` & `uvpipx-0.3.1/uvpipx/internal_libs/http_utils.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/internal_libs/misc.py` & `uvpipx-0.3.1/uvpipx/internal_libs/misc.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/internal_libs/print.py` & `uvpipx-0.3.1/uvpipx/internal_libs/print.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/req_spec.py` & `uvpipx-0.3.1/uvpipx/req_spec.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_all.py` & `uvpipx-0.3.1/uvpipx/uvpipx_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from uvpipx.uvpipx_upgrade import upgrade
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from uvpipx import config
 from uvpipx.internal_libs.misc import log_info
```

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_args.py` & `uvpipx-0.3.1/uvpipx/uvpipx_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from uvpipx.internal_libs.args import Arg, ArgParser, ArgParserMode
```

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_bins.py` & `uvpipx-0.3.1/uvpipx/uvpipx_bins.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_infos.py` & `uvpipx-0.3.1/uvpipx/uvpipx_infos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from uvpipx.version import show_version
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import os
```

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_inject.py` & `uvpipx-0.3.1/uvpipx/uvpipx_inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
```

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_install.py` & `uvpipx-0.3.1/uvpipx/uvpipx_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from uvpipx.uvpipx_bins import relink_bins
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
@@ -137,15 +137,15 @@
 
 
 def uninstall(package_name: str, *, venv_name: Union[None, str] = None) -> None:
     venv_name_ = venv_name or package_name
     pck_venv = config.uvpipx_venvs / venv_name_
 
     if not (pck_venv / ".venv").exists():
-        msg = f"🔴 {package_name} not exist or ready (path {pck_venv})"
+        msg = f"🔴 {package_name} not exist (path {pck_venv})"
         raise RuntimeError(msg)
 
     with (pck_venv / "uvpipx.json").open() as outfile:
         uvpipx_dict = json.load(
             outfile,
         )
```

### Comparing `uvpipx-0.3.0/uvpipx/uvpipx_upgrade.py` & `uvpipx-0.3.1/uvpipx/uvpipx_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from uvpipx.uvpipx_bins import relink_bins
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.0"  # to bump
+__version__ = "0.3.1"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
```

### Comparing `uvpipx-0.3.0/PKG-INFO` & `uvpipx-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvpipx
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small tool like pipx using uv behind the scene. Fast, Small ...
 Home-page: https://gitlab.com/pytgaen-group/uvpipx
 License: GPL
 Author: Pytgaen
 Author-email: 32298455+pytgaen@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -17,15 +17,15 @@
 Requires-Dist: uv (>=0.1.45,<1.0.0)
 Project-URL: Repository, https://gitlab.com/pytgaen-group/uvpipx
 Description-Content-Type: text/markdown
 
 # uvpipx
 
 ![unpipx logo](https://gitlab.com/pytgaen-group/uvpipx/-/raw/main/uvpipx_logo.jpg)  
-_A small tool like **pipx** using **uv** behind the scene._ ___Fast, Small ...___
+_A small tool like **pipx** using **uv** behind the scene._ _**Fast, Small ...**_
 
 The first intention is to use it in a container or CI, (so with unix) and ⭕ dependency except uv
 
 ## Install the tool (himself 🎉)
 
 ```bash
 pip install uvpipx
@@ -81,7 +81,13 @@
 ```
 
 ## Run a package in venv
 
 ```bash
 wc README.md | uvpipx venv jc -- jc --wc 
 ```
+
+## More documentation
+
+[https://uvpipx-pytgaen-group-cc4651f865d7ce5bdaea510cdc656d736634827532.gitlab.io
+](Gitlab pages uvpipx)
+
```

