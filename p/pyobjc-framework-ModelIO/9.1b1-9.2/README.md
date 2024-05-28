# Comparing `tmp/pyobjc-framework-ModelIO-9.1b1.tar.gz` & `tmp/pyobjc-framework-ModelIO-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ModelIO-9.1b1.tar", last modified: Sun Mar 26 11:30:48 2023, max compression
+gzip compressed data, was "pyobjc-framework-ModelIO-9.2.tar", last modified: Wed Jun  7 00:21:15 2023, max compression
```

## Comparing `pyobjc-framework-ModelIO-9.1b1.tar` & `pyobjc-framework-ModelIO-9.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.172698 pyobjc-framework-ModelIO-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.029926 pyobjc-framework-ModelIO-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.041028 pyobjc-framework-ModelIO-9.1b1/Lib/ModelIO/
--rw-r--r--   0 ronald     (501) staff       (20)      712 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.1b1/Lib/ModelIO/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    75658 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.1b1/Lib/ModelIO/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.061820 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-03-26 11:30:48.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1237 2023-03-26 11:30:48.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:30:47.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:20.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:30:47.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:30:47.000000 pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ModelIO-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.078297 pyobjc-framework-ModelIO-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-ModelIO-9.1b1/Modules/_ModelIO.m
--rw-r--r--   0 ronald     (501) staff       (20)      996 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.1b1/Modules/_ModelIO_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-ModelIO-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-02-19 12:24:44.000000 pyobjc-framework-ModelIO-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2023-03-26 11:30:48.171806 pyobjc-framework-ModelIO-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.144074 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    24522 2022-10-21 10:39:50.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlanimatedvaluetypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      638 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2545 2022-10-21 10:39:50.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlasset.py
--rw-r--r--   0 ronald     (501) staff       (20)      480 2022-06-25 20:08:24.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlassetresolver.py
--rw-r--r--   0 ronald     (501) staff       (20)     3461 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlcamera.py
--rw-r--r--   0 ronald     (501) staff       (20)     1575 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdllight.py
--rw-r--r--   0 ronald     (501) staff       (20)     6287 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmaterial.py
--rw-r--r--   0 ronald     (501) staff       (20)     9314 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmesh.py
--rw-r--r--   0 ronald     (501) staff       (20)     2756 2022-06-25 09:19:13.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmeshbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      789 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlobject.py
--rw-r--r--   0 ronald     (501) staff       (20)      862 2022-06-25 20:05:09.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlprimitive.py
--rw-r--r--   0 ronald     (501) staff       (20)     5324 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltexture.py
--rw-r--r--   0 ronald     (501) staff       (20)     5752 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     1631 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltransformstack.py
--rw-r--r--   0 ronald     (501) staff       (20)     2935 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1949 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvaluetypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     9053 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvertexdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     3271 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvoxelarray.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_modelio.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.146390 pyobjc-framework-ModelIO-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    42683 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.1b1/metadata/ModelIO.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:48.168793 pyobjc-framework-ModelIO-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   298319 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   298320 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ModelIO-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:30:48.172854 pyobjc-framework-ModelIO-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1190 2023-03-25 14:20:32.000000 pyobjc-framework-ModelIO-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.725213 pyobjc-framework-ModelIO-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.665036 pyobjc-framework-ModelIO-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.671918 pyobjc-framework-ModelIO-9.2/Lib/ModelIO/
+-rw-r--r--   0 ronald     (501) staff       (20)      712 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.2/Lib/ModelIO/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    75658 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.2/Lib/ModelIO/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.676890 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-06-07 00:21:15.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1252 2023-06-07 00:21:15.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:21:15.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:20.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:21:15.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:21:15.000000 pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ModelIO-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.679629 pyobjc-framework-ModelIO-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-ModelIO-9.2/Modules/_ModelIO.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1036 2023-05-04 11:00:07.000000 pyobjc-framework-ModelIO-9.2/Modules/_ModelIO_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-ModelIO-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-05-29 07:18:42.000000 pyobjc-framework-ModelIO-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:21:15.724801 pyobjc-framework-ModelIO-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.717809 pyobjc-framework-ModelIO-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24522 2022-10-21 10:39:50.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlanimatedvaluetypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      638 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2588 2023-05-04 11:00:07.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlasset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      480 2022-06-25 20:08:24.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlassetresolver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3461 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlcamera.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1575 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdllight.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6287 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmaterial.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9314 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmesh.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2756 2022-06-25 09:19:13.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmeshbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      862 2022-06-25 20:05:09.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlprimitive.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5322 2023-05-04 11:00:07.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5751 2023-05-04 11:00:07.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1631 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltransformstack.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2897 2023-05-04 11:00:07.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1949 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvaluetypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9053 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvertexdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3271 2022-10-21 10:39:51.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvoxelarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-ModelIO-9.2/PyObjCTest/test_modelio.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.719753 pyobjc-framework-ModelIO-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    42683 2022-10-20 21:08:30.000000 pyobjc-framework-ModelIO-9.2/metadata/ModelIO.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-ModelIO-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:21:15.722701 pyobjc-framework-ModelIO-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   298319 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   298320 2022-10-18 09:53:23.000000 pyobjc-framework-ModelIO-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ModelIO-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ModelIO-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:21:15.725329 pyobjc-framework-ModelIO-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1261 2023-05-29 10:07:46.000000 pyobjc-framework-ModelIO-9.2/setup.py
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/Lib/ModelIO/__init__.py` & `pyobjc-framework-ModelIO-9.2/Lib/ModelIO/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/Lib/ModelIO/_metadata.py` & `pyobjc-framework-ModelIO-9.2/Lib/ModelIO/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/PKG-INFO` & `pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ModelIO
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ModelIO on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ModelIO
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/Lib/pyobjc_framework_ModelIO.egg-info/SOURCES.txt` & `pyobjc-framework-ModelIO-9.2/Lib/pyobjc_framework_ModelIO.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ModelIO/__init__.py
 Lib/ModelIO/_metadata.py
 Lib/pyobjc_framework_ModelIO.egg-info/PKG-INFO
 Lib/pyobjc_framework_ModelIO.egg-info/SOURCES.txt
 Lib/pyobjc_framework_ModelIO.egg-info/dependency_links.txt
 Lib/pyobjc_framework_ModelIO.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/License.txt` & `pyobjc-framework-ModelIO-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/Modules/_ModelIO.m` & `pyobjc-framework-ModelIO-9.2/Modules/_ModelIO.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/Modules/_ModelIO_protocols.m` & `pyobjc-framework-ModelIO-9.2/Modules/_ModelIO_protocols.m`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 static void __attribute__((__used__)) use_protocols(void)
 {
     PyObject* p __attribute__((__unused__));
     p = PyObjC_IdToPython(@protocol(MDLComponent));
     Py_XDECREF(p);
-    p = PyObjC_IdToPython(@protocol(MDLLightProbeIrradianceDataSource));
-    Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLMeshBuffer));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLMeshBufferAllocator));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLMeshBufferZone));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLNamed));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLObjectContainerComponent));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLTransformComponent));
     Py_XDECREF(p);
+#if PyObjC_BUILD_RELEASE >= 1012
+    p = PyObjC_IdToPython(@protocol(MDLLightProbeIrradianceDataSource));
+    Py_XDECREF(p);
+#endif
 #if PyObjC_BUILD_RELEASE >= 1013
     p = PyObjC_IdToPython(@protocol(MDLAssetResolver));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLJointAnimation));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MDLTransformOp));
     Py_XDECREF(p);
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ModelIO-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ModelIO-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PKG-INFO` & `pyobjc-framework-ModelIO-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ModelIO
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ModelIO on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ModelIO
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlanimatedvaluetypes.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlanimatedvaluetypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlanimation.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlasset.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlasset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase, min_os_level
+from PyObjCTools.TestSupport import TestCase, min_os_level, min_sdk_level
 import objc
 import ModelIO
 from objc import simd
 
 
 class TestMDLAssetHelper(ModelIO.NSObject):
     def sphericalHarmonicsLevel(self):
@@ -75,9 +75,10 @@
         self.assertResultHasType(
             ModelIO.MDLAsset.upAxis, simd.vector_float3.__typestr__
         )
         self.assertArgHasType(
             ModelIO.MDLAsset.setUpAxis_, 0, simd.vector_float3.__typestr__
         )
 
+    @min_sdk_level("10.12")
     def testProtocolObjects(self):
         self.assertProtocolExists("MDLLightProbeIrradianceDataSource")
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlcamera.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlcamera.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdllight.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdllight.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmaterial.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmaterial.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmesh.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmesh.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlmeshbuffer.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlmeshbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlobject.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlprimitive.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlprimitive.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltexture.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltexture.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,20 +60,14 @@
             simd.vector_int2.__typestr__,
         )
         self.assertArgIsBOOL(
             ModelIO.MDLNoiseTexture.initScalarNoiseWithSmoothness_name_textureDimensions_channelCount_channelEncoding_grayscale_,
             5,
         )
 
-        self.assertArgHasType(
-            ModelIO.MDLNoiseTexture.initCellularNoiseWithFrequency_name_textureDimensions_channelEncoding_,
-            2,
-            simd.vector_int2.__typestr__,
-        )
-
         self.assertResultHasType(
             ModelIO.MDLTexture.dimensions, simd.vector_int2.__typestr__
         )
 
         self.assertArgHasType(
             ModelIO.MDLTexture.irradianceTextureCubeWithTexture_name_dimensions_,
             2,
@@ -87,25 +81,14 @@
 
         self.assertArgHasType(
             ModelIO.MDLCheckerboardTexture.initWithDivisions_name_dimensions_channelCount_channelEncoding_color1_color2_,
             2,
             simd.vector_int2.__typestr__,
         )
 
-        self.assertArgHasType(
-            ModelIO.MDLSkyCubeTexture.initWithName_channelEncoding_textureDimensions_turbidity_sunElevation_upperAtmosphereScattering_groundAlbedo_,
-            2,
-            simd.vector_int2.__typestr__,
-        )
-        self.assertArgHasType(
-            ModelIO.MDLSkyCubeTexture.initWithName_channelEncoding_textureDimensions_turbidity_sunElevation_sunAzimuth_upperAtmosphereScattering_groundAlbedo_,
-            2,
-            simd.vector_int2.__typestr__,
-        )
-
         self.assertResultHasType(
             ModelIO.MDLSkyCubeTexture.highDynamicRangeCompression,
             simd.vector_float2.__typestr__,
         )
         self.assertArgHasType(
             ModelIO.MDLSkyCubeTexture.setHighDynamicRangeCompression_,
             0,
@@ -126,9 +109,24 @@
     @min_os_level("10.12")
     def testMethods10_12(self):
         self.assertResultIsBOOL(ModelIO.MDLTexture.hasAlphaValues)
         self.assertArgIsBOOL(ModelIO.MDLTexture.setHasAlphaValues_, 0)
 
     @min_os_level("10.13")
     def testMethods10_13(self):
+        self.assertArgHasType(
+            ModelIO.MDLSkyCubeTexture.initWithName_channelEncoding_textureDimensions_turbidity_sunElevation_upperAtmosphereScattering_groundAlbedo_,
+            2,
+            simd.vector_int2.__typestr__,
+        )
+        self.assertArgHasType(
+            ModelIO.MDLSkyCubeTexture.initWithName_channelEncoding_textureDimensions_turbidity_sunElevation_sunAzimuth_upperAtmosphereScattering_groundAlbedo_,
+            2,
+            simd.vector_int2.__typestr__,
+        )
+        self.assertArgHasType(
+            ModelIO.MDLNoiseTexture.initCellularNoiseWithFrequency_name_textureDimensions_channelEncoding_,
+            2,
+            simd.vector_int2.__typestr__,
+        )
         self.assertResultIsBOOL(ModelIO.MDLTexture.writeToURL_level_)
         self.assertResultIsBOOL(ModelIO.MDLTexture.writeToURL_type_level_)
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltransform.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltransform.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,38 +103,28 @@
             objc._C_DBL,
         )
 
         self.assertArgHasType(
             ModelIO.MDLTransform.initWithMatrix_, 0, simd.matrix_float4x4.__typestr__
         )
 
-        self.assertArgHasType(
-            ModelIO.MDLTransform.initWithMatrix_resetsTransform_,
-            0,
-            simd.matrix_float4x4.__typestr__,
-        )
-        self.assertArgIsBOOL(ModelIO.MDLTransform.initWithMatrix_resetsTransform_, 1)
-
         self.assertResultHasType(
             ModelIO.MDLTransform.translationAtTime_, simd.vector_float3.__typestr__
         )
         self.assertResultHasType(
             ModelIO.MDLTransform.rotationAtTime_, simd.vector_float3.__typestr__
         )
         self.assertResultHasType(
             ModelIO.MDLTransform.shearAtTime_, simd.vector_float3.__typestr__
         )
         self.assertResultHasType(
             ModelIO.MDLTransform.scaleAtTime_, simd.vector_float3.__typestr__
         )
 
         self.assertArgHasType(
-            ModelIO.MDLTransform.setMatrix_forTime_, 0, simd.matrix_float4x4.__typestr__
-        )
-        self.assertArgHasType(
             ModelIO.MDLTransform.setTranslation_forTime_,
             0,
             simd.vector_float3.__typestr__,
         )
         self.assertArgHasType(
             ModelIO.MDLTransform.setRotation_forTime_, 0, simd.vector_float3.__typestr__
         )
@@ -173,13 +163,22 @@
         )
         self.assertArgHasType(
             ModelIO.MDLTransform.setScale_, 0, simd.vector_float3.__typestr__
         )
 
     @min_os_level("10.12")
     def testMethods10_12(self):
+        self.assertArgHasType(
+            ModelIO.MDLTransform.initWithMatrix_resetsTransform_,
+            0,
+            simd.matrix_float4x4.__typestr__,
+        )
+        self.assertArgHasType(
+            ModelIO.MDLTransform.setMatrix_forTime_, 0, simd.matrix_float4x4.__typestr__
+        )
+        self.assertArgIsBOOL(ModelIO.MDLTransform.initWithMatrix_resetsTransform_, 1)
         self.assertArgIsBOOL(
             ModelIO.MDLTransform.initWithTransformComponent_resetsTransform_, 1
         )
 
     def testProtocolObjects(self):
         self.assertProtocolExists("MDLTransformComponent")
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltransformstack.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltransformstack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdltypes.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdltypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase, min_os_level, expectedFailure
+from PyObjCTools.TestSupport import TestCase, min_os_level
 import objc
 import ModelIO
 
 
 class TestMDLTypesHelper(ModelIO.NSObject):
     def objectAtIndexedSubscript_(self, i):
         return 1
@@ -58,15 +58,14 @@
         self.assertProtocolExists("MDLObjectContainerComponent")
 
     def testMethods(self):
         self.assertArgHasType(
             TestMDLTypesHelper.objectAtIndexedSubscript_, 0, objc._C_NSUInteger
         )
 
-    @expectedFailure
     def testStructs(self):
         self.assertEqual(
             ModelIO.MDLAxisAlignedBoundingBox.__typestr__,
             b"{_MDLAxisAlignedBoundingBox=<3f><3f>}",
         )
         v = ModelIO.MDLAxisAlignedBoundingBox()
         self.assertIs(v.maxBounds, None)
```

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvaluetypes.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvaluetypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvertexdescriptor.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvertexdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/PyObjCTest/test_mdlvoxelarray.py` & `pyobjc-framework-ModelIO-9.2/PyObjCTest/test_mdlvoxelarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/metadata/ModelIO.fwinfo` & `pyobjc-framework-ModelIO-9.2/metadata/ModelIO.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-ModelIO-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-ModelIO-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ModelIO-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ModelIO-9.1b1/setup.py` & `pyobjc-framework-ModelIO-9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-ModelIO",
     description="Wrappers for the framework ModelIO on macOS",
     min_os_level="10.11",
     packages=["ModelIO"],
     ext_modules=[
```

