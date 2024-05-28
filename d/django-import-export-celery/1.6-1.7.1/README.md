# Comparing `tmp/django-import-export-celery-1.6.tar.gz` & `tmp/django_import_export_celery-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-celery-1.6.tar", last modified: Sat Jul 29 10:17:31 2023, max compression
+gzip compressed data, was "django_import_export_celery-1.7.1.tar", last modified: Tue May 28 10:28:23 2024, max compression
```

## Comparing `django-import-export-celery-1.6.tar` & `django_import_export_celery-1.7.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/django_import_export_celery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/admin_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/locale/pt/LC_MESSAGES/django.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0002_auto_20190923_1132.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0003_exportjob.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0004_exportjob_email_on_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0005_exportjob_site_of_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0006_auto_20191125_1236.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0007_auto_20210210_1831.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/models/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/exportjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/importjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/templates/email/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/templates/email/export_job_completion.html
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 10:28:22.000000 django_import_export_celery-1.7.1/django_import_export_celery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/import_export_celery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/admin_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.992227 django_import_export_celery-1.7.1/import_export_celery/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.992227 django_import_export_celery-1.7.1/import_export_celery/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/import_export_celery/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/locale/pt/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/import_export_celery/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0002_auto_20190923_1132.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0003_exportjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0004_exportjob_email_on_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0005_exportjob_site_of_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0006_auto_20191125_1236.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0007_auto_20210210_1831.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/0010_auto_20231013_0904.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/import_export_celery/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/models/exportjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/models/importjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.992227 django_import_export_celery-1.7.1/import_export_celery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/import_export_celery/templates/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/templates/email/export_job_completion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/import_export_celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 10:28:22.996227 django_import_export_celery-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-28 10:28:13.000000 django_import_export_celery-1.7.1/setup.py
```

### Comparing `django-import-export-celery-1.6/LICENSE` & `django_import_export_celery-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/PKG-INFO` & `django_import_export_celery-1.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export-celery
-Version: 1.6
+Version: 1.7.1
 Summary: Process long running django imports and exports in celery
 Home-page: https://github.com/auto-mat/django-import-export-celery
 Download-URL: http://pypi.python.org/pypi/django-import-export-celery/
 Author: Timothy Hobbs
 Author-email: timothy.hobbs@auto-mat.cz
 License: License :: OSI Approved :: GNU Lesser General Public License v3.0 or later (LGPLv3.0+)
 Classifier: Topic :: Utilities
@@ -14,14 +14,18 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: django-import-export
+Requires-Dist: django-author
+Requires-Dist: html2text
 
 .. image:: https://img.shields.io/pypi/v/django-import-export-celery.svg
    :target: https://pypi.org/project/django-import-export-celery/#history
 
 django-import-export-celery: process slow django imports and exports in celery
 ==============================================================================
 
@@ -75,15 +79,15 @@
 By default a dry run of the import is initiated when the import object is created. To instead import the file immediately without a dry-run set the `IMPORT_DRY_RUN_FIRST_TIME` to `False`
 
     ::
 
         IMPORT_DRY_RUN_FIRST_TIME = False
 
 
-Preforming an import
+Performing an import
 --------------------
 
 You will find an example django application that uses django-import-export-celery for importing data. There are instructions for running the example application in the example directory's README file. Once you have it running, you can perform an import with the following steps.
 
 1. Navigate to the example applications admin page:
 
    .. image:: screenshots/admin.png
@@ -186,23 +190,57 @@
 
 To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
 
     ::
 
         IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
 
+
 Customizing File Storage Backend
 --------------------------------
 
+**If you are using the new Django 4.2 STORAGES**:
+
+By default, `import_export_celery` uses Django `default` storage.
+To use your own storage, use the the `IMPORT_EXPORT_CELERY_STORAGE_ALIAS` variable in your Django settings and adding the STORAGES definition.
+For instance:
+
+    ::
+
+        STORAGES = {
+            "import_export_celery": {
+                "BACKEND": "storages.backends.s3boto3.S3Boto3Storage",
+            },
+        }
+        IMPORT_EXPORT_CELERY_STORAGE_ALIAS = 'import_export_celery'
+
+**DEPRECATED: If you are using old style storages**:
+
 Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
 
     ::
 
         IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
+
+Customizing Task Time Limits
+----------------------------
+
+By default, there is no time limit on celery import/export tasks. This can be customized by setting the following variables in your Django settings file.
+
+    ::
+
+        # set import time limits (in seconds)
+        IMPORT_EXPORT_CELERY_IMPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_IMPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
+        # set export time limits (in seconds)
+        IMPORT_EXPORT_CELERY_EXPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_EXPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
     ::
```

### Comparing `django-import-export-celery-1.6/README.rst` & `django_import_export_celery-1.7.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 By default a dry run of the import is initiated when the import object is created. To instead import the file immediately without a dry-run set the `IMPORT_DRY_RUN_FIRST_TIME` to `False`
 
     ::
 
         IMPORT_DRY_RUN_FIRST_TIME = False
 
 
