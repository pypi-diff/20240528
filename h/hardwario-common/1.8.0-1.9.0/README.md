# Comparing `tmp/hardwario_common-1.8.0.tar.gz` & `tmp/hardwario_common-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardwario_common-1.8.0.tar", max compression
+gzip compressed data, was "hardwario_common-1.9.0.tar", max compression
```

## Comparing `hardwario_common-1.8.0.tar` & `hardwario_common-1.9.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-02-23 09:54:23.984190 hardwario_common-1.8.0/LICENSE
--rw-r--r--   0        0        0     1260 2023-02-23 09:54:23.984190 hardwario_common-1.8.0/README.md
--rw-r--r--   0        0        0     1306 2023-02-23 09:54:39.260301 hardwario_common-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-02-23 09:54:39.260301 hardwario_common-1.8.0/src/hardwario/common/__init__.py
--rw-r--r--   0        0        0     2679 2023-02-23 09:54:23.988190 hardwario_common-1.8.0/src/hardwario/common/cli.py
--rw-r--r--   0        0        0     9319 2023-02-23 09:54:23.988190 hardwario_common-1.8.0/src/hardwario/common/pib.py
--rw-r--r--   0        0        0      331 2023-02-23 09:54:23.988190 hardwario_common-1.8.0/src/hardwario/common/util.py
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 hardwario_common-1.8.0/setup.py
--rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 hardwario_common-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-28 15:05:05.322001 hardwario_common-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1240 2024-05-28 15:05:05.322001 hardwario_common-1.9.0/README.md
+-rw-r--r--   0        0        0     1330 2024-05-28 15:05:14.998010 hardwario_common-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-28 15:05:14.998010 hardwario_common-1.9.0/src/hardwario/common/__init__.py
+-rw-r--r--   0        0        0     2679 2024-05-28 15:05:05.322001 hardwario_common-1.9.0/src/hardwario/common/cli.py
+-rw-r--r--   0        0        0     9319 2024-05-28 15:05:05.322001 hardwario_common-1.9.0/src/hardwario/common/pib.py
+-rw-r--r--   0        0        0      331 2024-05-28 15:05:05.322001 hardwario_common-1.9.0/src/hardwario/common/util.py
+-rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 hardwario_common-1.9.0/PKG-INFO
```

### Comparing `hardwario_common-1.8.0/LICENSE` & `hardwario_common-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hardwario_common-1.8.0/README.md` & `hardwario_common-1.9.0/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-<a href="https://www.hardwario.com/"><img src="https://www.hardwario.com/ci/assets/hw-logo.svg" width="200" alt="HARDWARIO Logo" align="right"></a>
-
-# HARDWARIO Common
-
-[![Main](https://github.com/hardwario/py-hardwario-common/actions/workflows/main.yaml/badge.svg)](https://github.com/hardwario/py-hardwario-common/actions/workflows/main.yaml)
-[![Release](https://img.shields.io/github/release/hardwario/py-hardwario-common.svg)](https://github.com/hardwario/py-hardwario-common/releases)
-[![PyPI](https://img.shields.io/pypi/v/hardwario-common.svg)](https://pypi.org/project/hardwario-common/)
-[![License](https://img.shields.io/github/license/hardwario/py-hardwario-common.svg)](https://github.com/hardwario/py-hardwario-common/blob/master/LICENSE)
-[![Twitter](https://img.shields.io/twitter/follow/hardwario_en.svg?style=social&label=Follow)](https://twitter.com/hardwario_en)
-
-This repository contains Python package [hardwario-common](https://pypi.org/project/hardwario-common/)
-
-
-## License
-
-This project is licensed under the [MIT License](https://opensource.org/licenses/MIT/) - see the [LICENSE](LICENSE) file for details.
-
----
-
-Made with &#x2764;&nbsp; by [**HARDWARIO a.s.**](https://www.hardwario.com/) in the heart of Europe.
+<a href="https://www.hardwario.com/"><img src="https://www.hardwario.com/ci/assets/hw-logo.svg" width="200" alt="HARDWARIO Logo" align="right"></a>
+
+# HARDWARIO Common
+
+[![Main](https://github.com/hardwario/py-hardwario-common/actions/workflows/main.yaml/badge.svg)](https://github.com/hardwario/py-hardwario-common/actions/workflows/main.yaml)
+[![Release](https://img.shields.io/github/release/hardwario/py-hardwario-common.svg)](https://github.com/hardwario/py-hardwario-common/releases)
+[![PyPI](https://img.shields.io/pypi/v/hardwario-common.svg)](https://pypi.org/project/hardwario-common/)
+[![License](https://img.shields.io/github/license/hardwario/py-hardwario-common.svg)](https://github.com/hardwario/py-hardwario-common/blob/master/LICENSE)
+[![Twitter](https://img.shields.io/twitter/follow/hardwario_en.svg?style=social&label=Follow)](https://twitter.com/hardwario_en)
+
+This repository contains Python package [hardwario-common](https://pypi.org/project/hardwario-common/)
+
+
+## License
+
+This project is licensed under the [MIT License](https://opensource.org/licenses/MIT/) - see the [LICENSE](LICENSE) file for details.
+
+---
+
+Made with &#x2764;&nbsp; by [**HARDWARIO a.s.**](https://www.hardwario.com/) in the heart of Europe.
```

### Comparing `hardwario_common-1.8.0/pyproject.toml` & `hardwario_common-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardwario-common"
-version = "v1.8.0"
+version = "v1.9.0"
 description = "HARDWARIO Common"
 authors = ["Karel Blavka <karel.blavka@hardwario.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hardwario/py-hardwario-common"
 repository = "https://github.com/hardwario/py-hardwario-common"
 classifiers = [
@@ -34,17 +34,18 @@
     "LICENSE",
 ]
 
 [tool.poetry.scripts]
 hardwario = "hardwario.common.cli:main"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
-click = "^8.1.3"
-loguru = "^0.6.0"
+python = ">=3.8"
+click = "^8.1.7"
+loguru = "^0.7.2"
+pycodestyle = "^2.11.1"
 
 [tool.poetry.dev-dependencies]
 pycodestyle = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.10.0"
```

### Comparing `hardwario_common-1.8.0/src/hardwario/common/cli.py` & `hardwario_common-1.9.0/src/hardwario/common/cli.py`

 * *Files identical despite different names*

### Comparing `hardwario_common-1.8.0/src/hardwario/common/pib.py` & `hardwario_common-1.9.0/src/hardwario/common/pib.py`

 * *Files identical despite different names*

### Comparing `hardwario_common-1.8.0/PKG-INFO` & `hardwario_common-1.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: hardwario-common
-Version: 1.8.0
+Version: 1.9.0
 Summary: HARDWARIO Common
 Home-page: https://github.com/hardwario/py-hardwario-common
 License: MIT
 Author: Karel Blavka
 Author-email: karel.blavka@hardwario.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: pycodestyle (>=2.11.1,<3.0.0)
 Project-URL: Repository, https://github.com/hardwario/py-hardwario-common
 Description-Content-Type: text/markdown
 
 <a href="https://www.hardwario.com/"><img src="https://www.hardwario.com/ci/assets/hw-logo.svg" width="200" alt="HARDWARIO Logo" align="right"></a>
 
 # HARDWARIO Common
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1 Name: hardwario-common Version: 1.8.0 Summary: HARDWARIO
+Metadata-Version: 2.1 Name: hardwario-common Version: 1.9.0 Summary: HARDWARIO
 Common Home-page: https://github.com/hardwario/py-hardwario-common License: MIT
 Author: Karel Blavka Author-email: karel.blavka@hardwario.com Requires-Python:
->=3.7 Classifier: Development Status :: 5 - Production/Stable Classifier:
+>=3.8 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
-:: Utilities Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Project-URL: Repository, https://github.com/hardwario/py-
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Utilities Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist: pycodestyle
+(>=2.11.1,<3.0.0) Project-URL: Repository, https://github.com/hardwario/py-
 hardwario-common Description-Content-Type: text/markdown _[_H_A_R_D_W_A_R_I_O_ _L_o_g_o_]#
 HARDWARIO Common [![Main](https://github.com/hardwario/py-hardwario-common/
 actions/workflows/main.yaml/badge.svg)](https://github.com/hardwario/py-
 hardwario-common/actions/workflows/main.yaml) [![Release](https://
 img.shields.io/github/release/hardwario/py-hardwario-common.svg)](https://
 github.com/hardwario/py-hardwario-common/releases) [![PyPI](https://
 img.shields.io/pypi/v/hardwario-common.svg)](https://pypi.org/project/
```

