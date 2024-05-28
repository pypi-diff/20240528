# Comparing `tmp/monisha-0.0.76.tar.gz` & `tmp/monisha-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.76.tar", last modified: Sat May 25 16:09:19 2024, max compression
+gzip compressed data, was "monisha-0.0.77.tar", last modified: Tue May 28 03:24:18 2024, max compression
```

## Comparing `monisha-0.0.76.tar` & `monisha-0.0.77.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:19.029308 monisha-0.0.76/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-25 16:09:06.000000 monisha-0.0.76/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:19.021308 monisha-0.0.76/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:19.025308 monisha-0.0.76/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/functions/function20.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:19.025308 monisha-0.0.76/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-25 16:09:06.000000 monisha-0.0.76/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-25 16:09:19.025308 monisha-0.0.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-25 16:09:06.000000 monisha-0.0.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:19.025308 monisha-0.0.76/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-25 16:09:19.000000 monisha-0.0.76/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-25 16:09:19.000000 monisha-0.0.76/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:09:19.000000 monisha-0.0.76/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 16:09:19.000000 monisha-0.0.76/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 16:09:19.000000 monisha-0.0.76/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:09:19.029308 monisha-0.0.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-25 16:09:06.000000 monisha-0.0.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:24:18.152899 monisha-0.0.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-28 03:24:13.000000 monisha-0.0.77/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:24:18.144899 monisha-0.0.77/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:24:18.148899 monisha-0.0.77/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/functions/function21.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:24:18.152899 monisha-0.0.77/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 03:24:13.000000 monisha-0.0.77/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 03:24:18.152899 monisha-0.0.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 03:24:13.000000 monisha-0.0.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:24:18.152899 monisha-0.0.77/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 03:24:18.000000 monisha-0.0.77/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-28 03:24:18.000000 monisha-0.0.77/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:24:18.000000 monisha-0.0.77/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 03:24:18.000000 monisha-0.0.77/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 03:24:18.000000 monisha-0.0.77/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:24:18.152899 monisha-0.0.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 03:24:13.000000 monisha-0.0.77/setup.py
```

### Comparing `monisha-0.0.76/LICENSE` & `monisha-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/__init__.py` & `monisha-0.0.77/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.76"
+version = "0.0.77"
 
 install = ["hachoir",
            "requests",
            "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
```

### Comparing `monisha-0.0.76/Monisha/functions/__init__.py` & `monisha-0.0.77/Monisha/functions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from .function01 import timend, uptime, Timemod, Timesod, Timesed
-from .function14 import CDirectory, UDirectory, BDirectory
 from .function06 import Okeys, Ukeys, Bkeys, Mkeys
 from .function02 import Dbytes, Hbytes, Gbytes
 from .function04 import Eimes, Mimeo, Mimes
 from .function03 import progress, Progress
 from .function06 import Skeys, Uname
-from .function07 import Cmd, Wosd
 from .function18 import Metadatas
 from .function15 import Location
 from .function17 import Filename
+from .function07 import commandR
 from .function09 import Storage
+from .function21 import readers
 from .function16 import FMagic
 from .function20 import Money
 from .function10 import Fonts
+from .function14 import Files
 from .function19 import views
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function13 import Guid
 from .function08 import Num
```

### Comparing `monisha-0.0.76/Monisha/functions/function01.py` & `monisha-0.0.77/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function02.py` & `monisha-0.0.77/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function03.py` & `monisha-0.0.77/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function04.py` & `monisha-0.0.77/Monisha/functions/function04.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #============================================================================================================================
 
 class Eimes(object):
 
-    DATA00 = (".DMY", ".TMP")
+    DATA00 = (".ARIA2", ".DMY")
 
     DATA01 = (".TXT", ".PDF", ".APK", ".EXE", ".ZIP", ".RAR", ".TAR", ".ISO")
 
     DATA02 = (".MKV", ".MP4", ".MOV", ".WMV", ".3GP", ".MPG", ".WEBM", ".AVI", ".FLV", ".M4V", ".GIF")
 
     DATA03 = (".MP3", ".M4A", ".M4B", ".FLAC", ".WAV", ".AIF", ".OGG", ".AAC", ".DTS", ".MID", ".AMR", ".MKA")
```

### Comparing `monisha-0.0.76/Monisha/functions/function06.py` & `monisha-0.0.77/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function10.py` & `monisha-0.0.77/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function16.py` & `monisha-0.0.77/Monisha/functions/function16.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-
-class SMessages:
-    def __init__(self, **kwargs):
-        self.types = kwargs.get("types", None)
-        self.error = kwargs.get("types", None)
-
-#====================================================================
+from .collections import SMessage
+#========================================================================
 
 class FMagic:
 
     def get01(file):
         try:
             from magic import Magic
             mimees = Magic(mime=True)
             mimeos = mimees.from_file(file)
             mimemo = mimeos or "text/plain"
-            return SMessages(types=mimemo)
+            return SMessages(filetype=mimemo)
         except Exception as errors:
-            return SMessages(types="application/zip", error=errors)
+            return SMessage(filetype="application/zip", errors=errors)
 
-#====================================================================
+#========================================================================
 
     async def get02(file):
         try:
             from magic import Magic
             mimees = Magic(mime=True)
             mimeos = mimees.from_file(file)
             mimemo = mimeos or "text/plain"
-            return SMessages(types=mimemo)
+            return SMessages(filetype=mimemo)
         except Exception as errors:
-            return SMessages(types="application/zip", error=errors)
+            return SMessage(filetype="application/zip", errors=errors)
 
-#====================================================================
+#========================================================================
```

### Comparing `monisha-0.0.76/Monisha/functions/function17.py` & `monisha-0.0.77/Monisha/functions/function17.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 import os
 import random
 from ..scripts import Scripted
 from urllib.parse import unquote
 from urllib.parse import urlparse
-#=========================================================================
-
-
-class SMessages:
-    def __init__(self, **kwargs):
-        self.errors = kwargs.get("errors", None)
-        self.result = kwargs.get("result", None)
-        self.filename = kwargs.get("filename", None)
-        self.extension = kwargs.get("extension", None)
-
+from .collections import SMessage
 #=========================================================================
 
 class Filename:
 
     async def get01(extension=None):
         mainos = str(random.randint(10000, 100000000000000))
         moonus = mainos + extension if extension else mainos
@@ -26,30 +17,30 @@
 
     async def get02(filename):
         nameas = str(filename)
         finame = os.path.splitext(nameas)[0]
         exexon = os.path.splitext(nameas)[1]
         exoexo = exexon if exexon else Scripted.DATA06
         moonus = finame if finame else Scripted.DATA13
-        return SMessages(filename=moonus, extension=exoexo)
+        return SMessage(filename=moonus, extension=exoexo)
 
 #=========================================================================
 
     async def get03(filelink):
         try:
             findne = urlparse(filelink)
             fnameo = os.path.basename(findne.path)
             moonus = unquote(fnameo)
-            return SMessages(filename=moonus, errors=None)
+            return SMessage(filename=moonus, errors=None)
         except Exception as errors:
-            return SMessages(filename=Scripted.DATA14, errors=errors)
+            return SMessage(filename=Scripted.DATA14, errors=errors)
 
 #=========================================================================
 
     async def get04(location):
         try:
             moonus = str(os.path.basename(location))
-            return SMessages(filename=moonus, errors=None)
+            return SMessage(filename=moonus, errors=None)
         except Exception as errors:
-            return SMessages(filename=Scripted.DATA14, errors=errors)
+            return SMessage(filename=Scripted.DATA14, errors=errors)
 
 #=========================================================================
```

### Comparing `monisha-0.0.76/Monisha/functions/function18.py` & `monisha-0.0.77/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function19.py` & `monisha-0.0.77/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/functions/function20.py` & `monisha-0.0.77/Monisha/functions/function20.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/Monisha/scripts/es.py` & `monisha-0.0.77/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.76/PKG-INFO` & `monisha-0.0.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.76
+Version: 0.0.77
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.76 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.77 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.76/monisha.egg-info/PKG-INFO` & `monisha-0.0.77/monisha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.76
+Version: 0.0.77
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.76 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.77 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.76/monisha.egg-info/SOURCES.txt` & `monisha-0.0.77/monisha.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 Monisha/__init__.py
 Monisha/functions/__init__.py
+Monisha/functions/collections.py
 Monisha/functions/function01.py
 Monisha/functions/function02.py
 Monisha/functions/function03.py
 Monisha/functions/function04.py
 Monisha/functions/function05.py
 Monisha/functions/function06.py
 Monisha/functions/function07.py
@@ -19,14 +20,15 @@
 Monisha/functions/function14.py
 Monisha/functions/function15.py
 Monisha/functions/function16.py
 Monisha/functions/function17.py
 Monisha/functions/function18.py
 Monisha/functions/function19.py
 Monisha/functions/function20.py
+Monisha/functions/function21.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 Monisha/scripts/eu.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
```

### Comparing `monisha-0.0.76/setup.py` & `monisha-0.0.77/setup.py`

 * *Files identical despite different names*

