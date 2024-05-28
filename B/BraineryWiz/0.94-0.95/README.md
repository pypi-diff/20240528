# Comparing `tmp/BraineryWiz-0.94.tar.gz` & `tmp/brainerywiz-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BraineryWiz-0.94.tar", last modified: Sun Dec 17 14:17:25 2023, max compression
+gzip compressed data, was "brainerywiz-0.95.tar", last modified: Tue May 28 21:11:05 2024, max compression
```

## Comparing `BraineryWiz-0.94.tar` & `brainerywiz-0.95.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 14:17:25.386861 BraineryWiz-0.94/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 14:17:25.386861 BraineryWiz-0.94/BraineryWiz/
--rw-r--r--   0 runner    (1001) docker     (127)    77312 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/FEMWiz.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    92672 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/FEMWiz10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    77312 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/FEMWiz11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   225280 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotAnimation.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   239104 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotAnimation10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   225280 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotAnimation11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   132608 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotDefo.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   148992 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotDefo10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   132608 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotDefo11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   135680 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModeShape.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   151552 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModeShape10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   135680 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModeShape11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   143360 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModel.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   159232 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModel10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   143360 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/PlotModel11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   171008 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/RealTime.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   187392 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/RealTime10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   171008 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/RealTime11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   677376 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_DFunctions.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   716800 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_DFunctions10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   677376 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_DFunctions11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   798720 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_PlotData.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   807936 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_PlotData10.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   798720 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/_PlotData11.pyd
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-17 14:17:10.000000 BraineryWiz-0.94/BraineryWiz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 14:17:25.386861 BraineryWiz-0.94/BraineryWiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-12-17 14:17:25.000000 BraineryWiz-0.94/BraineryWiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-12-17 14:17:25.000000 BraineryWiz-0.94/BraineryWiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 14:17:25.000000 BraineryWiz-0.94/BraineryWiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-17 14:17:25.000000 BraineryWiz-0.94/BraineryWiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-17 14:17:25.000000 BraineryWiz-0.94/BraineryWiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-12-17 14:17:25.386861 BraineryWiz-0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-17 14:17:10.000000 BraineryWiz-0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 14:17:25.386861 BraineryWiz-0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-12-17 14:17:10.000000 BraineryWiz-0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:11:05.639715 brainerywiz-0.95/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:11:05.639715 brainerywiz-0.95/BraineryWiz/
+-rw-r--r--   0 runner    (1001) docker     (127)    94208 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/FEMWiz.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    78336 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/FEMWiz.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    78336 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/FEMWiz.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   246272 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotAnimation.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   234496 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotAnimation.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   234496 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotAnimation.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   151552 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotDefo.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   136192 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotDefo.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   136192 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotDefo.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   154112 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModeShape.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   139776 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModeShape.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   139776 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModeShape.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   161792 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModel.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   147456 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModel.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   147456 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/PlotModel.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   192000 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/RealTime.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   176640 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/RealTime.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   176640 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/RealTime.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   791552 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_DFunctions.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   765952 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_DFunctions.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   765952 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_DFunctions.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   807936 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_PlotData.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   798720 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_PlotData.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   798720 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/_PlotData.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 21:10:57.000000 brainerywiz-0.95/BraineryWiz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:11:05.639715 brainerywiz-0.95/BraineryWiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-28 21:11:05.000000 brainerywiz-0.95/BraineryWiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 21:11:05.000000 brainerywiz-0.95/BraineryWiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:11:05.000000 brainerywiz-0.95/BraineryWiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 21:11:05.000000 brainerywiz-0.95/BraineryWiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:11:05.000000 brainerywiz-0.95/BraineryWiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-28 21:11:05.639715 brainerywiz-0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-28 21:10:57.000000 brainerywiz-0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:11:05.639715 brainerywiz-0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-28 21:10:57.000000 brainerywiz-0.95/setup.py
```

### Comparing `BraineryWiz-0.94/BraineryWiz/__init__.py` & `brainerywiz-0.95/BraineryWiz/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,22 +66,22 @@
             if os.path.isfile('PlotDefo.pyd'): os.remove('PlotDefo.pyd')
             if os.path.isfile('PlotModeShape.pyd'): os.remove('PlotModeShape.pyd')
             if os.path.isfile('RealTime.pyd'): os.remove('RealTime.pyd')
             if os.path.isfile('FEMWiz.pyd'): os.remove('FEMWiz.pyd')
             # print('remove has done')              
                 
             #Rename files from the above version  