-Preforming an import
+Performing an import
 --------------------
 
 You will find an example django application that uses django-import-export-celery for importing data. There are instructions for running the example application in the example directory's README file. Once you have it running, you can perform an import with the following steps.
 
 1. Navigate to the example applications admin page:
 
    .. image:: screenshots/admin.png
@@ -165,23 +165,57 @@
 
 To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
 
     ::
 
         IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
 
+
 Customizing File Storage Backend
 --------------------------------
 
+**If you are using the new Django 4.2 STORAGES**:
+
+By default, `import_export_celery` uses Django `default` storage.
+To use your own storage, use the the `IMPORT_EXPORT_CELERY_STORAGE_ALIAS` variable in your Django settings and adding the STORAGES definition.
+For instance:
+
+    ::
+
+        STORAGES = {
+            "import_export_celery": {
+                "BACKEND": "storages.backends.s3boto3.S3Boto3Storage",
+            },
+        }
+        IMPORT_EXPORT_CELERY_STORAGE_ALIAS = 'import_export_celery'
+
+**DEPRECATED: If you are using old style storages**:
+
 Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
 
     ::
 
         IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
+
+Customizing Task Time Limits
+----------------------------
+
+By default, there is no time limit on celery import/export tasks. This can be customized by setting the following variables in your Django settings file.
+
+    ::
+
+        # set import time limits (in seconds)
+        IMPORT_EXPORT_CELERY_IMPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_IMPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
+        # set export time limits (in seconds)
+        IMPORT_EXPORT_CELERY_EXPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_EXPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
     ::
```

### Comparing `django-import-export-celery-1.6/django_import_export_celery.egg-info/PKG-INFO` & `django_import_export_celery-1.7.1/django_import_export_celery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export-celery
-Version: 1.6
+Version: 1.7.1
 Summary: Process long running django imports and exports in celery
 Home-page: https://github.com/auto-mat/django-import-export-celery
 Download-URL: http://pypi.python.org/pypi/django-import-export-celery/
 Author: Timothy Hobbs
 Author-email: timothy.hobbs@auto-mat.cz
 License: License :: OSI Approved :: GNU Lesser General Public License v3.0 or later (LGPLv3.0+)
 Classifier: Topic :: Utilities
@@ -14,14 +14,18 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: django-import-export
+Requires-Dist: django-author
+Requires-Dist: html2text
 
 .. image:: https://img.shields.io/pypi/v/django-import-export-celery.svg
    :target: https://pypi.org/project/django-import-export-celery/#history
 
 django-import-export-celery: process slow django imports and exports in celery
 ==============================================================================
 
@@ -75,15 +79,15 @@
 By default a dry run of the import is initiated when the import object is created. To instead import the file immediately without a dry-run set the `IMPORT_DRY_RUN_FIRST_TIME` to `False`
 
     ::
 
         IMPORT_DRY_RUN_FIRST_TIME = False
 
 
-Preforming an import
+Performing an import
 --------------------
 
 You will find an example django application that uses django-import-export-celery for importing data. There are instructions for running the example application in the example directory's README file. Once you have it running, you can perform an import with the following steps.
 
 1. Navigate to the example applications admin page:
 
    .. image:: screenshots/admin.png
@@ -186,23 +190,57 @@
 
 To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
 
     ::
 
         IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
 
+
 Customizing File Storage Backend
 --------------------------------
 
+**If you are using the new Django 4.2 STORAGES**:
+
+By default, `import_export_celery` uses Django `default` storage.
+To use your own storage, use the the `IMPORT_EXPORT_CELERY_STORAGE_ALIAS` variable in your Django settings and adding the STORAGES definition.
+For instance:
+
+    ::
+
+        STORAGES = {
+            "import_export_celery": {
+                "BACKEND": "storages.backends.s3boto3.S3Boto3Storage",
+            },
+        }
+        IMPORT_EXPORT_CELERY_STORAGE_ALIAS = 'import_export_celery'
+
+**DEPRECATED: If you are using old style storages**:
+
 Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
 
     ::
 
         IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
+
+Customizing Task Time Limits
+----------------------------
+
+By default, there is no time limit on celery import/export tasks. This can be customized by setting the following variables in your Django settings file.
+
+    ::
+
+        # set import time limits (in seconds)
+        IMPORT_EXPORT_CELERY_IMPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_IMPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
+        # set export time limits (in seconds)
+        IMPORT_EXPORT_CELERY_EXPORT_SOFT_TIME_LIMIT = 300  # 5 minutes
+        IMPORT_EXPORT_CELERY_EXPORT_HARD_TIME_LIMIT = 360  # 6 minutes
+
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
     ::
