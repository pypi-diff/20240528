# Comparing `tmp/python_115-0.0.8.4.tar.gz` & `tmp/python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.4.tar", max compression
+gzip compressed data, was "python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar", max compression
```

## Comparing `python_115-0.0.8.4.tar` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.4/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.4/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.4/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.4/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.4/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.4/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.4/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.4/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.4/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.4/p115/component/cipher.py
--rwxr-xr-x   0        0        0   242824 2024-05-27 16:36:52.623847 python_115-0.0.8.4/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.4/p115/component/exception.py
--rwxr-xr-x   0        0        0    65840 2024-05-27 16:29:09.478683 python_115-0.0.8.4/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.4/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.4/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.4/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.4/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.4/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.4/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.4/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.4/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.4/p115/tool/__init__.py
--rw-r--r--   0        0        0     1679 2024-05-27 16:45:21.674629 python_115-0.0.8.4/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.4/readme.md
--rw-r--r--   0        0        0    36397 1970-01-01 00:00:00.000000 python_115-0.0.8.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-28 03:49:01.522633 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:41:14.537317 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1651 2024-05-28 08:38:46.854217 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8757 2024-05-28 08:37:09.063956 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1925 2024-05-28 05:18:42.776331 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   244595 2024-05-28 08:30:52.768102 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/exception.py
+-rwxr-xr-x   0        0        0    65840 2024-05-27 16:29:09.478683 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1697 2024-05-28 08:42:36.073070 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/readme.md
+-rw-r--r--   0        0        0    36415 1970-01-01 00:00:00.000000 python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/PKG-INFO
```

### Comparing `python_115-0.0.8.4/LICENSE` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/cmd/iterdir.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/iterdir.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 )
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
+    from argparse import RawTextHelpFormatter
     from .init import subparsers
 
-    parser = subparsers.add_parser("iterdir", description=__doc__)
+    parser = subparsers.add_parser("iterdir", description=__doc__, formatter_class=RawTextHelpFormatter)
 
 
 def main(args):
-    from p115 import P115FileSystem, P115Path, __version__
+    from p115 import P115Client, P115Path, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
     from os.path import expanduser, dirname, join as joinpath
     from sys import stdout
@@ -38,17 +39,19 @@
             try:
                 cookies = open(joinpath(dir_, "115-cookies.txt")).read()
                 if cookies:
                     break
             except FileNotFoundError:
                 pass
 
-    fs = P115FileSystem.login(cookies)
-    if fs.client.cookies != cookies:
-        open("115-cookies.txt", "w").write(fs.client.cookies)
+    client = P115Client(cookies)
+    if client.cookies != cookies:
+        open("115-cookies.txt", "w").write(client.cookies)
+
+    fs = client.fs
 
     if args.password and not fs.hidden_mode:
         fs.hidden_switch(True, password=args.password)
 
     keys = args.keys or KEYS
     output_type = args.output_type
```

### Comparing `python_115-0.0.8.4/p115/cmd/qrcode.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/cmd/qrcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
+    from argparse import RawTextHelpFormatter
     from .init import subparsers
 
-    parser = subparsers.add_parser("qrcode", description=__doc__)
+    parser = subparsers.add_parser("qrcode", description=__doc__, formatter_class=RawTextHelpFormatter)
 
 
 def main(args):
     from p115 import P115Client, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
```

### Comparing `python_115-0.0.8.4/p115/component/__init__.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/cipher.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/client.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1273,14 +1273,78 @@
         """获取（并可修改）此账户的网页版设置（提示：较为复杂，自己抓包研究）
         POST https://115.com/?ac=setting&even=saveedit&is_wl_tpl=1
         """
         api = "https://115.com/?ac=setting&even=saveedit&is_wl_tpl=1"
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
+    @overload
+    def user_points_sign(
+        self, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def user_points_sign(
+        self, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def user_points_sign(
+        self, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取签到信息
+        GET https://proapi.115.com/android/2.0/user/points_sign
+        """
+        api = "https://proapi.115.com/android/2.0/user/points_sign"
+        request_kwargs.pop("parse", None)
+        return self.request(api, async_=async_, **request_kwargs)
+
+    @overload
+    def user_points_sign_post(
+        self, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def user_points_sign_post(
+        self, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def user_points_sign_post(
+        self, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """进行自动签到
+        POST https://proapi.115.com/android/2.0/user/points_sign
+        """
+        api = "https://proapi.115.com/android/2.0/user/points_sign"
+        t = int(time())
+        text = str(self.user_id)+"-Points_Sign@#115-"+str(t)
+        request_kwargs["data"] = {
+            "token": sha1(text.encode()).hexdigest(), 
+            "token_time": t, 
+        }
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", async_=async_, **request_kwargs)
+
     ########## App API ##########
 
     @overload
     @staticmethod
     def app_version_list(
         async_: Literal[False] = False, 
         **request_kwargs
```

### Comparing `python_115-0.0.8.4/p115/component/fs.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/fs_base.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/fs_share.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/fs_zip.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/labellist.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/offline.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/recyclebin.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/component/sharing.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/p115/tool/__init__.py` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/pyproject.toml` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.4"
+version = "0.0.8.4.1.1.1.1.1.1.1.1.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.4/readme.md` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.4/PKG-INFO` & `python_115-0.0.8.4.1.1.1.1.1.1.1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.4
+Version: 0.0.8.4.1.1.1.1.1.1.1.1.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

