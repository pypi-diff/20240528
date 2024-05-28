# Comparing `tmp/phones_local-0.0.32.tar.gz` & `tmp/phones_local-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.32.tar", last modified: Tue May 28 13:40:37 2024, max compression
+gzip compressed data, was "phones_local-0.0.33.tar", last modified: Tue May 28 14:25:53 2024, max compression
```

## Comparing `phones_local-0.0.32.tar` & `phones_local-0.0.33.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:40:37.166343 phones_local-0.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 13:40:00.000000 phones_local-0.0.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.162343 phones_local-0.0.32/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-28 13:40:00.000000 phones_local-0.0.32/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:40:37.166343 phones_local-0.0.32/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 13:40:37.000000 phones_local-0.0.32/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 13:40:09.000000 phones_local-0.0.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:40:37.166343 phones_local-0.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 13:40:00.000000 phones_local-0.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:25:53.486787 phones_local-0.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 14:25:21.000000 phones_local-0.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.482787 phones_local-0.0.33/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-05-28 14:25:21.000000 phones_local-0.0.33/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:25:53.486787 phones_local-0.0.33/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:25:53.000000 phones_local-0.0.33/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 14:25:27.000000 phones_local-0.0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:25:53.486787 phones_local-0.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 14:25:21.000000 phones_local-0.0.33/setup.py
```

### Comparing `phones_local-0.0.32/PKG-INFO` & `phones_local-0.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.32
+Version: 0.0.33
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.32/README.md` & `phones_local-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.32/phones_local/src/phone_local_constans.py` & `phones_local-0.0.33/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.32/phones_local/src/phones_local.py` & `phones_local-0.0.33/phones_local/src/phones_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,20 +86,16 @@
                 "extension": parsed_number.extension,
             }
             return number_info
         except NumberParseException as e:
             logger.exception(f"Invalid phone number: {original_number}.", object=e)
             raise e
 
-    def get_country_iso_code(self) -> str:
-        contact_id = None  # user_context.get_effective_contact_id()
-        profile_id = user_context.get_effective_profile_id()
-        location_id = None  # user_context.get_effective_location_id()
-        country_id = None  # user_context.get_effective_country_id()
-
+    def get_country_iso_code(self, location_id: int = None, contact_id: int = None,  profile_id: int = None,
+                             country_id: int = None) -> str:
         if not country_id:  # get country_id from location_id
             if not location_id:  # get location_id from contact_id or profile_id
                 if contact_id and not profile_id:  # get profile_id from contact_id
                     profile_id = self.select_one_value_by_column_and_value(
                         schema_name="contact_profile",
                         view_table_name='contact_profile_view', select_clause_value='profile_id',
                         column_name='contact_id', column_value=contact_id)
@@ -119,24 +115,27 @@
             column_name='country_id', column_value=country_id)
         return country_iso_code
 
     # TODO: Is it really necessary to access the database for location?
     # I think it's possible to get the normalized phone number and the international code
     # from original_phone_number
     def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None,
-                      profile_id: int = None, person_id: str = None) -> dict:
+                      profile_id: int = None, person_id: str = None, location_id: int = None,
+                      country_id: int = None) -> dict:
         """
         Process phone number and return normalized phone number.
         :param original_phone_number: Original phone number.
         :param country_iso_code: Country ISO code.
         :param contact_id: Contact id.
         :return: Dictionary with the normalized phone number and the international code.
         """
         logger.start(object={'original_phone_number': original_phone_number})
-        country_iso_code = country_iso_code or self.get_country_iso_code()
+        country_iso_code = country_iso_code or self.get_country_iso_code(
+            location_id=location_id, contact_id=contact_id, profile_id=profile_id, country_id=country_id
+        )
         normalized_phone_number = self.normalize_phone_number(
             original_number=original_phone_number, region=country_iso_code)
         phone_dict = {
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
```

### Comparing `phones_local-0.0.32/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.33/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.32
+Version: 0.0.33
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.32/pyproject.toml` & `phones_local-0.0.33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.32/setup.py` & `phones_local-0.0.33/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.32',  # https://pypi.org/project/phones-local/
+    version='0.0.33',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

