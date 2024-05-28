# Comparing `tmp/django-admin-export-action-0.3.1.tar.gz` & `tmp/django_admin_export_action-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-export-action-0.3.1.tar", last modified: Thu Nov  3 09:20:59 2022, max compression
+gzip compressed data, was "django_admin_export_action-0.3.2.tar", last modified: Tue May 28 16:03:28 2024, max compression
```

## Comparing `django-admin-export-action-0.3.1.tar` & `django_admin_export_action-0.3.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.800523 django-admin-export-action-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5842 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/introspection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.792523 django-admin-export-action-0.3.1/admin_export_action/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.792523 django-admin-export-action-0.3.1/admin_export_action/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8930 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/admin_export_action/templates/export_action/
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/templates/export_action/export.html
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/templates/export_action/fields.html
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/templates/export_action/report_html.html
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/admin_export_action/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 09:20:59.796523 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-11-03 09:20:59.000000 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-11-03 09:20:59.000000 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 09:20:59.000000 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-03 09:20:59.000000 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-03 09:20:59.000000 django-admin-export-action-0.3.1/django_admin_export_action.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 09:20:59.800523 django-admin-export-action-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-11-03 09:20:45.000000 django-admin-export-action-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/introspection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/admin_export_action/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/admin_export_action/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/admin_export_action/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.784839 django_admin_export_action-0.3.2/admin_export_action/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/admin_export_action/templates/export_action/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/templates/export_action/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/templates/export_action/fields.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/templates/export_action/report_html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/admin_export_action/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-28 16:03:28.000000 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-28 16:03:28.000000 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:03:28.000000 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 16:03:28.000000 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 16:03:28.000000 django_admin_export_action-0.3.2/django_admin_export_action.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:03:28.788839 django_admin_export_action-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-28 16:03:19.000000 django_admin_export_action-0.3.2/setup.py
```

### Comparing `django-admin-export-action-0.3.1/LICENSE` & `django_admin_export_action-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/PKG-INFO` & `django_admin_export_action-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-export-action
-Version: 0.3.1
+Version: 0.3.2
 Summary: Export action for django admin
 Home-page: http://github.com/otto-torino/django-admin-export-action
 Author: abidibo
 Author-email: abidibo@gmail.com
 License: MIT License
 Project-URL: Documentation, http://github.com/otto-torino/django-admin-export-action/blob/master/README.md
 Project-URL: Source, http://github.com/otto-torino/django-admin-export-action
