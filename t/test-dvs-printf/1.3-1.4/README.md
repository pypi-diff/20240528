# Comparing `tmp/test_dvs_printf-1.3.tar.gz` & `tmp/test_dvs_printf-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_dvs_printf-1.3.tar", last modified: Tue May 28 12:09:32 2024, max compression
+gzip compressed data, was "test_dvs_printf-1.4.tar", last modified: Tue May 28 12:14:00 2024, max compression
```

## Comparing `test_dvs_printf-1.3.tar` & `test_dvs_printf-1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:09:32.805252 test_dvs_printf-1.3/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 test_dvs_printf-1.3/LICENSE
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       73 2024-05-27 04:55:17.000000 test_dvs_printf-1.3/MANIFEST.in
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4622 2024-05-28 12:09:32.805025 test_dvs_printf-1.3/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3818 2024-05-26 15:52:22.000000 test_dvs_printf-1.3/README.md
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 test_dvs_printf-1.3/pyproject.toml
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-05-28 12:09:32.805300 test_dvs_printf-1.3/setup.cfg
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1027 2024-05-28 12:08:39.000000 test_dvs_printf-1.3/setup.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:09:32.802395 test_dvs_printf-1.3/test_dvs_printf/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-05-28 12:08:56.000000 test_dvs_printf-1.3/test_dvs_printf/__Loding__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 test_dvs_printf-1.3/test_dvs_printf/__init.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-28 12:08:57.000000 test_dvs_printf-1.3/test_dvs_printf/__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-28 12:08:53.000000 test_dvs_printf-1.3/test_dvs_printf/__printf__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-28 12:08:52.000000 test_dvs_printf-1.3/test_dvs_printf/oth_styles.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:09:32.804736 test_dvs_printf-1.3/test_dvs_printf.egg-info/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4622 2024-05-28 12:09:32.000000 test_dvs_printf-1.3/test_dvs_printf.egg-info/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      537 2024-05-28 12:09:32.000000 test_dvs_printf-1.3/test_dvs_printf.egg-info/SOURCES.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-05-28 12:09:32.000000 test_dvs_printf-1.3/test_dvs_printf.egg-info/dependency_links.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       16 2024-05-28 12:09:32.000000 test_dvs_printf-1.3/test_dvs_printf.egg-info/top_level.txt
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:09:32.804551 test_dvs_printf-1.3/tests/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-05-28 12:08:48.000000 test_dvs_printf-1.3/tests/test_Numpy.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      973 2024-05-28 12:08:47.000000 test_dvs_printf-1.3/tests/test_Pandas.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      967 2024-05-28 12:08:45.000000 test_dvs_printf-1.3/tests/test_PyTorch.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1228 2024-05-28 12:08:43.000000 test_dvs_printf-1.3/tests/test_Tensorflow.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      900 2024-05-28 12:08:50.000000 test_dvs_printf-1.3/tests/test__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      377 2024-05-28 12:08:38.000000 test_dvs_printf-1.3/tests/test_arrayToList.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1548 2024-05-28 12:08:49.000000 test_dvs_printf-1.3/tests/test_listfunction.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      215 2024-05-28 12:08:41.000000 test_dvs_printf-1.3/tests/test_loding.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:14:00.180513 test_dvs_printf-1.4/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 test_dvs_printf-1.4/LICENSE
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       73 2024-05-27 04:55:17.000000 test_dvs_printf-1.4/MANIFEST.in
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4632 2024-05-28 12:14:00.180283 test_dvs_printf-1.4/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3828 2024-05-28 12:13:10.000000 test_dvs_printf-1.4/README.md
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 test_dvs_printf-1.4/pyproject.toml
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-05-28 12:14:00.180560 test_dvs_printf-1.4/setup.cfg
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1027 2024-05-28 12:13:34.000000 test_dvs_printf-1.4/setup.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:14:00.176910 test_dvs_printf-1.4/test_dvs_printf/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-05-28 12:08:56.000000 test_dvs_printf-1.4/test_dvs_printf/__Loding__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 test_dvs_printf-1.4/test_dvs_printf/__init.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-28 12:08:57.000000 test_dvs_printf-1.4/test_dvs_printf/__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-28 12:08:53.000000 test_dvs_printf-1.4/test_dvs_printf/__printf__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-28 12:08:52.000000 test_dvs_printf-1.4/test_dvs_printf/oth_styles.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:14:00.179970 test_dvs_printf-1.4/test_dvs_printf.egg-info/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4632 2024-05-28 12:14:00.000000 test_dvs_printf-1.4/test_dvs_printf.egg-info/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      537 2024-05-28 12:14:00.000000 test_dvs_printf-1.4/test_dvs_printf.egg-info/SOURCES.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-05-28 12:14:00.000000 test_dvs_printf-1.4/test_dvs_printf.egg-info/dependency_links.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       16 2024-05-28 12:14:00.000000 test_dvs_printf-1.4/test_dvs_printf.egg-info/top_level.txt
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-28 12:14:00.179647 test_dvs_printf-1.4/tests/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-05-28 12:08:48.000000 test_dvs_printf-1.4/tests/test_Numpy.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      973 2024-05-28 12:08:47.000000 test_dvs_printf-1.4/tests/test_Pandas.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      967 2024-05-28 12:08:45.000000 test_dvs_printf-1.4/tests/test_PyTorch.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1228 2024-05-28 12:08:43.000000 test_dvs_printf-1.4/tests/test_Tensorflow.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      900 2024-05-28 12:08:50.000000 test_dvs_printf-1.4/tests/test__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      377 2024-05-28 12:08:38.000000 test_dvs_printf-1.4/tests/test_arrayToList.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1548 2024-05-28 12:08:49.000000 test_dvs_printf-1.4/tests/test_listfunction.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      215 2024-05-28 12:08:41.000000 test_dvs_printf-1.4/tests/test_loding.py
```

### Comparing `test_dvs_printf-1.3/LICENSE` & `test_dvs_printf-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/PKG-INFO` & `test_dvs_printf-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_dvs_printf
-Version: 1.3
+Version: 1.4
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: dhruvan_vyas
 License: MIT License
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: hii, https://pypi.org/project/dvs-printf
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/test-dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.3 Summary: Animated
+Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.4 Summary: Animated
 Visual appearance for console-based applications, with different animation
 styles Home-page: https://github.com/dhruvan-vyas/dvs_printf Author:
 dhruvan_vyas License: MIT License Project-URL: Documentation, https://
 github.com/dhruvan-vyas/dvs_printf/blob/main/README.md Project-URL: hii, https:
 //pypi.org/project/dvs-printf Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Utilities Classifier: Environment :: Console Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-      [![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
