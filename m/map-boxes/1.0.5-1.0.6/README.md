# Comparing `tmp/map_boxes-1.0.5.tar.gz` & `tmp/map_boxes-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\map_boxes-1.0.5.tar", last modified: Wed Oct  2 20:33:36 2019, max compression
+gzip compressed data, was "map_boxes-1.0.6.tar", last modified: Tue May 28 18:46:19 2024, max compression
```

## Comparing `map_boxes-1.0.5.tar` & `map_boxes-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2019-10-02 20:33:36.000000 map_boxes-1.0.5/
-drwxrwxrwx   0        0        0        0 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes/
--rw-rw-rw-   0        0        0     1764 2019-09-22 15:47:52.000000 map_boxes-1.0.5/map_boxes/compute_overlap.pyx
--rw-rw-rw-   0        0        0     1274 2019-09-22 16:00:39.000000 map_boxes-1.0.5/map_boxes/compute_overlap_slow.py
--rw-rw-rw-   0        0        0     8275 2019-10-02 20:30:38.000000 map_boxes-1.0.5/map_boxes/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/
--rw-rw-rw-   0        0        0        1 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      500 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       13 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/requires.txt
--rw-rw-rw-   0        0        0      268 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2019-10-02 20:33:36.000000 map_boxes-1.0.5/map_boxes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      500 2019-10-02 20:33:36.000000 map_boxes-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2019-09-22 18:52:00.000000 map_boxes-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2019-10-02 20:33:36.000000 map_boxes-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      786 2019-10-02 20:32:53.000000 map_boxes-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:46:19.571924 map_boxes-1.0.6/
+-rw-rw-rw-   0        0        0      347 2024-05-28 18:46:19.571924 map_boxes-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2165 2023-02-05 23:02:11.000000 map_boxes-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 18:46:19.551924 map_boxes-1.0.6/map_boxes/
+-rw-rw-rw-   0        0        0     8349 2024-05-25 08:21:36.000000 map_boxes-1.0.6/map_boxes/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-02-05 23:02:11.000000 map_boxes-1.0.6/map_boxes/compute_overlap_slow.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:46:19.570923 map_boxes-1.0.6/map_boxes.egg-info/
+-rw-rw-rw-   0        0        0      347 2024-05-28 18:46:19.000000 map_boxes-1.0.6/map_boxes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-28 18:46:19.000000 map_boxes-1.0.6/map_boxes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 18:46:19.000000 map_boxes-1.0.6/map_boxes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 18:46:19.000000 map_boxes-1.0.6/map_boxes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 18:46:19.571924 map_boxes-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      515 2024-05-28 18:45:43.000000 map_boxes-1.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `map_boxes-1.0.5/map_boxes/compute_overlap_slow.py` & `map_boxes-1.0.6/map_boxes/compute_overlap_slow.py`

 * *Files identical despite different names*

### Comparing `map_boxes-1.0.5/map_boxes/__init__.py` & `map_boxes-1.0.6/map_boxes/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 except:
     print("Couldn't import fast version of function compute_overlap, will use slow one. Check cython intallation")
     from .compute_overlap_slow import compute_overlap
 
 
 def get_real_annotations(table):
     res = dict()
-    ids = table['ImageID'].values.astype(np.str)
-    labels = table['LabelName'].values.astype(np.str)
+    ids = table['ImageID'].values.astype(str)
+    labels = table['LabelName'].values.astype(str)
     xmin = table['XMin'].values.astype(np.float32)
     xmax = table['XMax'].values.astype(np.float32)
     ymin = table['YMin'].values.astype(np.float32)
     ymax = table['YMax'].values.astype(np.float32)
 
     for i in range(len(ids)):
         id = ids[i]
@@ -36,16 +36,16 @@
         res[id][label].append(box)
 
     return res
 
 
 def get_detections(table):
     res = dict()
-    ids = table['ImageID'].values.astype(np.str)
-    labels = table['LabelName'].values.astype(np.str)
+    ids = table['ImageID'].values.astype(str)
+    labels = table['LabelName'].values.astype(str)
     scores = table['Conf'].values.astype(np.float32)
     xmin = table['XMin'].values.astype(np.float32)
     xmax = table['XMax'].values.astype(np.float32)
     ymin = table['YMin'].values.astype(np.float32)
     ymax = table['YMax'].values.astype(np.float32)
 
     for i in range(len(ids)):
