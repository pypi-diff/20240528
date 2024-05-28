# Comparing `tmp/py-cdhit-0.8.0.tar.gz` & `tmp/py-cdhit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-cdhit-0.8.0.tar", last modified: Mon Dec  4 14:04:59 2023, max compression
+gzip compressed data, was "py-cdhit-0.9.0.tar", last modified: Sat Dec 16 09:51:08 2023, max compression
```

## Comparing `py-cdhit-0.8.0.tar` & `py-cdhit-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-04 14:04:59.602944 py-cdhit-0.8.0/
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)    18092 2023-05-25 10:50:44.000000 py-cdhit-0.8.0/LICENSE
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)    23677 2023-12-04 14:04:59.582168 py-cdhit-0.8.0/PKG-INFO
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1878 2023-12-04 14:02:44.000000 py-cdhit-0.8.0/README.md
-drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-04 14:04:59.550923 py-cdhit-0.8.0/py_cdhit.egg-info/
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)    23677 2023-12-04 14:04:59.000000 py-cdhit-0.8.0/py_cdhit.egg-info/PKG-INFO
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)      325 2023-12-04 14:04:59.000000 py-cdhit-0.8.0/py_cdhit.egg-info/SOURCES.txt
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)        1 2023-12-04 14:04:59.000000 py-cdhit-0.8.0/py_cdhit.egg-info/dependency_links.txt
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)      122 2023-12-04 14:04:59.000000 py-cdhit-0.8.0/py_cdhit.egg-info/requires.txt
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)        8 2023-12-04 14:04:59.000000 py-cdhit-0.8.0/py_cdhit.egg-info/top_level.txt
-drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-04 14:04:59.439878 py-cdhit-0.8.0/pycdhit/
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)      431 2023-12-04 13:34:42.000000 py-cdhit-0.8.0/pycdhit/__init__.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     4157 2023-10-07 05:44:09.000000 py-cdhit-0.8.0/pycdhit/_class.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     2131 2023-10-08 06:44:01.000000 py-cdhit-0.8.0/pycdhit/_commands.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     3205 2023-05-27 14:26:21.000000 py-cdhit-0.8.0/pycdhit/_io.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1090 2023-11-14 14:46:09.000000 py-cdhit-0.8.0/pyproject.toml
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)       38 2023-12-04 14:04:59.603623 py-cdhit-0.8.0/setup.cfg
-drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-04 14:04:59.518539 py-cdhit-0.8.0/tests/
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1186 2023-05-28 07:59:04.000000 py-cdhit-0.8.0/tests/test_class.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)      830 2023-05-26 06:48:11.000000 py-cdhit-0.8.0/tests/test_commands.py
--rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1615 2023-05-23 09:39:16.000000 py-cdhit-0.8.0/tests/test_io.py
+drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-16 09:51:08.853747 py-cdhit-0.9.0/
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)    18092 2023-05-25 10:50:44.000000 py-cdhit-0.9.0/LICENSE
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)    23791 2023-12-16 09:51:08.850445 py-cdhit-0.9.0/PKG-INFO
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1992 2023-12-16 09:47:01.000000 py-cdhit-0.9.0/README.md
+drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-16 09:51:08.822802 py-cdhit-0.9.0/py_cdhit.egg-info/
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)    23791 2023-12-16 09:51:08.000000 py-cdhit-0.9.0/py_cdhit.egg-info/PKG-INFO
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)      325 2023-12-16 09:51:08.000000 py-cdhit-0.9.0/py_cdhit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)        1 2023-12-16 09:51:08.000000 py-cdhit-0.9.0/py_cdhit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)      122 2023-12-16 09:51:08.000000 py-cdhit-0.9.0/py_cdhit.egg-info/requires.txt
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)        8 2023-12-16 09:51:08.000000 py-cdhit-0.9.0/py_cdhit.egg-info/top_level.txt
+drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-16 09:51:08.733725 py-cdhit-0.9.0/pycdhit/
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)      431 2023-12-16 09:47:24.000000 py-cdhit-0.9.0/pycdhit/__init__.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     4157 2023-12-06 15:57:33.000000 py-cdhit-0.9.0/pycdhit/_class.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     2131 2023-12-06 15:57:33.000000 py-cdhit-0.9.0/pycdhit/_commands.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     3205 2023-12-06 15:57:33.000000 py-cdhit-0.9.0/pycdhit/_io.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1090 2023-12-06 15:57:33.000000 py-cdhit-0.9.0/pyproject.toml
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)       38 2023-12-16 09:51:08.853747 py-cdhit-0.9.0/setup.cfg
+drwxrwxrwx   0 xiao      (1000) xiao      (1000)        0 2023-12-16 09:51:08.795361 py-cdhit-0.9.0/tests/
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1186 2023-12-06 15:57:33.000000 py-cdhit-0.9.0/tests/test_class.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)      830 2023-05-26 06:48:11.000000 py-cdhit-0.9.0/tests/test_commands.py
+-rwxrwxrwx   0 xiao      (1000) xiao      (1000)     1615 2023-05-23 09:39:16.000000 py-cdhit-0.9.0/tests/test_io.py
```

### Comparing `py-cdhit-0.8.0/LICENSE` & `py-cdhit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/PKG-INFO` & `py-cdhit-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-cdhit
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python interface for CD-HIT package.
 Author-email: Xiao Yuan <yuanx749@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -362,14 +362,15 @@
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: notebook>=6.5.4; extra == "dev"
 
 # py-cdhit
 
 [![PyPI version](https://badge.fury.io/py/py-cdhit.svg)](https://badge.fury.io/py/py-cdhit)
+[![Downloads](https://static.pepy.tech/badge/py-cdhit/month)](https://pepy.tech/project/py-cdhit)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/197a0be6dcd14961b919e666a0de39eb)](https://app.codacy.com/gh/yuanx749/py-cdhit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 A Python interface for CD-HIT package.
 
 Read the documentation [here](https://yuanx749.github.io/py-cdhit/).
 
 ## Description
@@ -404,15 +405,15 @@
 
 ```bash
 mamba create -n myenv python=3.10
 mamba activate myenv
 ```
 
 ```bash
-mamba install -c bioconda cd-hit
+mamba install -c bioconda cd-hit cd-hit-auxtools
 ```
 
 Then install this package from PyPI:
 
 ```bash
 pip install py-cdhit
 ```
```

### Comparing `py-cdhit-0.8.0/README.md` & `py-cdhit-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # py-cdhit
 
 [![PyPI version](https://badge.fury.io/py/py-cdhit.svg)](https://badge.fury.io/py/py-cdhit)
+[![Downloads](https://static.pepy.tech/badge/py-cdhit/month)](https://pepy.tech/project/py-cdhit)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/197a0be6dcd14961b919e666a0de39eb)](https://app.codacy.com/gh/yuanx749/py-cdhit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 A Python interface for CD-HIT package.
 
 Read the documentation [here](https://yuanx749.github.io/py-cdhit/).
 
 ## Description
@@ -39,15 +40,15 @@
 
 ```bash
 mamba create -n myenv python=3.10
 mamba activate myenv
 ```
 
 ```bash
-mamba install -c bioconda cd-hit
+mamba install -c bioconda cd-hit cd-hit-auxtools
 ```
 
 Then install this package from PyPI:
 
 ```bash
 pip install py-cdhit
 ```
```

### Comparing `py-cdhit-0.8.0/py_cdhit.egg-info/PKG-INFO` & `py-cdhit-0.9.0/py_cdhit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-cdhit
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python interface for CD-HIT package.
 Author-email: Xiao Yuan <yuanx749@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -362,14 +362,15 @@
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: notebook>=6.5.4; extra == "dev"
 
 # py-cdhit
 
 [![PyPI version](https://badge.fury.io/py/py-cdhit.svg)](https://badge.fury.io/py/py-cdhit)
+[![Downloads](https://static.pepy.tech/badge/py-cdhit/month)](https://pepy.tech/project/py-cdhit)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/197a0be6dcd14961b919e666a0de39eb)](https://app.codacy.com/gh/yuanx749/py-cdhit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 A Python interface for CD-HIT package.
 
 Read the documentation [here](https://yuanx749.github.io/py-cdhit/).
 
 ## Description
@@ -404,15 +405,15 @@
 
 ```bash
 mamba create -n myenv python=3.10
 mamba activate myenv
 ```
 
 ```bash
-mamba install -c bioconda cd-hit
+mamba install -c bioconda cd-hit cd-hit-auxtools
 ```
 
 Then install this package from PyPI:
 
 ```bash
 pip install py-cdhit
 ```
```

### Comparing `py-cdhit-0.8.0/pycdhit/_class.py` & `py-cdhit-0.9.0/pycdhit/_class.py`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/pycdhit/_commands.py` & `py-cdhit-0.9.0/pycdhit/_commands.py`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/pycdhit/_io.py` & `py-cdhit-0.9.0/pycdhit/_io.py`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/pyproject.toml` & `py-cdhit-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/tests/test_class.py` & `py-cdhit-0.9.0/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/tests/test_commands.py` & `py-cdhit-0.9.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `py-cdhit-0.8.0/tests/test_io.py` & `py-cdhit-0.9.0/tests/test_io.py`

 * *Files identical despite different names*

