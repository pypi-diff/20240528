# Comparing `tmp/pyvmo-0.0.4.tar.gz` & `tmp/pyvmo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvmo-0.0.4.tar", last modified: Mon May 27 21:32:31 2024, max compression
+gzip compressed data, was "pyvmo-0.0.5.tar", last modified: Tue May 28 15:54:21 2024, max compression
```

## Comparing `pyvmo-0.0.4.tar` & `pyvmo-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-21 19:42:01.000000 pyvmo-0.0.4/LICENSE
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-21 19:42:01.000000 pyvmo-0.0.4/MANIFEST.in
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-27 21:32:31.000000 pyvmo-0.0.4/PKG-INFO
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2320 2024-05-27 21:30:06.000000 pyvmo-0.0.4/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      360 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       41 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/entry_points.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        6 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyVMO.egg-info/top_level.txt
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyvmo/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       26 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/__init__.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     5665 2024-05-21 21:34:47.000000 pyvmo-0.0.4/pyvmo/cli.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-27 21:32:31.000000 pyvmo-0.0.4/pyvmo/distance/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       91 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/distance/__init__.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     9662 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/distance/ibs.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7257 2024-05-27 21:25:34.000000 pyvmo-0.0.4/pyvmo/format.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7007 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/operation.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      917 2024-05-27 21:03:17.000000 pyvmo-0.0.4/pyvmo/versions.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     3372 2024-05-21 19:42:01.000000 pyvmo-0.0.4/pyvmo/vmo.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-27 21:32:31.000000 pyvmo-0.0.4/setup.cfg
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      803 2024-05-21 21:06:24.000000 pyvmo-0.0.4/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-28 15:54:21.000000 pyvmo-0.0.5/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-21 19:42:01.000000 pyvmo-0.0.5/LICENSE
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-21 19:42:01.000000 pyvmo-0.0.5/MANIFEST.in
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-28 15:54:21.000000 pyvmo-0.0.5/PKG-INFO
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2320 2024-05-27 21:30:06.000000 pyvmo-0.0.5/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2742 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      360 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       41 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/entry_points.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        6 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyVMO.egg-info/top_level.txt
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyvmo/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       26 2024-05-21 19:42:01.000000 pyvmo-0.0.5/pyvmo/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     5656 2024-05-28 15:46:57.000000 pyvmo-0.0.5/pyvmo/cli.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-28 15:54:21.000000 pyvmo-0.0.5/pyvmo/distance/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       91 2024-05-21 19:42:01.000000 pyvmo-0.0.5/pyvmo/distance/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     9662 2024-05-21 19:42:01.000000 pyvmo-0.0.5/pyvmo/distance/ibs.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7263 2024-05-28 02:23:04.000000 pyvmo-0.0.5/pyvmo/format.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     7007 2024-05-21 19:42:01.000000 pyvmo-0.0.5/pyvmo/operation.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1108 2024-05-28 02:24:28.000000 pyvmo-0.0.5/pyvmo/versions.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     3372 2024-05-21 19:42:01.000000 pyvmo-0.0.5/pyvmo/vmo.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-28 15:54:21.000000 pyvmo-0.0.5/setup.cfg
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      803 2024-05-21 21:06:24.000000 pyvmo-0.0.5/setup.py
```

### Comparing `pyvmo-0.0.4/LICENSE` & `pyvmo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvmo-0.0.4/PKG-INFO` & `pyvmo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVMO
-Version: 0.0.4
+Version: 0.0.5
 Summary: A test python toolkit for variant site analysis
 Home-page: https://github.com/SouthernCD/pyVMO
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyvmo-0.0.4/README.md` & `pyvmo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyvmo-0.0.4/pyVMO.egg-info/PKG-INFO` & `pyvmo-0.0.5/pyVMO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVMO
-Version: 0.0.4
+Version: 0.0.5
 Summary: A test python toolkit for variant site analysis
 Home-page: https://github.com/SouthernCD/pyVMO
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyvmo-0.0.4/pyvmo/cli.py` & `pyvmo-0.0.5/pyvmo/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     vmo = VMO(args.input_vmo_path)
 
     # load sample list
     sample_id_list = [line.strip() for line in open(args.sample_id_list_file)]
     
     # extract by sample list
     spl_idx_list = vmo.get_samples_index(sample_id_list)
-    spl_vmo_path = args.output_vmo_path + "_spl"
+    spl_vmo_path = args.output_vmo_path
     spl_vmo = vmo.extract_sub_vmo(spl_vmo_path, spl_idx_list=spl_idx_list)
 
     # extract by variant site quality control
     var_idx_list = spl_vmo.site_filter(maf_thr=args.maf_thr, mis_thr=args.mis_thr, chunk_size=args.chunk_size, n_jobs=args.n_jobs)
     var_vmo_path = args.output_vmo_path
     var_vmo = spl_vmo.extract_sub_vmo(var_vmo_path, var_idx_list=var_idx_list)
```

### Comparing `pyvmo-0.0.4/pyvmo/distance/ibs.py` & `pyvmo-0.0.5/pyvmo/distance/ibs.py`

 * *Files identical despite different names*

### Comparing `pyvmo-0.0.4/pyvmo/format.py` & `pyvmo-0.0.5/pyvmo/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 
                 variant_dict = {
                     'CHROM': variant.CHROM,
                     'POS': variant.POS,
                     'ID': variant.ID,
                     'REF': variant.REF,
                     'ALT': pickle_dump_obj(variant.ALT),
-                    'QUAL': pickle_dump_obj(variant.QUAL),
-                    'FILTER': pickle_dump_obj(variant.FILTERS),
-                    'INFO': pickle_dump_obj(dict(variant.INFO))
+                    # 'QUAL': pickle_dump_obj(variant.QUAL),
+                    # 'FILTER': pickle_dump_obj(variant.FILTERS),
+                    # 'INFO': pickle_dump_obj(dict(variant.INFO))
                 }                
 
                 variants_list.append(variant_dict)                
 
                 num += 1
                 if num % 100000 == 0:
                     logger_handle.write("%s: read %d/%d variants (%.2f%%)\n" % (time.strftime(
```

### Comparing `pyvmo-0.0.4/pyvmo/operation.py` & `pyvmo-0.0.5/pyvmo/operation.py`

 * *Files identical despite different names*

### Comparing `pyvmo-0.0.4/pyvmo/versions.py` & `pyvmo-0.0.5/pyvmo/versions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 def get_versions():
     return versions[0]["number"]
 
 
 versions = [
     {
+        "number": "0.0.5",
+        "features": [
+            "1. remove QUAL, FILTER and INFO from vmo, because it is too big and not necessary to store them in vmo",
+        ],
+    },
+    {
         "number": "0.0.4",
         "features": [
             "1. Add stores QUAL, FILTER and INFO to vmo",
         ],
     },
     {
         "number": "0.0.3",
```

### Comparing `pyvmo-0.0.4/pyvmo/vmo.py` & `pyvmo-0.0.5/pyvmo/vmo.py`

 * *Files identical despite different names*

### Comparing `pyvmo-0.0.4/setup.py` & `pyvmo-0.0.5/setup.py`

 * *Files identical despite different names*

