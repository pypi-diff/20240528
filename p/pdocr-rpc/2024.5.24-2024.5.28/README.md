# Comparing `tmp/pdocr_rpc-2024.5.24.tar.gz` & `tmp/pdocr_rpc-2024.5.28.tar.gz`

## Comparing `pdocr_rpc-2024.5.24.tar` & `pdocr_rpc-2024.5.28.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/server.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/LICENSE
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/NOTICE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/PKG-INFO
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/NOTICE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.28/PKG-INFO
```

### Comparing `pdocr_rpc-2024.5.24/pdocr_rpc/__init__.py` & `pdocr_rpc-2024.5.28/pdocr_rpc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 # SPDX-License-Identifier: Apache Software License
 import json
 import os
 import time
 from xmlrpc.client import Binary
 from xmlrpc.client import ServerProxy
 
+import easyprocess
+
 from pdocr_rpc.conf import setting
 
 os.environ["DISPLAY"] = ":0"
 
-if setting.IS_LINUX:
+if setting.IS_LINUX or setting.IS_MACOS:
     import pyscreenshot as ImageGrab
 elif setting.IS_WINDOWS:
     from PIL import ImageGrab
 
 from funnylog import logger
 
 
 
 class OCR:
 
+    wayland_screen_dbus = "qdbus org.kde.KWin /Screenshot screenshotFullscreen"
+
     @classmethod
     def server_url(cls):
         return f"http://{setting.SERVER_IP}:{setting.PORT}"
 
     @classmethod
     def server(cls):
         return ServerProxy(cls.server_url(), allow_none=True)
@@ -44,22 +48,30 @@
     def _pdocr_client(cls, lang, picture_abspath=None, network_retry: int = 1):
         """
          通过 RPC 协议进行 OCR 识别。
         :return: 返回 PaddleOCR 的原始数据
         """
         if not picture_abspath:
             picture_abspath = setting.SCREEN_CACHE
-            if setting.IS_X11:
+            if setting.IS_LINUX:
+                if setting.IS_X11:
+                    try:
+                        ImageGrab.grab().save(os.path.expanduser(picture_abspath))
+                    except easyprocess.EasyProcessError:
+                        ...
+                else:
+                    # setting.IS_WAYLAND:
+                    picture_abspath = (os.popen(cls.wayland_screen_dbus).read().strip("\n"))
+            elif setting.IS_MACOS:
+                # for macos
                 ImageGrab.grab().save(os.path.expanduser(picture_abspath))
+
             else:
-                picture_abspath = (
-                    os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
-                    .read()
-                    .strip("\n")
-                )
+                # for windows
+                ImageGrab.grab().save(os.path.expanduser(picture_abspath))
 
         put_handle = open(os.path.expanduser(picture_abspath), "rb")
         for _ in range(network_retry + 1):
             try:
                 # 将图片上传到服务端
                 pic_dir = cls.server().image_put(Binary(put_handle.read()))
                 put_handle.close()
```

### Comparing `pdocr_rpc-2024.5.24/pdocr_rpc/conf.py` & `pdocr_rpc-2024.5.28/pdocr_rpc/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,56 +2,64 @@
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: Apache Software License
 import enum
 import os
-import sys
+import platform
+import tempfile
+from os import popen
 
 
 @enum.unique
 class DisplayServer(enum.Enum):
     wayland = "wayland"
     x11 = "x11"
 
 
 @enum.unique
 class PlatForm(enum.Enum):
-    win = "win32"
-    linux = "linux"
+    # win = "win32"
+    # linux = "linux"
+    win = "Windows"
+    linux = "Linux"
+    macos = "Darwin"
 
 
 class _Setting:
     """配置模块"""
 
     SERVER_IP = "127.0.0.1"
     PORT = 8890
     NETWORK_RETRY = 1
     PAUSE = 1
     TIMEOUT = 5
     MAX_MATCH_NUMBER = 100
 
     IS_LINUX = False
     IS_WINDOWS = False
-    if sys.platform == PlatForm.win.value:
+    IS_MACOS = False
+
+    SCREEN_CACHE = os.path.join(tempfile.gettempdir(), 'screen.png')  # SCREEN_CACHE = "/tmp/screen.png"
+
+    if platform.system() == PlatForm.win.value:
         # windows
         IS_WINDOWS = True
-        # TODO
-        ...
-    elif sys.platform == PlatForm.linux.value:
+    elif platform.system() == PlatForm.macos.value:
+        # MacOS
+        IS_MACOS = True
+    elif platform.system() == PlatForm.linux.value:
         # Linux
         IS_LINUX = True
         # 显示服务器
         DISPLAY_SERVER = (
-            os.popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
-            .read()
-            .split("=")[-1]
-            .strip("\n")
-        )
-
+                             popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
+                             .read()
+                             .split("=")[-1]
+                             .strip("\n")
+                         ) or ("x11" if popen("ps -ef | grep -v grep | grep kwin_x11").read() else "wayland")
         IS_X11 = DISPLAY_SERVER == DisplayServer.x11.value
         IS_WAYLAND = DISPLAY_SERVER == DisplayServer.wayland.value
-        SCREEN_CACHE = "/tmp/screen.png"
 
 
 setting = _Setting()
```

### Comparing `pdocr_rpc-2024.5.24/pdocr_rpc/server.py` & `pdocr_rpc-2024.5.28/pdocr_rpc/server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.24/LICENSE` & `pdocr_rpc-2024.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.24/NOTICE` & `pdocr_rpc-2024.5.28/NOTICE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.24/README.md` & `pdocr_rpc-2024.5.28/README.md`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.24/pyproject.toml` & `pdocr_rpc-2024.5.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.24/PKG-INFO` & `pdocr_rpc-2024.5.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2024.5.24
+Version: 2024.5.28
 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc
 Project-URL: Documentation, https://linuxdeepin.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 License-File: NOTICE
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.24 Summary: PaddleOCR-RPC
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.28 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc Project-URL:
 Documentation, https://linuxdeepin.github.io/pdocr-rpc Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE License-File: NOTICE Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.6 Requires-Dist: funnylog Requires-Dist: pillow; sys_platform ==
 'win32' Requires-Dist: pyscreenshot; sys_platform == 'linux' Provides-Extra:
```

