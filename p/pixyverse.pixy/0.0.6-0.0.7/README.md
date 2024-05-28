# Comparing `tmp/pixyverse_pixy-0.0.6.tar.gz` & `tmp/pixyverse_pixy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixyverse_pixy-0.0.6.tar", last modified: Mon May 20 12:56:44 2024, max compression
+gzip compressed data, was "pixyverse_pixy-0.0.7.tar", last modified: Tue May 28 07:12:23 2024, max compression
```

## Comparing `pixyverse_pixy-0.0.6.tar` & `pixyverse_pixy-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.358226 pixyverse_pixy-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/DESIGN.md
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-05-20 12:56:44.358226 pixyverse_pixy-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:56:44.358226 pixyverse_pixy-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.350226 pixyverse_pixy-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.354226 pixyverse_pixy-0.0.6/src/pixyverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.354226 pixyverse_pixy-0.0.6/src/pixyverse/pixy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/genparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.354226 pixyverse_pixy-0.0.6/src/pixyverse/pixy/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89004 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/grammar/pypixie.gram
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/pixyverse/pixy/transpile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.358226 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 12:56:44.000000 pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.354226 pixyverse_pixy-0.0.6/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:56:44.358226 pixyverse_pixy-0.0.6/src/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/data/invalid0.pix
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/data/invalid1.pix
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/data/invalid2.pix
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-20 12:56:36.000000 pixyverse_pixy-0.0.6/src/tests/test_transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.922517 pixyverse_pixy-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/DESIGN.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:12:23.922517 pixyverse_pixy-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.914517 pixyverse_pixy-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.914517 pixyverse_pixy-0.0.7/src/pixyverse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/src/pixyverse/pixy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/genparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/src/pixyverse/pixy/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89004 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/grammar/pypixie.gram
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/pixyverse/pixy/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 07:12:23.000000 pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:12:23.918517 pixyverse_pixy-0.0.7/src/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/data/invalid0.pix
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/data/invalid1.pix
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/data/invalid2.pix
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-28 07:12:19.000000 pixyverse_pixy-0.0.7/src/tests/test_transpile.py
```

### Comparing `pixyverse_pixy-0.0.6/DESIGN.md` & `pixyverse_pixy-0.0.7/DESIGN.md`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/LICENSE` & `pixyverse_pixy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/PKG-INFO` & `pixyverse_pixy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixyverse.pixy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to parse pixy component files which allow you to author components in python
 Author-email: Pradeep Roark <pradeep.roark@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -255,31 +255,32 @@
     </div>
     )
 ```
 
 Development
 -------------
 
-1. ```git checkout github.com/versionprime/pixy.git```
+1. ```git checkout github.com/pixyverse/pixy.git```
 2.  ```cd pixy```
-3.  create a virtualenv environment and activate it.
+3.  create/install deps in a virtualenv environment and activate it.
 
     ```shell
-    python3 -m venv .venv
+    make venv
     source .venv/bin/activate
     ```
-4.  Install dependencies
+4. lint and typecheck
     ```shell
-    pip install ".[dev]"
+    make lint
+    make pie
     ```
 
 5.  Run Tests
     ```shell
     # Run Tests
-    cd src && python -m unittest
+    make test
     ```
 6. Example Pixy file
     ```python
     # a.pix
     comp=<div>"Hello World"</div>
     print(comp)
     ```
```

### Comparing `pixyverse_pixy-0.0.6/README.md` & `pixyverse_pixy-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,31 +21,32 @@
     </div>
     )
 ```
 
 Development
 -------------
 
-1. ```git checkout github.com/versionprime/pixy.git```
+1. ```git checkout github.com/pixyverse/pixy.git```
 2.  ```cd pixy```
-3.  create a virtualenv environment and activate it.
+3.  create/install deps in a virtualenv environment and activate it.
 
     ```shell
-    python3 -m venv .venv
+    make venv
     source .venv/bin/activate
     ```
-4.  Install dependencies
+4. lint and typecheck
     ```shell
