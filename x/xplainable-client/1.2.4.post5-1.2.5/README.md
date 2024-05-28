# Comparing `tmp/xplainable_client-1.2.4.post5.tar.gz` & `tmp/xplainable_client-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.4.post5.tar", last modified: Sun May 19 00:48:44 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.5.tar", last modified: Tue May 28 05:10:22 2024, max compression
```

## Comparing `xplainable_client-1.2.4.post5.tar` & `xplainable_client-1.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.339080 xplainable_client-1.2.4.post5/
--rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.4.post5/.gitignore
--rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post5/LICENSE
--rw-rw-rw-   0        0        0    45260 2024-05-19 00:48:44.338081 xplainable_client-1.2.4.post5/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post5/README.md
--rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.4.post5/_build.py
--rw-rw-rw-   0        0        0       29 2024-05-19 00:48:35.000000 xplainable_client-1.2.4.post5/_version.py
--rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post5/config.py
--rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/docker-compose.yaml
--rw-rw-rw-   0        0        0      783 2024-05-19 00:48:35.000000 xplainable_client-1.2.4.post5/pyproject.toml
--rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.4.post5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 00:48:44.339080 xplainable_client-1.2.4.post5/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-05-19 00:48:35.000000 xplainable_client-1.2.4.post5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.296580 xplainable_client-1.2.4.post5/tests/
--rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/tests/nanoid.sql
--rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/tests/prod-db.sql
--rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/tests/test_model.py
--rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/tests/test_test.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.299581 xplainable_client-1.2.4.post5/thebadboycorner/
--rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.4.post5/thebadboycorner/clf_model_test_jason.py
--rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post5/thebadboycorner/test.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.302581 xplainable_client-1.2.4.post5/xplainable_client/
--rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.4.post5/xplainable_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.325581 xplainable_client-1.2.4.post5/xplainable_client/client/
--rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post5/xplainable_client/client/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_client_cog_base.py
--rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_collections.py
--rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_datasets.py
--rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_deployments.py
--rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_gpt.py
--rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_inference.py
--rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_misc.py
--rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_models.py
--rw-rw-rw-   0        0        0     9609 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_preprocessing.py
--rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.4.post5/xplainable_client/client/_session.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.334580 xplainable_client-1.2.4.post5/xplainable_client/client/utils/
--rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/encoders.py
--rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/helpers.py
--rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/metrics.py
--rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/model_parsers.py
--rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post5/xplainable_client/client/utils/scanner.py
--rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post5/xplainable_client/pytest.ini
-drwxrwxrwx   0        0        0        0 2024-05-19 00:48:44.336582 xplainable_client-1.2.4.post5/xplainable_client.egg-info/
--rw-rw-rw-   0        0        0    45260 2024-05-19 00:48:43.000000 xplainable_client-1.2.4.post5/xplainable_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-05-19 00:48:44.000000 xplainable_client-1.2.4.post5/xplainable_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 00:48:43.000000 xplainable_client-1.2.4.post5/xplainable_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-19 00:48:43.000000 xplainable_client-1.2.4.post5/xplainable_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-05-19 00:48:43.000000 xplainable_client-1.2.4.post5/xplainable_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.690183 xplainable_client-1.2.5/
+-rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.5/.gitignore
+-rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    45254 2024-05-28 05:10:22.689186 xplainable_client-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/README.md
+-rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.5/_build.py
+-rw-rw-rw-   0        0        0       23 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/_version.py
+-rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/config.py
+-rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/docker-compose.yaml
+-rw-rw-rw-   0        0        0      777 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:10:22.690183 xplainable_client-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      824 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.661683 xplainable_client-1.2.5/tests/
+-rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/nanoid.sql
+-rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/prod-db.sql
+-rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/test_model.py
+-rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/test_test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.663683 xplainable_client-1.2.5/thebadboycorner/
+-rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.5/thebadboycorner/clf_model_test_jason.py
+-rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.5/thebadboycorner/test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.665184 xplainable_client-1.2.5/xplainable_client/
+-rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.5/xplainable_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.680683 xplainable_client-1.2.5/xplainable_client/client/
+-rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.5/xplainable_client/client/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.5/xplainable_client/client/_client_cog_base.py
+-rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.5/xplainable_client/client/_collections.py
+-rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.5/xplainable_client/client/_datasets.py
+-rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.5/xplainable_client/client/_deployments.py
+-rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/xplainable_client/client/_gpt.py
+-rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.5/xplainable_client/client/_inference.py
+-rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.5/xplainable_client/client/_misc.py
+-rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.5/xplainable_client/client/_models.py
+-rw-rw-rw-   0        0        0    10934 2024-05-28 01:15:50.000000 xplainable_client-1.2.5/xplainable_client/client/_preprocessing.py
+-rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.5/xplainable_client/client/_session.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.686685 xplainable_client-1.2.5/xplainable_client/client/utils/
+-rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.5/xplainable_client/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/xplainable_client/client/utils/encoders.py
+-rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.5/xplainable_client/client/utils/helpers.py
+-rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.5/xplainable_client/client/utils/metrics.py
+-rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/xplainable_client/client/utils/model_parsers.py
+-rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.5/xplainable_client/client/utils/scanner.py
+-rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/xplainable_client/pytest.ini
+drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.688185 xplainable_client-1.2.5/xplainable_client.egg-info/
+-rw-rw-rw-   0        0        0    45254 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.4.post5/.gitignore` & `xplainable_client-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/LICENSE` & `xplainable_client-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/PKG-INFO` & `xplainable_client-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4.post5
+Version: 1.2.5
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.4.post5/README.md` & `xplainable_client-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/_build.py` & `xplainable_client-1.2.5/_build.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/pyproject.toml` & `xplainable_client-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.4.post5"
+version = "1.2.5"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `xplainable_client-1.2.4.post5/setup.py` & `xplainable_client-1.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setuptools.setup(
     name="xplainable-client",
-    version="1.2.4.post5",
+    version="1.2.5",
     author="xplainable pty ltd",
     author_email="contact@xplainable.io",
     packages=["xplainable_client"],
     description="The client for persisting and deploying models to Xplainable cloud.",
     long_description=description,
     long_description_content_type="text/markdown",
     license=license,
```

