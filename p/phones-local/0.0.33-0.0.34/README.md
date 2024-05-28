# Comparing `tmp/phones_local-0.0.33.tar.gz` & `tmp/phones_local-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.33.tar", last modified: Tue May 28 14:25:53 2024, max compression
+gzip compressed data, was "phones_local-0.0.34.tar", last modified: Tue May 28 14:32:51 2024, max compression
```

## Comparing `phones_local-0.0.33.tar` & `phones_local-0.0.34.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:25:53.486787 phones_local-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 14:25:21.000000 phones_local-0.0.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.482787 phones_local-0.0.33/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 14:25:27.000000 phones_local-0.0.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:25:53.486787 phones_local-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 14:25:21.000000 phones_local-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:32:51.848637 phones_local-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:32:51.848637 phones_local-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 14:32:23.000000 phones_local-0.0.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:32:51.848637 phones_local-0.0.34/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:32:51.848637 phones_local-0.0.34/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:32:23.000000 phones_local-0.0.34/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 14:32:23.000000 phones_local-0.0.34/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-28 14:32:23.000000 phones_local-0.0.34/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:32:51.848637 phones_local-0.0.34/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:32:51.000000 phones_local-0.0.34/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 14:32:51.000000 phones_local-0.0.34/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:32:51.000000 phones_local-0.0.34/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 14:32:51.000000 phones_local-0.0.34/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:32:51.000000 phones_local-0.0.34/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 14:32:31.000000 phones_local-0.0.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:32:51.848637 phones_local-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 14:32:23.000000 phones_local-0.0.34/setup.py
```

### Comparing `phones_local-0.0.33/PKG-INFO` & `phones_local-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.33
+Version: 0.0.34
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.33/README.md` & `phones_local-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.33/phones_local/src/phone_local_constans.py` & `phones_local-0.0.34/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.33/phones_local/src/phones_local.py` & `phones_local-0.0.34/phones_local/src/phones_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,18 @@
         Process phone number and return normalized phone number.
         :param original_phone_number: Original phone number.
         :param country_iso_code: Country ISO code.
         :param contact_id: Contact id.
         :return: Dictionary with the normalized phone number and the international code.
         """
         logger.start(object={'original_phone_number': original_phone_number})
-        country_iso_code = country_iso_code or self.get_country_iso_code(
-            location_id=location_id, contact_id=contact_id, profile_id=profile_id, country_id=country_id
-        )
+        if location_id is not None or country_id is not None:
+            country_iso_code = country_iso_code or self.get_country_iso_code(
+                location_id=location_id, contact_id=contact_id, profile_id=profile_id, country_id=country_id
+            )
         normalized_phone_number = self.normalize_phone_number(
             original_number=original_phone_number, region=country_iso_code)
         phone_dict = {
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
```

### Comparing `phones_local-0.0.33/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.34/phones_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.33
+Version: 0.0.34
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.33/pyproject.toml` & `phones_local-0.0.34/pyproject.toml`

 * *Files identical despite different names*