-    pip install ".[dev]"
+    make lint
+    make pie
     ```
 
 5.  Run Tests
     ```shell
     # Run Tests
-    cd src && python -m unittest
+    make test
     ```
 6. Example Pixy file
     ```python
     # a.pix
     comp=<div>"Hello World"</div>
     print(comp)
     ```
```

### Comparing `pixyverse_pixy-0.0.6/pyproject.toml` & `pixyverse_pixy-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/setup.py` & `pixyverse_pixy-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse/pixy/cli.py` & `pixyverse_pixy-0.0.7/src/pixyverse/pixy/cli.py`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse/pixy/genparser.py` & `pixyverse_pixy-0.0.7/src/pixyverse/pixy/genparser.py`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse/pixy/grammar/pypixie.gram` & `pixyverse_pixy-0.0.7/src/pixyverse/pixy/grammar/pypixie.gram`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse/pixy/transpile.py` & `pixyverse_pixy-0.0.7/src/pixyverse/pixy/transpile.py`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/PKG-INFO` & `pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixyverse.pixy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to parse pixy component files which allow you to author components in python
 Author-email: Pradeep Roark <pradeep.roark@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -255,31 +255,32 @@
     </div>
     )
 ```
 
 Development
 -------------
 
-1. ```git checkout github.com/versionprime/pixy.git```
+1. ```git checkout github.com/pixyverse/pixy.git```
 2.  ```cd pixy```
-3.  create a virtualenv environment and activate it.
+3.  create/install deps in a virtualenv environment and activate it.
 
     ```shell
-    python3 -m venv .venv
+    make venv
     source .venv/bin/activate
     ```
-4.  Install dependencies
+4. lint and typecheck
     ```shell
-    pip install ".[dev]"
+    make lint
+    make pie
     ```
 
 5.  Run Tests
     ```shell
     # Run Tests
-    cd src && python -m unittest
+    make test
     ```
 6. Example Pixy file
     ```python
     # a.pix
     comp=<div>"Hello World"</div>
     print(comp)
     ```
```

### Comparing `pixyverse_pixy-0.0.6/src/pixyverse.pixy.egg-info/SOURCES.txt` & `pixyverse_pixy-0.0.7/src/pixyverse.pixy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixyverse_pixy-0.0.6/src/tests/test_parse.py` & `pixyverse_pixy-0.0.7/src/tests/test_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """,
             ),
             ("empty_is_ok", ""),
         ]
         for testcase in testcases:
             with self.subTest(msg=testcase[0]):
                 try:
-                    TestPixieGrammar.parserModule.parse_string(testcase[1], mode="exec")
+                    TestPixyGrammar.parserModule.parse_string(testcase[1], mode="exec")
                 except SyntaxError:
                     self.fail("No exception expected")
 
     def test_invalidPyReportsBroken(self) -> None:
         testcases = [
             ("single_line", "a = 1print(a)"),
             (
@@ -45,28 +45,28 @@
             ),
             ("unfinished_business", "-"),
         ]
         for testcase in testcases:
             with self.subTest(msg=testcase[0]):
                 self.assertRaises(
                     SyntaxError,
-                    TestPixieGrammar.parserModule.parse_string,
+                    TestPixyGrammar.parserModule.parse_string,
                     testcase[1],
                     mode="exec",
                 )
 
     def test_psxAssignment(self) -> None:
         testcases = [
             ("assign_closed_element", "a=<Hello/>"),
             ("assign_block_element", "a=<Hello></Hello>"),
         ]
         for testcase in testcases:
             with self.subTest(msg=testcase[0]):
                 try:
-                    TestPixieGrammar.parserModule.parse_string(testcase[1], mode="exec")
+                    TestPixyGrammar.parserModule.parse_string(testcase[1], mode="exec")
                 except SyntaxError:
                     self.fail("No exception expected")
 
     def test_ComponentAttributes(self) -> None:
         testcases = [
             ("attribute_val", "<Victory claps={10}/>"),
             ("plain_string", "<p title='Hover Here'></p>"),
@@ -76,87 +76,87 @@
                 "<Layout grid={(10,10)}><Nested palette={'RGB'}/></Layout>",
             ),
             ("attribute_expression", "<Grid Width={200+300}></Grid>"),
         ]
         for testcase in testcases:
             with self.subTest(msg=testcase[0]):
                 try:
