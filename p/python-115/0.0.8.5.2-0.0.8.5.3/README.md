# Comparing `tmp/python_115-0.0.8.5.2.tar.gz` & `tmp/python_115-0.0.8.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.5.2.tar", max compression
+gzip compressed data, was "python_115-0.0.8.5.3.tar", max compression
```

## Comparing `python_115-0.0.8.5.2.tar` & `python_115-0.0.8.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.5.2/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-28 12:40:13.113995 python_115-0.0.8.5.2/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.5.2/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.5.2/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.5.2/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.5.2/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.5.2/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2024 2024-05-28 08:51:24.074103 python_115-0.0.8.5.2/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.5.2/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.2/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.5.2/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.5.2/p115/component/cipher.py
--rwxr-xr-x   0        0        0   244560 2024-05-28 12:12:17.132740 python_115-0.0.8.5.2/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.5.2/p115/component/exception.py
--rwxr-xr-x   0        0        0    65841 2024-05-28 08:52:45.311883 python_115-0.0.8.5.2/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.5.2/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.5.2/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.5.2/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.5.2/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.5.2/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.5.2/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.5.2/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.5.2/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.5.2/p115/tool/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-28 12:40:22.508837 python_115-0.0.8.5.2/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.5.2/readme.md
--rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.5.3/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-28 12:42:36.566609 python_115-0.0.8.5.3/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.5.3/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.5.3/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.5.3/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.5.3/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.5.3/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2024 2024-05-28 08:51:24.074103 python_115-0.0.8.5.3/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.5.3/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5.3/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.5.3/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.5.3/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   244560 2024-05-28 12:12:17.132740 python_115-0.0.8.5.3/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.5.3/p115/component/exception.py
+-rwxr-xr-x   0        0        0    65841 2024-05-28 08:52:45.311883 python_115-0.0.8.5.3/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.5.3/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.5.3/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.5.3/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.5.3/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.5.3/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.5.3/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.5.3/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.5.3/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.5.3/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-28 12:42:44.494644 python_115-0.0.8.5.3/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.5.3/readme.md
+-rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.5.3/PKG-INFO
```

### Comparing `python_115-0.0.8.5.2/LICENSE` & `python_115-0.0.8.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/cmd/check.py` & `python_115-0.0.8.5.3/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/cmd/iterdir.py` & `python_115-0.0.8.5.3/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/cmd/qrcode.py` & `python_115-0.0.8.5.3/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/__init__.py` & `python_115-0.0.8.5.3/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/cipher.py` & `python_115-0.0.8.5.3/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/client.py` & `python_115-0.0.8.5.3/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/fs.py` & `python_115-0.0.8.5.3/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/fs_base.py` & `python_115-0.0.8.5.3/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/fs_share.py` & `python_115-0.0.8.5.3/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/fs_zip.py` & `python_115-0.0.8.5.3/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/labellist.py` & `python_115-0.0.8.5.3/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/offline.py` & `python_115-0.0.8.5.3/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/recyclebin.py` & `python_115-0.0.8.5.3/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/component/sharing.py` & `python_115-0.0.8.5.3/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/p115/tool/__init__.py` & `python_115-0.0.8.5.3/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/pyproject.toml` & `python_115-0.0.8.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.5.2"
+version = "0.0.8.5.3"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.5.2/readme.md` & `python_115-0.0.8.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.5.2/PKG-INFO` & `python_115-0.0.8.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.5.2
+Version: 0.0.8.5.3
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

