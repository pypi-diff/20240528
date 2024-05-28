# Comparing `tmp/rtpsynth-1.0.tar.gz` & `tmp/rtpsynth-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtpsynth-1.0.tar", last modified: Tue Apr 23 21:40:20 2024, max compression
+gzip compressed data, was "rtpsynth-1.1.tar", last modified: Tue May 28 04:11:35 2024, max compression
```

## Comparing `rtpsynth-1.0.tar` & `rtpsynth-1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.064748 rtpsynth-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-23 21:40:11.000000 rtpsynth-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 21:40:11.000000 rtpsynth-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-23 21:40:20.064748 rtpsynth-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 21:40:11.000000 rtpsynth-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.060748 rtpsynth-1.0/python/
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-23 21:40:11.000000 rtpsynth-1.0/python/RtpJBuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-23 21:40:11.000000 rtpsynth-1.0/python/RtpSynth.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:11.000000 rtpsynth-1.0/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-23 21:40:11.000000 rtpsynth-1.0/python/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.064748 rtpsynth-1.0/rtpsynth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-23 21:40:20.000000 rtpsynth-1.0/rtpsynth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 21:40:20.000000 rtpsynth-1.0/rtpsynth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:40:20.000000 rtpsynth-1.0/rtpsynth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 21:40:20.000000 rtpsynth-1.0/rtpsynth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.060748 rtpsynth-1.0/setup/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 21:40:11.000000 rtpsynth-1.0/setup/RunCTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:11.000000 rtpsynth-1.0/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:40:20.064748 rtpsynth-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-23 21:40:11.000000 rtpsynth-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.064748 rtpsynth-1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/Symbol.map
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rsth_timeops.h
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtp.c
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtp_info.h
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtpjbuf.c
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtpjbuf.h
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtpsynth.c
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-23 21:40:11.000000 rtpsynth-1.0/src/rtpsynth.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:40:20.064748 rtpsynth-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-23 21:40:11.000000 rtpsynth-1.0/tests/test_jbuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.196154 rtpsynth-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-28 04:11:24.000000 rtpsynth-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 04:11:24.000000 rtpsynth-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-28 04:11:35.196154 rtpsynth-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-28 04:11:24.000000 rtpsynth-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.192155 rtpsynth-1.1/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-28 04:11:24.000000 rtpsynth-1.1/python/RtpJBuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-28 04:11:24.000000 rtpsynth-1.1/python/RtpSynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:24.000000 rtpsynth-1.1/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-28 04:11:24.000000 rtpsynth-1.1/python/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.196154 rtpsynth-1.1/rtpsynth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-28 04:11:35.000000 rtpsynth-1.1/rtpsynth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 04:11:35.000000 rtpsynth-1.1/rtpsynth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:11:35.000000 rtpsynth-1.1/rtpsynth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 04:11:35.000000 rtpsynth-1.1/rtpsynth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.192155 rtpsynth-1.1/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-28 04:11:24.000000 rtpsynth-1.1/setup/RunCTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:24.000000 rtpsynth-1.1/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:11:35.196154 rtpsynth-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-28 04:11:24.000000 rtpsynth-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.196154 rtpsynth-1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/Symbol.map
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rsth_timeops.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtp_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtpjbuf.c
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtpjbuf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtpsynth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-28 04:11:24.000000 rtpsynth-1.1/src/rtpsynth.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:11:35.196154 rtpsynth-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-28 04:11:24.000000 rtpsynth-1.1/tests/test_jbuf.py
```

### Comparing `rtpsynth-1.0/LICENSE` & `rtpsynth-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/PKG-INFO` & `rtpsynth-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtpsynth
-Version: 1.0
+Version: 1.1
 Summary: Library optimized to generate/process sequence of the RTP packets
 Home-page: https://github.com/sippy/librtpsynth.git
 Author: Maksym Sobolyev
 Author-email: sobomax@gmail.com
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
```

### Comparing `rtpsynth-1.0/README.md` & `rtpsynth-1.1/README.md`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/python/RtpJBuf.py` & `rtpsynth-1.1/python/RtpJBuf.py`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/python/RtpSynth.py` & `rtpsynth-1.1/python/RtpSynth.py`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/python/env.py` & `rtpsynth-1.1/python/env.py`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/rtpsynth.egg-info/PKG-INFO` & `rtpsynth-1.1/rtpsynth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtpsynth
-Version: 1.0
+Version: 1.1
 Summary: Library optimized to generate/process sequence of the RTP packets
 Home-page: https://github.com/sippy/librtpsynth.git
 Author: Maksym Sobolyev
 Author-email: sobomax@gmail.com
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
```

### Comparing `rtpsynth-1.0/setup/RunCTest.py` & `rtpsynth-1.1/setup/RunCTest.py`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/setup.py` & `rtpsynth-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import os
 
 from distutils.core import setup
 from distutils.core import Extension
+from sysconfig import get_platform
 
 from python.env import RSTH_MOD_NAME
 from setup.RunCTest import RunCTest
 
 rs_srcs = ['src/rtpsynth.c', 'src/rtp.c', 'src/rtpjbuf.c']
 
 extra_compile_args = ['--std=c11', '-Wno-zero-length-array', '-Wall', '-pedantic', '-flto']
@@ -24,26 +25,27 @@
 module1 = Extension(RSTH_MOD_NAME, sources = rs_srcs, \
     extra_link_args = extra_link_args, \
     extra_compile_args = extra_compile_args)
 
 RunCTest.extra_link_args = extra_link_args.copy()
 RunCTest.extra_compile_args = extra_compile_args
 
-extra_link_args.append('-Wl,--version-script=src/Symbol.map')
+if not get_platform().startswith('macosx-'):
+    extra_link_args.append('-Wl,--version-script=src/Symbol.map')
 
 def get_ex_mod():
     if 'NO_PY_EXT' in os.environ:
         return None
     return [module1]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 kwargs = {'name':'rtpsynth',
-      'version':'1.0',
+      'version':'1.1',
       'description':'Library optimized to generate/process sequence of the RTP packets',
       'long_description': long_description,
       'long_description_content_type': "text/markdown",
       'author':'Maksym Sobolyev',
       'author_email':'sobomax@gmail.com',
       'url':'https://github.com/sippy/librtpsynth.git',
       'packages':['rtpsynth',],
```

### Comparing `rtpsynth-1.0/src/rsth_timeops.h` & `rtpsynth-1.1/src/rsth_timeops.h`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtp.c` & `rtpsynth-1.1/src/rtp.c`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtp.h` & `rtpsynth-1.1/src/rtp.h`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtp_info.h` & `rtpsynth-1.1/src/rtp_info.h`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtpjbuf.c` & `rtpsynth-1.1/src/rtpjbuf.c`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtpjbuf.h` & `rtpsynth-1.1/src/rtpjbuf.h`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtpsynth.c` & `rtpsynth-1.1/src/rtpsynth.c`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/src/rtpsynth.h` & `rtpsynth-1.1/src/rtpsynth.h`

 * *Files identical despite different names*

### Comparing `rtpsynth-1.0/tests/test_jbuf.py` & `rtpsynth-1.1/tests/test_jbuf.py`

 * *Files identical despite different names*

