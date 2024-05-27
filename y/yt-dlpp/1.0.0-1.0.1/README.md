# Comparing `tmp/yt_dlpp-1.0.0.tar.gz` & `tmp/yt_dlpp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_dlpp-1.0.0.tar", last modified: Mon May 27 22:34:50 2024, max compression
+gzip compressed data, was "yt_dlpp-1.0.1.tar", last modified: Mon May 27 22:44:30 2024, max compression
```

## Comparing `yt_dlpp-1.0.0.tar` & `yt_dlpp-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 geoffrey  (1000) geoffrey  (1001)        0 2024-05-27 22:34:50.745781 yt_dlpp-1.0.0/
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     1211 2024-05-27 22:30:38.000000 yt_dlpp-1.0.0/LICENSE.md
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     3489 2024-05-27 22:34:50.745781 yt_dlpp-1.0.0/PKG-INFO
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     1445 2024-03-15 22:18:15.000000 yt_dlpp-1.0.0/README.md
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)      799 2024-05-27 22:33:12.000000 yt_dlpp-1.0.0/pyproject.toml
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)       38 2024-05-27 22:34:50.745781 yt_dlpp-1.0.0/setup.cfg
-drwxr-xr-x   0 geoffrey  (1000) geoffrey  (1001)        0 2024-05-27 22:34:50.742447 yt_dlpp-1.0.0/yt_dlpp/
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        0 2024-01-21 23:16:52.000000 yt_dlpp-1.0.0/yt_dlpp/__init__.py
-drwxr-xr-x   0 geoffrey  (1000) geoffrey  (1001)        0 2024-05-27 22:34:50.742447 yt_dlpp-1.0.0/yt_dlpp/interceptors/
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        0 2024-03-15 07:09:00.000000 yt_dlpp-1.0.0/yt_dlpp/interceptors/__init__.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     2547 2024-03-15 22:04:28.000000 yt_dlpp-1.0.0/yt_dlpp/interceptors/interceptor.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     4823 2024-03-15 22:13:34.000000 yt_dlpp-1.0.0/yt_dlpp/main.py
-drwxr-xr-x   0 geoffrey  (1000) geoffrey  (1001)        0 2024-05-27 22:34:50.745781 yt_dlpp-1.0.0/yt_dlpp/workers/
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        0 2024-01-21 22:47:26.000000 yt_dlpp-1.0.0/yt_dlpp/workers/__init__.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)      567 2024-03-14 21:30:51.000000 yt_dlpp-1.0.0/yt_dlpp/workers/dedup_worker.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     2346 2024-03-31 12:56:22.000000 yt_dlpp-1.0.0/yt_dlpp/workers/download_worker.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     2773 2024-03-15 07:21:46.000000 yt_dlpp-1.0.0/yt_dlpp/workers/info_worker.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     6728 2024-03-31 16:18:06.000000 yt_dlpp-1.0.0/yt_dlpp/workers/progress_worker.py
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     3468 2024-03-15 22:13:30.000000 yt_dlpp-1.0.0/yt_dlpp/workers/worker.py
-drwxr-xr-x   0 geoffrey  (1000) geoffrey  (1001)        0 2024-05-27 22:34:50.745781 yt_dlpp-1.0.0/yt_dlpp.egg-info/
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)     3489 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)      515 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        1 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)       46 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        5 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/requires.txt
--rw-r--r--   0 geoffrey  (1000) geoffrey  (1001)        8 2024-05-27 22:34:50.000000 yt_dlpp-1.0.0/yt_dlpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:30.204493 yt_dlpp-1.0.1/yt_dlpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/yt_dlpp/interceptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/interceptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/interceptors/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/yt_dlpp/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/dedup_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/download_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/info_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/progress_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-27 22:44:25.000000 yt_dlpp-1.0.1/yt_dlpp/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:44:30.208493 yt_dlpp-1.0.1/yt_dlpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 22:44:30.000000 yt_dlpp-1.0.1/yt_dlpp.egg-info/top_level.txt
```

### Comparing `yt_dlpp-1.0.0/LICENSE.md` & `yt_dlpp-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/PKG-INFO` & `yt_dlpp-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-dlpp
-Version: 1.0.0
+Version: 1.0.1
 Summary: A thin wrapper around yt-dlp for parallel downloads
 Author-email: Geoffrey Coulaud <geoffrey.coulaud@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -47,15 +47,18 @@
 `yt-dlpp` is just `yt-dlp` but starts downloads in parallel.   
 It supports passing multiple download URLs and unwrapping playlists.
 
 ## Installation
 
 ### From pypi
 
