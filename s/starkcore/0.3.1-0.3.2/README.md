# Comparing `tmp/starkcore-0.3.1.tar.gz` & `tmp/starkcore-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkcore-0.3.1.tar", last modified: Thu May 23 17:32:26 2024, max compression
+gzip compressed data, was "starkcore-0.3.2.tar", last modified: Mon May 27 22:24:48 2024, max compression
```

## Comparing `starkcore-0.3.1.tar` & `starkcore-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.605886 starkcore-0.3.1/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.3.1/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.3.1/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-23 17:32:26.605676 starkcore-0.3.1/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.3.1/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-05-23 17:32:26.606121 starkcore-0.3.1/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.3.1/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.565849 starkcore-0.3.1/starkcore/
--rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-05-23 17:31:54.000000 starkcore-0.3.1/starkcore/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.3.1/starkcore/environment.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/error.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/key.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.573201 starkcore-0.3.1/starkcore/user/
--rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/user/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__organization.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__project.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/user/__publicuser.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/user/__user.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.604874 starkcore-0.3.1/starkcore/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/api.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/cache.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/case.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/utils/checks.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/compatibility.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/enum.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.3.1/starkcore/utils/host.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.3.1/starkcore/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2911 2024-05-23 17:31:07.000000 starkcore-0.3.1/starkcore/utils/request.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/resource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9228 2024-05-23 17:31:07.000000 starkcore-0.3.1/starkcore/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.3.1/starkcore/utils/subresource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.3.1/starkcore/utils/url.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-23 17:32:26.567179 starkcore-0.3.1/starkcore.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-05-23 17:32:26.000000 starkcore-0.3.1/starkcore.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-27 22:24:48.479442 starkcore-0.3.2/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.3.2/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.3.2/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-27 22:24:48.479243 starkcore-0.3.2/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.3.2/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-05-27 22:24:48.479512 starkcore-0.3.2/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.3.2/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-27 22:24:48.441904 starkcore-0.3.2/starkcore/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-05-27 22:24:24.000000 starkcore-0.3.2/starkcore/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.3.2/starkcore/environment.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/error.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/key.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-27 22:24:48.448635 starkcore-0.3.2/starkcore/user/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.3.2/starkcore/user/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/user/__organization.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/user/__project.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.3.2/starkcore/user/__publicuser.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/user/__user.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-27 22:24:48.478834 starkcore-0.3.2/starkcore/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/api.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/cache.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/case.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.3.2/starkcore/utils/checks.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/compatibility.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/enum.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.3.2/starkcore/utils/host.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2511 2024-05-27 22:23:51.000000 starkcore-0.3.2/starkcore/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2911 2024-05-23 17:31:07.000000 starkcore-0.3.2/starkcore/utils/request.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/resource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9228 2024-05-23 17:31:07.000000 starkcore-0.3.2/starkcore/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.3.2/starkcore/utils/subresource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.3.2/starkcore/utils/url.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-27 22:24:48.443704 starkcore-0.3.2/starkcore.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-27 22:24:48.000000 starkcore-0.3.2/starkcore.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-05-27 22:24:48.000000 starkcore-0.3.2/starkcore.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-05-27 22:24:48.000000 starkcore-0.3.2/starkcore.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-05-27 22:24:48.000000 starkcore-0.3.2/starkcore.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-05-27 22:24:48.000000 starkcore-0.3.2/starkcore.egg-info/top_level.txt
```

### Comparing `starkcore-0.3.1/LICENSE.txt` & `starkcore-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/PKG-INFO` & `starkcore-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.3.1
+Version: 0.3.2
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `starkcore-0.3.1/setup.py` & `starkcore-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/error.py` & `starkcore-0.3.2/starkcore/error.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/key.py` & `starkcore-0.3.2/starkcore/key.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/user/__organization.py` & `starkcore-0.3.2/starkcore/user/__organization.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/user/__project.py` & `starkcore-0.3.2/starkcore/user/__project.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/api.py` & `starkcore-0.3.2/starkcore/utils/api.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/checks.py` & `starkcore-0.3.2/starkcore/utils/checks.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/parse.py` & `starkcore-0.3.2/starkcore/utils/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,12 +69,12 @@
         sdk_version=sdk_version,
         host=host,
         api_version=api_version,
         path="/public-key",
         user=user,
         language=language,
         timeout=timeout,
-        limit=1,
+        query={"limit": 1}
     )["publicKeys"][0]["content"]
     public_key = PublicKey.fromPem(pem)
     cache["stark-public-key"] = public_key
     return public_key
```

### Comparing `starkcore-0.3.1/starkcore/utils/request.py` & `starkcore-0.3.2/starkcore/utils/request.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/rest.py` & `starkcore-0.3.2/starkcore/utils/rest.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/subresource.py` & `starkcore-0.3.2/starkcore/utils/subresource.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore/utils/url.py` & `starkcore-0.3.2/starkcore/utils/url.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.3.1/starkcore.egg-info/PKG-INFO` & `starkcore-0.3.2/starkcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.3.1
+Version: 0.3.2
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `starkcore-0.3.1/starkcore.egg-info/SOURCES.txt` & `starkcore-0.3.2/starkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

