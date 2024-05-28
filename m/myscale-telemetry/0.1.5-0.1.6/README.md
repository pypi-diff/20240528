# Comparing `tmp/myscale-telemetry-0.1.5.tar.gz` & `tmp/myscale-telemetry-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale-telemetry-0.1.5.tar", last modified: Mon May 27 03:58:54 2024, max compression
+gzip compressed data, was "myscale-telemetry-0.1.6.tar", last modified: Mon May 27 04:35:02 2024, max compression
```

## Comparing `myscale-telemetry-0.1.5.tar` & `myscale-telemetry-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.595193 myscale-telemetry-0.1.5/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.5/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 03:58:54.594895 myscale-telemetry-0.1.5/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)     6384 2024-05-27 03:53:11.000000 myscale-telemetry-0.1.5/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.593755 myscale-telemetry-0.1.5/myscale_telemetry/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    23749 2024-05-27 03:48:32.000000 myscale-telemetry-0.1.5/myscale_telemetry/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6815 2024-05-27 03:50:06.000000 myscale-telemetry-0.1.5/myscale_telemetry/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.594602 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)      101 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-27 03:58:54.595230 myscale-telemetry-0.1.5/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      920 2024-05-27 03:54:39.000000 myscale-telemetry-0.1.5/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 04:35:02.827545 myscale-telemetry-0.1.6/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.6/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 04:35:02.827341 myscale-telemetry-0.1.6/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)     6384 2024-05-27 03:53:11.000000 myscale-telemetry-0.1.6/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 04:35:02.826201 myscale-telemetry-0.1.6/myscale_telemetry/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.6/myscale_telemetry/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.6/myscale_telemetry/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    23749 2024-05-27 03:48:32.000000 myscale-telemetry-0.1.6/myscale_telemetry/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.6/myscale_telemetry/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6815 2024-05-27 03:50:06.000000 myscale-telemetry-0.1.6/myscale_telemetry/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 04:35:02.827079 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 04:35:02.000000 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-27 04:35:02.000000 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-27 04:35:02.000000 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)      103 2024-05-27 04:35:02.000000 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-27 04:35:02.000000 myscale-telemetry-0.1.6/myscale_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-27 04:35:02.827584 myscale-telemetry-0.1.6/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      922 2024-05-27 04:34:39.000000 myscale-telemetry-0.1.6/setup.py
```

### Comparing `myscale-telemetry-0.1.5/LICENSE` & `myscale-telemetry-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/PKG-INFO` & `myscale-telemetry-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.5
+Version: 0.1.6
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `myscale-telemetry-0.1.5/README.md` & `myscale-telemetry-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/myscale_telemetry/consumer.py` & `myscale-telemetry-0.1.6/myscale_telemetry/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/myscale_telemetry/handler.py` & `myscale-telemetry-0.1.6/myscale_telemetry/handler.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/myscale_telemetry/span_data.py` & `myscale-telemetry-0.1.6/myscale_telemetry/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/myscale_telemetry/task_manager.py` & `myscale-telemetry-0.1.6/myscale_telemetry/task_manager.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.5/myscale_telemetry.egg-info/PKG-INFO` & `myscale-telemetry-0.1.6/myscale_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.5
+Version: 0.1.6
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `myscale-telemetry-0.1.5/setup.py` & `myscale-telemetry-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="myscale-telemetry",
-    version="0.1.5",
+    version="0.1.6",
     description="Open-source observability for your LLM application.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Xu Jing",
     author_email="xuj@myscale.com",
     url="https://github.com/myscale/myscale-telemetry",
     packages=find_packages(),
     install_requires=[
         "backoff>=2.2.1",
-        "langchain>=0.2.0",
-        "langchain-community>=0.2.0",
+        "langchain>=0.1.20",
+        "langchain-community>=0.0.38",
         "clickhouse-connect>=0.7.8",
         "tiktoken>=0.7.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

