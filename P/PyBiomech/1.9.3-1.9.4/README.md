# Comparing `tmp/PyBiomech-1.9.3.tar.gz` & `tmp/PyBiomech-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyBiomech-1.9.3.tar", last modified: Fri Feb 18 09:56:49 2022, max compression
+gzip compressed data, was "dist\PyBiomech-1.9.4.tar", last modified: Fri Feb 18 11:16:39 2022, max compression
```

## Comparing `PyBiomech-1.9.3.tar` & `PyBiomech-1.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-02-18 09:56:49.000000 PyBiomech-1.9.3/
--rw-rw-rw-   0        0        0     1312 2022-02-18 09:56:49.000000 PyBiomech-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0      721 2019-03-01 11:02:10.000000 PyBiomech-1.9.3/README.rst
--rw-rw-rw-   0        0        0       42 2022-02-18 09:56:49.000000 PyBiomech-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0      708 2022-02-18 09:56:21.000000 PyBiomech-1.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-18 09:56:48.000000 PyBiomech-1.9.3/src/
-drwxrwxrwx   0        0        0        0 2022-02-18 09:56:49.000000 PyBiomech-1.9.3/src/PyBiomech/
--rw-rw-rw-   0        0        0       27 2021-03-12 10:53:25.000000 PyBiomech-1.9.3/src/PyBiomech/__init__.py
--rw-rw-rw-   0        0        0     3349 2021-05-14 12:00:23.000000 PyBiomech-1.9.3/src/PyBiomech/btkio.py
--rw-rw-rw-   0        0        0     1357 2020-07-27 13:32:56.000000 PyBiomech-1.9.3/src/PyBiomech/contacts.py
--rw-rw-rw-   0        0        0    16337 2022-02-18 09:52:56.000000 PyBiomech-1.9.3/src/PyBiomech/fio.py
--rw-rw-rw-   0        0        0     1406 2021-11-29 16:23:52.000000 PyBiomech-1.9.3/src/PyBiomech/geom.py
--rw-rw-rw-   0        0        0    63532 2022-01-26 13:57:15.000000 PyBiomech-1.9.3/src/PyBiomech/kine.py
--rw-rw-rw-   0        0        0     2492 2021-03-17 15:05:05.000000 PyBiomech-1.9.3/src/PyBiomech/kine_fr.py
--rw-rw-rw-   0        0        0     6189 2022-01-24 15:59:16.000000 PyBiomech-1.9.3/src/PyBiomech/kine_or.py
--rw-rw-rw-   0        0        0     5607 2021-03-17 14:08:27.000000 PyBiomech-1.9.3/src/PyBiomech/kine_sr.py
--rw-rw-rw-   0        0        0     1055 2020-07-27 15:18:01.000000 PyBiomech-1.9.3/src/PyBiomech/kine_wr.py
--rw-rw-rw-   0        0        0     9411 2022-01-10 08:26:38.000000 PyBiomech-1.9.3/src/PyBiomech/ligaments.py
--rw-rw-rw-   0        0        0      989 2017-05-02 09:42:41.000000 PyBiomech-1.9.3/src/PyBiomech/mplh.py
--rw-rw-rw-   0        0        0    44292 2021-03-11 10:30:21.000000 PyBiomech-1.9.3/src/PyBiomech/procedure_or.py
--rw-rw-rw-   0        0        0    18642 2022-02-01 13:09:41.000000 PyBiomech-1.9.3/src/PyBiomech/procedure_rig.py
--rw-rw-rw-   0        0        0    19256 2022-01-10 08:21:46.000000 PyBiomech-1.9.3/src/PyBiomech/procedure_spine.py
--rw-rw-rw-   0        0        0     6838 2021-03-11 10:30:52.000000 PyBiomech-1.9.3/src/PyBiomech/procedure_sr.py
--rw-rw-rw-   0        0        0       73 2021-03-11 10:28:26.000000 PyBiomech-1.9.3/src/PyBiomech/pyver.py
--rw-rw-rw-   0        0        0    71314 2018-04-27 10:05:23.000000 PyBiomech-1.9.3/src/PyBiomech/rotations.py
--rw-rw-rw-   0        0        0     1687 2021-03-09 09:49:02.000000 PyBiomech-1.9.3/src/PyBiomech/spine.py
--rw-rw-rw-   0        0        0     8281 2022-01-26 13:29:11.000000 PyBiomech-1.9.3/src/PyBiomech/utils.py
--rw-rw-rw-   0        0        0     6730 2021-09-15 08:26:10.000000 PyBiomech-1.9.3/src/PyBiomech/viconio.py
--rw-rw-rw-   0        0        0    12411 2021-11-29 16:32:55.000000 PyBiomech-1.9.3/src/PyBiomech/vtkh.py
-drwxrwxrwx   0        0        0        0 2022-02-18 09:56:49.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/
--rw-rw-rw-   0        0        0     1312 2022-02-18 09:56:43.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      759 2022-02-18 09:56:44.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-18 09:56:43.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-02-18 09:56:43.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-02-18 09:56:43.000000 PyBiomech-1.9.3/src/PyBiomech.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-02-18 11:16:39.000000 PyBiomech-1.9.4/
+-rw-rw-rw-   0        0        0     1312 2022-02-18 11:16:39.000000 PyBiomech-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2019-03-01 11:02:10.000000 PyBiomech-1.9.4/README.rst
+-rw-rw-rw-   0        0        0       42 2022-02-18 11:16:39.000000 PyBiomech-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      708 2022-02-18 11:16:28.000000 PyBiomech-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-18 11:16:38.000000 PyBiomech-1.9.4/src/
+drwxrwxrwx   0        0        0        0 2022-02-18 11:16:39.000000 PyBiomech-1.9.4/src/PyBiomech/
+-rw-rw-rw-   0        0        0       27 2021-03-12 10:53:25.000000 PyBiomech-1.9.4/src/PyBiomech/__init__.py
+-rw-rw-rw-   0        0        0     3349 2021-05-14 12:00:23.000000 PyBiomech-1.9.4/src/PyBiomech/btkio.py
+-rw-rw-rw-   0        0        0     1357 2020-07-27 13:32:56.000000 PyBiomech-1.9.4/src/PyBiomech/contacts.py
+-rw-rw-rw-   0        0        0    16318 2022-02-18 11:10:35.000000 PyBiomech-1.9.4/src/PyBiomech/fio.py
+-rw-rw-rw-   0        0        0     1406 2021-11-29 16:23:52.000000 PyBiomech-1.9.4/src/PyBiomech/geom.py
+-rw-rw-rw-   0        0        0    63532 2022-01-26 13:57:15.000000 PyBiomech-1.9.4/src/PyBiomech/kine.py
+-rw-rw-rw-   0        0        0     2492 2021-03-17 15:05:05.000000 PyBiomech-1.9.4/src/PyBiomech/kine_fr.py
+-rw-rw-rw-   0        0        0     6189 2022-01-24 15:59:16.000000 PyBiomech-1.9.4/src/PyBiomech/kine_or.py
+-rw-rw-rw-   0        0        0     5607 2021-03-17 14:08:27.000000 PyBiomech-1.9.4/src/PyBiomech/kine_sr.py
+-rw-rw-rw-   0        0        0     1055 2020-07-27 15:18:01.000000 PyBiomech-1.9.4/src/PyBiomech/kine_wr.py
+-rw-rw-rw-   0        0        0     9411 2022-01-10 08:26:38.000000 PyBiomech-1.9.4/src/PyBiomech/ligaments.py
+-rw-rw-rw-   0        0        0      989 2017-05-02 09:42:41.000000 PyBiomech-1.9.4/src/PyBiomech/mplh.py
+-rw-rw-rw-   0        0        0    44292 2021-03-11 10:30:21.000000 PyBiomech-1.9.4/src/PyBiomech/procedure_or.py
+-rw-rw-rw-   0        0        0    18964 2022-02-18 11:09:12.000000 PyBiomech-1.9.4/src/PyBiomech/procedure_rig.py
+-rw-rw-rw-   0        0        0    19256 2022-01-10 08:21:46.000000 PyBiomech-1.9.4/src/PyBiomech/procedure_spine.py
+-rw-rw-rw-   0        0        0     6838 2021-03-11 10:30:52.000000 PyBiomech-1.9.4/src/PyBiomech/procedure_sr.py
+-rw-rw-rw-   0        0        0       73 2021-03-11 10:28:26.000000 PyBiomech-1.9.4/src/PyBiomech/pyver.py
+-rw-rw-rw-   0        0        0    71314 2018-04-27 10:05:23.000000 PyBiomech-1.9.4/src/PyBiomech/rotations.py
+-rw-rw-rw-   0        0        0     1687 2021-03-09 09:49:02.000000 PyBiomech-1.9.4/src/PyBiomech/spine.py
+-rw-rw-rw-   0        0        0     8281 2022-01-26 13:29:11.000000 PyBiomech-1.9.4/src/PyBiomech/utils.py
+-rw-rw-rw-   0        0        0     6730 2021-09-15 08:26:10.000000 PyBiomech-1.9.4/src/PyBiomech/viconio.py
+-rw-rw-rw-   0        0        0    12411 2021-11-29 16:32:55.000000 PyBiomech-1.9.4/src/PyBiomech/vtkh.py
+drwxrwxrwx   0        0        0        0 2022-02-18 11:16:39.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/
+-rw-rw-rw-   0        0        0     1312 2022-02-18 11:16:37.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      759 2022-02-18 11:16:37.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-18 11:16:37.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2022-02-18 11:16:37.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-02-18 11:16:37.000000 PyBiomech-1.9.4/src/PyBiomech.egg-info/top_level.txt
```

### Comparing `PyBiomech-1.9.3/PKG-INFO` & `PyBiomech-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyBiomech
-Version: 1.9.3
+Version: 1.9.4
 Summary: Collection of tools for certain biomechanical pipelines
 Home-page: https://github.com/u0078867/PyBiomech
 Author: u0078867
 Author-email: davide.monari@kuleuven.be
 License: MIT
 Description: Requirements:
         -------------