-TODO: package, publish and document installation
+```sh
+pip install yt-dlpp
+```
+
 
 ### From source, on Linux
 
 ```sh
 git clone "$YT_DLPP_REPO"
 cd yt-dlpp
 python3 -m venv .venv
```

### Comparing `yt_dlpp-1.0.0/README.md` & `yt_dlpp-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 `yt-dlpp` is just `yt-dlp` but starts downloads in parallel.   
 It supports passing multiple download URLs and unwrapping playlists.
 
 ## Installation
 
 ### From pypi
 
-TODO: package, publish and document installation
+```sh
+pip install yt-dlpp
+```
+
 
 ### From source, on Linux
 
 ```sh
 git clone "$YT_DLPP_REPO"
 cd yt-dlpp
 python3 -m venv .venv
```

### Comparing `yt_dlpp-1.0.0/pyproject.toml` & `yt_dlpp-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	{ name = "Geoffrey Coulaud", email = "geoffrey.coulaud@gmail.com" },
 ]
 classifiers = [
 	"License :: OSI Approved :: The Unlicense (Unlicense)",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3",
 ]
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.11"
 dependencies = [
 	"rich",
 ]
 
 [project.urls]
 Homepage = "https://github.com/GeoffreyCoulaud/yt-dlpp"
```

### Comparing `yt_dlpp-1.0.0/yt_dlpp/interceptors/interceptor.py` & `yt_dlpp-1.0.1/yt_dlpp/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/main.py` & `yt_dlpp-1.0.1/yt_dlpp/main.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/workers/dedup_worker.py` & `yt_dlpp-1.0.1/yt_dlpp/workers/dedup_worker.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/workers/download_worker.py` & `yt_dlpp-1.0.1/yt_dlpp/workers/download_worker.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/workers/info_worker.py` & `yt_dlpp-1.0.1/yt_dlpp/workers/info_worker.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/workers/progress_worker.py` & `yt_dlpp-1.0.1/yt_dlpp/workers/progress_worker.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp/workers/worker.py` & `yt_dlpp-1.0.1/yt_dlpp/workers/worker.py`

 * *Files identical despite different names*

### Comparing `yt_dlpp-1.0.0/yt_dlpp.egg-info/PKG-INFO` & `yt_dlpp-1.0.1/yt_dlpp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-dlpp
-Version: 1.0.0
+Version: 1.0.1
 Summary: A thin wrapper around yt-dlp for parallel downloads
 Author-email: Geoffrey Coulaud <geoffrey.coulaud@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -47,15 +47,18 @@
 `yt-dlpp` is just `yt-dlp` but starts downloads in parallel.   
 It supports passing multiple download URLs and unwrapping playlists.
 
 ## Installation
 
 ### From pypi
 
-TODO: package, publish and document installation
+```sh
+pip install yt-dlpp
+```
+
 
 ### From source, on Linux
 
 ```sh
 git clone "$YT_DLPP_REPO"
 cd yt-dlpp
 python3 -m venv .venv
```

### Comparing `yt_dlpp-1.0.0/yt_dlpp.egg-info/SOURCES.txt` & `yt_dlpp-1.0.1/yt_dlpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

