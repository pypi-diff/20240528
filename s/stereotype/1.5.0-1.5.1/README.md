# Comparing `tmp/stereotype-1.5.0.tar.gz` & `tmp/stereotype-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stereotype-1.5.0.tar", last modified: Thu Mar 23 12:14:11 2023, max compression
+gzip compressed data, was "stereotype-1.5.1.tar", last modified: Tue May 28 08:49:08 2024, max compression
```

## Comparing `stereotype-1.5.0.tar` & `stereotype-1.5.1.tar`

### file list

```diff
@@ -1,54 +1,44 @@
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.789138 stereotype-1.5.0/
--rw-r--r--   0 petee     (1000) petee     (1000)     1069 2021-01-04 12:20:14.000000 stereotype-1.5.0/LICENSE
--rw-rw-r--   0 petee     (1000) petee     (1000)     4195 2023-03-23 12:14:11.789138 stereotype-1.5.0/PKG-INFO
--rw-rw-r--   0 petee     (1000) petee     (1000)     3145 2022-10-12 09:36:30.000000 stereotype-1.5.0/README.md
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.785138 stereotype-1.5.0/bench/
--rw-rw-r--   0 petee     (1000) petee     (1000)     1166 2022-07-08 10:45:43.000000 stereotype-1.5.0/bench/__init__.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     2208 2022-09-10 08:10:39.000000 stereotype-1.5.0/bench/bench_attrs.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1535 2022-09-10 08:10:23.000000 stereotype-1.5.0/bench/bench_pydantic.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     2317 2022-07-08 10:45:43.000000 stereotype-1.5.0/bench/bench_schematics.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1518 2022-09-09 08:07:20.000000 stereotype-1.5.0/bench/bench_schematics2.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1284 2022-10-26 22:20:28.000000 stereotype-1.5.0/bench/bench_stereotype.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1047 2022-07-08 10:45:43.000000 stereotype-1.5.0/bench/bench_stereotype_dynamic.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     2290 2022-07-08 10:45:43.000000 stereotype-1.5.0/bench/bench_utils.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     3031 2022-09-09 07:59:07.000000 stereotype-1.5.0/bench/common.py
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.785138 stereotype-1.5.0/examples/
--rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.0/examples/__init__.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1890 2022-10-19 12:30:10.000000 stereotype-1.5.0/examples/atomic_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1247 2022-10-12 09:36:30.000000 stereotype-1.5.0/examples/compound_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1340 2022-10-12 09:36:30.000000 stereotype-1.5.0/examples/model_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     1062 2022-08-03 08:31:49.000000 stereotype-1.5.0/examples/schematics_field.py
--rw-rw-r--   0 petee     (1000) petee     (1000)       38 2023-03-23 12:14:11.789138 stereotype-1.5.0/setup.cfg
--rw-rw-r--   0 petee     (1000) petee     (1000)      715 2023-03-23 12:13:15.000000 stereotype-1.5.0/setup.py
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.785138 stereotype-1.5.0/stereotype/
--rw-rw-r--   0 petee     (1000) petee     (1000)      531 2022-10-12 09:36:30.000000 stereotype-1.5.0/stereotype/__init__.py
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.785138 stereotype-1.5.0/stereotype/contrib/
--rw-rw-r--   0 petee     (1000) petee     (1000)        0 2022-08-03 08:31:49.000000 stereotype-1.5.0/stereotype/contrib/__init__.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     3325 2022-10-27 10:47:49.000000 stereotype-1.5.0/stereotype/contrib/schematics.py
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.789138 stereotype-1.5.0/stereotype/fields/
--rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.0/stereotype/fields/__init__.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     3457 2022-10-27 10:47:49.000000 stereotype-1.5.0/stereotype/fields/annotations.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    12324 2022-10-12 09:36:30.000000 stereotype-1.5.0/stereotype/fields/atomic.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    10312 2023-03-23 12:13:15.000000 stereotype-1.5.0/stereotype/fields/base.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    11247 2022-10-27 10:47:49.000000 stereotype-1.5.0/stereotype/fields/compound.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     7936 2022-10-27 10:47:49.000000 stereotype-1.5.0/stereotype/fields/model.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     2030 2022-10-28 07:45:16.000000 stereotype-1.5.0/stereotype/fields/serializable.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    12061 2023-03-23 12:13:15.000000 stereotype-1.5.0/stereotype/meta.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    11776 2023-03-23 12:13:15.000000 stereotype-1.5.0/stereotype/model.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     4300 2022-10-19 12:30:10.000000 stereotype-1.5.0/stereotype/roles.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     3727 2022-10-27 11:36:12.000000 stereotype-1.5.0/stereotype/utils.py
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.785138 stereotype-1.5.0/stereotype.egg-info/
--rw-r--r--   0 petee     (1000) petee     (1000)     4195 2023-03-23 12:14:11.000000 stereotype-1.5.0/stereotype.egg-info/PKG-INFO
--rw-r--r--   0 petee     (1000) petee     (1000)     1088 2023-03-23 12:14:11.000000 stereotype-1.5.0/stereotype.egg-info/SOURCES.txt
--rw-r--r--   0 petee     (1000) petee     (1000)        1 2023-03-23 12:14:11.000000 stereotype-1.5.0/stereotype.egg-info/dependency_links.txt
--rw-r--r--   0 petee     (1000) petee     (1000)       20 2023-03-23 12:14:11.000000 stereotype-1.5.0/stereotype.egg-info/top_level.txt
-drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2023-03-23 12:14:11.789138 stereotype-1.5.0/tests/
--rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.0/tests/__init__.py
--rw-rw-r--   0 petee     (1000) petee     (1000)      338 2022-08-15 14:52:43.000000 stereotype-1.5.0/tests/common.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    17888 2023-03-23 12:13:15.000000 stereotype-1.5.0/tests/test_atomic_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    21734 2023-03-23 12:13:15.000000 stereotype-1.5.0/tests/test_compound_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)      487 2022-07-11 15:41:15.000000 stereotype-1.5.0/tests/test_examples.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    11112 2022-10-27 10:47:49.000000 stereotype-1.5.0/tests/test_model_fields.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    19787 2023-03-23 12:13:15.000000 stereotype-1.5.0/tests/test_models.py
--rw-rw-r--   0 petee     (1000) petee     (1000)    10442 2022-10-19 12:30:10.000000 stereotype-1.5.0/tests/test_roles.py
--rw-rw-r--   0 petee     (1000) petee     (1000)     7018 2022-10-28 07:45:24.000000 stereotype-1.5.0/tests/test_serializable.py
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.232863 stereotype-1.5.1/
+-rw-r--r--   0 petee     (1000) petee     (1000)     1069 2021-01-04 12:20:14.000000 stereotype-1.5.1/LICENSE
+-rw-rw-r--   0 petee     (1000) petee     (1000)     4195 2024-05-28 08:49:08.232863 stereotype-1.5.1/PKG-INFO
+-rw-rw-r--   0 petee     (1000) petee     (1000)     3145 2022-10-12 09:36:30.000000 stereotype-1.5.1/README.md
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.224863 stereotype-1.5.1/examples/
+-rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.1/examples/__init__.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     1890 2022-10-19 12:30:10.000000 stereotype-1.5.1/examples/atomic_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     1247 2022-10-12 09:36:30.000000 stereotype-1.5.1/examples/compound_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     1340 2022-10-12 09:36:30.000000 stereotype-1.5.1/examples/model_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     1062 2022-08-03 08:31:49.000000 stereotype-1.5.1/examples/schematics_field.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)       38 2024-05-28 08:49:08.232863 stereotype-1.5.1/setup.cfg
+-rw-rw-r--   0 petee     (1000) petee     (1000)      715 2024-05-28 08:48:43.000000 stereotype-1.5.1/setup.py
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.228863 stereotype-1.5.1/stereotype/
+-rw-rw-r--   0 petee     (1000) petee     (1000)      531 2022-10-12 09:36:30.000000 stereotype-1.5.1/stereotype/__init__.py
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.228863 stereotype-1.5.1/stereotype/contrib/
+-rw-rw-r--   0 petee     (1000) petee     (1000)        0 2022-08-03 08:31:49.000000 stereotype-1.5.1/stereotype/contrib/__init__.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     3325 2022-10-27 10:47:49.000000 stereotype-1.5.1/stereotype/contrib/schematics.py
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.228863 stereotype-1.5.1/stereotype/fields/
+-rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.1/stereotype/fields/__init__.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     3457 2022-10-27 10:47:49.000000 stereotype-1.5.1/stereotype/fields/annotations.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    12324 2022-10-12 09:36:30.000000 stereotype-1.5.1/stereotype/fields/atomic.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    10312 2023-03-23 12:13:15.000000 stereotype-1.5.1/stereotype/fields/base.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    11247 2022-10-27 10:47:49.000000 stereotype-1.5.1/stereotype/fields/compound.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     7936 2022-10-27 10:47:49.000000 stereotype-1.5.1/stereotype/fields/model.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     2030 2022-10-28 07:45:16.000000 stereotype-1.5.1/stereotype/fields/serializable.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    12061 2023-03-23 12:13:15.000000 stereotype-1.5.1/stereotype/meta.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    11776 2023-03-23 12:13:15.000000 stereotype-1.5.1/stereotype/model.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     4300 2022-10-19 12:30:10.000000 stereotype-1.5.1/stereotype/roles.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     3992 2024-05-28 08:48:43.000000 stereotype-1.5.1/stereotype/utils.py
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.228863 stereotype-1.5.1/stereotype.egg-info/
+-rw-r--r--   0 petee     (1000) petee     (1000)     4195 2024-05-28 08:49:08.000000 stereotype-1.5.1/stereotype.egg-info/PKG-INFO
+-rw-r--r--   0 petee     (1000) petee     (1000)      875 2024-05-28 08:49:08.000000 stereotype-1.5.1/stereotype.egg-info/SOURCES.txt
+-rw-r--r--   0 petee     (1000) petee     (1000)        1 2024-05-28 08:49:08.000000 stereotype-1.5.1/stereotype.egg-info/dependency_links.txt
+-rw-r--r--   0 petee     (1000) petee     (1000)       20 2024-05-28 08:49:08.000000 stereotype-1.5.1/stereotype.egg-info/top_level.txt
+drwxrwxr-x   0 petee     (1000) petee     (1000)        0 2024-05-28 08:49:08.232863 stereotype-1.5.1/tests/
+-rw-r--r--   0 petee     (1000) petee     (1000)        0 2021-01-04 12:20:14.000000 stereotype-1.5.1/tests/__init__.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)      338 2022-08-15 14:52:43.000000 stereotype-1.5.1/tests/common.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    17888 2023-03-23 12:13:15.000000 stereotype-1.5.1/tests/test_atomic_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    22619 2024-05-28 08:48:43.000000 stereotype-1.5.1/tests/test_compound_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)      487 2022-07-11 15:41:15.000000 stereotype-1.5.1/tests/test_examples.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    11112 2022-10-27 10:47:49.000000 stereotype-1.5.1/tests/test_model_fields.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    19787 2023-03-23 12:13:15.000000 stereotype-1.5.1/tests/test_models.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)    10442 2022-10-19 12:30:10.000000 stereotype-1.5.1/tests/test_roles.py
+-rw-rw-r--   0 petee     (1000) petee     (1000)     7018 2022-10-28 07:45:24.000000 stereotype-1.5.1/tests/test_serializable.py
```

### Comparing `stereotype-1.5.0/LICENSE` & `stereotype-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/PKG-INFO` & `stereotype-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereotype
-Version: 1.5.0
+Version: 1.5.1
 Summary: Models for conversion and validation of rich data structures.
 Home-page: https://github.com/petee-d/stereotype
 Author: Peter Dolák
 Author-email: peter@dolak.sk
 License: UNKNOWN
 Description: # stereotype