### Comparing `xplainable_client-1.2.4.post5/tests/nanoid.sql` & `xplainable_client-1.2.5/tests/nanoid.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/tests/prod-db.sql` & `xplainable_client-1.2.5/tests/prod-db.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/thebadboycorner/clf_model_test_jason.py` & `xplainable_client-1.2.5/thebadboycorner/clf_model_test_jason.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/__init__.py` & `xplainable_client-1.2.5/xplainable_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_collections.py` & `xplainable_client-1.2.5/xplainable_client/client/_collections.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_datasets.py` & `xplainable_client-1.2.5/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_deployments.py` & `xplainable_client-1.2.5/xplainable_client/client/_deployments.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_gpt.py` & `xplainable_client-1.2.5/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_inference.py` & `xplainable_client-1.2.5/xplainable_client/client/_inference.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_misc.py` & `xplainable_client-1.2.5/xplainable_client/client/_misc.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_models.py` & `xplainable_client-1.2.5/xplainable_client/client/_models.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_preprocessing.py` & `xplainable_client-1.2.5/xplainable_client/client/_preprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ._client_cog_base import *
 import pandas as pd
 import json
 from xplainable_client.client.utils import get_df_delta
 from xplainable.preprocessing.pipeline import XPipeline
+from xplainable.preprocessing import transformers as xtf
 
 
 class Preprocessing(Client_Cog):
 
     def create_preprocessor_id(
         self, preprocessor_name: str, preprocessor_description: str) -> str:
         """ Creates a new preprocessor and returns the preprocessor id.
@@ -24,83 +25,108 @@
             url=f'{self.session.hostname}/v1/{self.session._ext}/create-preprocessor',
             json=payoad
         )
 
         preprocessor_id = self.session.get_response_content(response)
 
         return preprocessor_id
-    
 
-    def create_preprocessor_version(
-        self, preprocessor_id: str, pipeline: list, df: pd.DataFrame = None
-        ) -> str:
-        """ Creates a new preprocessor version and returns the version id.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            pipeline (xplainable.preprocessing.pipeline.Pipeline): pipeline
-        Returns:
-            int: The preprocessor version id
-        """
+    def prepare_pipeline(self, pipeline, df):
         # Structure the stages and deltas
         stages = []
         deltas = []
         if df is not None:
             before = df.copy()
-            deltas.append({"start": json.loads(before.head(10).to_json(
-                orient='records'))})
+            deltas.append({"start": json.loads(before.head(10).to_json(orient='records'))})
             delta_gen = pipeline.transform_generator(before)
         for stage in pipeline.stages:
             step = {
                 'feature': stage['feature'],
                 'name': stage['name'],
                 'params': stage['transformer'].__dict__
             }
+            if "code_def" in stage.keys():
+                step["code_def"] = stage["code_def"]
             stages.append(step)
             if df is not None:
                 after = delta_gen.__next__()
                 delta = get_df_delta(before.copy(), after.copy())
                 deltas.append(delta)
                 before = after.copy()
         # Get current versions
         versions = {
-                "xplainable_version": self.xplainable_version,
-                "python_version": self.python_version
-            }
+            "xplainable_version": self.xplainable_version,
+            "python_version": self.python_version
+        }
         # Create payload
         payload = {
             "stages": stages,
             "deltas": deltas,
             "versions": versions
-            }
+        }
+        return payload
+
+    def create_preprocessor_version(
+        self, preprocessor_id: str, pipeline: XPipeline, df: pd.DataFrame = None
+    ) -> str:
+        """ Creates a new preprocessor version and returns the version id.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            pipeline (xplainable.preprocessing.pipeline.Pipeline): pipeline
+        Returns:
+            int: The preprocessor version id
+        """
+        payload = self.prepare_pipeline(pipeline, df)
 
         # Create a new version and fetch id
         url = (
             f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/'
             f'{preprocessor_id}/add-version'
             )
 
         response = self.session._session.post(url=url, json=payload)
         version_id = self.session.get_response_content(response)
         return version_id
 
+    def update_preprocessor_version(
+        self, preprocessor_id: str, version_id: str, pipeline: XPipeline, df: pd.DataFrame = None
+    ) -> str:
+        """ Updates version.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            version_id (int): The preprocessor version id
+            pipeline (xplainable.preprocessing.pipeline.Pipeline): pipeline
+        Returns:
+            int: The preprocessor version id
+        """
+        payload = self.prepare_pipeline(pipeline, df)
+
+        # Create a new version and fetch id
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/'
+            f'{preprocessor_id}/update-version/{version_id}'
+            )
+
+        response = self.session._session.post(url=url, json=payload)
+        version_id = self.session.get_response_content(response)
+        return version_id
+
     def list_preprocessors(self) -> list:
         """ Lists all preprocessors of the active user's team.
         Returns:
             dict: Dictionary of preprocessors.
         """
         response = self.session._session.get(
             url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors'
             )
         data = self.session.get_response_content(response)
         [i.pop('user') for i in data]
         return data
-    
-    # get_preprocessor
-    
 
+    # get_preprocessor
 
     def list_preprocessor_versions(self, preprocessor_id: int) -> list:
         """ Lists all versions of a preprocessor.
         Args:
             preprocessor_id (int): The preprocessor id
         Returns:
             dict: Dictionary of preprocessor versions.
