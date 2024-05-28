# Comparing `tmp/phones_local-0.0.29.tar.gz` & `tmp/phones_local-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.29.tar", last modified: Mon May 27 19:31:44 2024, max compression
+gzip compressed data, was "phones_local-0.0.30.tar", last modified: Tue May 28 12:28:18 2024, max compression
```

## Comparing `phones_local-0.0.29.tar` & `phones_local-0.0.30.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 19:31:44.023930 phones_local-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-27 19:31:18.000000 phones_local-0.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.019930 phones_local-0.0.29/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-27 19:31:18.000000 phones_local-0.0.29/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:31:44.023930 phones_local-0.0.29/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 19:31:44.000000 phones_local-0.0.29/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 19:31:24.000000 phones_local-0.0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:31:44.023930 phones_local-0.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-27 19:31:18.000000 phones_local-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:28:18.026443 phones_local-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 12:28:18.026443 phones_local-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 12:27:42.000000 phones_local-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:28:18.026443 phones_local-0.0.30/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:28:18.026443 phones_local-0.0.30/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:27:42.000000 phones_local-0.0.30/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 12:27:42.000000 phones_local-0.0.30/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-05-28 12:27:42.000000 phones_local-0.0.30/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:28:18.026443 phones_local-0.0.30/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 12:28:18.000000 phones_local-0.0.30/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 12:28:18.000000 phones_local-0.0.30/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:28:18.000000 phones_local-0.0.30/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 12:28:18.000000 phones_local-0.0.30/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 12:28:18.000000 phones_local-0.0.30/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 12:27:49.000000 phones_local-0.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:28:18.026443 phones_local-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 12:27:42.000000 phones_local-0.0.30/setup.py
```

### Comparing `phones_local-0.0.29/PKG-INFO` & `phones_local-0.0.30/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.29
+Version: 0.0.30
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.29/README.md` & `phones_local-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.29/phones_local/src/phone_local_constans.py` & `phones_local-0.0.30/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.29/phones_local/src/phones_local.py` & `phones_local-0.0.30/phones_local/src/phones_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,60 +118,68 @@
             schema_name="country", view_table_name='country_ml_view', select_clause_value='iso',
             column_name='country_id', column_value=country_id)
         return country_iso_code
 
     # TODO: Is it really necessary to access the database for location?
     # I think it's possible to get the normalized phone number and the international code
     # from original_phone_number
-    def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None) -> dict:
+    def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None,
+                      profile_id: int = None, person_id: str = None) -> dict:
         """
         Process phone number and return normalized phone number.
         :param original_phone_number: Original phone number.
         :param country_iso_code: Country ISO code.
         :param contact_id: Contact id.
         :return: Dictionary with the normalized phone number and the international code.
         """
         logger.start(object={'original_phone_number': original_phone_number})
         country_iso_code = country_iso_code or self.get_country_iso_code()
         normalized_phone_number = self.normalize_phone_number(
             original_number=original_phone_number, region=country_iso_code)
-        phone_data = {
+        phone_dict = {
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
-        # TODO phone_data -> phone_dict
-        phone_id = self.insert(data_dict=phone_data)
+        phone_id = self.insert(data_dict=phone_dict)
 
         # link phone to profile
-        profile_id = user_context.get_effective_profile_id()
-        if profile_id:
+        if profile_id is not None:
             phone_profile_id = self.insert_mapping(
                 schema_name='phone_profile',
                 entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
         else:
             phone_profile_id = None
 
         # link phone to contact
-        if contact_id:
+        if contact_id is not None:
             contact_phone_id = self.insert_mapping(
                 schema_name='contact_phone', entity_name1='contact', entity_name2='phone',
                 entity_id1=contact_id, entity_id2=phone_id)
         else:
             contact_phone_id = None
 
+        # link phone to person
+        if person_id is not None:
+            phone_person_id = self.insert_mapping(
+                schema_name='person_phone', entity_name1='person', entity_name2='phone',
+                entity_id1=person_id, entity_id2=phone_id)
+        else:
+            phone_person_id = None
+
         result = {
             'phone_profile_id': phone_profile_id,
             'phone_id': phone_id,
             'normalized_phone_number': normalized_phone_number,
             'original_phone_number': original_phone_number,
             'contact_phone_id': contact_phone_id,
+            'phone_person_id': phone_person_id,
         }
         logger.end("success processing phone number", object=result)
         return result
 
     def insert_phone(self, phone_data: dict) -> int:
         """
         Insert phone data into the phone table.
```

### Comparing `phones_local-0.0.29/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.30/phones_local.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.29
+Version: 0.0.30
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.29/pyproject.toml` & `phones_local-0.0.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.29/setup.py` & `phones_local-0.0.30/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.29',  # https://pypi.org/project/phones-local/
+    version='0.0.30',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