```

### Comparing `stereotype-1.5.0/README.md` & `stereotype-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/examples/atomic_fields.py` & `stereotype-1.5.1/examples/atomic_fields.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/examples/compound_fields.py` & `stereotype-1.5.1/examples/compound_fields.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/examples/model_fields.py` & `stereotype-1.5.1/examples/model_fields.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/examples/schematics_field.py` & `stereotype-1.5.1/examples/schematics_field.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/__init__.py` & `stereotype-1.5.1/stereotype/__init__.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/contrib/schematics.py` & `stereotype-1.5.1/stereotype/contrib/schematics.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/annotations.py` & `stereotype-1.5.1/stereotype/fields/annotations.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/atomic.py` & `stereotype-1.5.1/stereotype/fields/atomic.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/base.py` & `stereotype-1.5.1/stereotype/fields/base.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/compound.py` & `stereotype-1.5.1/stereotype/fields/compound.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/model.py` & `stereotype-1.5.1/stereotype/fields/model.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/fields/serializable.py` & `stereotype-1.5.1/stereotype/fields/serializable.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/meta.py` & `stereotype-1.5.1/stereotype/meta.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/model.py` & `stereotype-1.5.1/stereotype/model.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/roles.py` & `stereotype-1.5.1/stereotype/roles.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/stereotype/utils.py` & `stereotype-1.5.1/stereotype/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 
 class DataError(StereotypeError):
     """Encapsulates one or multiple errors that happened during conversion or validation, mapped by field paths."""
 
     error_list: List[PathErrorType]
 
