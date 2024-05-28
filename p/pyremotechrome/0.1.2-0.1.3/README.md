# Comparing `tmp/pyremotechrome-0.1.2.tar.gz` & `tmp/pyremotechrome-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.1.2.tar", last modified: Sun May 26 09:48:54 2024, max compression
+gzip compressed data, was "pyremotechrome-0.1.3.tar", last modified: Tue May 28 14:33:31 2024, max compression
```

## Comparing `pyremotechrome-0.1.2.tar` & `pyremotechrome-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.072851 pyremotechrome-0.1.2/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.2/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.2/README.md
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-26 09:47:54.000000 pyremotechrome-0.1.2/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.2/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.2/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.2/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.2/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.2/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.2/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     7348 2024-05-26 09:19:02.000000 pyremotechrome-0.1.2/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4635 2024-05-26 06:59:33.000000 pyremotechrome-0.1.2/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    16367 2024-05-26 09:35:44.000000 pyremotechrome-0.1.2/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2893 2024-05-26 09:19:08.000000 pyremotechrome-0.1.2/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-26 06:59:48.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     7462 2024-05-26 09:26:18.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1344 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2435 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1752 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1451 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1713 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     3797 2024-05-26 04:51:07.000000 pyremotechrome-0.1.2/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1062 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-26 09:48:54.072851 pyremotechrome-0.1.2/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.3/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.3/README.md
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-28 14:33:28.000000 pyremotechrome-0.1.3/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.3/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.3/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.3/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.3/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.3/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.3/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7462 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/server/manager.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     4635 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.3/pyremotechrome/session/__init__.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)    16074 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/base.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     2893 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/monitor/
+-rwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/audio.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     5187 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.418877 pyremotechrome-0.1.3/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/support/common/
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1344 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/__init__.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     2435 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/directory.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1752 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/info.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1451 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/result.py
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1713 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-28 04:38:29.000000 pyremotechrome-0.1.3/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     3797 2024-05-26 04:51:07.000000 pyremotechrome-0.1.3/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1062 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-28 14:33:31.000000 pyremotechrome-0.1.3/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-28 14:33:31.422877 pyremotechrome-0.1.3/setup.cfg
```

### Comparing `pyremotechrome-0.1.2/LICENSE` & `pyremotechrome-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/PKG-INFO` & `pyremotechrome-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyRemoteChrome
 Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyremotechrome-0.1.2/pyproject.toml` & `pyremotechrome-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Wes-KW", email="dotdotdashdash2024@hotmail.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.1.2/pyremotechrome/__main__.py` & `pyremotechrome-0.1.3/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/config/__init__.py` & `pyremotechrome-0.1.3/pyremotechrome/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/config/config.py` & `pyremotechrome-0.1.3/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.1.3/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/server/manager.py` & `pyremotechrome-0.1.3/pyremotechrome/server/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,18 @@
                     return Result(False, "DENIED_API_ACTION")                
 
                 query.pop("request")
                 query.pop("action")
                 query.pop("session_id")
 
                 for q in query:
-                    query[q] = literal_eval(query[q][0])
+                    try:
+                        query[q] = literal_eval(query[q][0])
+                    except Exception:
+                        query[q] = query[q][0]
 
                 if get_value_in_dict(query, "encoded_url") is not None:
                     query["url"] = atob(query["encoded_url"])
                     query.pop("encoded_url")
 
                 res = func(**query)
                 return Result(True, "" , res)
```

### Comparing `pyremotechrome-0.1.2/pyremotechrome/server/server.py` & `pyremotechrome-0.1.3/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/__init__.py` & `pyremotechrome-0.1.3/pyremotechrome/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/base.py` & `pyremotechrome-0.1.3/pyremotechrome/session/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,17 @@
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
 
         self.display.init_audio(self.service.process.pid)
         self.display.init_ffmpeg(ffmpeg_options)
+
+        width = int(width * self._scale)
+        height = int(height * self._scale)
         self.display.start_capturing(bw, bh, width, height)
 
     # Zoom
     def zoom(self) -> None:
         super().get("chrome://settings/")
         self.execute_script("chrome.settingsPrivate.setDefaultZoom(arguments[0]);", self._scale)
         self.get(self._default_url)
@@ -162,27 +165,18 @@
         """Return window display size"""
         width, height = self.get_window_raw_size()
         return width / self._scale, height / self._scale
 
     def set_window_size(self, width: Numbers, height: Numbers) -> None:
         """DOCSTRING"""
         x, y, bw, bh, _, _ = self.get_current_html_rect()()
-        bwidth = int(width * self._scale + bw)
-        bheight = int(height * self._scale + bh)
-        super().set_window_size(bwidth, bheight)
-        self.display.restart_capturing(x + bw, y + bh, width, height)
-
-    def set_window_position(self, x: Numbers, y: Numbers) -> dict:
-        """DOCSTRING"""
-        _, _, bw, bh, width, height = self.get_current_html_rect()()
-        x = int(x * self._scale)
-        y = int(y * self._scale)
-        res = super().set_window_position(x, y)
+        width = int(width * self._scale)
+        height = int(height * self._scale)
+        super().set_window_size(width, height)
         self.display.restart_capturing(x + bw, y + bh, width, height)
-        return res
 
     # Window handle
     def get_current_window(self) -> str:
         """Return current window handle"""
         curr_handle = self.current_window_handle
         if curr_handle not in self.window_handles:
             return ""
```

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/mega.py` & `pyremotechrome-0.1.3/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.1.3/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/common/__init__.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/common/result.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/common/result.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/options/__init__.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/session/support/options/ffmpeg.py` & `pyremotechrome-0.1.3/pyremotechrome/session/support/options/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome/util.py` & `pyremotechrome-0.1.3/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.2/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.1.3/pyremotechrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyRemoteChrome
 Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyremotechrome-0.1.2/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.1.3/pyremotechrome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

