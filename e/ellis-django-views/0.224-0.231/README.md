# Comparing `tmp/ellis_django_views-0.224.tar.gz` & `tmp/ellis_django_views-0.231.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellis_django_views-0.224.tar", last modified: Tue May 21 12:30:26 2024, max compression
+gzip compressed data, was "ellis_django_views-0.231.tar", last modified: Tue May 28 01:27:47 2024, max compression
```

## Comparing `ellis_django_views-0.224.tar` & `ellis_django_views-0.231.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.790841 ellis_django_views-0.224/
--rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.224/LICENSE
--rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.224/MANIFEST.in
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-21 12:30:26.790474 ellis_django_views-0.224/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)     3579 2024-05-21 12:30:17.000000 ellis_django_views-0.224/README.md
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.772335 ellis_django_views-0.224/ellis_django_views/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.224/ellis_django_views/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.224/ellis_django_views/apps.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.782706 ellis_django_views-0.224/ellis_django_views/migrations/
--rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.224/ellis_django_views/migrations/0001_initial.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.224/ellis_django_views/migrations/__init__.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.786813 ellis_django_views-0.224/ellis_django_views/tests/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.224/ellis_django_views/tests/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.224/ellis_django_views/tests/models.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.224/ellis_django_views/tests/serializers.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)    17410 2024-05-21 10:28:29.000000 ellis_django_views-0.224/ellis_django_views/tests/test_views.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.224/ellis_django_views/tests/urls.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.224/ellis_django_views/tests/views.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.789831 ellis_django_views-0.224/ellis_django_views/utils/
--rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.224/ellis_django_views/utils/__init__.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.224/ellis_django_views/utils/error_messages.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.224/ellis_django_views/utils/request_params.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.224/ellis_django_views/utils/url_names.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.224/ellis_django_views/utils/url_paths.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.224/ellis_django_views/views_abstract.py
--rw-r--r--   0 carl.ellis   (501) staff       (20)     6007 2024-05-21 10:29:50.000000 ellis_django_views-0.224/ellis_django_views/views_implementation.py
-drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-21 12:30:26.781279 ellis_django_views-0.224/ellis_django_views.egg-info/
--rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-21 12:30:26.000000 ellis_django_views-0.224/ellis_django_views.egg-info/PKG-INFO
--rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-21 12:30:26.000000 ellis_django_views-0.224/ellis_django_views.egg-info/SOURCES.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-21 12:30:26.000000 ellis_django_views-0.224/ellis_django_views.egg-info/dependency_links.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-21 12:30:26.000000 ellis_django_views-0.224/ellis_django_views.egg-info/requires.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-21 12:30:26.000000 ellis_django_views-0.224/ellis_django_views.egg-info/top_level.txt
--rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-21 12:30:26.790919 ellis_django_views-0.224/setup.cfg
--rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-21 12:30:23.000000 ellis_django_views-0.224/setup.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.138745 ellis_django_views-0.231/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    35148 2024-05-21 07:03:41.000000 ellis_django_views-0.231/LICENSE
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       33 2024-05-21 11:05:27.000000 ellis_django_views-0.231/MANIFEST.in
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 01:27:47.138269 ellis_django_views-0.231/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     3579 2024-05-21 12:30:17.000000 ellis_django_views-0.231/README.md
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.127105 ellis_django_views-0.231/ellis_django_views/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      166 2024-05-21 10:30:16.000000 ellis_django_views-0.231/ellis_django_views/apps.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.130710 ellis_django_views-0.231/ellis_django_views/migrations/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      653 2024-05-21 10:17:22.000000 ellis_django_views-0.231/ellis_django_views/migrations/0001_initial.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:05.000000 ellis_django_views-0.231/ellis_django_views/migrations/__init__.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.134523 ellis_django_views-0.231/ellis_django_views/tests/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 09:03:01.000000 ellis_django_views-0.231/ellis_django_views/tests/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      721 2024-05-21 10:47:11.000000 ellis_django_views-0.231/ellis_django_views/tests/models.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      245 2024-05-21 10:27:58.000000 ellis_django_views-0.231/ellis_django_views/tests/serializers.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)    17640 2024-05-28 01:24:34.000000 ellis_django_views-0.231/ellis_django_views/tests/test_views.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      712 2024-05-21 10:01:17.000000 ellis_django_views-0.231/ellis_django_views/tests/urls.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1016 2024-05-21 10:29:40.000000 ellis_django_views-0.231/ellis_django_views/tests/views.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.137503 ellis_django_views-0.231/ellis_django_views/utils/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        0 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/__init__.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      264 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/error_messages.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      623 2024-05-21 10:01:41.000000 ellis_django_views-0.231/ellis_django_views/utils/request_params.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      121 2024-05-21 08:51:03.000000 ellis_django_views-0.231/ellis_django_views/utils/url_names.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      206 2024-05-21 10:26:54.000000 ellis_django_views-0.231/ellis_django_views/utils/url_paths.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     2437 2024-05-21 10:01:54.000000 ellis_django_views-0.231/ellis_django_views/views_abstract.py
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     6010 2024-05-22 00:22:52.000000 ellis_django_views-0.231/ellis_django_views/views_implementation.py
+drwxr-xr-x   0 carl.ellis   (501) staff       (20)        0 2024-05-28 01:27:47.129679 ellis_django_views-0.231/ellis_django_views.egg-info/
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     4518 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/PKG-INFO
+-rw-r--r--   0 carl.ellis   (501) staff       (20)      890 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/SOURCES.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)        1 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/dependency_links.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       34 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/requires.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       19 2024-05-28 01:27:47.000000 ellis_django_views-0.231/ellis_django_views.egg-info/top_level.txt
+-rw-r--r--   0 carl.ellis   (501) staff       (20)       38 2024-05-28 01:27:47.138839 ellis_django_views-0.231/setup.cfg
+-rw-r--r--   0 carl.ellis   (501) staff       (20)     1407 2024-05-28 01:27:12.000000 ellis_django_views-0.231/setup.py
```

### Comparing `ellis_django_views-0.224/LICENSE` & `ellis_django_views-0.231/LICENSE`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/PKG-INFO` & `ellis_django_views-0.231/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis_django_views
-Version: 0.224
+Version: 0.231
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.224/README.md` & `ellis_django_views-0.231/README.md`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/migrations/0001_initial.py` & `ellis_django_views-0.231/ellis_django_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/tests/models.py` & `ellis_django_views-0.231/ellis_django_views/tests/models.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/tests/test_views.py` & `ellis_django_views-0.231/ellis_django_views/tests/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from django.conf import settings
 from rest_framework import status
 from django.test import TestCase, Client
 from django.core.files.uploadedfile import SimpleUploadedFile
 from ellis_django_views.utils import url_paths, request_params, error_messages
 from ellis_django_views.tests.models import TestImageModel
 from PIL import Image as PilImage
 import tempfile
