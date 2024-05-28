# Comparing `tmp/geoh5_interop-1.0.0rc3.tar.gz` & `tmp/geoh5_interop-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5_interop-1.0.0rc3.tar", max compression
+gzip compressed data, was "geoh5_interop-1.0.0rc4.tar", max compression
```

## Comparing `geoh5_interop-1.0.0rc3.tar` & `geoh5_interop-1.0.0rc4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      710 2024-05-15 19:24:07.529542 geoh5_interop-1.0.0rc3/geoh5_interop/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 geoh5_interop-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     2020 2024-05-15 19:24:07.517457 geoh5_interop-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2348 2024-05-06 20:54:07.468238 geoh5_interop-1.0.0rc3/README.rst
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 geoh5_interop-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      710 2024-05-28 16:35:44.020060 geoh5_interop-1.0.0rc4/geoh5_interop/__init__.py
+-rw-r--r--   0        0        0     1093 2024-05-18 03:12:25.093921 geoh5_interop-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     2026 2024-05-28 16:35:19.441762 geoh5_interop-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     2348 2024-05-18 03:12:25.093921 geoh5_interop-1.0.0rc4/README.rst
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 geoh5_interop-1.0.0rc4/PKG-INFO
```

### Comparing `geoh5_interop-1.0.0rc3/geoh5_interop/__init__.py` & `geoh5_interop-1.0.0rc4/geoh5_interop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 #                                                                                 '
 #  This file is part of geoh5-interop meta-package.                               '
 #                                                                                 '
 #  geoh5-interop is distributed under the terms and conditions of the MIT License '
 #  (see LICENSE file at the root of this source code package).                    '
 # '''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
-__version__ = "1.0.0-rc.3"
+__version__ = "1.0.0-rc.4"
```

### Comparing `geoh5_interop-1.0.0rc3/LICENSE` & `geoh5_interop-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `geoh5_interop-1.0.0rc3/pyproject.toml` & `geoh5_interop-1.0.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5-interop"
-version = "1.0.0-rc.3"
+version = "1.0.0-rc.4"
 license = "MIT"
 description = "A meta-package that groups together packages for interoperability between GEOH5 and other file formats."
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 readme = "README.rst"
 keywords = ["geology", "geophysics", "data", "interoperability"]
 classifiers = [
@@ -24,26 +24,26 @@
     "COPYING.LESSER",
     "LICENSE",
     "README.rst",
     "THIRD_PARTY_SOFTWARE.rst",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.10,<3.11"
 
 # geoh5py is a dependency of other apps: not strictly needed here, but good to ensure version
 geoh5py = {version = "~0.9.0rc3", source = "pypi", allow-prereleases = true}
 #geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 #geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
-mira-omf = {version = "~3.2.0rc1", source = "pypi", allow-prereleases = true}
+mira-omf = {version = "~3.2.0rc2", source = "pypi", allow-prereleases = true}
 #mira-omf = {url = "https://github.com/MiraGeoscience/omf/archive/refs/heads/release/3.2.0.zip#sha256="}
 #mira-omf = {url = "http://localhost:8888/mira-omf.tar.gz#sha256="}
 
-las-geoh5 = { version = "~0.2.0rc2", source = "pypi", allow-prereleases = true}
+las-geoh5 = { version = "~0.2.0rc4", source = "pypi", allow-prereleases = true}
 #las-geoh5 = {url = "https://github.com/MiraGeoscience/las-geoh5/archive/refs/heads/release/0.2.0.zip#sha256="}
 #las-geoh5 = {url = "http://localhost:8888/las-geoh5.tar.gz#sha256="}
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geoh5_interop-1.0.0rc3/README.rst` & `geoh5_interop-1.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `geoh5_interop-1.0.0rc3/PKG-INFO` & `geoh5_interop-1.0.0rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: geoh5-interop
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: A meta-package that groups together packages for interoperability between GEOH5 and other file formats.
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: geoh5py (>=0.9.0rc3,<0.10.0)
-Requires-Dist: las-geoh5 (>=0.2.0rc2,<0.3.0)
-Requires-Dist: mira-omf (>=3.2.0rc1,<3.3.0)
+Requires-Dist: las-geoh5 (>=0.2.0rc4,<0.3.0)
+Requires-Dist: mira-omf (>=3.2.0rc2,<3.3.0)
 Description-Content-Type: text/x-rst
 
 |version| |status| |pyversions|
 
 
 .. |version| image:: https://img.shields.io/pypi/v/geoh5-interop.svg
     :alt: version on PyPI
```

