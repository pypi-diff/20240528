# Comparing `tmp/aggregate_root-0.0.3.tar.gz` & `tmp/aggregate_root-0.0.4.tar.gz`

## Comparing `aggregate_root-0.0.3.tar` & `aggregate_root-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/__init__.py
--rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/aggregate_root.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/domain_event.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_aggregate_root.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_domain_event.py
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_sample.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/LICENSE
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/src/aggregate_root/__init__.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/src/aggregate_root/aggregate_root.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/src/aggregate_root/domain_event.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/src/aggregate_root/repository.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/tests/test_aggregate_root.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/tests/test_domain_event.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/tests/test_sample.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/LICENSE
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 aggregate_root-0.0.4/PKG-INFO
```

### Comparing `aggregate_root-0.0.3/src/aggregate_root/aggregate_root.py` & `aggregate_root-0.0.4/src/aggregate_root/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/src/aggregate_root/domain_event.py` & `aggregate_root-0.0.4/src/aggregate_root/domain_event.py`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/tests/test_aggregate_root.py` & `aggregate_root-0.0.4/tests/test_aggregate_root.py`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/tests/test_domain_event.py` & `aggregate_root-0.0.4/tests/test_domain_event.py`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/tests/test_sample.py` & `aggregate_root-0.0.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/LICENSE` & `aggregate_root-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/README.md` & `aggregate_root-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.3/pyproject.toml` & `aggregate_root-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aggregate-root"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jeremy Willemse", email="jeremy@willemse.co" },
 ]
 description = "A small Python library for defining domain-driven design aggregates and domain events."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `aggregate_root-0.0.3/PKG-INFO` & `aggregate_root-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aggregate-root
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small Python library for defining domain-driven design aggregates and domain events.
 Project-URL: Homepage, https://github.com/willemse-and-co/aggregate-root
 Project-URL: Issues, https://github.com/willemse-and-co/aggregate-root/issues
 Author-email: Jeremy Willemse <jeremy@willemse.co>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

