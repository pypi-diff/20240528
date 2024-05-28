# Comparing `tmp/onetomultipleimage-1.0.4.tar.gz` & `tmp/onetomultipleimage-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetomultipleimage-1.0.4.tar", last modified: Mon May 13 19:31:18 2024, max compression
+gzip compressed data, was "onetomultipleimage-1.0.5.tar", last modified: Tue May 28 03:08:23 2024, max compression
```

## Comparing `onetomultipleimage-1.0.4.tar` & `onetomultipleimage-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:31:18.475150 onetomultipleimage-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 19:31:18.475150 onetomultipleimage-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:31:18.471150 onetomultipleimage-1.0.4/onetomultipleimage/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:31:18.475150 onetomultipleimage-1.0.4/onetomultipleimage/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/onetomultipleimage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:31:18.475150 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 19:31:18.000000 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 19:31:18.000000 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:31:18.000000 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 19:31:18.000000 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 19:31:18.000000 onetomultipleimage-1.0.4/onetomultipleimage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:31:18.475150 onetomultipleimage-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-13 19:31:10.000000 onetomultipleimage-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:08:23.341425 onetomultipleimage-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-28 03:08:23.341425 onetomultipleimage-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:08:23.337425 onetomultipleimage-1.0.5/onetomultipleimage/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:08:23.341425 onetomultipleimage-1.0.5/onetomultipleimage/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/onetomultipleimage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:08:23.341425 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-28 03:08:23.000000 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 03:08:23.000000 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:08:23.000000 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 03:08:23.000000 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 03:08:23.000000 onetomultipleimage-1.0.5/onetomultipleimage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:08:23.341425 onetomultipleimage-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-28 03:08:10.000000 onetomultipleimage-1.0.5/setup.py
```

### Comparing `onetomultipleimage-1.0.4/LICENSE` & `onetomultipleimage-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onetomultipleimage-1.0.4/PKG-INFO` & `onetomultipleimage-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetomultipleimage
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert one image to several sizes in django REST and django models
 Home-page: https://github.com/ahmadekhalili/onetomultipleimage
 Author: Ahmad Khalili
 Author-email: ahmadkhalili2020@gmail.com
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onetomultipleimage-1.0.4/README.md` & `onetomultipleimage-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `onetomultipleimage-1.0.4/onetomultipleimage/fields.py` & `onetomultipleimage-1.0.5/onetomultipleimage/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         return value
 
 
 class OneToMultipleImage(serializers.Serializer):
     def __init__(self, sizes=None, upload_to=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not self.instance:      # in writing, sizes and upload_to required
-            if not sizes or not upload_to:
+            if not sizes and not upload_to:
                 raise ValueError("both of 'sizes' and 'upload_to' arguments must be provided")
             self.sizes = sizes
             self.upload_to = upload_to
 
     def to_representation(self, value):
         result = {}
         for image_icon in value:
             size = image_icon.size
-            result[size] = {'image': image_icon.url, 'alt': image_icon.alt}
+            result[size] = {'image': image_icon.url, 'alt': getattr(image_icon, 'alt', '')}
         return result
 
     def to_internal_value(self, data):
         obj = ImageCreationSizes(data=data, sizes=self.sizes)
         instances = obj.upload(upload_to=self.upload_to)
         return instances
```

### Comparing `onetomultipleimage-1.0.4/onetomultipleimage/methods.py` & `onetomultipleimage-1.0.5/onetomultipleimage/methods.py`

 * *Files identical despite different names*

### Comparing `onetomultipleimage-1.0.4/onetomultipleimage/migrations/0001_initial.py` & `onetomultipleimage-1.0.5/onetomultipleimage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `onetomultipleimage-1.0.4/onetomultipleimage/models.py` & `onetomultipleimage-1.0.5/onetomultipleimage/models.py`

 * *Files identical despite different names*

### Comparing `onetomultipleimage-1.0.4/onetomultipleimage.egg-info/PKG-INFO` & `onetomultipleimage-1.0.5/onetomultipleimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetomultipleimage
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert one image to several sizes in django REST and django models
 Home-page: https://github.com/ahmadekhalili/onetomultipleimage
 Author: Ahmad Khalili
 Author-email: ahmadkhalili2020@gmail.com
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onetomultipleimage-1.0.4/setup.py` & `onetomultipleimage-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='onetomultipleimage',
-    version='1.0.4',
+    version='1.0.5',
     packages=['onetomultipleimage'],
     install_requires=["django", "djangorestframework", "pillow"],
     extras_require={
         'jalali': ['jdatetime']
     },
     author='Ahmad Khalili',
     author_email='ahmadkhalili2020@gmail.com',
```

