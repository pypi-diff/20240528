# Comparing `tmp/pytorrplay-0.0.1.tar.gz` & `tmp/pytorrplay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorrplay-0.0.1.tar", max compression
+gzip compressed data, was "pytorrplay-0.0.2.tar", max compression
```

## Comparing `pytorrplay-0.0.1.tar` & `pytorrplay-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3990 2024-05-26 20:05:02.638832 pytorrplay-0.0.1/README.md
--rw-r--r--   0        0        0      690 2024-05-27 22:27:59.435494 pytorrplay-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       28 2024-05-22 07:15:14.883458 pytorrplay-0.0.1/pytorrplay/__init__.py
--rw-r--r--   0        0        0      568 2024-05-25 13:10:55.669674 pytorrplay-0.0.1/pytorrplay/__main__.py
--rw-r--r--   0        0        0      864 2024-05-22 18:59:03.876477 pytorrplay-0.0.1/pytorrplay/arg_parser.py
--rw-r--r--   0        0        0     1138 2024-05-25 13:11:03.972895 pytorrplay-0.0.1/pytorrplay/config_utils.py
--rwxr-xr-x   0        0        0     5875 2024-05-26 20:48:06.791557 pytorrplay-0.0.1/pytorrplay/pytorr_play.py
--rw-r--r--   0        0        0     5845 2024-05-26 20:47:49.238424 pytorrplay-0.0.1/pytorrplay/streamer.py
--rw-r--r--   0        0        0     5245 2024-05-22 05:16:32.310713 pytorrplay-0.0.1/pytorrplay/ui_methods.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pytorrplay-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3990 2024-05-26 20:05:02.638832 pytorrplay-0.0.2/README.md
+-rw-r--r--   0        0        0      688 2024-05-27 22:38:05.576725 pytorrplay-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-05-22 07:15:14.883458 pytorrplay-0.0.2/pytorrplay/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-25 13:10:55.669674 pytorrplay-0.0.2/pytorrplay/__main__.py
+-rw-r--r--   0        0        0      864 2024-05-22 18:59:03.876477 pytorrplay-0.0.2/pytorrplay/arg_parser.py
+-rw-r--r--   0        0        0     1138 2024-05-25 13:11:03.972895 pytorrplay-0.0.2/pytorrplay/config_utils.py
+-rwxr-xr-x   0        0        0     5875 2024-05-26 20:48:06.791557 pytorrplay-0.0.2/pytorrplay/pytorr_play.py
+-rw-r--r--   0        0        0     5845 2024-05-26 20:47:49.238424 pytorrplay-0.0.2/pytorrplay/streamer.py
+-rw-r--r--   0        0        0     5245 2024-05-22 05:16:32.310713 pytorrplay-0.0.2/pytorrplay/ui_methods.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pytorrplay-0.0.2/PKG-INFO
```

### Comparing `pytorrplay-0.0.1/README.md` & `pytorrplay-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pyproject.toml` & `pytorrplay-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorrplay"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tool for streaming videos from torrrents"
 authors = ["imithrellas"]
 license = "MIT"
 repository = "https://gitlab.com/imithrellas/PyTorr-Play"
 readme = "README.md"
 keywords = ["torrent", "jackett", "curses", "rofi", "mpv", "media"]
 
@@ -22,8 +22,8 @@
 dbus-python = "^1.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-pytorr-play = "pytorr_play.__main__:main"
+pytorrplay = "pytorrplay.__main__:main"
```

### Comparing `pytorrplay-0.0.1/pytorrplay/__main__.py` & `pytorrplay-0.0.2/pytorrplay/__main__.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pytorrplay/arg_parser.py` & `pytorrplay-0.0.2/pytorrplay/arg_parser.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pytorrplay/config_utils.py` & `pytorrplay-0.0.2/pytorrplay/config_utils.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pytorrplay/pytorr_play.py` & `pytorrplay-0.0.2/pytorrplay/pytorr_play.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pytorrplay/streamer.py` & `pytorrplay-0.0.2/pytorrplay/streamer.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/pytorrplay/ui_methods.py` & `pytorrplay-0.0.2/pytorrplay/ui_methods.py`

 * *Files identical despite different names*

### Comparing `pytorrplay-0.0.1/PKG-INFO` & `pytorrplay-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrplay
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for streaming videos from torrrents
 Home-page: https://gitlab.com/imithrellas/PyTorr-Play
 License: MIT
 Keywords: torrent,jackett,curses,rofi,mpv,media
 Author: imithrellas
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

