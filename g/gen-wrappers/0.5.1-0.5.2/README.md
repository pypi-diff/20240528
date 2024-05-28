# Comparing `tmp/gen_wrappers-0.5.1.tar.gz` & `tmp/gen_wrappers-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.5.1.tar", last modified: Wed May 22 21:12:50 2024, max compression
+gzip compressed data, was "gen_wrappers-0.5.2.tar", last modified: Tue May 28 16:17:54 2024, max compression
```

## Comparing `gen_wrappers-0.5.1.tar` & `gen_wrappers-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.486911 gen_wrappers-0.5.1/
--rw-rw-rw-   0        0        0      847 2024-05-22 21:12:50.485911 gen_wrappers-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.449200 gen_wrappers-0.5.1/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.5.1/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.453744 gen_wrappers-0.5.1/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.5.1/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.5.1/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.5.1/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.5.1/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.458357 gen_wrappers-0.5.1/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.5.1/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.5.1/creator/base/base_app.py
--rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.5.1/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.5.1/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.5.1/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.462359 gen_wrappers-0.5.1/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.5.1/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.5.1/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.5.1/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.5.1/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.467871 gen_wrappers-0.5.1/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.5.1/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     7207 2024-05-22 21:04:16.000000 gen_wrappers-0.5.1/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     6160 2024-05-22 21:12:40.000000 gen_wrappers-0.5.1/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.5.1/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.469272 gen_wrappers-0.5.1/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.5.1/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.5.1/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:12:50.483792 gen_wrappers-0.5.1/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-22 21:12:50.000000 gen_wrappers-0.5.1/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-22 21:12:50.000000 gen_wrappers-0.5.1/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 21:12:50.000000 gen_wrappers-0.5.1/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-22 21:12:50.000000 gen_wrappers-0.5.1/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 21:12:50.000000 gen_wrappers-0.5.1/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 21:12:50.487415 gen_wrappers-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-22 21:12:46.000000 gen_wrappers-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.925667 gen_wrappers-0.5.2/
+-rw-rw-rw-   0        0        0      847 2024-05-28 16:17:54.920814 gen_wrappers-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.525208 gen_wrappers-0.5.2/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.5.2/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.598340 gen_wrappers-0.5.2/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.5.2/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.5.2/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.5.2/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.5.2/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.682856 gen_wrappers-0.5.2/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.5.2/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.5.2/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.5.2/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.5.2/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.5.2/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.730364 gen_wrappers-0.5.2/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.5.2/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0    11720 2024-05-28 16:17:46.000000 gen_wrappers-0.5.2/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.5.2/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.5.2/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.815775 gen_wrappers-0.5.2/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.5.2/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     7207 2024-05-22 21:04:16.000000 gen_wrappers-0.5.2/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     6160 2024-05-22 21:12:40.000000 gen_wrappers-0.5.2/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.5.2/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.844931 gen_wrappers-0.5.2/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.5.2/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.5.2/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:17:54.917800 gen_wrappers-0.5.2/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-28 16:17:54.000000 gen_wrappers-0.5.2/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-28 16:17:54.000000 gen_wrappers-0.5.2/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 16:17:54.000000 gen_wrappers-0.5.2/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-28 16:17:54.000000 gen_wrappers-0.5.2/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-28 16:17:54.000000 gen_wrappers-0.5.2/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 16:17:54.925667 gen_wrappers-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-28 16:17:46.000000 gen_wrappers-0.5.2/setup.py
```

### Comparing `gen_wrappers-0.5.1/PKG-INFO` & `gen_wrappers-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.5.1/creator/auto/creator_auto.py` & `gen_wrappers-0.5.2/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/auto/request_auto.py` & `gen_wrappers-0.5.2/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/auto/response_auto.py` & `gen_wrappers-0.5.2/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/base/base_app.py` & `gen_wrappers-0.5.2/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/base/base_request.py` & `gen_wrappers-0.5.2/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/base/base_response.py` & `gen_wrappers-0.5.2/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.5.2/creator/cmfy/creator_cmfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,18 +132,19 @@
             if 'images' in node_output:
                 logger.debug(f"Node output: {node_output}")
                 for image in node_output['images']:
                     logger.debug(f"Getting image: {image['filename']}")
                     print(f"Getting image: {image['filename']}")
                     image_data = await self._get_image(image['filename'], image['subfolder'], image['type'])
                     images_output.append(image_data)
-                print(f"We are returning {len(images_output)} images")
-                response_data = ResponseData(data=images_output, data_type=ResponseDataType.IMAGE,
-                                             total_count=len(images_output))
-                return ResponseCmfy.success(data=response_data)
+        if len(images_output) > 0:
+            print(f"We are returning {len(images_output)} images")
+            response_data = ResponseData(data=images_output, data_type=ResponseDataType.IMAGE,
+                                         total_count=len(images_output))
+            return ResponseCmfy.success(data=response_data)
         response = ResponseCmfy.running(job_id)
         return response
 
     async def get_models(self) -> List[Any]:
         url = f"http://localhost:{os.environ.get('PORT_CMFY', 8889)}/object_info"
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
```

### Comparing `gen_wrappers-0.5.1/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.5.2/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.5.2/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.5.2/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.5.2/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/creator/util/helper.py` & `gen_wrappers-0.5.2/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.5.2/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.5.1/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.5.2/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.5.1/setup.py` & `gen_wrappers-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.5.1',
+    version='0.5.2',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

