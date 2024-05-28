# Comparing `tmp/gammarers.aws-secure-log-bucket-1.6.6.tar.gz` & `tmp/gammarers.aws-secure-log-bucket-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-log-bucket-1.6.6.tar", last modified: Sun May 26 18:23:30 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-log-bucket-1.7.0.tar", last modified: Tue May 28 04:31:09 2024, max compression
```

## Comparing `gammarers.aws-secure-log-bucket-1.6.6.tar` & `gammarers.aws-secure-log-bucket-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.276251 gammarers.aws-secure-log-bucket-1.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.276251 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:23:16.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:23:30.280251 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-26 18:23:30.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 18:23:30.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:23:30.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-26 18:23:30.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 18:23:30.000000 gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.980647 gammarers.aws-secure-log-bucket-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.980647 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24076 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.7.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:30:58.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:31:09.984647 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-28 04:31:09.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-28 04:31:09.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:31:09.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 04:31:09.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 04:31:09.000000 gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/LICENSE` & `gammarers.aws-secure-log-bucket-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/PKG-INFO` & `gammarers.aws-secure-log-bucket-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-log-bucket
-Version: 1.6.6
+Version: 1.7.0
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarers/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -45,20 +45,38 @@
 | GLACIER             | 180 days                     |
 | DEEP_ARCHIVE        | 360 days                     |
 
 ## Install
 
 ### TypeScript
 
+#### install by npm
+
 ```shell
 npm install @gammarers/aws-secure-log-bucket
-# or
+```
+
+#### install by yarn
+
+```shell
 yarn add @gammarers/aws-secure-log-bucket
 ```
 
+#### install by pnpm
+
+```shell
+pnpm add @gammarers/aws-secure-log-bucket
+```
+
+#### install by bun
+
+```shell
+bun add @gammarers/aws-secure-log-bucket
+```
+
 ### Python
 
 ```shell
 pip install gammarers.aws-secure-log-bucket
 ```
 
 ### C# / .NET
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/README.md` & `gammarers.aws-secure-log-bucket-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,38 @@
 | GLACIER             | 180 days                     |
 | DEEP_ARCHIVE        | 360 days                     |
 
 ## Install
 
 ### TypeScript
 
+#### install by npm
+
 ```shell
 npm install @gammarers/aws-secure-log-bucket
-# or
+```
+
+#### install by yarn
+
+```shell
 yarn add @gammarers/aws-secure-log-bucket
 ```
 
+#### install by pnpm
+
+```shell
+pnpm add @gammarers/aws-secure-log-bucket
+```
+
+#### install by bun
+
+```shell
+bun add @gammarers/aws-secure-log-bucket
+```
+
 ### Python
 
 ```shell
 pip install gammarers.aws-secure-log-bucket
 ```
 
 ### C# / .NET
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/setup.py` & `gammarers.aws-secure-log-bucket-1.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-log-bucket",
-    "version": "1.6.6",
+    "version": "1.7.0",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarers.aws_secure_log_bucket",
         "gammarers.aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@1.6.6.jsii.tgz"
+            "aws-secure-log-bucket@1.7.0.jsii.tgz"
         ],
         "gammarers.aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarers.aws-secure-bucket>=1.3.1, <1.4.0",
+        "gammarers.aws-secure-bucket>=1.4.1, <1.5.0",
         "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/__init__.py` & `gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,38 @@
 | GLACIER             | 180 days                     |
 | DEEP_ARCHIVE        | 360 days                     |
 
 ## Install
 
 ### TypeScript
 
+#### install by npm
+
 ```shell
 npm install @gammarers/aws-secure-log-bucket
-# or
+```
+
+#### install by yarn
+
+```shell
 yarn add @gammarers/aws-secure-log-bucket
 ```
 
+#### install by pnpm
+
+```shell
+pnpm add @gammarers/aws-secure-log-bucket
+```
+
+#### install by bun
+
+```shell
+bun add @gammarers/aws-secure-log-bucket
+```
+
 ### Python
 
 ```shell
 pip install gammarers.aws-secure-log-bucket
 ```
 
 ### C# / .NET
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py` & `gammarers.aws-secure-log-bucket-1.7.0/src/gammarers/aws_secure_log_bucket/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-log-bucket",
-    "1.6.6",
+    "1.7.0",
     __name__[0:-6],
-    "aws-secure-log-bucket@1.6.6.jsii.tgz",
+    "aws-secure-log-bucket@1.7.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-log-bucket
-Version: 1.6.6
+Version: 1.7.0
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarers/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -45,20 +45,38 @@
 | GLACIER             | 180 days                     |
 | DEEP_ARCHIVE        | 360 days                     |
 
 ## Install
 
 ### TypeScript
 
+#### install by npm
+
 ```shell
 npm install @gammarers/aws-secure-log-bucket
-# or
+```
+
+#### install by yarn
+
+```shell
 yarn add @gammarers/aws-secure-log-bucket
 ```
 
+#### install by pnpm
+
+```shell
+pnpm add @gammarers/aws-secure-log-bucket
+```
+
+#### install by bun
+
+```shell
+bun add @gammarers/aws-secure-log-bucket
+```
+
 ### Python
 
 ```shell
 pip install gammarers.aws-secure-log-bucket
 ```
 
 ### C# / .NET
```

### Comparing `gammarers.aws-secure-log-bucket-1.6.6/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-log-bucket-1.7.0/src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_log_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_log_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_log_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_log_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_log_bucket/__init__.py
 src/gammarers/aws_secure_log_bucket/py.typed
 src/gammarers/aws_secure_log_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.6.6.jsii.tgz
+src/gammarers/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.7.0.jsii.tgz
```