@@ -107,29 +107,29 @@
         valid = pd.DataFrame(ann, columns=['ImageID', 'LabelName', 'XMin', 'XMax', 'YMin', 'YMax'])
 
     if isinstance(pred, str):
         preds = pd.read_csv(pred)
     else:
         preds = pd.DataFrame(pred, columns=['ImageID', 'LabelName', 'Conf', 'XMin', 'XMax', 'YMin', 'YMax'])
 
-    ann_unique = valid['ImageID'].unique()
-    preds_unique = preds['ImageID'].unique()
+    ann_unique = valid['ImageID'].unique().astype(str)
+    preds_unique = preds['ImageID'].unique().astype(str)
 
     if verbose:
         print('Number of files in annotations: {}'.format(len(ann_unique)))
         print('Number of files in predictions: {}'.format(len(preds_unique)))
 
     # Exclude files not in annotations!
     if exclude_not_in_annotations:
         preds = preds[preds['ImageID'].isin(ann_unique)]
         preds_unique = preds['ImageID'].unique()
         if verbose:
             print('Number of files in detection after reduction: {}'.format(len(preds_unique)))
 
-    unique_classes = valid['LabelName'].unique().astype(np.str)
+    unique_classes = valid['LabelName'].unique().astype(str)
     if verbose:
         print('Unique classes: {}'.format(len(unique_classes)))
 
     all_detections = get_detections(preds)
     all_annotations = get_real_annotations(valid)
     if verbose:
         print('Detections length: {}'.format(len(all_detections)))
@@ -215,11 +215,14 @@
 
     present_classes = 0
     precision = 0
     for label, (average_precision, num_annotations) in average_precisions.items():
         if num_annotations > 0:
             present_classes += 1
             precision += average_precision
-    mean_ap = precision / present_classes
+    if present_classes > 0:
+        mean_ap = precision / present_classes
+    else:
+        mean_ap = 0
     if verbose:
         print('mAP: {:.6f}'.format(mean_ap))
     return mean_ap, average_precisions