@@ -123,15 +149,19 @@
             response_only (bool, optional): Returns the preprocessor metadata.
         Returns:
             xplainable.preprocessing.pipeline.Pipeline: The loaded pipeline
         """
         def build_transformer(stage):
             """Build transformer from metadata"""
             if not hasattr(xtf, stage["name"]):
-                raise ValueError(f"{stage['name']} does not exist in the transformers module")
+                if "code_def" in dict(stage).keys():
+                    exec(stage["code_def"])
+                    return globals()[stage["name"]](**stage['params'])
+                else:
+                    raise ValueError(f"{stage['name']} does not exist in the transformers module")
             # Get transformer function
             func = getattr(xtf, stage["name"])
             return func(**stage['params'])
 
         try:
             preprocessor_response = self.session._session.get(
                 url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
@@ -189,15 +219,15 @@
 
     def restore_preprocessor_version(self, preprocessor_id: str, version_id: str):
         """ Restores a preprocessor version.
         Args:
             preprocessor_id (int): The preprocessor id
             version_id (int): The version id
         Return:
-            json: A json response. 
+            json: A json response.
         """
         response = self.session._session.put(
             url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/restore'
             )
         return response
 
     def delete_preprocessor(self, preprocessor_id: str):
@@ -230,21 +260,21 @@
             preprocessor_id (int): The preprocessor id
             preprocessor_version_id (int): The preprocessor version id
             model_id (int): The model id
             model_version_id (int): The model version id
         Return:
             dict: A json response of signatures_match, pipeline_columns, model_columns.
         """
-        
+
         payload = {
             'model_id': model_id,
             'version_id': model_version_id
         }
         response = self.session._session.post(
             url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{preprocessor_version_id}/check-signature',
             json=payload
         )
         output = self.session.get_response_content(response)
         return output
 
 
-    
+
```

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/_session.py` & `xplainable_client-1.2.5/xplainable_client/client/_session.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/utils/encoders.py` & `xplainable_client-1.2.5/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/utils/helpers.py` & `xplainable_client-1.2.5/xplainable_client/client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/utils/metrics.py` & `xplainable_client-1.2.5/xplainable_client/client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/utils/model_parsers.py` & `xplainable_client-1.2.5/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client/client/utils/scanner.py` & `xplainable_client-1.2.5/xplainable_client/client/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post5/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.5/xplainable_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4.post5
+Version: 1.2.5
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.4.post5/xplainable_client.egg-info/SOURCES.txt` & `xplainable_client-1.2.5/xplainable_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*