-                    TestPixieGrammar.parserModule.parse_string(testcase[1], mode="exec")
+                    TestPixyGrammar.parserModule.parse_string(testcase[1], mode="exec")
                 except SyntaxError:
                     self.fail("No exception expected")
 
     def test_nestedComponents(self) -> None:
         input = """
 c=<Hello>
 <World/>
 </Hello>
 """
         try:
-            TestPixieGrammar.parserModule.parse_string(input, mode="exec")
+            TestPixyGrammar.parserModule.parse_string(input, mode="exec")
         except SyntaxError:
             self.fail("No exception expected")
 
     def test_passComponentAsProp(self) -> None:
         input = """
 w=<World/>
 c=<Hello greet={w}>
 </Hello>
 """
         try:
-            TestPixieGrammar.parserModule.parse_string(input, mode="exec")
+            TestPixyGrammar.parserModule.parse_string(input, mode="exec")
         except SyntaxError:
             self.fail("No exception expected")
 
     def test_ExpressionsInBlockElement(self) -> None:
         input = """
 c=<Hello>
 {1+2}
 {True}
 </Hello>
 """
         try:
-            TestPixieGrammar.parserModule.parse_string(input, mode="exec")
+            TestPixyGrammar.parserModule.parse_string(input, mode="exec")
         except SyntaxError:
             self.fail("No exception expected")
 
     def test_GenExpressionsInBlockElement(self) -> None:
         input = """
 names = ['Alice','Bob','Charlie']
 c=<Hello>
 <ul>
 {map(lambda name: <li>{name}</li>, names)}
 </ul>
 </Hello>
 """
         try:
-            TestPixieGrammar.parserModule.parse_string(input, mode="exec")
+            TestPixyGrammar.parserModule.parse_string(input, mode="exec")
         except SyntaxError:
             self.fail("No exception expected")
 
     def test_LiteralStringsInBlockElement(self) -> None:
         input = """
 c=<Hello>
 "This is a literal string"
 </Hello>
 """
         try:
-            TestPixieGrammar.parserModule.parse_string(input, mode="exec")
+            TestPixyGrammar.parserModule.parse_string(input, mode="exec")
         except SyntaxError:
             self.fail("No exception expected")
 
     def test_invalidPixieComponentsFail(self) -> None:
         testcases = [
             ("broken_selfclose", "<Victory claps={10}>"),
             ("mismatched_tagname", "<Hello></ello>"),
         ]
         for testcase in testcases:
             with self.subTest(msg=testcase[0]):
                 self.assertRaises(
                     SyntaxError,
-                    TestPixieGrammar.parserModule.parse_string,
+                    TestPixyGrammar.parserModule.parse_string,
                     testcase[1],
                     mode="exec",
                 )
 
     def test_invalidPixieComponentsErrorReport(self) -> None:
         testcases = [
             ("broken_selfclose_1", "./data/invalid0.pix"),
@@ -165,14 +165,14 @@
         ]
         for testcase in testcases:
             TESTDATA_FILENAME = os.path.join(os.path.dirname(__file__), testcase[1])
             with self.subTest(msg=testcase[0]):
                 if testcase[0] == "broken_selfclose_1":
                     self.skipTest("pegen parser throws error in invalid line number and fails")
                 try:
-                    TestPixieGrammar.parserModule.parse_file(TESTDATA_FILENAME)
+                    TestPixyGrammar.parserModule.parse_file(TESTDATA_FILENAME)
                 except SyntaxError as err:
                     print(err)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pixyverse_pixy-0.0.6/src/tests/test_transpile.py` & `pixyverse_pixy-0.0.7/src/tests/test_transpile.py`

 * *Files identical despite different names*

