# Comparing `tmp/airbyte_serverless-0.8.tar.gz` & `tmp/airbyte_serverless-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_serverless-0.8.tar", last modified: Thu Sep  7 12:01:38 2023, max compression
+gzip compressed data, was "airbyte_serverless-0.9.tar", last modified: Thu Sep  7 12:42:26 2023, max compression
```

## Comparing `airbyte_serverless-0.8.tar` & `airbyte_serverless-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-07 12:01:38.799170 airbyte_serverless-0.8/
--rw-rw-rw-   0        0        0       58 2023-09-07 08:31:37.000000 airbyte_serverless-0.8/.gitignore
--rw-rw-rw-   0        0        0     1083 2023-08-31 15:34:17.000000 airbyte_serverless-0.8/LICENSE
--rw-rw-rw-   0        0        0     8539 2023-09-07 12:01:38.798213 airbyte_serverless-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8027 2023-09-07 09:47:40.000000 airbyte_serverless-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-09-07 12:01:38.780853 airbyte_serverless-0.8/airbyte_serverless/
--rw-rw-rw-   0        0        0       31 2023-08-31 14:55:32.000000 airbyte_serverless-0.8/airbyte_serverless/__init__.py
--rw-rw-rw-   0        0        0     8339 2023-09-01 11:35:21.000000 airbyte_serverless-0.8/airbyte_serverless/airbyte_utils.py
--rw-rw-rw-   0        0        0     5121 2023-09-06 20:25:20.000000 airbyte_serverless-0.8/airbyte_serverless/destinations.py
--rw-rw-rw-   0        0        0     4615 2023-09-07 12:00:58.000000 airbyte_serverless-0.8/airbyte_serverless/sources.py
-drwxrwxrwx   0        0        0        0 2023-09-07 12:01:38.795166 airbyte_serverless-0.8/airbyte_serverless.egg-info/
--rw-rw-rw-   0        0        0     8539 2023-09-07 12:01:38.000000 airbyte_serverless-0.8/airbyte_serverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-09-07 12:01:38.000000 airbyte_serverless-0.8/airbyte_serverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-07 12:01:38.000000 airbyte_serverless-0.8/airbyte_serverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-09-07 12:01:38.000000 airbyte_serverless-0.8/airbyte_serverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-09-07 12:01:38.000000 airbyte_serverless-0.8/airbyte_serverless.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    72596 2023-09-06 19:59:31.000000 airbyte_serverless-0.8/logo_and_name.png
--rw-rw-rw-   0        0        0       42 2023-09-07 12:01:38.799170 airbyte_serverless-0.8/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-09-07 12:01:25.000000 airbyte_serverless-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-07 12:42:26.071816 airbyte_serverless-0.9/
+-rw-rw-rw-   0        0        0       58 2023-09-07 08:31:37.000000 airbyte_serverless-0.9/.gitignore
+-rw-rw-rw-   0        0        0     1083 2023-08-31 15:34:17.000000 airbyte_serverless-0.9/LICENSE
+-rw-rw-rw-   0        0        0     8539 2023-09-07 12:42:26.069815 airbyte_serverless-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8027 2023-09-07 09:47:40.000000 airbyte_serverless-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-09-07 12:42:26.053816 airbyte_serverless-0.9/airbyte_serverless/
+-rw-rw-rw-   0        0        0       31 2023-08-31 14:55:32.000000 airbyte_serverless-0.9/airbyte_serverless/__init__.py
+-rw-rw-rw-   0        0        0     8339 2023-09-01 11:35:21.000000 airbyte_serverless-0.9/airbyte_serverless/airbyte_utils.py
+-rw-rw-rw-   0        0        0     5121 2023-09-06 20:25:20.000000 airbyte_serverless-0.9/airbyte_serverless/destinations.py
+-rw-rw-rw-   0        0        0     4652 2023-09-07 12:42:05.000000 airbyte_serverless-0.9/airbyte_serverless/sources.py
+drwxrwxrwx   0        0        0        0 2023-09-07 12:42:26.067827 airbyte_serverless-0.9/airbyte_serverless.egg-info/
+-rw-rw-rw-   0        0        0     8539 2023-09-07 12:42:25.000000 airbyte_serverless-0.9/airbyte_serverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-09-07 12:42:25.000000 airbyte_serverless-0.9/airbyte_serverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-07 12:42:25.000000 airbyte_serverless-0.9/airbyte_serverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-09-07 12:42:25.000000 airbyte_serverless-0.9/airbyte_serverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-09-07 12:42:25.000000 airbyte_serverless-0.9/airbyte_serverless.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    72596 2023-09-06 19:59:31.000000 airbyte_serverless-0.9/logo_and_name.png
+-rw-rw-rw-   0        0        0       42 2023-09-07 12:42:26.071816 airbyte_serverless-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-09-07 12:42:17.000000 airbyte_serverless-0.9/setup.py
```

### Comparing `airbyte_serverless-0.8/LICENSE` & `airbyte_serverless-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airbyte_serverless-0.8/PKG-INFO` & `airbyte_serverless-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: airbyte_serverless
-Version: 0.8
+Version: 0.9
 Summary: Airbyte made easy (no UI, no database, no cluster)
-Download-URL: https://github.com/unytics/airbyte_serverless/archive/refs/tags/v0.8.tar.gz
+Download-URL: https://github.com/unytics/airbyte_serverless/archive/refs/tags/v0.9.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `airbyte_serverless-0.8/README.md` & `airbyte_serverless-0.9/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_serverless-0.8/airbyte_serverless/airbyte_utils.py` & `airbyte_serverless-0.9/airbyte_serverless/airbyte_utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_serverless-0.8/airbyte_serverless/destinations.py` & `airbyte_serverless-0.9/airbyte_serverless/destinations.py`

 * *Files identical despite different names*

### Comparing `airbyte_serverless-0.8/airbyte_serverless/sources.py` & `airbyte_serverless-0.9/airbyte_serverless/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,10 +129,10 @@
     def extract(self, state=None):
         return self._run('read', state=state)
 
 
 class DockerAirbyteSource(AirbyteSource):
 
     def __init__(self, docker_image, *args, **kwargs):
-        exec = f'docker run --rm -i --volume ./:/mnt/temp {docker_image}'
-        super().__init__(exec, *args, **kwargs)
+        super().__init__('', *args, **kwargs)
         self.temp_dir_for_executable = '/mnt/temp'
+        self.exec = f'docker run --rm -i --volume {self.temp_dir}:{self.temp_dir_for_executable} {docker_image}'
```

### Comparing `airbyte_serverless-0.8/airbyte_serverless.egg-info/PKG-INFO` & `airbyte_serverless-0.9/airbyte_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: airbyte-serverless
-Version: 0.8
+Version: 0.9
 Summary: Airbyte made easy (no UI, no database, no cluster)
-Download-URL: https://github.com/unytics/airbyte_serverless/archive/refs/tags/v0.8.tar.gz
+Download-URL: https://github.com/unytics/airbyte_serverless/archive/refs/tags/v0.9.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `airbyte_serverless-0.8/logo_and_name.png` & `airbyte_serverless-0.9/logo_and_name.png`

 * *Files identical despite different names*

### Comparing `airbyte_serverless-0.8/setup.py` & `airbyte_serverless-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.8'
+VERSION = '0.9'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```