+    ERRORS_DICT_SELF_KEY = '_global'
+
     def __init__(self, errors: List[PathErrorType]):
         self.error_list = errors
         super().__init__(self._error_string())
 
     def _error_string(self) -> str:
         for path, error in self.error_list:
             if not path:
@@ -73,21 +75,24 @@
         Keys in the dictionaries are field (primitive) names.
         Values are either lists of error messages from simple fields, or recursive dictionaries for compound fields.
         """
         errors = {}
         for path, error in self.error_list:
             container = errors
             if not path:
-                path = ('_global',)
+                path = (self.ERRORS_DICT_SELF_KEY,)
             for item in path[:-1]:
                 value = container.setdefault(item, {})
                 if isinstance(value, list):
-                    value = container[item] = cast(dict, {'_global': value})
+                    value = container[item] = cast(dict, {self.ERRORS_DICT_SELF_KEY: value})
                 container = value
             array = container.setdefault(path[-1], [])
+            if isinstance(array, dict):
+                # The target container is not an array as it has some deeper error
+                array = array.setdefault(self.ERRORS_DICT_SELF_KEY, [])
             array.append(error)
         return errors
 
     @classmethod
     def new(cls, message: str, *path: str):
         return cls([(path, message)])
```

### Comparing `stereotype-1.5.0/stereotype.egg-info/PKG-INFO` & `stereotype-1.5.1/stereotype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereotype
-Version: 1.5.0
+Version: 1.5.1
 Summary: Models for conversion and validation of rich data structures.
 Home-page: https://github.com/petee-d/stereotype
 Author: Peter Dolák
 Author-email: peter@dolak.sk
 License: UNKNOWN
 Description: # stereotype
```

### Comparing `stereotype-1.5.0/stereotype.egg-info/SOURCES.txt` & `stereotype-1.5.1/stereotype.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 LICENSE
 README.md
 setup.py
-bench/__init__.py
-bench/bench_attrs.py
-bench/bench_pydantic.py
-bench/bench_schematics.py
-bench/bench_schematics2.py
-bench/bench_stereotype.py
-bench/bench_stereotype_dynamic.py
-bench/bench_utils.py
-bench/common.py
 examples/__init__.py
 examples/atomic_fields.py
 examples/compound_fields.py
 examples/model_fields.py
 examples/schematics_field.py
 stereotype/__init__.py
 stereotype/meta.py
```

### Comparing `stereotype-1.5.0/tests/test_atomic_fields.py` & `stereotype-1.5.1/tests/test_atomic_fields.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/tests/test_compound_fields.py` & `stereotype-1.5.1/tests/test_compound_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -413,14 +413,32 @@
                               'False': ['This field is required']},
             'str_to_opt_dict': {'y': ['Provide at least 1 item']},
             'validators': {'None': ['This field is required', 'Not really optional'],
                            'key': ['Must be numeric'],
                            '400': ['Must be numeric']}
         }, ctx.exception.errors)
 
+    def test_conflicting_field_and_item_errors(self):
+        def is_valid_dict(value, context=None):
+            if "err" in value:
+                raise ValueError("Dict contains an error key")
+
+        class HasDict(Model):
+            field: Dict[str, str] = DictField(key_field=StrField(max_length=4), value_field=StrField(max_length=3),
+                                              validators=[is_valid_dict], max_length=2)
+
+        model = HasDict({"field": {"bad": "too long", "ok": "ok", "err": "ok", "worse": "key"}})
+        with self.assertRaises(ValidationError) as ctx:
+            model.validate()
+        self.assertEqual({'field': {
+            '_global': ['Provide at most 2 items', 'Dict contains an error key'],
+            'bad': ['Must be at most 3 characters long'],
+            'worse': ['Must be at most 4 characters long']
+        }}, ctx.exception.errors)
+
     def test_double_required_error(self):
         class RequiredDict(Model):
             dict: Dict[int, int]
 
         model = RequiredDict({'dict': {4: 2}})
         model.validate()
         self.assertEqual(2, model.dict[4])
```

### Comparing `stereotype-1.5.0/tests/test_model_fields.py` & `stereotype-1.5.1/tests/test_model_fields.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/tests/test_models.py` & `stereotype-1.5.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/tests/test_roles.py` & `stereotype-1.5.1/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `stereotype-1.5.0/tests/test_serializable.py` & `stereotype-1.5.1/tests/test_serializable.py`

 * *Files identical despite different names*