-import os, shutil
+import shutil
 
 class ViewsImplTests(TestCase):
     def setUp(self):
         self.client = Client()
         self.urls = url_paths
         self.test_image = 'test_image.png'
         self.test_updated_image = 'test_updated_image.png'
@@ -67,15 +68,15 @@
             path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_UPDATE_missing_auth_token(self):
         # Test case to check handling of missing authorization token in PUT request
         # Simulates sending a PUT request without an authorization token
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
@@ -95,15 +96,15 @@
         response = self.client.post(
             path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_DELETE_missing_auth_token(self):
         # Test case to check handling of missing authorization token in DELETE request
         # Simulates sending a DELETE request without an authorization token
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing auth token
         uploaded_file = self.upload_image(self.test_image)
@@ -123,15 +124,15 @@
         self.assertEqual(
             response.json()[error_messages.ERROR],
             f'{error_messages.MISSING_HEADER_PARAMETER}{request_params.AUTH_TOKEN}')
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 1)
         image = TestImageModel.objects.get(pk=pk)
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_POST_missing_image(self):
         # Test case to check handling of missing image file in POST request
         # Simulates sending a POST request without an image file
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing image file
         headers = {request_params.AUTH_TOKEN :
@@ -167,15 +168,15 @@
         self.assertEqual(
             response.status_code, status.HTTP_400_BAD_REQUEST)
         self.assertEqual(
             response.json()[error_messages.ERROR],
             {request_params.IMAGE:[error_messages.FILE_NOT_SUBMITTED]})
         image = TestImageModel.objects.get(pk=pk)
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_REQUEST_missing_pk(self):
         # Test case to check handling of missing primary key in GET request
         # Simulates sending a GET request without a primary key
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
@@ -191,15 +192,15 @@
         response = self.client.post(
             path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_UPDATE_missing_pk(self):
         # Test case to check handling of missing primary key in PUT request
         # Simulates sending a PUT request without a primary key
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
@@ -218,39 +219,41 @@
             path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         image = TestImageModel.objects.get(pk=pk)
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_DELETE_missing_pk(self):
         # Test case to check handling of missing primary key in DELETE request
         # Simulates sending a DELETE request without a primary key
         # Asserts that the response returns a 400 Bad Request status
         # and an appropriate error message about the missing primary key
         uploaded_file = self.upload_image(self.test_image)
         request = {request_params.IMAGE : uploaded_file}
         headers = {request_params.AUTH_TOKEN :
                    request_params.getBearer(request_params.AUTH_TOKEN)}
         response = self.client.post(
             path=f'/{self.urls.TEST_POST}', data=request, **headers)
+        pk = response.json()[request_params.ID]
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         request = {}
         response = self.client.post(
             path=f'/{self.urls.TEST_DELETE}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_400_BAD_REQUEST)
         self.assertEqual(response.json()[error_messages.ERROR],
                          f'{error_messages.MISSING_PARAMETER}pk')
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 1)
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        images.first().delete()
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_CREATE_correct(self):
         # Test case to check correct creation of an image
         # Simulates sending a POST request with correct parameters
         # Asserts that the response returns a 200 OK status
         # and the image is created successfully in the database
         uploaded_file = self.upload_image(self.test_image)
@@ -262,15 +265,15 @@
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         pk = response.json()[request_params.ID]
         image = TestImageModel.objects.get(pk=pk)
         self.assertEqual(image.image.url,
                          response.json()[request_params.IMAGE])
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
     
     def test_image_REQUEST_correct(self):
         # Test case to check correct retrieval of an image
         # Simulates sending a GET request with correct parameters
         # Asserts that the response returns a 200 OK status
         # and the requested image is returned successfully
         uploaded_file = self.upload_image(self.test_image)
@@ -284,15 +287,15 @@
         image = TestImageModel.objects.get(pk=pk)
         request = {request_params.PK : pk}
         response = self.client.post(
             path=f'/{self.urls.TEST_GET}', data=request, **headers)
         self.assertEqual(image.image.url,
                          response.json()[request_params.IMAGE])
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
 
     def test_image_UPDATE_correct(self):
         # Test case to check correct updating of an image
         # Simulates sending a PUT request with correct parameters
         # Asserts that the response returns a 200 OK status
         # and the image is updated successfully in the database
         uploaded_file = self.upload_image(self.test_image)
@@ -312,15 +315,15 @@
             path=f'/{self.urls.TEST_PUT}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         image = TestImageModel.objects.get(pk=pk)
         self.assertEqual(image.image.name,
                          f'{url_paths.IMAGES}{pk}/{self.test_updated_image}')
         image.delete()
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
     
     def test_image_DELETE_correct(self):
         # Test case to check correct deletion of an image
         # Simulates sending a DELETE request with correct parameters
         # Asserts that the response returns a 200 OK status
         # and the image is deleted successfully from the database
         uploaded_file = self.upload_image(self.test_image)
@@ -335,8 +338,8 @@
         request = {request_params.PK : pk}
         response = self.client.post(
             path=f'/{self.urls.TEST_DELETE}', data=request, **headers)
         self.assertEqual(response.status_code,
                          status.HTTP_200_OK)
         images = TestImageModel.objects.all()
         self.assertEqual(len(images), 0)
-        shutil.rmtree(f'{os.getcwd()}/{url_paths.IMAGES}')
+        shutil.rmtree(f'{settings.MEDIA_ROOT}{url_paths.IMAGES}{pk}')
```

### Comparing `ellis_django_views-0.224/ellis_django_views/tests/urls.py` & `ellis_django_views-0.231/ellis_django_views/tests/urls.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/tests/views.py` & `ellis_django_views-0.231/ellis_django_views/tests/views.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/utils/request_params.py` & `ellis_django_views-0.231/ellis_django_views/utils/request_params.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/views_abstract.py` & `ellis_django_views-0.231/ellis_django_views/views_abstract.py`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/ellis_django_views/views_implementation.py` & `ellis_django_views-0.231/ellis_django_views/views_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def post(self, request):
         try:
             # Check if the request is authorized
             if self.is_authorised(check_authorization(
                 request=request, auth_token_key=self.auth_token_key)):
                 # Get primary key from request parameters
                 pk = request_params.get_request_param_value(
-                    request,request_params.PK)
+                    request, request_params.PK)
                 # Retrieve the object or return 404 if not found
                 object = get_object_or_404(self.model, pk=pk)
                 # Serialize the retrieved object
                 serializer = self.serializer_model(instance=object)
                 return Response(
                     serializer.data,status=status.HTTP_200_OK)
             # Return unauthorized status if authorization fails
@@ -68,15 +68,15 @@
     def post(self, request):
         try:
             # Check if the request is authorized
             if self.is_authorised(check_authorization(
                 request=request, auth_token_key=self.auth_token_key)):
                 # Get primary key from request parameters
                 pk = request_params.get_request_param_value(
-                    request,request_params.PK)
+                    request, request_params.PK)
                 # Retrieve the object or return 404 if not found
                 object = get_object_or_404(self.model, pk=pk)
                 # Deserialize request data with the existing object instance
                 serializer = self.serializer_model(
                     instance=object,data=request.data)
                 # Validate and save the serialized data
                 if serializer.is_valid():
@@ -99,15 +99,15 @@
     def post(self, request):
         try:
             # Check if the request is authorized
             if self.is_authorised(check_authorization(
                 request=request, auth_token_key=self.auth_token_key)):
                 # Get primary key from request parameters
                 pk = request_params.get_request_param_value(
-                    request,request_params.PK)
+                    request, request_params.PK)
                 # Retrieve the object or return 404 if not found
                 object = get_object_or_404(self.model, pk=pk)
                 # Delete the retrieved object
                 object.delete()
                 return Response(status=status.HTTP_200_OK)
             # Return unauthorized status if authorization fails
             return Response(status=status.HTTP_401_UNAUTHORIZED)
```

### Comparing `ellis_django_views-0.224/ellis_django_views.egg-info/PKG-INFO` & `ellis_django_views-0.231/ellis_django_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellis-django-views
-Version: 0.224
+Version: 0.231
 Summary: Generic views for Model View Serializer (MVS) pattern
 Home-page: https://carlellis.io
 Author: Carl Victor Ellis
 Author-email: carl.ellis@hotmail.com.au
 License: GNU
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `ellis_django_views-0.224/ellis_django_views.egg-info/SOURCES.txt` & `ellis_django_views-0.231/ellis_django_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ellis_django_views-0.224/setup.py` & `ellis_django_views-0.231/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     include_package_data=True,
     name='ellis_django_views',
-    version='0.224',
+    version='0.231',
     packages=find_packages(),
     description='Generic views for Model View Serializer (MVS) pattern',
     author='Carl Victor Ellis',
     author_email='carl.ellis@hotmail.com.au',
     license='GNU',
     url='https://carlellis.io',
     long_description=open('README.md').read(),
```

