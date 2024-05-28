# Comparing `tmp/nanosense-0.1.3.tar.gz` & `tmp/nanosense-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosense-0.1.3.tar", last modified: Mon May 27 06:09:51 2024, max compression
+gzip compressed data, was "nanosense-0.2.0.tar", last modified: Mon May 27 06:14:34 2024, max compression
```

## Comparing `nanosense-0.1.3.tar` & `nanosense-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.975132 nanosense-0.1.3/
--rw-r--r--   0 shankardutt   (501) staff       (20)       98 2024-05-27 06:08:37.000000 nanosense-0.1.3/MANIFEST.in
--rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-27 06:09:51.974936 nanosense-0.1.3/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.1.3/README.md
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.970053 nanosense-0.1.3/nanosense/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.971104 nanosense-0.1.3/nanosense/Clustering and Data Reduction/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Clustering and Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   107280 2024-05-20 03:54:27.000000 nanosense-0.1.3/nanosense/Clustering and Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.971410 nanosense-0.1.3/nanosense/Combine Datasets/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Combine Datasets/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)     5973 2024-05-08 03:18:56.000000 nanosense-0.1.3/nanosense/Combine Datasets/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.971854 nanosense-0.1.3/nanosense/Data Reduction/
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.972108 nanosense-0.1.3/nanosense/Data Reduction/Docs/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Data Reduction/Docs/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Data Reduction/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   228038 2024-05-20 04:16:55.000000 nanosense-0.1.3/nanosense/Data Reduction/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.972319 nanosense-0.1.3/nanosense/Data Visualisation/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Data Visualisation/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)   101413 2024-05-19 00:30:33.000000 nanosense-0.1.3/nanosense/Data Visualisation/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.972626 nanosense-0.1.3/nanosense/Event Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Event Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    32048 2024-05-19 00:26:20.000000 nanosense-0.1.3/nanosense/Event Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.972898 nanosense-0.1.3/nanosense/Frequency and multi-plots/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Frequency and multi-plots/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    39035 2024-05-19 00:31:20.000000 nanosense-0.1.3/nanosense/Frequency and multi-plots/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.973182 nanosense-0.1.3/nanosense/ML Analysis/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/ML Analysis/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    60685 2024-05-07 07:33:17.000000 nanosense-0.1.3/nanosense/ML Analysis/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.973475 nanosense-0.1.3/nanosense/Nanopore Size Calc/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Nanopore Size Calc/__init__.py
--rwx------   0 shankardutt   (501) staff       (20)     5069 2024-05-08 03:29:30.000000 nanosense-0.1.3/nanosense/Nanopore Size Calc/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.973905 nanosense-0.1.3/nanosense/Plotting and selecting/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Plotting and selecting/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28580 2024-05-07 07:27:05.000000 nanosense-0.1.3/nanosense/Plotting and selecting/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.974168 nanosense-0.1.3/nanosense/Resource Monitor/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Resource Monitor/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    11105 2024-05-11 05:45:18.000000 nanosense-0.1.3/nanosense/Resource Monitor/main.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.974473 nanosense-0.1.3/nanosense/Spectrogram and PSD/
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/Spectrogram and PSD/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)    28223 2024-05-10 06:05:42.000000 nanosense-0.1.3/nanosense/Spectrogram and PSD/main.py
--rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.1.3/nanosense/__init__.py
--rw-r--r--   0 shankardutt   (501) staff       (20)      504 2024-04-26 09:46:44.000000 nanosense-0.1.3/nanosense/activation_codes.enc
--rw-r--r--   0 shankardutt   (501) staff       (20)     1101 2024-04-29 05:17:53.000000 nanosense-0.1.3/nanosense/crypt_activation.py
--rw-r--r--   0 shankardutt   (501) staff       (20)   989781 2024-03-21 23:51:54.000000 nanosense-0.1.3/nanosense/icons.icns
--rw-r--r--   0 shankardutt   (501) staff       (20)   256727 2024-03-21 23:31:47.000000 nanosense-0.1.3/nanosense/image_1.jpg
--rw-r--r--   0 shankardutt   (501) staff       (20)    15927 2024-05-10 07:48:43.000000 nanosense-0.1.3/nanosense/nanosense.py
-drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:09:51.974678 nanosense-0.1.3/nanosense.egg-info/
--rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/PKG-INFO
--rw-r--r--   0 shankardutt   (501) staff       (20)     1287 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/SOURCES.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/dependency_links.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       55 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/entry_points.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/requires.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-05-27 06:09:51.000000 nanosense-0.1.3/nanosense.egg-info/top_level.txt
--rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-05-27 06:09:51.975183 nanosense-0.1.3/setup.cfg
--rw-r--r--   0 shankardutt   (501) staff       (20)     1385 2024-05-27 06:09:18.000000 nanosense-0.1.3/setup.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.650162 nanosense-0.2.0/
+-rw-r--r--   0 shankardutt   (501) staff       (20)       98 2024-05-27 06:08:37.000000 nanosense-0.2.0/MANIFEST.in
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-27 06:14:34.649863 nanosense-0.2.0/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)       11 2024-04-05 23:59:28.000000 nanosense-0.2.0/README.md
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.617612 nanosense-0.2.0/nanosense/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.618821 nanosense-0.2.0/nanosense/Clustering and Data Reduction/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Clustering and Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)   107280 2024-05-20 03:54:27.000000 nanosense-0.2.0/nanosense/Clustering and Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.619902 nanosense-0.2.0/nanosense/Combine Datasets/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Combine Datasets/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)     5973 2024-05-08 03:18:56.000000 nanosense-0.2.0/nanosense/Combine Datasets/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.620340 nanosense-0.2.0/nanosense/Data Reduction/
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.621671 nanosense-0.2.0/nanosense/Data Reduction/Docs/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Data Reduction/Docs/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Data Reduction/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)   228038 2024-05-20 04:16:55.000000 nanosense-0.2.0/nanosense/Data Reduction/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.621909 nanosense-0.2.0/nanosense/Data Visualisation/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Data Visualisation/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)   101413 2024-05-19 00:30:33.000000 nanosense-0.2.0/nanosense/Data Visualisation/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.623201 nanosense-0.2.0/nanosense/Event Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Event Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    32048 2024-05-19 00:26:20.000000 nanosense-0.2.0/nanosense/Event Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.624570 nanosense-0.2.0/nanosense/Frequency and multi-plots/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Frequency and multi-plots/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    39035 2024-05-19 00:31:20.000000 nanosense-0.2.0/nanosense/Frequency and multi-plots/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.625404 nanosense-0.2.0/nanosense/ML Analysis/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/ML Analysis/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    60685 2024-05-07 07:33:17.000000 nanosense-0.2.0/nanosense/ML Analysis/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.625735 nanosense-0.2.0/nanosense/Nanopore Size Calc/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Nanopore Size Calc/__init__.py
+-rwx------   0 shankardutt   (501) staff       (20)     5069 2024-05-08 03:29:30.000000 nanosense-0.2.0/nanosense/Nanopore Size Calc/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.626710 nanosense-0.2.0/nanosense/Plotting and selecting/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Plotting and selecting/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    28580 2024-05-07 07:27:05.000000 nanosense-0.2.0/nanosense/Plotting and selecting/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.627737 nanosense-0.2.0/nanosense/Resource Monitor/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Resource Monitor/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    11105 2024-05-11 05:45:18.000000 nanosense-0.2.0/nanosense/Resource Monitor/main.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.648047 nanosense-0.2.0/nanosense/Spectrogram and PSD/
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/Spectrogram and PSD/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)    28223 2024-05-10 06:05:42.000000 nanosense-0.2.0/nanosense/Spectrogram and PSD/main.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)        0 2024-05-26 06:25:29.000000 nanosense-0.2.0/nanosense/__init__.py
+-rw-r--r--   0 shankardutt   (501) staff       (20)      504 2024-04-26 09:46:44.000000 nanosense-0.2.0/nanosense/activation_codes.enc
+-rw-r--r--   0 shankardutt   (501) staff       (20)   989781 2024-03-21 23:51:54.000000 nanosense-0.2.0/nanosense/icons.icns
+-rw-r--r--   0 shankardutt   (501) staff       (20)   256727 2024-03-21 23:31:47.000000 nanosense-0.2.0/nanosense/image_1.jpg
+-rw-r--r--   0 shankardutt   (501) staff       (20)    15927 2024-05-10 07:48:43.000000 nanosense-0.2.0/nanosense/nanosense.py
+drwxr-xr-x   0 shankardutt   (501) staff       (20)        0 2024-05-27 06:14:34.648639 nanosense-0.2.0/nanosense.egg-info/
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1054 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/PKG-INFO
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1257 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/SOURCES.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)        1 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/dependency_links.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       55 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/entry_points.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)      235 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/requires.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       10 2024-05-27 06:14:34.000000 nanosense-0.2.0/nanosense.egg-info/top_level.txt
+-rw-r--r--   0 shankardutt   (501) staff       (20)       38 2024-05-27 06:14:34.650227 nanosense-0.2.0/setup.cfg
+-rw-r--r--   0 shankardutt   (501) staff       (20)     1385 2024-05-27 06:14:25.000000 nanosense-0.2.0/setup.py
```

### Comparing `nanosense-0.1.3/PKG-INFO` & `nanosense-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.1.3
+Version: 0.2.0
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosense-0.1.3/nanosense/Clustering and Data Reduction/main.py` & `nanosense-0.2.0/nanosense/Clustering and Data Reduction/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Combine Datasets/main.py` & `nanosense-0.2.0/nanosense/Combine Datasets/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Data Reduction/main.py` & `nanosense-0.2.0/nanosense/Data Reduction/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Data Visualisation/main.py` & `nanosense-0.2.0/nanosense/Data Visualisation/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Event Analysis/main.py` & `nanosense-0.2.0/nanosense/Event Analysis/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Frequency and multi-plots/main.py` & `nanosense-0.2.0/nanosense/Frequency and multi-plots/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/ML Analysis/main.py` & `nanosense-0.2.0/nanosense/ML Analysis/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Nanopore Size Calc/main.py` & `nanosense-0.2.0/nanosense/Nanopore Size Calc/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Plotting and selecting/main.py` & `nanosense-0.2.0/nanosense/Plotting and selecting/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Resource Monitor/main.py` & `nanosense-0.2.0/nanosense/Resource Monitor/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/Spectrogram and PSD/main.py` & `nanosense-0.2.0/nanosense/Spectrogram and PSD/main.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/icons.icns` & `nanosense-0.2.0/nanosense/icons.icns`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/image_1.jpg` & `nanosense-0.2.0/nanosense/image_1.jpg`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense/nanosense.py` & `nanosense-0.2.0/nanosense/nanosense.py`

 * *Files identical despite different names*

### Comparing `nanosense-0.1.3/nanosense.egg-info/PKG-INFO` & `nanosense-0.2.0/nanosense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosense
-Version: 0.1.3
+Version: 0.2.0
 Summary: A comprehensive package for nanosense data analysis and visualization.
 Home-page: https://github.com/shankardutt/nanosense
 Author: Shankar Dutt
 Author-email: shankar.dutt@anu.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosense-0.1.3/nanosense.egg-info/SOURCES.txt` & `nanosense-0.2.0/nanosense.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 nanosense/__init__.py
 nanosense/activation_codes.enc
-nanosense/crypt_activation.py
 nanosense/icons.icns
 nanosense/image_1.jpg
 nanosense/nanosense.py
 nanosense.egg-info/PKG-INFO
 nanosense.egg-info/SOURCES.txt
 nanosense.egg-info/dependency_links.txt
 nanosense.egg-info/entry_points.txt
```

### Comparing `nanosense-0.1.3/setup.py` & `nanosense-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nanosense',
-    version='0.1.3',
+    version='0.2.0',
     description='A comprehensive package for nanosense data analysis and visualization.',
     author='Shankar Dutt',
     author_email='shankar.dutt@anu.edu.au',
     url='https://github.com/shankardutt/nanosense',
     packages=find_packages(include=['nanosense', 'nanosense.*']),
     include_package_data=True,
     package_data={
```