```

### Comparing `PyBiomech-1.9.3/README.rst` & `PyBiomech-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/setup.py` & `PyBiomech-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='PyBiomech',
-    version='1.9.3',
+    version='1.9.4',
     description='Collection of tools for certain biomechanical pipelines',
     long_description=open('README.rst').read(),
     packages=find_packages('src'),
     package_dir={'':'src'},
     install_requires=[
         'numpy',
         'scipy',
```

### Comparing `PyBiomech-1.9.3/src/PyBiomech/btkio.py` & `PyBiomech-1.9.4/src/PyBiomech/btkio.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/contacts.py` & `PyBiomech-1.9.4/src/PyBiomech/contacts.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/fio.py` & `PyBiomech-1.9.4/src/PyBiomech/fio.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     # Get events
     events = {}
     allList = []
     for i in range(reader.getNEvents()):
         label, context, frame = reader.getEvent(i)
         allList.append(frame)
     events['allMixedList'] = sorted(allList)
-    print(events)
             
     freq = reader.getVectorFrequency()
 
     if 'markers' in sections:
         data['markers'] = {}
         data['markers']['data'] = markers
         data['markers']['unit'] = markerUnit
```

### Comparing `PyBiomech-1.9.3/src/PyBiomech/geom.py` & `PyBiomech-1.9.4/src/PyBiomech/geom.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/kine.py` & `PyBiomech-1.9.4/src/PyBiomech/kine.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/kine_fr.py` & `PyBiomech-1.9.4/src/PyBiomech/kine_fr.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/kine_or.py` & `PyBiomech-1.9.4/src/PyBiomech/kine_or.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/kine_sr.py` & `PyBiomech-1.9.4/src/PyBiomech/kine_sr.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/kine_wr.py` & `PyBiomech-1.9.4/src/PyBiomech/kine_wr.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/ligaments.py` & `PyBiomech-1.9.4/src/PyBiomech/ligaments.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/mplh.py` & `PyBiomech-1.9.4/src/PyBiomech/mplh.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/procedure_or.py` & `PyBiomech-1.9.4/src/PyBiomech/procedure_or.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/procedure_rig.py` & `PyBiomech-1.9.4/src/PyBiomech/procedure_rig.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,23 @@
     linePaths = {}
 
     side = params['side']
     
     mkrsLoc = {m: np.array(params['mkrsLoc'][m]['pos']) for m in params['mkrsLoc']}
     
     mkrsSegs = {}
+    segsMkrs = {}
     for m in params['mkrsLoc']:
         if 'fixedTo' in params['mkrsLoc'][m]:
-            mkrsSegs[m] = params['mkrsLoc'][m]['fixedTo']
+            fixedTo = params['mkrsLoc'][m]['fixedTo']
+            mkrsSegs[m] = fixedTo
+            if fixedTo not in segsMkrs:
+                segsMkrs[fixedTo] = []
+            segsMkrs[fixedTo].append(m)
+            
             
     ALs = {m: np.array(params['mkrsLoc'][m]['pos']) for m in params['mkrsLoc']}
 
     mkrs = markers
     N = markers[list(markers.keys())[0]].shape[0]
     
     t = np.arange(N)
@@ -98,14 +104,16 @@
         funName = defSegPose['defFun']
 
         if type == 'markers_fitting':
 
             R, T, info = kine.rigidBodySVDFun(mkrs, mkrList, args)
             RT = kine.composeRotoTranslMatrix(R, T)
             RTs[segName] = RT
+            usedALs = {m: ALs[m] for m in segsMkrs[segName]}
+            allALs.update(kine.changeMarkersReferenceFrame(usedALs, RT))
             pose = {}
             pose['matrix'] = RT
             pose['RMSE'] = info['RMSE']
             pose['err_max'] = info['eMax']
             pose['err_max_marker'] = info['eMaxMarker']
             poses[segName] = pose
```

### Comparing `PyBiomech-1.9.3/src/PyBiomech/procedure_spine.py` & `PyBiomech-1.9.4/src/PyBiomech/procedure_spine.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/procedure_sr.py` & `PyBiomech-1.9.4/src/PyBiomech/procedure_sr.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/rotations.py` & `PyBiomech-1.9.4/src/PyBiomech/rotations.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/spine.py` & `PyBiomech-1.9.4/src/PyBiomech/spine.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/utils.py` & `PyBiomech-1.9.4/src/PyBiomech/utils.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/viconio.py` & `PyBiomech-1.9.4/src/PyBiomech/viconio.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech/vtkh.py` & `PyBiomech-1.9.4/src/PyBiomech/vtkh.py`

 * *Files identical despite different names*

### Comparing `PyBiomech-1.9.3/src/PyBiomech.egg-info/PKG-INFO` & `PyBiomech-1.9.4/src/PyBiomech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyBiomech
-Version: 1.9.3
+Version: 1.9.4
 Summary: Collection of tools for certain biomechanical pipelines
 Home-page: https://github.com/u0078867/PyBiomech
 Author: u0078867
 Author-email: davide.monari@kuleuven.be
 License: MIT
 Description: Requirements:
         -------------
```

### Comparing `PyBiomech-1.9.3/src/PyBiomech.egg-info/SOURCES.txt` & `PyBiomech-1.9.4/src/PyBiomech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

