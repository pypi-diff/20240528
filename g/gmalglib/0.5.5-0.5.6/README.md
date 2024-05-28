# Comparing `tmp/gmalglib-0.5.5.tar.gz` & `tmp/gmalglib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.5.tar", last modified: Wed May 22 15:53:43 2024, max compression
+gzip compressed data, was "gmalglib-0.5.6.tar", last modified: Tue May 28 00:55:53 2024, max compression
```

## Comparing `gmalglib-0.5.5.tar` & `gmalglib-0.5.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 15:53:39.000000 gmalglib-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:53:43.793902 gmalglib-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-22 15:53:39.000000 gmalglib-0.5.5/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-22 15:53:39.000000 gmalglib-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.785902 gmalglib-0.5.5/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.789902 gmalglib-0.5.5/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 15:53:39.000000 gmalglib-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:53:43.793902 gmalglib-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 15:53:39.000000 gmalglib-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.785902 gmalglib-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.789902 gmalglib-0.5.5/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 00:55:37.000000 gmalglib-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-28 00:55:53.186000 gmalglib-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-28 00:55:37.000000 gmalglib-0.5.6/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-28 00:55:37.000000 gmalglib-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.174000 gmalglib-0.5.6/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.178001 gmalglib-0.5.6/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2table.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 00:55:37.000000 gmalglib-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:55:53.186000 gmalglib-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 00:55:37.000000 gmalglib-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.174000 gmalglib-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.178001 gmalglib-0.5.6/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19181 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)  2810569 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2table.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.5/LICENSE` & `gmalglib-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/PKG-INFO` & `gmalglib-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 pip install gmalglib
 ```
 
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
-  - Key exchange 
+  - Key exchange
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
 - ZUC Stream Cipher Algorithm
 
 ## Usage
 
@@ -72,15 +72,15 @@
 
 If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
 
 ## Benchmark Test
 
-The benchmark test code can be found in `benchmark.py`. The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
+The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
 SM2.encrypt             : 2.391558s
 SM2.decrypt             : 1.092445s
 SM2.sign_digest         : 1.062552s
 SM2.verify_digest       : 2.096187s
```

### Comparing `gmalglib-0.5.5/README.en.md` & `gmalglib-0.5.6/README.en.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pip install gmalglib
 ```
 
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
-  - Key exchange 
+  - Key exchange
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
 - ZUC Stream Cipher Algorithm
 
 ## Usage
 
@@ -55,15 +55,15 @@
 
 If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
 
 ## Benchmark Test
 
-The benchmark test code can be found in `benchmark.py`. The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
+The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
 SM2.encrypt             : 2.391558s
 SM2.decrypt             : 1.092445s
 SM2.sign_digest         : 1.062552s
 SM2.verify_digest       : 2.096187s
```