+badge.fury.io/py/test-dvs-printf) [![Build Status](https://github.com/dhruvan-
+    vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://
+github.com/dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)]
+  (https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://
+             github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.3/README.md` & `test_dvs_printf-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/test-dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-      [![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
+badge.fury.io/py/test-dvs-printf) [![Build Status](https://github.com/dhruvan-
+    vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://
+github.com/dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)]
+  (https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://
+             github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.3/setup.py` & `test_dvs_printf-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib, setuptools
 
 setuptools.setup(
     name="test_dvs_printf",
-    version="1.3",
+    version="1.4",
     description=
 "Animated Visual appearance for console-based applications, with different animation styles",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/dhruvan-vyas/dvs_printf",
     author="dhruvan_vyas",
     license="MIT License",
```

### Comparing `test_dvs_printf-1.3/test_dvs_printf/__Loding__.py` & `test_dvs_printf-1.4/test_dvs_printf/__Loding__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/test_dvs_printf/__init.py` & `test_dvs_printf-1.4/test_dvs_printf/__init.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/test_dvs_printf/__init__.py` & `test_dvs_printf-1.4/test_dvs_printf/__init__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/test_dvs_printf/__printf__.py` & `test_dvs_printf-1.4/test_dvs_printf/__printf__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/test_dvs_printf/oth_styles.py` & `test_dvs_printf-1.4/test_dvs_printf/oth_styles.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/test_dvs_printf.egg-info/PKG-INFO` & `test_dvs_printf-1.4/test_dvs_printf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_dvs_printf
-Version: 1.3
+Version: 1.4
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: dhruvan_vyas
 License: MIT License
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: hii, https://pypi.org/project/dvs-printf
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/test-dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.3 Summary: Animated
+Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.4 Summary: Animated
 Visual appearance for console-based applications, with different animation
 styles Home-page: https://github.com/dhruvan-vyas/dvs_printf Author:
 dhruvan_vyas License: MIT License Project-URL: Documentation, https://
 github.com/dhruvan-vyas/dvs_printf/blob/main/README.md Project-URL: hii, https:
 //pypi.org/project/dvs-printf Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Utilities Classifier: Environment :: Console Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-      [![PyPI Version](https://badge.fury.io/py/dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
+badge.fury.io/py/test-dvs-printf) [![Build Status](https://github.com/dhruvan-
+    vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://
+github.com/dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)]
+  (https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://
+             github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.3/test_dvs_printf.egg-info/SOURCES.txt` & `test_dvs_printf-1.4/test_dvs_printf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test_Numpy.py` & `test_dvs_printf-1.4/tests/test_Numpy.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test_Pandas.py` & `test_dvs_printf-1.4/tests/test_Pandas.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test_PyTorch.py` & `test_dvs_printf-1.4/tests/test_PyTorch.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test_Tensorflow.py` & `test_dvs_printf-1.4/tests/test_Tensorflow.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test__init__.py` & `test_dvs_printf-1.4/tests/test__init__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.3/tests/test_listfunction.py` & `test_dvs_printf-1.4/tests/test_listfunction.py`

 * *Files identical despite different names*

