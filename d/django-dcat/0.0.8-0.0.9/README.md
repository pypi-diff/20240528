# Comparing `tmp/django-dcat-0.0.8.tar.gz` & `tmp/django_dcat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dcat-0.0.8.tar", last modified: Sun Jan  7 15:03:42 2024, max compression
+gzip compressed data, was "django_dcat-0.0.9.tar", last modified: Tue May 28 15:46:48 2024, max compression
```

## Comparing `django-dcat-0.0.8.tar` & `django_dcat-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.804526 django-dcat-0.0.8/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1060 2023-12-12 08:26:00.000000 django-dcat-0.0.8/LICENSE
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       34 2023-12-18 20:34:28.000000 django-dcat-0.0.8/MANIFEST.in
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     5064 2024-01-07 15:03:42.804526 django-dcat-0.0.8/PKG-INFO
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     4062 2024-01-05 16:05:48.000000 django-dcat-0.0.8/README.rst
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.800526 django-dcat-0.0.8/dcat/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/__init__.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      812 2024-01-07 14:03:36.000000 django-dcat-0.0.8/dcat/admin.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      140 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/apps.py
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.800526 django-dcat-0.0.8/dcat/management/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/management/__init__.py
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.800526 django-dcat-0.0.8/dcat/management/commands/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/management/commands/__init__.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     2111 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/management/commands/dump_from_datajson.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1625 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/management/commands/import_filetypes.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     6143 2024-01-07 14:22:36.000000 django-dcat-0.0.8/dcat/management/commands/import_from_datajson.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     2534 2024-01-07 14:22:35.000000 django-dcat-0.0.8/dcat/management/commands/import_licences.py
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.804526 django-dcat-0.0.8/dcat/migrations/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     7711 2023-12-18 20:23:20.000000 django-dcat-0.0.8/dcat/migrations/0001_initial.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      495 2023-12-18 20:49:58.000000 django-dcat-0.0.8/dcat/migrations/0002_rename_license_catalog_licence_and_more.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      398 2023-12-20 22:23:54.000000 django-dcat-0.0.8/dcat/migrations/0003_catalog_homepage.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      737 2023-12-20 23:41:49.000000 django-dcat-0.0.8/dcat/migrations/0004_alter_catalog_themes_alter_dataset_description_and_more.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      948 2023-12-21 00:22:06.000000 django-dcat-0.0.8/dcat/migrations/0005_keyword_dataset_keywords.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      401 2023-12-21 17:05:26.000000 django-dcat-0.0.8/dcat/migrations/0006_alter_datatheme_code.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      551 2023-12-21 22:30:16.000000 django-dcat-0.0.8/dcat/migrations/0007_dataset_issued_dataset_modified.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1445 2023-12-21 22:39:25.000000 django-dcat-0.0.8/dcat/migrations/0008_dataservice.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      382 2024-01-05 15:39:49.000000 django-dcat-0.0.8/dcat/migrations/0009_alter_agent_type.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      379 2024-01-05 16:06:40.000000 django-dcat-0.0.8/dcat/migrations/0010_dataset_landing_page.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      486 2024-01-05 16:33:39.000000 django-dcat-0.0.8/dcat/migrations/0011_alter_distribution_file.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      410 2024-01-05 16:39:48.000000 django-dcat-0.0.8/dcat/migrations/0012_distribution_external_access_url.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      590 2024-01-06 20:55:36.000000 django-dcat-0.0.8/dcat/migrations/0013_alter_catalog_licence.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     9014 2024-01-07 14:59:46.000000 django-dcat-0.0.8/dcat/migrations/0014_alter_agent_mbox_alter_agent_name_alter_agent_type_and_more.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/migrations/__init__.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)    10669 2024-01-07 14:53:46.000000 django-dcat-0.0.8/dcat/models.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       60 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/tests.py
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       63 2023-12-12 08:26:00.000000 django-dcat-0.0.8/dcat/views.py
-drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-01-07 15:03:42.804526 django-dcat-0.0.8/django_dcat.egg-info/
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     5064 2024-01-07 15:03:42.000000 django-dcat-0.0.8/django_dcat.egg-info/PKG-INFO
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1312 2024-01-07 15:03:42.000000 django-dcat-0.0.8/django_dcat.egg-info/SOURCES.txt
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        1 2024-01-07 15:03:42.000000 django-dcat-0.0.8/django_dcat.egg-info/dependency_links.txt
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       12 2024-01-07 15:03:42.000000 django-dcat-0.0.8/django_dcat.egg-info/requires.txt
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        5 2024-01-07 15:03:42.000000 django-dcat-0.0.8/django_dcat.egg-info/top_level.txt
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      974 2024-01-07 15:03:42.804526 django-dcat-0.0.8/setup.cfg
--rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       38 2023-12-12 08:26:00.000000 django-dcat-0.0.8/setup.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.127582 django_dcat-0.0.9/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1060 2023-12-12 08:26:00.000000 django_dcat-0.0.9/LICENSE
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       34 2023-12-18 20:34:28.000000 django_dcat-0.0.9/MANIFEST.in
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     5444 2024-05-28 15:46:48.127582 django_dcat-0.0.9/PKG-INFO
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     4442 2024-05-28 15:42:33.000000 django_dcat-0.0.9/README.rst
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.107582 django_dcat-0.0.9/dcat/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/__init__.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      812 2024-01-07 14:03:36.000000 django_dcat-0.0.9/dcat/admin.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      140 2024-03-23 13:07:12.000000 django_dcat-0.0.9/dcat/apps.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.107582 django_dcat-0.0.9/dcat/management/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/management/__init__.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.107582 django_dcat-0.0.9/dcat/management/commands/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/management/commands/__init__.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     2111 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/management/commands/dump_from_datajson.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1625 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/management/commands/import_filetypes.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     6143 2024-01-07 14:22:36.000000 django_dcat-0.0.9/dcat/management/commands/import_from_datajson.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     2534 2024-01-07 14:22:35.000000 django_dcat-0.0.9/dcat/management/commands/import_licences.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.127582 django_dcat-0.0.9/dcat/migrations/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     7711 2023-12-18 20:23:20.000000 django_dcat-0.0.9/dcat/migrations/0001_initial.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      495 2023-12-18 20:49:58.000000 django_dcat-0.0.9/dcat/migrations/0002_rename_license_catalog_licence_and_more.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      398 2023-12-20 22:23:54.000000 django_dcat-0.0.9/dcat/migrations/0003_catalog_homepage.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      737 2023-12-20 23:41:49.000000 django_dcat-0.0.9/dcat/migrations/0004_alter_catalog_themes_alter_dataset_description_and_more.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      948 2023-12-21 00:22:06.000000 django_dcat-0.0.9/dcat/migrations/0005_keyword_dataset_keywords.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      401 2023-12-21 17:05:26.000000 django_dcat-0.0.9/dcat/migrations/0006_alter_datatheme_code.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      551 2023-12-21 22:30:16.000000 django_dcat-0.0.9/dcat/migrations/0007_dataset_issued_dataset_modified.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1445 2023-12-21 22:39:25.000000 django_dcat-0.0.9/dcat/migrations/0008_dataservice.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      382 2024-01-05 15:39:49.000000 django_dcat-0.0.9/dcat/migrations/0009_alter_agent_type.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      379 2024-01-05 16:06:40.000000 django_dcat-0.0.9/dcat/migrations/0010_dataset_landing_page.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      486 2024-01-05 16:33:39.000000 django_dcat-0.0.9/dcat/migrations/0011_alter_distribution_file.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      410 2024-01-05 16:39:48.000000 django_dcat-0.0.9/dcat/migrations/0012_distribution_external_access_url.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      590 2024-01-06 20:55:36.000000 django_dcat-0.0.9/dcat/migrations/0013_alter_catalog_licence.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     9014 2024-01-07 14:59:46.000000 django_dcat-0.0.9/dcat/migrations/0014_alter_agent_mbox_alter_agent_name_alter_agent_type_and_more.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        0 2023-12-12 08:26:00.000000 django_dcat-0.0.9/dcat/migrations/__init__.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)    12153 2024-05-28 15:42:33.000000 django_dcat-0.0.9/dcat/models.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       60 2024-05-18 08:19:00.000000 django_dcat-0.0.9/dcat/tests.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       63 2024-05-26 11:51:09.000000 django_dcat-0.0.9/dcat/views.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.127582 django_dcat-0.0.9/django_dcat.egg-info/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     5444 2024-05-28 15:46:48.000000 django_dcat-0.0.9/django_dcat.egg-info/PKG-INFO
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1375 2024-05-28 15:46:48.000000 django_dcat-0.0.9/django_dcat.egg-info/SOURCES.txt
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        1 2024-05-28 15:46:48.000000 django_dcat-0.0.9/django_dcat.egg-info/dependency_links.txt
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       12 2024-05-28 15:46:48.000000 django_dcat-0.0.9/django_dcat.egg-info/requires.txt
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)        5 2024-05-28 15:46:48.000000 django_dcat-0.0.9/django_dcat.egg-info/top_level.txt
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     1044 2024-05-28 15:46:48.127582 django_dcat-0.0.9/setup.cfg
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)       38 2024-05-19 08:04:22.000000 django_dcat-0.0.9/setup.py
+drwxr-xr-x   0 pdelboca  (1000) pdelboca  (1000)        0 2024-05-28 15:46:48.127582 django_dcat-0.0.9/tests/
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)     3536 2024-05-28 15:42:33.000000 django_dcat-0.0.9/tests/test_dcat_jsonld_serialization.py
+-rw-r--r--   0 pdelboca  (1000) pdelboca  (1000)      214 2024-05-28 15:42:33.000000 django_dcat-0.0.9/tests/test_settings.py
```

### Comparing `django-dcat-0.0.8/LICENSE` & `django_dcat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/PKG-INFO` & `django_dcat-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dcat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app that provides a model layer and tools for DCAT applications.
 Home-page: https://github.com/pdelboca/django-dcat/
 Author: Patricio Del Boca
 Author-email: patriciodelboca@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,16 +28,16 @@
 ===========
 django-dcat
 ===========
 
 django-dcat is a Django app that provides a model layer for `DCAT 3.0 <https://www.w3.org/TR/vocab-dcat-3/>`_
 metadata and some command line tools to import data to it, to create vocabularies and more.
 