```

### Comparing `map_boxes-1.0.5/README.md` & `map_boxes-1.0.6/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-Function to calculate mean average precision (mAP) for set of boxes. Useful for object detection pipelines.
-
-# Requirements
-
-python 3.*, numpy, pandas
-
-# Installation
-
-```
-pip install map-boxes
-```
-
-## Usage example:
-
-You can provide paths to CSV-files:
-
-```python
-from map_boxes import mean_average_precision_for_boxes
-
-annotations_file = 'example/annotations.csv'
-detections_file = 'example/detections.csv'
-mean_ap, average_precisions = mean_average_precision_for_boxes(annotations_file, detections_file)
-```
-
-or you can pass directly numpy arrays of shapes **(N, 6)** and **(M, 7)**. **Be careful about order of variables in arrays!**:
-
-```python
-from map_boxes import mean_average_precision_for_boxes
-import pandas as pd
-
-ann = pd.read_csv('example/annotations.csv')
-det = pd.read_csv('example/detections.csv')
-ann = ann[['ImageID', 'LabelName', 'XMin', 'XMax', 'YMin', 'YMax']].values
-det = det[['ImageID', 'LabelName', 'Conf', 'XMin', 'XMax', 'YMin', 'YMax']].values
-mean_ap, average_precisions = mean_average_precision_for_boxes(ann, det)
-```
-
-
-## Input files format
-
-Boxes must be in normalized form e.g. coordinates must be in range: `[0, 1]`. To normalize pixel values you need to recalculate them as: `x_norm = x / width`, `y_norm = y / height`
-
-* Annotation CSV-file:
-
-```csv
-ImageID,LabelName,XMin,XMax,YMin,YMax
-i0.jpg,Shellfish,0.0875,0.8171875,0.35625,0.8958333
-i0.jpg,Seafood,0.0875,0.8171875,0.35625,0.8958333
-i1.jpg,Tin can,0.1296875,0.3375,0.31875,0.68958336
-i1.jpg,Drink,0.4234375,0.546875,0.58958334,0.92083335
-i1.jpg,Drink,0.5375,0.7375,0.16666667,0.575
-...
-```
-
-* Detection CSV-file:
-
-```csv
-ImageID,LabelName,Conf,XMin,XMax,YMin,YMax
-i0.jpg,Turtle,0.41471,0.1382,0.7440,0.3585,0.8951
-i0.jpg,Reptile,0.32093,0.1391,0.7439,0.3582,0.8944
-i0.jpg,Seahorse,0.11860,0.1393,0.7434,0.3589,0.8943
-i0.jpg,Caterpillar,0.11275,0.1390,0.7438,0.3588,0.8948
-i1.jpg,Personal care,0.42326,0.2624,0.5473,0.1112,0.7274
-i1.jpg,Personal care,0.31120,0.1318,0.3381,0.3149,0.6863
-i1.jpg,Personal care,0.34866,0.4277,0.5446,0.5861,0.9211
-i1.jpg,Blender,0.10578,0.7678,0.9476,0.2674,0.5847
-...
-```
+Function to calculate mean average precision (mAP) for set of boxes. Useful for object detection pipelines.
+
+# Requirements
+
+python 3.*, numpy, pandas
+
+# Installation
+
+```
+pip install map-boxes
+```
+
+## Usage example:
+
+You can provide paths to CSV-files:
+
+```python
+from map_boxes import mean_average_precision_for_boxes
+
+annotations_file = 'example/annotations.csv'
+detections_file = 'example/detections.csv'
+mean_ap, average_precisions = mean_average_precision_for_boxes(annotations_file, detections_file)
+```
+
+or you can pass directly numpy arrays of shapes **(N, 6)** and **(M, 7)**. **Be careful about order of variables in arrays!**:
+
+```python
+from map_boxes import mean_average_precision_for_boxes
+import pandas as pd
+
+ann = pd.read_csv('example/annotations.csv')
+det = pd.read_csv('example/detections.csv')
+ann = ann[['ImageID', 'LabelName', 'XMin', 'XMax', 'YMin', 'YMax']].values
+det = det[['ImageID', 'LabelName', 'Conf', 'XMin', 'XMax', 'YMin', 'YMax']].values
+mean_ap, average_precisions = mean_average_precision_for_boxes(ann, det)
+```
+
+
+## Input files format
+
+Boxes must be in normalized form e.g. coordinates must be in range: `[0, 1]`. To normalize pixel values you need to recalculate them as: `x_norm = x / width`, `y_norm = y / height`
+
+* Annotation CSV-file:
+
+```csv
+ImageID,LabelName,XMin,XMax,YMin,YMax
+i0.jpg,Shellfish,0.0875,0.8171875,0.35625,0.8958333
+i0.jpg,Seafood,0.0875,0.8171875,0.35625,0.8958333
+i1.jpg,Tin can,0.1296875,0.3375,0.31875,0.68958336
+i1.jpg,Drink,0.4234375,0.546875,0.58958334,0.92083335
+i1.jpg,Drink,0.5375,0.7375,0.16666667,0.575
+...
+```
+
+* Detection CSV-file:
+
+```csv
+ImageID,LabelName,Conf,XMin,XMax,YMin,YMax
+i0.jpg,Turtle,0.41471,0.1382,0.7440,0.3585,0.8951
+i0.jpg,Reptile,0.32093,0.1391,0.7439,0.3582,0.8944
+i0.jpg,Seahorse,0.11860,0.1393,0.7434,0.3589,0.8943
+i0.jpg,Caterpillar,0.11275,0.1390,0.7438,0.3588,0.8948
+i1.jpg,Personal care,0.42326,0.2624,0.5473,0.1112,0.7274
+i1.jpg,Personal care,0.31120,0.1318,0.3381,0.3149,0.6863
+i1.jpg,Personal care,0.34866,0.4277,0.5446,0.5861,0.9211
+i1.jpg,Blender,0.10578,0.7678,0.9476,0.2674,0.5847
+...
+```
```

### Comparing `map_boxes-1.0.5/setup.py` & `map_boxes-1.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 try:
     from setuptools import setup
-except:
+except ImportError:
     from distutils.core import setup
 
 setup(
     name='map_boxes',
-    version='1.0.5',
+    version='1.0.6',
     author='Roman Sol (ZFTurbo)',
-    packages=['map_boxes', ],
+    packages=['map_boxes'],
     url='https://github.com/ZFTurbo/Mean-Average-Precision-for-Boxes',
-    license='MIT License',
-    description='Function to calculate mAP for set of detected boxes and annotated boxes. ',
-    long_description='Function to calculate mean average precision (mAP) for set of boxes. Useful for object detection pipelines.'
-                     'More details: https://github.com/ZFTurbo/Mean-Average-Precision-for-Boxes',
-    install_requires=[
-        "numpy",
-        "pandas",
-    ],
-    package_data={'': ['compute_overlap.pyx']},
-    include_package_data=True,
+    description='Function to calculate mean average precision (mAP) for set of boxes.',
+    long_description='Function to calculate mean average precision (mAP) for set of boxes. Useful for object detection pipelines.',
 )
```

