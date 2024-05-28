# Comparing `tmp/imecilabt-gpulab-cli-3.9.4.tar.gz` & `tmp/imecilabt_gpulab_cli-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imecilabt-gpulab-cli-3.9.4.tar", last modified: Tue Feb 27 14:35:12 2024, max compression
+gzip compressed data, was "imecilabt_gpulab_cli-3.9.5.tar", last modified: Tue May 28 13:55:07 2024, max compression
```

## Comparing `imecilabt-gpulab-cli-3.9.4.tar` & `imecilabt_gpulab_cli-3.9.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-02-27 14:35:12.646140 imecilabt-gpulab-cli-3.9.4/
--rw-r--r--   0 wim       (1000) users      (100)    32423 2021-05-04 07:44:59.000000 imecilabt-gpulab-cli-3.9.4/LICENSE
--rw-r--r--   0 wim       (1000) users      (100)     2183 2024-02-27 14:35:12.646140 imecilabt-gpulab-cli-3.9.4/PKG-INFO
--rw-r--r--   0 wim       (1000) users      (100)     1025 2021-05-04 10:26:30.000000 imecilabt-gpulab-cli-3.9.4/README.md
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-02-27 14:35:12.639473 imecilabt-gpulab-cli-3.9.4/imecilabt/
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-02-27 14:35:12.639473 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-02-27 14:35:12.642806 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/
--rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/__init__.py
--rw-r--r--   0 wim       (1000) users      (100)    97044 2024-02-27 14:32:19.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/__main__.py
--rw-r--r--   0 wim       (1000) users      (100)       21 2024-02-27 14:34:46.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/_version.py
--rw-r--r--   0 wim       (1000) users      (100)    11398 2023-03-21 06:49:27.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/apiclient.py
--rw-r--r--   0 wim       (1000) users      (100)     2082 2023-03-21 06:58:13.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/cert_processor.py
--rw-r--r--   0 wim       (1000) users      (100)     6109 2021-08-04 14:24:52.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/ssh_config_manager.py
--rw-r--r--   0 wim       (1000) users      (100)      827 2019-12-06 15:13:31.000000 imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/util.py
-drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-02-27 14:35:12.642806 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/
--rw-r--r--   0 wim       (1000) users      (100)     2183 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/PKG-INFO
--rw-r--r--   0 wim       (1000) users      (100)      579 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wim       (1000) users      (100)        1 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wim       (1000) users      (100)       66 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/entry_points.txt
--rw-r--r--   0 wim       (1000) users      (100)        1 2019-12-06 15:24:01.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/not-zip-safe
--rw-r--r--   0 wim       (1000) users      (100)       82 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/requires.txt
--rw-r--r--   0 wim       (1000) users      (100)       10 2024-02-27 14:35:12.000000 imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/top_level.txt
--rw-r--r--   0 wim       (1000) users      (100)       38 2024-02-27 14:35:12.646140 imecilabt-gpulab-cli-3.9.4/setup.cfg
--rw-r--r--   0 wim       (1000) users      (100)     2978 2023-12-12 10:47:36.000000 imecilabt-gpulab-cli-3.9.4/setup.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-05-28 13:55:07.130249 imecilabt_gpulab_cli-3.9.5/
+-rw-r--r--   0 wim       (1000) users      (100)    32423 2021-05-04 07:44:59.000000 imecilabt_gpulab_cli-3.9.5/LICENSE
+-rw-r--r--   0 wim       (1000) users      (100)     2183 2024-05-28 13:55:07.130249 imecilabt_gpulab_cli-3.9.5/PKG-INFO
+-rw-r--r--   0 wim       (1000) users      (100)     1025 2021-05-04 10:26:30.000000 imecilabt_gpulab_cli-3.9.5/README.md
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-05-28 13:55:07.123582 imecilabt_gpulab_cli-3.9.5/imecilabt/
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-05-28 13:55:07.123582 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-05-28 13:55:07.126916 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/
+-rw-r--r--   0 wim       (1000) users      (100)        0 2019-12-06 15:13:31.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/__init__.py
+-rw-r--r--   0 wim       (1000) users      (100)    97044 2024-02-27 14:32:19.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/__main__.py
+-rw-r--r--   0 wim       (1000) users      (100)       21 2024-05-28 13:54:19.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/_version.py
+-rw-r--r--   0 wim       (1000) users      (100)    11398 2023-03-21 06:49:27.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/apiclient.py
+-rw-r--r--   0 wim       (1000) users      (100)     2082 2023-03-21 06:58:13.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/cert_processor.py
+-rw-r--r--   0 wim       (1000) users      (100)     6109 2021-08-04 14:24:52.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/ssh_config_manager.py
+-rw-r--r--   0 wim       (1000) users      (100)      827 2019-12-06 15:13:31.000000 imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/util.py
+drwxr-xr-x   0 wim       (1000) users      (100)        0 2024-05-28 13:55:07.126916 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/
+-rw-r--r--   0 wim       (1000) users      (100)     2183 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wim       (1000) users      (100)      579 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wim       (1000) users      (100)        1 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wim       (1000) users      (100)       66 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wim       (1000) users      (100)        1 2019-12-06 15:24:01.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/not-zip-safe
+-rw-r--r--   0 wim       (1000) users      (100)       82 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/requires.txt
+-rw-r--r--   0 wim       (1000) users      (100)       10 2024-05-28 13:55:07.000000 imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/top_level.txt
+-rw-r--r--   0 wim       (1000) users      (100)       38 2024-05-28 13:55:07.130249 imecilabt_gpulab_cli-3.9.5/setup.cfg
+-rw-r--r--   0 wim       (1000) users      (100)     3070 2024-05-28 13:54:03.000000 imecilabt_gpulab_cli-3.9.5/setup.py
```

### Comparing `imecilabt-gpulab-cli-3.9.4/LICENSE` & `imecilabt_gpulab_cli-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/PKG-INFO` & `imecilabt_gpulab_cli-3.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imecilabt-gpulab-cli
-Version: 3.9.4
+Version: 3.9.5
 Summary: GPULab CLI
 Home-page: https://gpulab.ilabt.imec.be
 Author: Thijs Walcarius <Thijs.Walcarius@ugent.be>, Wim Van de Meerssche <wim.vandemeerssche@ugent.be>
 Author-email: gpulab@ilabt.imec.be
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.ilabt.imec.be/ilabt/gpulab/gpulab-cli/-/issues
 Project-URL: Documentation, https://doc.ilabt.imec.be/ilabt/gpulab/
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.18.4
+Requires-Dist: requests==2.31.0
 Requires-Dist: click>=6.7
 Requires-Dist: cryptography==3.4.8
 Requires-Dist: imecilabt-gpulab-common<6,>=5.0.0
 
 GPULab CLI
 ==========
