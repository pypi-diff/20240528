# Comparing `tmp/ellis_django_views-0.231.tar.gz` & `tmp/ellis_django_views-0.232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.231.tar", last modified: Tue May 28 01:27:47 2024, max compression
+gzip compressed data, was "ellis_django_views-0.232.tar", last modified: Tue May 28 03:31:43 2024, max compression
```

## Comparing `ellis_django_views-0.231.tar` & `ellis_django_views-0.232.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.138745 ellis_django_views-0.231/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.231/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.231/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 01:27:47.138269 ellis_django_views-0.231/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)     3579 2024-05-21 12:30:17.000000 ellis_django_views-0.231/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.127105 ellis_django_views-0.231/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.231/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.130710 ellis_django_views-0.231/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.231/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.231/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.134523 ellis_django_views-0.231/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.231/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.231/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.231/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17640 2024-05-28 01:24:34.000000 ellis_django_views-0.231/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.231/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.231/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.137503 ellis_django_views-0.231/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.231/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.231/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.231/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6010 2024-05-22 00:22:52.000000 ellis_django_views-0.231/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.129679 ellis_django_views-0.231/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-28 01:27:47.138839 ellis_django_views-0.231/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-28 01:27:12.000000 ellis_django_views-0.231/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.536926 ellis_django_views-0.232/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.232/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.232/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 03:31:43.536635 ellis_django_views-0.232/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     3579 2024-05-21 12:30:17.000000 ellis_django_views-0.232/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.525197 ellis_django_views-0.232/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.232/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.232/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.528976 ellis_django_views-0.232/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.232/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.232/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.532896 ellis_django_views-0.232/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.232/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      732 2024-05-28 03:31:12.000000 ellis_django_views-0.232/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.232/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17640 2024-05-28 01:24:34.000000 ellis_django_views-0.232/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.232/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.232/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.535945 ellis_django_views-0.232/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.232/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.232/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.232/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.232/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.232/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.232/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6010 2024-05-22 00:22:52.000000 ellis_django_views-0.232/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 03:31:43.527974 ellis_django_views-0.232/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 03:31:43.000000 ellis_django_views-0.232/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-28 03:31:43.000000 ellis_django_views-0.232/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-28 03:31:43.000000 ellis_django_views-0.232/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-28 03:31:43.000000 ellis_django_views-0.232/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-28 03:31:43.000000 ellis_django_views-0.232/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-28 03:31:43.537018 ellis_django_views-0.232/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-28 03:31:29.000000 ellis_django_views-0.232/setup.py
```

### Comparing `ellis_django_views-0.231/LICENSE` & `ellis_django_views-0.232/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/PKG-INFO` & `ellis_django_views-0.232/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.231
+Version: 0.232
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.231/README.md` & `ellis_django_views-0.232/README.md`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.232/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/tests/models.py` & `ellis_django_views-0.232/ellis_django_views/tests/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models
 from ellis_django_views.utils import url_paths
 
 # Create your models here.
 
 def image_directory(self, image_name):
-    return f'{url_paths.IMAGES}{self.id}/{image_name}'
+    return f'testingEDV/{url_paths.IMAGES}{self.id}/{image_name}'
 
 class TestImageModel(models.Model):
     image = models.ImageField(upload_to=image_directory)
     datetime = models.DateTimeField(auto_now_add=True)
 
     def save(self, *args, **kwargs):
         if self.id is None:
```

### Comparing `ellis_django_views-0.231/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.232/ellis_django_views/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/tests/urls.py` & `ellis_django_views-0.232/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/tests/views.py` & `ellis_django_views-0.232/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.232/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/views_abstract.py` & `ellis_django_views-0.232/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views/views_implementation.py` & `ellis_django_views-0.232/ellis_django_views/views_implementation.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.232/ellis_django_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.231
+Version: 0.232
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.231/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.232/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.231/setup.py` & `ellis_django_views-0.232/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.231',
+    version='0.232',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description=open('README.md').read(),
```