-**Note:** This is a work in progress and it is not stable for production. If you wanna see an example of what can
-be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a data catalog implemented with django-dcat.
+If you wanna see an example of what can be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a
+data catalog implemented with django-dcat.
 
 Quick start
 ###########
 
 1. Install the package using pip::
 
     pip install django-dcat
@@ -94,14 +94,24 @@
 
 
 The goal of these commands is to provide data publishers with pre-filled options for the metadata fields. This will improve
 data quality and avoid common problems like duplicated metadata values for typos or inconsistent data entry (like distributions with
 .csv, .CSV, CSV, etc)
 
 
+DCAT Serialization
+##################
+
+Every object contains methods to serialize it to different formats. This way it is easy to implement a feed URL for your catalog.
+
+ - ``catalog.to_jsonld()``: (WIP) exports the catalog to a JSONLD format. The implementation has been inspired by the `FAO - Data in Emergencies feed <https://data-in-emergencies.fao.org/api/feed/dcat-ap/2.1.1.json>`_.
+ - ``catalog.to_turtle()``: TODO
+ - ``catalog.to_rdf()``: TODO
+
+
 Extending the model
 ###################
 
 ``django-dcat`` focuses on providing a model layer for DCAT metadata. However, if you require custom fields in your application,
 you can extend any model using a OneToOneField pattern (similar to what you use to extend Django's User model).
 
 .. code:: python
```

### Comparing `django-dcat-0.0.8/README.rst` & `django_dcat-0.0.9/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 ===========
 django-dcat
 ===========
 
 django-dcat is a Django app that provides a model layer for `DCAT 3.0 <https://www.w3.org/TR/vocab-dcat-3/>`_
 metadata and some command line tools to import data to it, to create vocabularies and more.
 
-**Note:** This is a work in progress and it is not stable for production. If you wanna see an example of what can
-be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a data catalog implemented with django-dcat.
+If you wanna see an example of what can be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a
+data catalog implemented with django-dcat.
 
 Quick start
 ###########
 
 1. Install the package using pip::
 
     pip install django-dcat
@@ -68,14 +68,24 @@
 
 
 The goal of these commands is to provide data publishers with pre-filled options for the metadata fields. This will improve
 data quality and avoid common problems like duplicated metadata values for typos or inconsistent data entry (like distributions with
 .csv, .CSV, CSV, etc)
 
 
+DCAT Serialization
+##################
+
+Every object contains methods to serialize it to different formats. This way it is easy to implement a feed URL for your catalog.
+
+ - ``catalog.to_jsonld()``: (WIP) exports the catalog to a JSONLD format. The implementation has been inspired by the `FAO - Data in Emergencies feed <https://data-in-emergencies.fao.org/api/feed/dcat-ap/2.1.1.json>`_.
+ - ``catalog.to_turtle()``: TODO
+ - ``catalog.to_rdf()``: TODO
+
+
 Extending the model
 ###################
 
 ``django-dcat`` focuses on providing a model layer for DCAT metadata. However, if you require custom fields in your application,
 you can extend any model using a OneToOneField pattern (similar to what you use to extend Django's User model).
 
 .. code:: python
```

### Comparing `django-dcat-0.0.8/dcat/admin.py` & `django_dcat-0.0.9/dcat/admin.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/management/commands/dump_from_datajson.py` & `django_dcat-0.0.9/dcat/management/commands/dump_from_datajson.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/management/commands/import_filetypes.py` & `django_dcat-0.0.9/dcat/management/commands/import_filetypes.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/management/commands/import_from_datajson.py` & `django_dcat-0.0.9/dcat/management/commands/import_from_datajson.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/management/commands/import_licences.py` & `django_dcat-0.0.9/dcat/management/commands/import_licences.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0001_initial.py` & `django_dcat-0.0.9/dcat/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0004_alter_catalog_themes_alter_dataset_description_and_more.py` & `django_dcat-0.0.9/dcat/migrations/0004_alter_catalog_themes_alter_dataset_description_and_more.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0005_keyword_dataset_keywords.py` & `django_dcat-0.0.9/dcat/migrations/0005_keyword_dataset_keywords.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0007_dataset_issued_dataset_modified.py` & `django_dcat-0.0.9/dcat/migrations/0007_dataset_issued_dataset_modified.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0008_dataservice.py` & `django_dcat-0.0.9/dcat/migrations/0008_dataservice.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0013_alter_catalog_licence.py` & `django_dcat-0.0.9/dcat/migrations/0013_alter_catalog_licence.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/migrations/0014_alter_agent_mbox_alter_agent_name_alter_agent_type_and_more.py` & `django_dcat-0.0.9/dcat/migrations/0014_alter_agent_mbox_alter_agent_name_alter_agent_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django-dcat-0.0.8/dcat/models.py` & `django_dcat-0.0.9/dcat/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,18 +28,26 @@
     type = models.CharField(
         max_length=20,
         blank=True,
         help_text="A type of the agent that makes the Catalogue or Dataset available.",
     )
 
     # Optional properties
+    # TODO: mbox is not defined in DCAT
     mbox = models.EmailField(
         blank=True, null=True, help_text="An email address of the Agent."
     )
 
+    def to_jsonld(self):
+        result = dict()
+        result["foaf:name"] = self.name
+        if self.type:
+            result["@type"] = self.type
+        return result
+
     def __str__(self):
         return self.name
 
 
 class Catalog(models.Model):
     """A catalogue that hosts the Datasets or Data Services being described."""
 
@@ -65,14 +73,27 @@
         blank=True,
         help_text="A knowledge organization system used to classify the Catalogue's Datasets.",
     )
     homepage = models.URLField(
         blank=True, help_text="A web page that acts as the main page for the Catalogue."
     )
 
+    def to_jsonld(self):
+        result = dict()
+        result["@type"] = "dcat:Catalog"
+        result["dct:title"] = self.title
+        result["dct:description"] = self.description
+        result["dct:publisher"] = self.publisher.to_jsonld()
+        if self.homepage:
+            result["foaf:homepage"] = {"@type": "foaf:Document", "foaf:Document": self.homepage}
+
+        result["dcat:dataset"] = [dataset.to_jsonld() for dataset in self.dataset_set.all()]
+
+        return result
+
     def __str__(self):
         return self.title
 
 
 # class CatalogRecord(models.Model):
 #     """A description of a Dataset's entry in the Catalogue.
 
@@ -90,14 +111,15 @@
     """A conceptual entity that represents the information published."""
 
     # Mandatory properties
     title = models.CharField(max_length=255, help_text="A name given to the Dataset.")
     catalog = models.ForeignKey("Catalog", on_delete=models.CASCADE)
 
     # Recommended properties
+    # TODO: description is mandatory
     description = models.TextField(
         blank=True, help_text="A free-text account of the Dataset."
     )
     publisher = models.ForeignKey(
         "Agent",
         on_delete=models.SET_NULL,
         null=True,
@@ -120,14 +142,23 @@
     )
     issued = models.DateField(blank=True, null=True)
     landing_page = models.URLField(
         blank=True,
         help_text="A web page that provides access to the Dataset, its Distributions and/or additional information. It is intended to point to a landing page at the original data provider, not to a page on a site of a third party, such as an aggregator.",
     )
 
+    def to_jsonld(self):
+        result = dict()
+        result["dct:title"] = self.title
+        if self.description:
+            result["dct:description"] = self.description
+        result["dcat:distribution"] = [d.to_jsonld() for d in self.distribution_set.all()]
+
+        return result
+
     def __str__(self):
         return self.title
 
 
 # class DatasetInSeries(models.Model):
 #     """Capture the case when a Dataset is a member of a Dataset Series."""
 #     pass
@@ -160,15 +191,18 @@
     def access_url(self):
         """Return the access url of the file.
 
         If the file is hosted in another portal, the access_url is provided
         in the distribution. Otherwise, the access_url is the URL to the
         distribution.
         """
-        pass
+        if self.external_access_url:
+            return self.external_access_url
+        # TODO: Implement views in django-dcat
+        return ""
 
     # Recomened properties
     title = models.CharField(
         max_length=255, blank=True, help_text="A name given to the Distribution."
     )
     description = models.TextField(
         blank=True, help_text="A free-text account of the Distribution."
@@ -230,14 +264,24 @@
         """Calculates the md5 checksum of the file."""
         md5_hash = hashlib.md5()
         with self.file.open(mode="rb") as f:
             while chunk := f.read(4096):
                 md5_hash.update(chunk)
         return md5_hash.hexdigest()
 
+    def to_jsonld(self):
+        result = dict()
+        result["@type"] = "dcat:Distribution"
+        result["dcat:accessURL"] = self.access_url
+        if self.title:
+            result["dct:title"] = self.title
+        if self.description:
+            result["dct:description"] = self.description
+        return result
+
     def __str__(self):
         return self.title
 
 
 class DataService(models.Model):
     """Operations that provides access to datasets or data processing functions.
```

### Comparing `django-dcat-0.0.8/django_dcat.egg-info/PKG-INFO` & `django_dcat-0.0.9/django_dcat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dcat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app that provides a model layer and tools for DCAT applications.
 Home-page: https://github.com/pdelboca/django-dcat/
 Author: Patricio Del Boca
 Author-email: patriciodelboca@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,16 +28,16 @@
 ===========
 django-dcat
 ===========
 
 django-dcat is a Django app that provides a model layer for `DCAT 3.0 <https://www.w3.org/TR/vocab-dcat-3/>`_
 metadata and some command line tools to import data to it, to create vocabularies and more.
 
-**Note:** This is a work in progress and it is not stable for production. If you wanna see an example of what can
-be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a data catalog implemented with django-dcat.
+If you wanna see an example of what can be done checkout `Catalogo Social <https://catalogosocial.fly.dev/>`_, a
+data catalog implemented with django-dcat.
 
 Quick start
 ###########
 
 1. Install the package using pip::
 
     pip install django-dcat
@@ -94,14 +94,24 @@
 
 
 The goal of these commands is to provide data publishers with pre-filled options for the metadata fields. This will improve
 data quality and avoid common problems like duplicated metadata values for typos or inconsistent data entry (like distributions with
 .csv, .CSV, CSV, etc)
 
 
+DCAT Serialization
+##################
+
+Every object contains methods to serialize it to different formats. This way it is easy to implement a feed URL for your catalog.
+
+ - ``catalog.to_jsonld()``: (WIP) exports the catalog to a JSONLD format. The implementation has been inspired by the `FAO - Data in Emergencies feed <https://data-in-emergencies.fao.org/api/feed/dcat-ap/2.1.1.json>`_.
+ - ``catalog.to_turtle()``: TODO
+ - ``catalog.to_rdf()``: TODO
+
+
 Extending the model
 ###################
 
 ``django-dcat`` focuses on providing a model layer for DCAT metadata. However, if you require custom fields in your application,
 you can extend any model using a OneToOneField pattern (similar to what you use to extend Django's User model).
 
 .. code:: python
```

### Comparing `django-dcat-0.0.8/django_dcat.egg-info/SOURCES.txt` & `django_dcat-0.0.9/django_dcat.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -30,8 +30,10 @@
 dcat/migrations/0013_alter_catalog_licence.py
 dcat/migrations/0014_alter_agent_mbox_alter_agent_name_alter_agent_type_and_more.py
 dcat/migrations/__init__.py
 django_dcat.egg-info/PKG-INFO
 django_dcat.egg-info/SOURCES.txt
 django_dcat.egg-info/dependency_links.txt
 django_dcat.egg-info/requires.txt
-django_dcat.egg-info/top_level.txt
+django_dcat.egg-info/top_level.txt
+tests/test_dcat_jsonld_serialization.py
+tests/test_settings.py
```

### Comparing `django-dcat-0.0.8/setup.cfg` & `django_dcat-0.0.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dcat
-version = 0.0.8
+version = 0.0.9
 description = A Django app that provides a model layer and tools for DCAT applications.
 long_description = file: README.rst
 url = https://github.com/pdelboca/django-dcat/
 author = Patricio Del Boca
 author_email = patriciodelboca@gmail.com
 license = MIT
 classifiers = 
@@ -26,11 +26,18 @@
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	Django >= 5.0
 
+[flake8]
+extend-ignore = E501
+exclude = 
+	.git,
+	.venv,
+	__pycache__
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