```

### Comparing `imecilabt-gpulab-cli-3.9.4/README.md` & `imecilabt_gpulab_cli-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/__main__.py` & `imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/apiclient.py` & `imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/apiclient.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/cert_processor.py` & `imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/cert_processor.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/ssh_config_manager.py` & `imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/ssh_config_manager.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt/gpulab/cli/util.py` & `imecilabt_gpulab_cli-3.9.5/imecilabt/gpulab/cli/util.py`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/PKG-INFO` & `imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imecilabt-gpulab-cli
-Version: 3.9.4
+Version: 3.9.5
 Summary: GPULab CLI
 Home-page: https://gpulab.ilabt.imec.be
 Author: Thijs Walcarius <Thijs.Walcarius@ugent.be>, Wim Van de Meerssche <wim.vandemeerssche@ugent.be>
 Author-email: gpulab@ilabt.imec.be
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.ilabt.imec.be/ilabt/gpulab/gpulab-cli/-/issues
 Project-URL: Documentation, https://doc.ilabt.imec.be/ilabt/gpulab/
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.18.4
+Requires-Dist: requests==2.31.0
 Requires-Dist: click>=6.7
 Requires-Dist: cryptography==3.4.8
 Requires-Dist: imecilabt-gpulab-common<6,>=5.0.0
 
 GPULab CLI
 ==========
```

### Comparing `imecilabt-gpulab-cli-3.9.4/imecilabt_gpulab_cli.egg-info/SOURCES.txt` & `imecilabt_gpulab_cli-3.9.5/imecilabt_gpulab_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imecilabt-gpulab-cli-3.9.4/setup.py` & `imecilabt_gpulab_cli-3.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,18 @@
 #     but now, gpulab-common uses dataclasses, so at least python 3.7 is required
 #        (python 3.7.0 was released June 27, 2018)
 #        (python 3.7 is available from ubuntu 19.04 Disco Dingo, released April 18, 2019)
 #            (the deadsnakes ppa can be used for earlier ubuntu's)
 #        (python 3.7 is available from debian 10.0 buster, released July 6th, 2019)
 #        (+ there's always https://github.com/pyenv/pyenv)
 
-    install_requires=["requests>=2.18.4",
+# Requests 2.32.2 broke GPULab CLI for some reason!
+# So we'll use 2.31.0 which works fine
+
+    install_requires=["requests==2.31.0",
                       "click>=6.7",
                       # "sentry-sdk==1.11.1"  # not yet
                       "cryptography==3.4.8",
                       "imecilabt-gpulab-common>=5.0.0, <6"],
     python_requires='>=3.7',
 
     entry_points={
```

