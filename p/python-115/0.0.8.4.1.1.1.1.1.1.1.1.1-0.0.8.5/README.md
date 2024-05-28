# Comparing `tmp/python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar.gz` & `tmp/python_115-0.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar", max compression
+gzip compressed data, was "python_115-0.0.8.5.tar", max compression
```

## Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar` & `python_115-0.0.8.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-28 03:49:01.522633 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:41:14.537317 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     1651 2024-05-28 08:38:46.854217 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8757 2024-05-28 08:37:09.063956 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1925 2024-05-28 05:18:42.776331 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/cipher.py
--rwxr-xr-x   0        0        0   244595 2024-05-28 08:30:52.768102 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/exception.py
--rwxr-xr-x   0        0        0    65840 2024-05-27 16:29:09.478683 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/tool/__init__.py
--rw-r--r--   0        0        0     1697 2024-05-28 08:42:36.073070 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/readme.md
--rw-r--r--   0        0        0    36415 1970-01-01 00:00:00.000000 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.5/LICENSE
+-rwxr-xr-x   0        0        0      154 2024-05-28 08:53:24.110531 python_115-0.0.8.5/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-28 03:49:01.522633 python_115-0.0.8.5/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.5/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.5/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.5/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.5/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2024 2024-05-28 08:51:24.074103 python_115-0.0.8.5/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.5/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.5/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.5/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.5/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   244595 2024-05-28 08:30:52.768102 python_115-0.0.8.5/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.5/p115/component/exception.py
+-rwxr-xr-x   0        0        0    65841 2024-05-28 08:52:45.311883 python_115-0.0.8.5/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.5/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.5/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.5/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.5/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.5/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.5/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.5/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.5/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.5/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1679 2024-05-28 08:43:32.210256 python_115-0.0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.5/readme.md
+-rw-r--r--   0        0        0    36397 1970-01-01 00:00:00.000000 python_115-0.0.8.5/PKG-INFO
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/LICENSE` & `python_115-0.0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/check.py` & `python_115-0.0.8.5/p115/cmd/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
 __doc__ = "115 签到"
 
-
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
+    from pathlib import Path
+    from sys import path
 
+    path[0] = str(Path(__file__).parents[2])
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
     from argparse import RawTextHelpFormatter
     from .init import subparsers
 
     parser = subparsers.add_parser("check", description=__doc__, formatter_class=RawTextHelpFormatter)
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/iterdir.py` & `python_115-0.0.8.5/p115/cmd/iterdir.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     "id", "parent_id", "name", "path", "relpath", "sha1", "pickcode", "is_directory", 
     "size", "ctime", "mtime", "atime", "hidden", "violated", "play_long", "thumb", 
     "star", "score", "labels", "description", 
 )
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
+    from pathlib import Path
+    from sys import path
 
+    path[0] = str(Path(__file__).parents[2])
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
     from argparse import RawTextHelpFormatter
     from .init import subparsers
 
     parser = subparsers.add_parser("iterdir", description=__doc__, formatter_class=RawTextHelpFormatter)
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/qrcode.py` & `python_115-0.0.8.5/p115/cmd/qrcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
 __doc__ = "扫码获取 115 cookies"
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
+    from pathlib import Path
+    from sys import path
 
+    path[0] = str(Path(__file__).parents[2])
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
     from argparse import RawTextHelpFormatter
     from .init import subparsers
 
     parser = subparsers.add_parser("qrcode", description=__doc__, formatter_class=RawTextHelpFormatter)
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/__init__.py` & `python_115-0.0.8.5/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/cipher.py` & `python_115-0.0.8.5/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/client.py` & `python_115-0.0.8.5/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs.py` & `python_115-0.0.8.5/p115/component/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             # {'state': False, 'code': 990002, 'message': '参数错误。'}
             case 990002:
                 raise OSError(errno.EINVAL, result)
             case _:
                 raise OSError(errno.EIO, result)
 
     def fs_files(self, /, payload: dict) -> AttrDict:
-        id = int(payload["id"])
+        id = int(payload["cid"])
         resp = check_response(self.client.fs_files(payload))
         if int(resp["path"][-1]["cid"]) != id:
             raise NotADirectoryError(errno.ENOTDIR, f"{id!r} is not a directory")
         return resp
 
     @check_response
     def fs_search(self, payload: str | dict, /) -> AttrDict:
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_base.py` & `python_115-0.0.8.5/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_share.py` & `python_115-0.0.8.5/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_zip.py` & `python_115-0.0.8.5/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/labellist.py` & `python_115-0.0.8.5/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/offline.py` & `python_115-0.0.8.5/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/recyclebin.py` & `python_115-0.0.8.5/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/sharing.py` & `python_115-0.0.8.5/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/tool/__init__.py` & `python_115-0.0.8.5/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/pyproject.toml` & `python_115-0.0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.4.1.1.1.1.1.1.1.1.1"
+version = "0.0.8.5"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/readme.md` & `python_115-0.0.8.5/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/PKG-INFO` & `python_115-0.0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.4.1.1.1.1.1.1.1.1.1
+Version: 0.0.8.5
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

