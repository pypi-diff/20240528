# Comparing `tmp/protoc_polyglot-0.0.1.post4.tar.gz` & `tmp/protoc_polyglot-0.0.1.post5.tar.gz`

## Comparing `protoc_polyglot-0.0.1.post4.tar` & `protoc_polyglot-0.0.1.post5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/cli.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/wrapper.py
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/cpp/cli.py
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/csharp/cli.py
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/go/cli.py
--rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/java/cli.py
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/js/cli.py
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/obj-c/cli.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/php/cli.py
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/python/cli.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/ruby/cli.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/core/rust/cli.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/.gitignore
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/pyproject.toml
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/__init__.py
+-rwxr-xr-x   0        0        0     6447 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/cli.py
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/wrapper.py
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/cpp/cli.py
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/csharp/cli.py
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/go/cli.py
+-rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/java/cli.py
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/js/cli.py
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/obj-c/cli.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/php/cli.py
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/python/cli.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/ruby/cli.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/core/rust/cli.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/.gitignore
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/pyproject.toml
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 protoc_polyglot-0.0.1.post5/PKG-INFO
```

### Comparing `protoc_polyglot-0.0.1.post4/core/cli.py` & `protoc_polyglot-0.0.1.post5/core/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/wrapper.py` & `protoc_polyglot-0.0.1.post5/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/cpp/cli.py` & `protoc_polyglot-0.0.1.post5/core/cpp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/csharp/cli.py` & `protoc_polyglot-0.0.1.post5/core/csharp/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/go/cli.py` & `protoc_polyglot-0.0.1.post5/core/go/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/java/cli.py` & `protoc_polyglot-0.0.1.post5/core/java/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/js/cli.py` & `protoc_polyglot-0.0.1.post5/core/js/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/obj-c/cli.py` & `protoc_polyglot-0.0.1.post5/core/obj-c/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/php/cli.py` & `protoc_polyglot-0.0.1.post5/core/php/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/python/cli.py` & `protoc_polyglot-0.0.1.post5/core/python/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/ruby/cli.py` & `protoc_polyglot-0.0.1.post5/core/ruby/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/core/rust/cli.py` & `protoc_polyglot-0.0.1.post5/core/rust/cli.py`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/README.md` & `protoc_polyglot-0.0.1.post5/README.md`

 * *Files identical despite different names*

### Comparing `protoc_polyglot-0.0.1.post4/pyproject.toml` & `protoc_polyglot-0.0.1.post5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.hatch.build.targets.wheel]
 include = [
   "core/*",
 ]
 
 [project]
 name = "protoc_polyglot"
-version = "0.0.1-4"
+version = "0.0.1-5"
 license = {text = "MIT License"}
 authors = [
   { name="Milan Pultar", email="milan.pultar@gmail.com" },
   { name="Hugo Kunák", email="author@example.com" },
 ]
 description = "Protoc wrapper for compilation into any language"
 readme = "README.md"
```

### Comparing `protoc_polyglot-0.0.1.post4/PKG-INFO` & `protoc_polyglot-0.0.1.post5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: protoc_polyglot
-Version: 0.0.1.post4
+Version: 0.0.1.post5
 Summary: Protoc wrapper for compilation into any language
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Milan Pultar <milan.pultar@gmail.com>, Hugo Kunák <author@example.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

