# Comparing `tmp/phones_local-0.0.31.tar.gz` & `tmp/phones_local-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.31.tar", last modified: Tue May 28 13:18:40 2024, max compression
+gzip compressed data, was "phones_local-0.0.32.tar", last modified: Tue May 28 13:40:37 2024, max compression
```

## Comparing `phones_local-0.0.31.tar` & `phones_local-0.0.32.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:18:40.856173 phones_local-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:18:40.856173 phones_local-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 13:18:13.000000 phones_local-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:18:40.852173 phones_local-0.0.31/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:18:40.852173 phones_local-0.0.31/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:18:13.000000 phones_local-0.0.31/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 13:18:13.000000 phones_local-0.0.31/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-28 13:18:13.000000 phones_local-0.0.31/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:18:40.856173 phones_local-0.0.31/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:18:40.000000 phones_local-0.0.31/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 13:18:40.000000 phones_local-0.0.31/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:18:40.000000 phones_local-0.0.31/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 13:18:40.000000 phones_local-0.0.31/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 13:18:40.000000 phones_local-0.0.31/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 13:18:19.000000 phones_local-0.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:18:40.856173 phones_local-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 13:18:13.000000 phones_local-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:40:37.166343 phones_local-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 13:40:00.000000 phones_local-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.162343 phones_local-0.0.32/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 13:40:09.000000 phones_local-0.0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:40:37.166343 phones_local-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 13:40:00.000000 phones_local-0.0.32/setup.py
```

### Comparing `phones_local-0.0.31/PKG-INFO` & `phones_local-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.31
+Version: 0.0.32
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.31/README.md` & `phones_local-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.31/phones_local/src/phone_local_constans.py` & `phones_local-0.0.32/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.31/phones_local/src/phones_local.py` & `phones_local-0.0.32/phones_local/src/phones_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,31 +152,34 @@
                                view_table_name="phone_view", table_name="phone_table",
                                compare_with_or=True)
 
         # link phone to profile
         if profile_id is not None:
             phone_profile_id = self.insert_mapping(
                 schema_name='phone_profile',
-                entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
+                entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id,
+                ignore_duplicate=True)
         else:
             phone_profile_id = None
 
         # link phone to contact
         if contact_id is not None:
             contact_phone_id = self.insert_mapping(
                 schema_name='contact_phone', entity_name1='contact', entity_name2='phone',
-                entity_id1=contact_id, entity_id2=phone_id)
+                entity_id1=contact_id, entity_id2=phone_id,
+                ignore_duplicate=True)
         else:
             contact_phone_id = None
 
         # link phone to person
         if person_id is not None:
             phone_person_id = self.insert_mapping(
                 schema_name='person_phone', entity_name1='person', entity_name2='phone',
-                entity_id1=person_id, entity_id2=phone_id)
+                entity_id1=person_id, entity_id2=phone_id,
+                ignore_duplicate=True)
         else:
             phone_person_id = None
 
         result = {
             'phone_profile_id': phone_profile_id,
             'phone_id': phone_id,
             'normalized_phone_number': normalized_phone_number,
```

### Comparing `phones_local-0.0.31/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.32/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.31
+Version: 0.0.32
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.31/pyproject.toml` & `phones_local-0.0.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.31/setup.py` & `phones_local-0.0.32/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.31',  # https://pypi.org/project/phones-local/
+    version='0.0.32',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