-            shutil.copy(curfol+"\\"+"_DFunctions11.pyd",curfol+"\\"+'_DFunctions.pyd');
-            shutil.copy(curfol+"\\"+"_PlotData11.pyd",curfol+"\\"+'_PlotData.pyd');
-            shutil.copy(curfol+"\\"+"PlotModel11.pyd",curfol+"\\"+'PlotModel.pyd');
-            shutil.copy(curfol+"\\"+"PlotAnimation11.pyd",curfol+"\\"+'PlotAnimation.pyd');
-            shutil.copy(curfol+"\\"+"PlotDefo11.pyd",curfol+"\\"+'PlotDefo.pyd');
-            shutil.copy(curfol+"\\"+"PlotModeShape11.pyd",curfol+"\\"+'PlotModeShape.pyd');
-            shutil.copy(curfol+"\\"+"RealTime11.pyd",curfol+"\\"+'RealTime.pyd');
-            shutil.copy(curfol+"\\"+"FEMWiz11.pyd",curfol+"\\"+'FEMWiz.pyd');
+            shutil.copy(curfol+"\\"+"_DFunctions.cp311-win_amd64.pyd",curfol+"\\"+'_DFunctions.pyd');
+            shutil.copy(curfol+"\\"+"_PlotData.cp311-win_amd64.pyd",curfol+"\\"+'_PlotData.pyd');
+            shutil.copy(curfol+"\\"+"PlotModel.cp311-win_amd64.pyd",curfol+"\\"+'PlotModel.pyd');
+            shutil.copy(curfol+"\\"+"PlotAnimation.cp311-win_amd64.pyd",curfol+"\\"+'PlotAnimation.pyd');
+            shutil.copy(curfol+"\\"+"PlotDefo.cp311-win_amd64.pyd",curfol+"\\"+'PlotDefo.pyd');
+            shutil.copy(curfol+"\\"+"PlotModeShape.cp311-win_amd64.pyd",curfol+"\\"+'PlotModeShape.pyd');
+            shutil.copy(curfol+"\\"+"RealTime.cp311-win_amd64.pyd",curfol+"\\"+'RealTime.pyd');
+            shutil.copy(curfol+"\\"+"FEMWiz.cp311-win_amd64.pyd",curfol+"\\"+'FEMWiz.pyd');
             # print('rename has done')
 
 
             from .PlotModel import PlotModel
             from .PlotAnimation import RecorderReset, Record, PlotAnime, PlotAnimeGif
             from .PlotDefo import PlotDefo
             from .PlotModeShape import PlotModeShape
@@ -102,22 +102,22 @@
                 if os.path.isfile('PlotDefo.pyd'): os.remove('PlotDefo.pyd')
                 if os.path.isfile('PlotModeShape.pyd'): os.remove('PlotModeShape.pyd')
                 if os.path.isfile('RealTime.pyd'): os.remove('RealTime.pyd')
                 if os.path.isfile('FEMWiz.pyd'): os.remove('FEMWiz.pyd')
                 # print('remove has done')              
 
                 #Rename files from the above version  
-                shutil.copy(curfol+"\\"+"_DFunctions10.pyd",curfol+"\\"+'_DFunctions.pyd');
-                shutil.copy(curfol+"\\"+"_PlotData10.pyd",curfol+"\\"+'_PlotData.pyd');
-                shutil.copy(curfol+"\\"+"PlotModel10.pyd",curfol+"\\"+'PlotModel.pyd');
-                shutil.copy(curfol+"\\"+"PlotAnimation10.pyd",curfol+"\\"+'PlotAnimation.pyd');
-                shutil.copy(curfol+"\\"+"PlotDefo10.pyd",curfol+"\\"+'PlotDefo.pyd');
-                shutil.copy(curfol+"\\"+"PlotModeShape10.pyd",curfol+"\\"+'PlotModeShape.pyd');
-                shutil.copy(curfol+"\\"+"RealTime10.pyd",curfol+"\\"+'RealTime.pyd');
-                shutil.copy(curfol+"\\"+"FEMWiz10.pyd",curfol+"\\"+'FEMWiz.pyd');
+                shutil.copy(curfol+"\\"+"_DFunctions.cp310-win_amd64.pyd",curfol+"\\"+'_DFunctions.pyd');
+                shutil.copy(curfol+"\\"+"_PlotData.cp310-win_amd64.pyd",curfol+"\\"+'_PlotData.pyd');
+                shutil.copy(curfol+"\\"+"PlotModel.cp310-win_amd64.pyd",curfol+"\\"+'PlotModel.pyd');
+                shutil.copy(curfol+"\\"+"PlotAnimation.cp310-win_amd64.pyd",curfol+"\\"+'PlotAnimation.pyd');
+                shutil.copy(curfol+"\\"+"PlotDefo.cp310-win_amd64.pyd",curfol+"\\"+'PlotDefo.pyd');
+                shutil.copy(curfol+"\\"+"PlotModeShape.cp310-win_amd64.pyd",curfol+"\\"+'PlotModeShape.pyd');
+                shutil.copy(curfol+"\\"+"RealTime.cp310-win_amd64.pyd",curfol+"\\"+'RealTime.pyd');
+                shutil.copy(curfol+"\\"+"FEMWiz.cp310-win_amd64.pyd",curfol+"\\"+'FEMWiz.pyd');
                 # print('rename has done')
                 
                 from .PlotModel import PlotModel
                 from .PlotAnimation import RecorderReset, Record, PlotAnime, PlotAnimeGif
                 from .PlotDefo import PlotDefo
                 from .PlotModeShape import PlotModeShape
                 from .RealTime import RealTimeObj, RealTimeUpdate
```

### Comparing `BraineryWiz-0.94/BraineryWiz.egg-info/PKG-INFO` & `brainerywiz-0.95/BraineryWiz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraineryWiz
-Version: 0.94
+Version: 0.95
 Summary: OpenSees Plotting Package
 Home-page: https://github.com/Silvia-s-Brainery/BraineryWiz
 Author: Bijan Sayyafzadeh - Silvia Mazzoni
 Author-email: <BraineryWiz@Gmail.com>
 Keywords: python,opensees,Modeling,Dynamic
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BraineryWiz-0.94/PKG-INFO` & `brainerywiz-0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraineryWiz
-Version: 0.94
+Version: 0.95
 Summary: OpenSees Plotting Package
 Home-page: https://github.com/Silvia-s-Brainery/BraineryWiz
 Author: Bijan Sayyafzadeh - Silvia Mazzoni
 Author-email: <BraineryWiz@Gmail.com>
 Keywords: python,opensees,Modeling,Dynamic
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BraineryWiz-0.94/README.md` & `brainerywiz-0.95/README.md`

 * *Files identical despite different names*

### Comparing `BraineryWiz-0.94/setup.py` & `brainerywiz-0.95/setup.py`

 * *Files identical despite different names*