@@ -21,17 +21,20 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl
 
 # Django Admin Export Action
 
 
 ![Version](https://img.shields.io/github/v/tag/otto-torino/django-admin-export-action?label=version)
 [![Build status](https://travis-ci.com/otto-torino/django-admin-export-action.svg?branch=master)](https://travis-ci.com/github/otto-torino/django-admin-export-action)
 ![License](https://img.shields.io/github/license/otto-torino/django-admin-export-action)
```

### Comparing `django-admin-export-action-0.3.1/README.md` & `django_admin_export_action-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/admin.py` & `django_admin_export_action-0.3.2/admin_export_action/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/introspection.py` & `django_admin_export_action-0.3.2/admin_export_action/introspection.py`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/es/LC_MESSAGES/django.mo` & `django_admin_export_action-0.3.2/admin_export_action/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/es/LC_MESSAGES/django.po` & `django_admin_export_action-0.3.2/admin_export_action/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/it/LC_MESSAGES/django.mo` & `django_admin_export_action-0.3.2/admin_export_action/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/it/LC_MESSAGES/django.po` & `django_admin_export_action-0.3.2/admin_export_action/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/pt/LC_MESSAGES/django.mo` & `django_admin_export_action-0.3.2/admin_export_action/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/pt/LC_MESSAGES/django.po` & `django_admin_export_action-0.3.2/admin_export_action/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/ru/LC_MESSAGES/django.mo` & `django_admin_export_action-0.3.2/admin_export_action/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/ru/LC_MESSAGES/django.po` & `django_admin_export_action-0.3.2/admin_export_action/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.po` & `django_admin_export_action-0.3.2/admin_export_action/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/report.py` & `django_admin_export_action-0.3.2/admin_export_action/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         from django.utils.encoding import force_str as force_text
 from django.template.loader import render_to_string
 from django.utils import timezone
 
 from openpyxl.styles import Font
 from openpyxl.utils import get_column_letter
 from openpyxl.workbook import Workbook
-from openpyxl.writer.excel import save_virtual_workbook
+from tempfile import NamedTemporaryFile
 
-from six import BytesIO, text_type
+from six import text_type
 
 from .introspection import get_model_from_path_string
 from .config import get_config
 
 
 DisplayField = namedtuple("DisplayField", "path field")
 
@@ -220,22 +220,25 @@
         build_sheet(data, ws, header=header, widths=widths)
     return wb
 
 
 def build_xlsx_response(wb, title="report"):
     """ Take a workbook and return a xlsx file response """
     title = generate_filename(title, '.xlsx')
-    myfile = BytesIO()
-    myfile.write(save_virtual_workbook(wb))
-    response = HttpResponse(
-        myfile.getvalue(),
-        content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-    response['Content-Disposition'] = 'attachment; filename=%s' % title
-    response['Content-Length'] = myfile.tell()
-    return response
+    response = HttpResponse(content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
+    with NamedTemporaryFile() as tmp:
+        wb.save(tmp.name)
+        tmp.seek(0)
+        response = HttpResponse(
+            tmp.read(),
+            content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
+        response['Content-Disposition'] = 'attachment; filename=%s' % title
+        response['Content-Length'] = tmp.tell()
+
+        return response
 
 
 def list_to_xlsx_response(data, title='report', header=None,
                           widths=None):
     """ Make 2D list into a xlsx response for download
     data can be a 2d array or a dict of 2d arrays
     like {'sheet_1': [['A1', 'B1']]}
```

### Comparing `django-admin-export-action-0.3.1/admin_export_action/templates/export_action/export.html` & `django_admin_export_action-0.3.2/admin_export_action/templates/export_action/export.html`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/templates/export_action/fields.html` & `django_admin_export_action-0.3.2/admin_export_action/templates/export_action/fields.html`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/admin_export_action/views.py` & `django_admin_export_action-0.3.2/admin_export_action/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,27 +49,31 @@
         field_name = self.request.GET.get('field', '')
         model_class = self.get_model_class()
         queryset = self.get_queryset(model_class)
         path = self.request.GET.get('path', '')
         context['opts'] = model_class._meta
         context['queryset'] = queryset
         context['model_ct'] = self.request.GET['ct']
-        context[
-            'related_fields'] = introspection.get_relation_fields_from_model(
-                model_class)
+
+        related = introspection.get_relation_fields_from_model(model_class)
+        context['related_fields'] = sorted(related, key=lambda x: x.verbose_name if hasattr(x, 'verbose_name') else x.get_accessor_name())
 
         # extra context
         try:
             model_admin = admin.site._registry[model_class]
         except KeyError:
             raise ValueError("Model %r not registered with admin" %
                              model_class)
+
         context.update(model_admin.admin_site.each_context(self.request))
 
-        context.update(introspection.get_fields(model_class, field_name, path))
+        struct = introspection.get_fields(model_class, field_name, path)
+        context.update({
+            "fields": sorted(struct.get("fields"), key=lambda x: x.verbose_name if hasattr(x, 'verbose_name') else x.name),
+        })
         return context
 
     def post(self, request, **kwargs):
         context = self.get_context_data(**kwargs)
         fields = []
         for field_name, value in request.POST.items():
             if value == "on":
```

### Comparing `django-admin-export-action-0.3.1/django_admin_export_action.egg-info/PKG-INFO` & `django_admin_export_action-0.3.2/django_admin_export_action.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-export-action
-Version: 0.3.1
+Version: 0.3.2
 Summary: Export action for django admin
 Home-page: http://github.com/otto-torino/django-admin-export-action
 Author: abidibo
 Author-email: abidibo@gmail.com
 License: MIT License
 Project-URL: Documentation, http://github.com/otto-torino/django-admin-export-action/blob/master/README.md
 Project-URL: Source, http://github.com/otto-torino/django-admin-export-action
@@ -21,17 +21,20 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl
 
 # Django Admin Export Action
 
 
 ![Version](https://img.shields.io/github/v/tag/otto-torino/django-admin-export-action?label=version)
 [![Build status](https://travis-ci.com/otto-torino/django-admin-export-action.svg?branch=master)](https://travis-ci.com/github/otto-torino/django-admin-export-action)
 ![License](https://img.shields.io/github/license/otto-torino/django-admin-export-action)
```

### Comparing `django-admin-export-action-0.3.1/django_admin_export_action.egg-info/SOURCES.txt` & `django_admin_export_action-0.3.2/django_admin_export_action.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-export-action-0.3.1/setup.py` & `django_admin_export_action-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 REPO_URL = 'http://github.com/otto-torino/django-admin-export-action'
 
 setup(
     name='django-admin-export-action',
-    version='0.3.1',
+    version='0.3.2',
     packages=['admin_export_action'],
     include_package_data=True,
     license='MIT License',
     description='Export action for django admin',
     long_description=README,
     long_description_content_type='text/markdown',
     url=REPO_URL,
@@ -37,14 +37,16 @@
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
     ],
     project_urls={
         'Documentation': REPO_URL + '/blob/master/README.md',
         'Source': REPO_URL,
         'Tracker': REPO_URL + '/issues',
     },
```

