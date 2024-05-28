# Comparing `tmp/pyobjc-framework-MediaPlayer-9.1b1.tar.gz` & `tmp/pyobjc-framework-MediaPlayer-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MediaPlayer-9.1b1.tar", last modified: Sun Mar 26 11:28:57 2023, max compression
+gzip compressed data, was "pyobjc-framework-MediaPlayer-9.2.tar", last modified: Wed Jun  7 00:19:31 2023, max compression
```

## Comparing `pyobjc-framework-MediaPlayer-9.1b1.tar` & `pyobjc-framework-MediaPlayer-9.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.875865 pyobjc-framework-MediaPlayer-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.831353 pyobjc-framework-MediaPlayer-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.835480 pyobjc-framework-MediaPlayer-9.1b1/Lib/MediaPlayer/
--rw-r--r--   0 ronald     (501) staff       (20)      713 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/MediaPlayer/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    23966 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/MediaPlayer/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.838628 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-03-26 11:28:57.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1192 2023-03-26 11:28:57.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:57.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:19.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       56 2023-03-26 11:28:57.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:28:57.000000 pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaPlayer-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-03-26 11:28:57.875383 pyobjc-framework-MediaPlayer-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.850113 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mediaplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      772 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpcontentitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      826 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mperror.py
--rw-r--r--   0 ronald     (501) staff       (20)      548 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpmediaentity.py
--rw-r--r--   0 ronald     (501) staff       (20)     4962 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpmediaitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     3346 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpnowplayinginfocenter.py
--rw-r--r--   0 ronald     (501) staff       (20)     2281 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpnowplayinginfolanguageoption.py
--rw-r--r--   0 ronald     (501) staff       (20)     1246 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecommand.py
--rw-r--r--   0 ronald     (501) staff       (20)      798 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecommandevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      995 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecontroltypes.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.851437 pyobjc-framework-MediaPlayer-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    13628 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/MediaPlayer.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:57.873359 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   136422 2021-07-30 09:00:38.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   137333 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   141807 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   141812 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65951 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   135760 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   136423 2021-07-30 09:00:38.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   137334 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   141808 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   141813 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaPlayer-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:57.875976 pyobjc-framework-MediaPlayer-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      703 2023-03-25 14:20:31.000000 pyobjc-framework-MediaPlayer-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.081133 pyobjc-framework-MediaPlayer-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.021593 pyobjc-framework-MediaPlayer-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.027070 pyobjc-framework-MediaPlayer-9.2/Lib/MediaPlayer/
+-rw-r--r--   0 ronald     (501) staff       (20)      713 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.2/Lib/MediaPlayer/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23966 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.2/Lib/MediaPlayer/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.033960 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-06-07 00:19:31.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1207 2023-06-07 00:19:31.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:30.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:19.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2023-06-07 00:19:30.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:19:30.000000 pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MediaPlayer-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-06-07 00:19:31.080748 pyobjc-framework-MediaPlayer-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.042451 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mediaplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      772 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpcontentitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      826 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mperror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      548 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpmediaentity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4962 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpmediaitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3346 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpnowplayinginfocenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2281 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpnowplayinginfolanguageoption.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1246 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecommand.py
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecommandevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      995 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecontroltypes.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.043843 pyobjc-framework-MediaPlayer-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    13628 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.2/metadata/MediaPlayer.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:31.078411 pyobjc-framework-MediaPlayer-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   136422 2021-07-30 09:00:38.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   137333 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   141807 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   141812 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65951 2020-11-30 18:45:15.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   135760 2021-03-21 10:08:23.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   136423 2021-07-30 09:00:38.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   137334 2022-02-24 08:47:16.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   141808 2022-06-15 11:57:00.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   141813 2023-02-19 10:50:35.000000 pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MediaPlayer-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MediaPlayer-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:31.081254 pyobjc-framework-MediaPlayer-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2023-05-29 10:07:46.000000 pyobjc-framework-MediaPlayer-9.2/setup.py
```

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/Lib/MediaPlayer/__init__.py` & `pyobjc-framework-MediaPlayer-9.2/Lib/MediaPlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/Lib/MediaPlayer/_metadata.py` & `pyobjc-framework-MediaPlayer-9.2/Lib/MediaPlayer/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/PKG-INFO` & `pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaPlayer
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaPlayer on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaPlayer
 Platform: MacOS X (>=10.12)
```

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/Lib/pyobjc_framework_MediaPlayer.egg-info/SOURCES.txt` & `pyobjc-framework-MediaPlayer-9.2/Lib/pyobjc_framework_MediaPlayer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MediaPlayer/__init__.py
 Lib/MediaPlayer/_metadata.py
 Lib/pyobjc_framework_MediaPlayer.egg-info/PKG-INFO
 Lib/pyobjc_framework_MediaPlayer.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MediaPlayer.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MediaPlayer.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/License.txt` & `pyobjc-framework-MediaPlayer-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PKG-INFO` & `pyobjc-framework-MediaPlayer-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MediaPlayer
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MediaPlayer on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MediaPlayer
 Platform: MacOS X (>=10.12)
```

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpcontentitem.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpcontentitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mperror.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mperror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpmediaentity.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpmediaentity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpmediaitem.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpmediaitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpnowplayinginfocenter.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpnowplayinginfocenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpnowplayinginfolanguageoption.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpnowplayinginfolanguageoption.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecommand.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecommand.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecommandevent.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecommandevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/PyObjCTest/test_mpremotecontroltypes.py` & `pyobjc-framework-MediaPlayer-9.2/PyObjCTest/test_mpremotecontroltypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/MediaPlayer.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/MediaPlayer.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-MediaPlayer-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MediaPlayer-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MediaPlayer-9.1b1/setup.py` & `pyobjc-framework-MediaPlayer-9.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "MediaPlayer" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MediaPlayer",
     description="Wrappers for the framework MediaPlayer on macOS",
     min_os_level="10.12",
     packages=["MediaPlayer"],
     version=VERSION,
```