```

### Comparing `django-import-export-celery-1.6/django_import_export_celery.egg-info/SOURCES.txt` & `django_import_export_celery-1.7.1/django_import_export_celery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 import_export_celery/migrations/0003_exportjob.py
 import_export_celery/migrations/0004_exportjob_email_on_completion.py
 import_export_celery/migrations/0005_exportjob_site_of_origin.py
 import_export_celery/migrations/0006_auto_20191125_1236.py
 import_export_celery/migrations/0007_auto_20210210_1831.py
 import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
 import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py
+import_export_celery/migrations/0010_auto_20231013_0904.py
 import_export_celery/migrations/__init__.py
 import_export_celery/models/__init__.py
 import_export_celery/models/exportjob.py
 import_export_celery/models/importjob.py
 import_export_celery/templates/email/export_job_completion.html
```

### Comparing `django-import-export-celery-1.6/import_export_celery/admin.py` & `django_import_export_celery-1.7.1/import_export_celery/admin.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/admin_actions.py` & `django_import_export_celery-1.7.1/import_export_celery/admin_actions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/locale/pt/LC_MESSAGES/django.mo` & `django_import_export_celery-1.7.1/import_export_celery/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0001_initial.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0003_exportjob.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0003_exportjob.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0004_exportjob_email_on_completion.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0004_exportjob_email_on_completion.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0006_auto_20191125_1236.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0006_auto_20191125_1236.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0007_auto_20210210_1831.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0007_auto_20210210_1831.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py` & `django_import_export_celery-1.7.1/import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/models/exportjob.py` & `django_import_export_celery-1.7.1/import_export_celery/models/exportjob.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/import_export_celery/models/importjob.py` & `django_import_export_celery-1.7.1/import_export_celery/models/importjob.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from django.utils import timezone
 
 from author.decorators import with_author
 
 from django.db import models, transaction
 from django.dispatch import receiver
 
-from django.db.models.signals import post_save
+from django.db.models.signals import post_save, post_delete
 from django.utils.translation import gettext_lazy as _
 
 from import_export.formats.base_formats import DEFAULT_FORMATS
 
 from ..fields import ImportExportFileField
 from ..tasks import run_import_job
 
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 @with_author
 class ImportJob(models.Model):
     file = ImportExportFileField(
         verbose_name=_("File to be imported"),
         upload_to="django-import-export-celery-import-jobs",
         blank=False,
@@ -91,7 +95,22 @@
         instance.save()
         transaction.on_commit(
             lambda: run_import_job.delay(
                 instance.pk,
                 dry_run=getattr(settings, "IMPORT_DRY_RUN_FIRST_TIME", True),
             )
         )
+
+
+@receiver(post_delete, sender=ImportJob)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file related to the import job
+    """
+    if instance.file:
+        try:
+            instance.file.delete()
+        except Exception as e:
+            logger.error(
+                "Some error occurred while deleting ImportJob file: {0}".format(e)
+            )
+        ImportJob.objects.filter(id=instance.id).delete()
```

### Comparing `django-import-export-celery-1.6/import_export_celery/tasks.py` & `django_import_export_celery-1.7.1/import_export_celery/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,28 +184,36 @@
         )
     else:
         import_job.imported = timezone.now()
     change_job_status(import_job, "import", "5/5 Import job finished", dry_run)
     import_job.save()
 
 
-@shared_task(bind=False)
+@shared_task(
+    bind=False,
+    soft_time_limit=getattr(settings, "IMPORT_EXPORT_CELERY_IMPORT_SOFT_TIME_LIMIT", 0),
+    time_limit=getattr(settings, "IMPORT_EXPORT_CELERY_IMPORT_HARD_TIME_LIMIT", 0),
+)
 def run_import_job(pk, dry_run=True):
     log.info(f"Importing {pk} dry-run {dry_run}")
     import_job = models.ImportJob.objects.get(pk=pk)
     try:
         _run_import_job(import_job, dry_run)
     except Exception as e:
         import_job.errors += _("Import error %s") % e + "\n"
         change_job_status(import_job, "import", "Import error", dry_run)
         import_job.save()
         return
 
 
-@shared_task(bind=False)
+@shared_task(
+    bind=False,
+    soft_time_limit=getattr(settings, "IMPORT_EXPORT_CELERY_EXPORT_SOFT_TIME_LIMIT", 0),
+    time_limit=getattr(settings, "IMPORT_EXPORT_CELERY_EXPORT_HARD_TIME_LIMIT", 0),
+)
 def run_export_job(pk):
     log.info("Exporting %s" % pk)
     export_job = models.ExportJob.objects.get(pk=pk)
     resource_class = export_job.get_resource_class()
     queryset = export_job.get_queryset()
     qs_len = len(queryset)
```

### Comparing `django-import-export-celery-1.6/import_export_celery/utils.py` & `django_import_export_celery-1.7.1/import_export_celery/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.6/setup.py` & `django_import_export_celery-1.7.1/setup.py`

 * *Files identical despite different names*

