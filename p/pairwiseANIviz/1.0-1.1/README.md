# Comparing `tmp/pairwiseANIviz-1.0.tar.gz` & `tmp/pairwiseaniviz-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pairwiseANIviz-1.0.tar", last modified: Sun Oct  8 02:34:16 2023, max compression
+gzip compressed data, was "pairwiseaniviz-1.1.tar", last modified: Tue May 28 00:37:00 2024, max compression
```

## Comparing `pairwiseANIviz-1.0.tar` & `pairwiseaniviz-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-08 02:34:16.085148 pairwiseANIviz-1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1086 2023-10-06 02:58:57.000000 pairwiseANIviz-1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5700 2023-10-08 02:34:16.074571 pairwiseANIviz-1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-10-08 02:31:28.000000 pairwiseANIviz-1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-08 02:34:15.942379 pairwiseANIviz-1.0/pairwiseANIviz/
--rwxrwxrwx   0 root         (0) root         (0)      899 2023-10-08 01:33:57.000000 pairwiseANIviz-1.0/pairwiseANIviz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4333 2023-10-08 01:33:50.000000 pairwiseANIviz-1.0/pairwiseANIviz/get_args.py
--rwxrwxrwx   0 root         (0) root         (0)     5972 2023-10-07 08:48:08.000000 pairwiseANIviz-1.0/pairwiseANIviz/pairwiseANI.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-08 02:34:16.053280 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5700 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       55 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-10-08 02:34:15.000000 pairwiseANIviz-1.0/pairwiseANIviz.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-10-08 02:34:16.086153 pairwiseANIviz-1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      732 2023-10-07 09:01:13.000000 pairwiseANIviz-1.0/setup.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2024-05-28 00:37:00.633377 pairwiseaniviz-1.1/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     1086 2023-10-06 02:58:57.000000 pairwiseaniviz-1.1/LICENSE
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     5700 2024-05-28 00:37:00.623344 pairwiseaniviz-1.1/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     5414 2023-10-08 02:31:28.000000 pairwiseaniviz-1.1/README.md
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2024-05-28 00:37:00.498052 pairwiseaniviz-1.1/pairwiseANIviz/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      899 2023-10-08 01:33:57.000000 pairwiseaniviz-1.1/pairwiseANIviz/__init__.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     4333 2024-05-28 00:35:31.000000 pairwiseaniviz-1.1/pairwiseANIviz/get_args.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     5974 2024-05-28 00:31:19.000000 pairwiseaniviz-1.1/pairwiseANIviz/pairwiseANI.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2024-05-28 00:37:00.616228 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     5700 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      340 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       55 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/entry_points.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       32 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/requires.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       15 2024-05-28 00:37:00.000000 pairwiseaniviz-1.1/pairwiseANIviz.egg-info/top_level.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2024-05-28 00:37:00.634379 pairwiseaniviz-1.1/setup.cfg
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      732 2024-05-28 00:36:02.000000 pairwiseaniviz-1.1/setup.py
```

### Comparing `pairwiseANIviz-1.0/LICENSE` & `pairwiseaniviz-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pairwiseANIviz-1.0/PKG-INFO` & `pairwiseaniviz-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pairwiseANIviz
-Version: 1.0
+Version: 1.1
 Summary: Pairwise ANI (Average Nucleotide Identity) visulization tool.
 Home-page: https://github.com/RunJiaJi/pairwiseANIviz
 Author: Runjia Ji
 Author-email: jirunjia@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
```

### Comparing `pairwiseANIviz-1.0/README.md` & `pairwiseaniviz-1.1/README.md`

 * *Files identical despite different names*

### Comparing `pairwiseANIviz-1.0/pairwiseANIviz/__init__.py` & `pairwiseaniviz-1.1/pairwiseANIviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pairwiseANIviz-1.0/pairwiseANIviz/get_args.py` & `pairwiseaniviz-1.1/pairwiseANIviz/get_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "ANI result visulization without classification info:\n"
         "   $ pairwiseANIviz ani_result.txt\n\n"
         "ANI result visulization with classification info:\n"
         "   $ pairwiseANIviz ani_result.txt --classificationFile classification_result.tsv\n\n"
         "Runjia Ji, 2023"
     )
 
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s 1.0', help='Show pairwiseANIviz version number and exit.')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 1.1', help='Show pairwiseANIviz version number and exit.')
     parser.add_argument('anifile', type=str, help='File containing pairwise ANI analysis result.')
     parser.add_argument('-o', '--outdir', type=str, default='./pairwiseANIviz', help="Directory to save the output figures (default 'pairwiseANIviz').")
     parser.add_argument('--method', type=str, choices=['single', 'complete', 'average', 'weighted', 'centroid', 'median', 'ward'], 
                         default='average',
                         help="Linkage method to use for calculating clusters (default 'average').\nSee https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage")
     parser.add_argument('--metric', type=str, 
                         choices=[
```

### Comparing `pairwiseANIviz-1.0/pairwiseANIviz/pairwiseANI.py` & `pairwiseaniviz-1.1/pairwiseANIviz/pairwiseANI.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             yticklabels = True, 
             cbar_kws={
                 "label": "ANI (%)",
                 "orientation": "vertical",
                 "spacing": "proportional"
             },
             tree_kws={"linewidths": 1.5},
-            fmt="d"
+            fmt=".3g"
             )
     
     # save figs
     if not os.path.exists(outdir):
         os.mkdir(outdir)
     
     suffix=['svg','png','jpg','pdf','tiff', 'eps']
```

### Comparing `pairwiseANIviz-1.0/pairwiseANIviz.egg-info/PKG-INFO` & `pairwiseaniviz-1.1/pairwiseANIviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pairwiseANIviz
-Version: 1.0
+Version: 1.1
 Summary: Pairwise ANI (Average Nucleotide Identity) visulization tool.
 Home-page: https://github.com/RunJiaJi/pairwiseANIviz
 Author: Runjia Ji
 Author-email: jirunjia@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
```

### Comparing `pairwiseANIviz-1.0/setup.py` & `pairwiseaniviz-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name='pairwiseANIviz',
-    version='1.0',
+    version='1.1',
     description="Pairwise ANI (Average Nucleotide Identity) visulization tool.",
     url="https://github.com/RunJiaJi/pairwiseANIviz",
     author='Runjia Ji',
     author_email='jirunjia@gmail.com',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