### Comparing `gmalglib-0.5.5/README.md` & `gmalglib-0.5.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,27 +58,27 @@
 
 如不传入随机数发生器, 则使用默认的系统相关随机数发生器, 在 Windows 下使用 `BCryptGenRandom`, 其余系统使用 `/dev/urandom` 实现, 其实现类似于 Python 标准库函数 [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 具体实现见 [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) 内 `OsRandomProc`.
 
 ## 性能测试
 
-性能测试代码见 `benchmark.py`, `13th Gen Intel(R) Core(TM) i7-13700H` 上测试结果如下:
+性能测试代码见 [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py), `13th Gen Intel(R) Core(TM) i7-13700H` 上测试结果如下:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 2.391558s
-SM2.decrypt             : 1.092445s
-SM2.sign_digest         : 1.062552s
-SM2.verify_digest       : 2.096187s
-SM2.sign                : 1.067850s
-SM2.verify              : 2.055190s
-SM2.begin_key_exchange  : 1.159822s
-SM2.end_key_exchange    : 1.633471s
+SM2.encrypt             : 0.766956s
+SM2.decrypt             : 0.678737s
+SM2.sign_digest         : 0.100963s
+SM2.verify_digest       : 0.707086s
+SM2.sign                : 0.100675s
+SM2.verify              : 0.729823s
+SM2.begin_key_exchange  : 0.153279s
+SM2.end_key_exchange    : 0.988622s
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 5.118763s
+SM3.update & SM3.digest : 3.014004s
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.369991s
-SM4.decrypt             : 0.297077s
+SM4.encrypt             : 0.185529s
+SM4.decrypt             : 0.184629s
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.050301s
+zuc.generate            : 0.029673s
 ```
```

### Comparing `gmalglib-0.5.5/include/gmalglib/bignum.h` & `gmalglib-0.5.6/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/include/gmalglib/random.h` & `gmalglib-0.5.6/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/include/gmalglib/sm2.h` & `gmalglib-0.5.6/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/include/gmalglib/sm2curve.h` & `gmalglib-0.5.6/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/include/gmalglib/sm3.h` & `gmalglib-0.5.6/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/pyproject.toml` & `gmalglib-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/setup.py` & `gmalglib-0.5.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,27 +5,29 @@
     sources=[
         "src/gmalglib/coremodule.c",
         "src/gmalglib/core/sm3.c",
         "src/gmalglib/core/sm4.c",
         "src/gmalglib/core/zuc.c",
         "src/gmalglib/core/bignum.c",
         "src/gmalglib/core/random.c",
+        "src/gmalglib/core/sm2table.c",
         "src/gmalglib/core/sm2curve.c",
         "src/gmalglib/core/sm2.c",
     ],
     include_dirs=[
         "include",
         "include/python3",
     ],
     depends=[
         "include/gmalglib/sm3.h",
         "include/gmalglib/sm4.h",
         "include/gmalglib/zuc.h",
         "include/gmalglib/bignum.h",
         "include/gmalglib/random.h",
+        "include/gmalglib/sm2table.h",
         "include/gmalglib/sm2curve.h",
         "include/gmalglib/sm2.h",
     ]
 )
 
 setup(
     ext_modules=[
```

### Comparing `gmalglib-0.5.5/src/gmalglib/core/bignum.c` & `gmalglib-0.5.6/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/core/random.c` & `gmalglib-0.5.6/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/core/sm2.c` & `gmalglib-0.5.6/src/gmalglib/core/sm2.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.6/src/gmalglib/core/sm2curve.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include <stdint.h>
 #include <gmalglib/bignum.h>
 #include <gmalglib/sm2curve.h>
+#include <gmalglib/sm2table.h>
 
 #ifdef _DEBUG
 
 #include <stdio.h>
 
 #endif // _DEBUG
 
@@ -628,15 +629,26 @@
     SM2JacobPointMont neg_Y = { 0 };
     SM2JacobPointMont_Neg(Y, &neg_Y);
     SM2JacobPointMont_Add(X, &neg_Y, Z);
 }
 
 void SM2JacobPointMont_MulG(const UInt256* k, SM2JacobPointMont* X)
 {
-    SM2JacobPointMont_Mul(k, CONSTS_JACOB_G, X);
+    uint32_t i;
+    uint32_t part_k;
+    SM2JacobPointMont_SetInf(X);
+
+    for (i = 0; i < 32; i++)
+    {
+        part_k = k->u8[i];
+        if (part_k > 0)
+        {
+            SM2JacobPointMont_Add(X, SM2_MULG_TABLE_U8 + i * 256 + part_k, X);
+        }
+    }
 }
 
 #ifdef _DEBUG
 
 void SM2Point_Print(const SM2Point* X)
 {
     printf("{ ");
```

### Comparing `gmalglib-0.5.5/src/gmalglib/core/sm3.c` & `gmalglib-0.5.6/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/core/sm4.c` & `gmalglib-0.5.6/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/core/zuc.c` & `gmalglib-0.5.6/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/coremodule.c` & `gmalglib-0.5.6/src/gmalglib/coremodule.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/sm2.pyi` & `gmalglib-0.5.6/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/sm3.pyi` & `gmalglib-0.5.6/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/wrapped.py` & `gmalglib-0.5.6/src/gmalglib/wrapped.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib/zuc.pyi` & `gmalglib-0.5.6/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.5/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.6/src/gmalglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 pip install gmalglib
 ```
 
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
-  - Key exchange 
+  - Key exchange
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
 - ZUC Stream Cipher Algorithm
 
 ## Usage
 
@@ -72,15 +72,15 @@
 
 If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
 
 ## Benchmark Test
 
-The benchmark test code can be found in `benchmark.py`. The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
+The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
 SM2.encrypt             : 2.391558s
 SM2.decrypt             : 1.092445s
 SM2.sign_digest         : 1.062552s
 SM2.verify_digest       : 2.096187s
```

### Comparing `gmalglib-0.5.5/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.6/src/gmalglib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 include/gmalglib/bignum.h
 include/gmalglib/random.h
 include/gmalglib/sm2.h
 include/gmalglib/sm2curve.h
+include/gmalglib/sm2table.h
 include/gmalglib/sm3.h
 include/gmalglib/sm4.h
 include/gmalglib/zuc.h
 src/gmalglib/__init__.py
 src/gmalglib/coremodule.c
 src/gmalglib/sm2.py
 src/gmalglib/sm2.pyi
@@ -25,10 +26,11 @@
 src/gmalglib.egg-info/SOURCES.txt
 src/gmalglib.egg-info/dependency_links.txt
 src/gmalglib.egg-info/top_level.txt
 src/gmalglib/core/bignum.c
 src/gmalglib/core/random.c
 src/gmalglib/core/sm2.c
 src/gmalglib/core/sm2curve.c
+src/gmalglib/core/sm2table.c
 src/gmalglib/core/sm3.c
 src/gmalglib/core/sm4.c
 src/gmalglib/core/zuc.c
```

