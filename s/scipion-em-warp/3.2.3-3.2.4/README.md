# Comparing `tmp/scipion-em-warp-3.2.3.tar.gz` & `tmp/scipion-em-warp-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-warp-3.2.3.tar", last modified: Thu Apr 18 12:45:36 2024, max compression
+gzip compressed data, was "scipion-em-warp-3.2.4.tar", last modified: Tue May 28 11:55:07 2024, max compression
```

## Comparing `scipion-em-warp-3.2.3.tar` & `scipion-em-warp-3.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/warp/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/warp/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_mics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_tomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/warp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/test_protocols_tomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/warp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 11:55:07.000000 scipion-em-warp-3.2.4/scipion_em_warp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/warp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_mics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:55:07.254725 scipion-em-warp-3.2.4/warp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/tests/test_protocols_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-05-28 11:54:41.000000 scipion-em-warp-3.2.4/warp/warp_logo.png
```

### Comparing `scipion-em-warp-3.2.3/LICENSE` & `scipion-em-warp-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/PKG-INFO` & `scipion-em-warp-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-warp
-Version: 3.2.3
+Version: 3.2.4
 Summary: Plugin to use Warp within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-warp
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-warp/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-warp/
```

### Comparing `scipion-em-warp-3.2.3/README.rst` & `scipion-em-warp-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/scipion_em_warp.egg-info/PKG-INFO` & `scipion-em-warp-3.2.4/scipion_em_warp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-warp
-Version: 3.2.3
+Version: 3.2.4
 Summary: Plugin to use Warp within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-warp
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-warp/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-warp/
```

### Comparing `scipion-em-warp-3.2.3/scipion_em_warp.egg-info/SOURCES.txt` & `scipion-em-warp-3.2.4/scipion_em_warp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/setup.py` & `scipion-em-warp-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/__init__.py` & `scipion-em-warp-3.2.4/warp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
 
-__version__ = '3.2.3'
+__version__ = '3.2.4'
 _references = ['Nickell2005', 'Tegunov2019']
 _logo = "warp_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-warp"
```

### Comparing `scipion-em-warp-3.2.3/warp/bibtex.py` & `scipion-em-warp-3.2.4/warp/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/protocols/__init__.py` & `scipion-em-warp-3.2.4/warp/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/protocols/protocol_base.py` & `scipion-em-warp-3.2.4/warp/protocols/protocol_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,18 +140,19 @@
             mrcOut.voxel_size = kwargs["angpix"]
             mrcOut.update_header_from_data()
 
     @staticmethod
     def _processStack(inputFn, outputFn, **kwargs):
         ih = ImageHandler()
         x, y, z, n = ih.getDimensions(inputFn)
-        stack_shape = (n, y, x)
+        nImages = max(z, n)  # Just handle ambiguity with mrc format
+        stack_shape = (nImages, y, x)
         mrc = mrcfile.new_mmap(outputFn, shape=stack_shape,
                                mrc_mode=2, overwrite=True)
-        for i in range(n):
+        for i in range(nImages):
             inputData = ih.read((i + 1, inputFn)).getData()
             mrc.data[i] = tom_deconv(inputData, **kwargs)
         mrc.reset_header_stats()
         mrc.update_header_from_data()
         mrc.set_image_stack()
         mrc.voxel_size = kwargs["angpix"]
         mrc.close()
```

### Comparing `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_mics.py` & `scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_tomo.py` & `scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_ts.py` & `scipion-em-warp-3.2.4/warp/protocols/protocol_deconv_ts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/protocols.conf` & `scipion-em-warp-3.2.4/warp/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/tests/__init__.py` & `scipion-em-warp-3.2.4/warp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/tests/test_protocols.py` & `scipion-em-warp-3.2.4/warp/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/tests/test_protocols_tomo.py` & `scipion-em-warp-3.2.4/warp/tests/test_protocols_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/utils.py` & `scipion-em-warp-3.2.4/warp/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.3/warp/warp_logo.png` & `scipion-em-warp-3.2.4/warp/warp_logo.png`

 * *Files identical despite different names*

