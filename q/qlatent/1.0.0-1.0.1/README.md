# Comparing `tmp/qlatent-1.0.0.tar.gz` & `tmp/qlatent-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlatent-1.0.0.tar", last modified: Tue Apr  2 08:25:34 2024, max compression
+gzip compressed data, was "qlatent-1.0.1.tar", last modified: Tue May 28 10:05:59 2024, max compression
```

## Comparing `qlatent-1.0.0.tar` & `qlatent-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.396327 qlatent-1.0.0/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)    11357 2024-04-01 12:16:49.000000 qlatent-1.0.0/LICENSE
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      399 2024-04-02 08:25:34.394323 qlatent-1.0.0/PKG-INFO
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     4444 2024-04-01 12:16:49.000000 qlatent-1.0.0/README.md
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.210297 qlatent-1.0.0/qlatent/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 11:53:41.000000 qlatent-1.0.0/qlatent/__init__.py
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.270297 qlatent-1.0.0/qlatent/qabstract/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:34.000000 qlatent-1.0.0/qlatent/qabstract/__init__.py
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)    21836 2024-03-26 16:23:34.000000 qlatent-1.0.0/qlatent/qabstract/qabstract.py
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.301298 qlatent-1.0.0/qlatent/qcola/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:58.000000 qlatent-1.0.0/qlatent/qcola/__init__.py
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     2582 2024-03-12 08:48:31.000000 qlatent-1.0.0/qlatent/qcola/qcola.py
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.329294 qlatent-1.0.0/qlatent/qmlm/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:04:10.000000 qlatent-1.0.0/qlatent/qmlm/__init__.py
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     5167 2024-03-19 15:32:43.000000 qlatent-1.0.0/qlatent/qmlm/qmlm.py
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.366297 qlatent-1.0.0/qlatent/qmnli/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:46.000000 qlatent-1.0.0/qlatent/qmnli/__init__.py
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     5356 2024-02-25 11:36:15.000000 qlatent-1.0.0/qlatent/qmnli/qmnli.py
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     6219 2024-03-21 09:57:30.000000 qlatent-1.0.0/qlatent/qmnli/utils.py
-drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-02 08:25:34.252296 qlatent-1.0.0/qlatent.egg-info/
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      399 2024-04-02 08:25:33.000000 qlatent-1.0.0/qlatent.egg-info/PKG-INFO
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      428 2024-04-02 08:25:33.000000 qlatent-1.0.0/qlatent.egg-info/SOURCES.txt
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        1 2024-04-02 08:25:33.000000 qlatent-1.0.0/qlatent.egg-info/dependency_links.txt
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      147 2024-04-02 08:25:33.000000 qlatent-1.0.0/qlatent.egg-info/requires.txt
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        8 2024-04-02 08:25:33.000000 qlatent-1.0.0/qlatent.egg-info/top_level.txt
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)       38 2024-04-02 08:25:34.397315 qlatent-1.0.0/setup.cfg
--rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      854 2024-04-02 08:25:21.000000 qlatent-1.0.0/setup.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.273076 qlatent-1.0.1/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)    11357 2024-04-01 12:16:49.000000 qlatent-1.0.1/LICENSE
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      417 2024-05-28 10:05:59.244084 qlatent-1.0.1/PKG-INFO
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     4444 2024-04-01 12:16:49.000000 qlatent-1.0.1/README.md
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.092082 qlatent-1.0.1/qlatent/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 11:53:41.000000 qlatent-1.0.1/qlatent/__init__.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.145081 qlatent-1.0.1/qlatent/qabstract/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:34.000000 qlatent-1.0.1/qlatent/qabstract/__init__.py
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)    23162 2024-04-16 10:18:45.000000 qlatent-1.0.1/qlatent/qabstract/qabstract.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.180082 qlatent-1.0.1/qlatent/qcola/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:58.000000 qlatent-1.0.1/qlatent/qcola/__init__.py
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     2582 2024-03-12 08:48:31.000000 qlatent-1.0.1/qlatent/qcola/qcola.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.188084 qlatent-1.0.1/qlatent/qmlm/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:04:10.000000 qlatent-1.0.1/qlatent/qmlm/__init__.py
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     5167 2024-03-19 15:32:43.000000 qlatent-1.0.1/qlatent/qmlm/qmlm.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.231083 qlatent-1.0.1/qlatent/qmnli/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-04-01 12:03:46.000000 qlatent-1.0.1/qlatent/qmnli/__init__.py
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     5356 2024-02-25 11:36:15.000000 qlatent-1.0.1/qlatent/qmnli/qmnli.py
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)     6219 2024-03-21 09:57:30.000000 qlatent-1.0.1/qlatent/qmnli/utils.py
+drwxr-xr-x   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        0 2024-05-28 10:05:59.239078 qlatent-1.0.1/qlatent.egg-info/
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      417 2024-05-28 10:05:59.000000 qlatent-1.0.1/qlatent.egg-info/PKG-INFO
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      398 2024-05-28 10:05:59.000000 qlatent-1.0.1/qlatent.egg-info/SOURCES.txt
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        1 2024-05-28 10:05:59.000000 qlatent-1.0.1/qlatent.egg-info/dependency_links.txt
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)        8 2024-05-28 10:05:59.000000 qlatent-1.0.1/qlatent.egg-info/top_level.txt
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)       38 2024-05-28 10:05:59.274077 qlatent-1.0.1/setup.cfg
+-rw-r--r--   0 maorreu@auth.ad.bgu.ac.il (1945775059) domain users@auth.ad.bgu.ac.il (1945600513)      589 2024-05-28 10:04:54.000000 qlatent-1.0.1/setup.py
```

### Comparing `qlatent-1.0.0/LICENSE` & `qlatent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qlatent-1.0.0/README.md` & `qlatent-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `qlatent-1.0.0/qlatent/qabstract/qabstract.py` & `qlatent-1.0.1/qlatent/qabstract/qabstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import copy
 from overrides import overrides
 from typing import * 
 from numbers import Number
 import itertools
 from typeguard import check_type
 from functools import partial
+import pingouin as pg
 
 
 SCALE = Dict[str,Number]
 DIMENSIONS = Dict[str,SCALE]
 FILTER = Dict[str,Collection[str]]
 IDXSELECT = Tuple[Union[slice,List[int]]]
 
@@ -447,14 +448,35 @@
 
     
     def print_gradient(self, raw_probabilities=False):
         df = self.to_dataframe(self, raw_probabilities=raw_probabilities)
         cm = sns.light_palette("green", as_cmap=True)
         return df.style.background_gradient(cmap=cm, axis=None)
 
+    
+    def inner_alpha(self, filter:FILTER={}):
+        df = self.to_dataframe(scale=self._scale, index=self._index, filter=filter)
+        if bool(self._filter):
+            indecies_list = self._filter[self._index[0]]
+            dict_items = self._dimensions[self._index[0]].items()
+            matches = [(key, value) for key, value in dict_items if key in indecies_list]
+            default_grouping_df = pd.DataFrame(matches, columns=['name', 'score'])
+        else:
+            default_grouping_df = pd.DataFrame(self._dimensions[self._index[0]].items(), columns=['name', 'score'])
+        grouping = [{self._index[0]: group_df['name'].tolist()} for group_score, group_df in default_grouping_df.groupby('score')]
+        group_scores = pd.DataFrame(self._dimensions[self._index[0]].items(), columns=['name', 'score'])['score']
+        for group in grouping:
+            vals = group[self._index[0]]
+            print(vals, 'Alpha:',pg.cronbach_alpha(data=df.T[vals])[0])
+        if not bool(self._filter):
+            a3 = pg.cronbach_alpha(pd.DataFrame((df.T.to_numpy() * group_scores.to_numpy())))
+            print('Global alpha:', a3[0])
+            return a3[0]
+        return pg.cronbach_alpha(data=df.T[vals])[0]
+        
 
     def report(self,scale:Union[str,int]=None, index:List[str]=None, filters:Dict[str,FILTER]={"unfiltered":{}}, grouping:List[FILTER]=[],):
         scale = self._scale if scale is None else scale
         if not fixed_check_type(scale, str):
             scale = self._field_names.index(scale)
         if index is None:
             if self._index:
@@ -466,15 +488,15 @@
         for label, filter_dict in filters.items():
             print(f"Mean score {label} [{self._weights_flat.min()}..{self._weights_flat.max()}]: {self.mean_score(filter=filter_dict)}")
 
          # Add default grouping for the index field
         if grouping is not None and len(grouping) == 0:
             group_field = index[0]
             grouping = self._create_default_grouping(group_field)
-
+        
         for label, filter_dict in filters.items():
             if self._grouping_suitable_for_consistency_check(grouping, filter=filter_dict):
                 partial_internal_consistency = partial(self.internal_consistency, grouping=grouping,filter=filter_dict, index=index , scale=scale)
                 print(f"Internal consistency (silhouette, correlation) for {label}: {partial_internal_consistency(measure='silhouette_score', metric='correlation')}")
                 print(f"Internal consistency (Calinski&Harabasz)  for {label}: {partial_internal_consistency(measure='calinski_harabasz_score')}")
                 print(f"Internal consistency (Davies&Bouldin) for {label}: {partial_internal_consistency(measure='davies_bouldin_score')}")
             else:
@@ -485,14 +507,16 @@
             display(
               print_gradient(
                   self.to_dataframe(
                     scale=scale,
                     index=index,
                     filter=filter_dict,
             )))
+            self.inner_alpha(filter=filter_dict)
+        
 
 
 class QDELEGATOR(QABSTRACT):
 
     
     def __init__(self, srcobj):
         """
```

### Comparing `qlatent-1.0.0/qlatent/qcola/qcola.py` & `qlatent-1.0.1/qlatent/qcola/qcola.py`

 * *Files identical despite different names*

### Comparing `qlatent-1.0.0/qlatent/qmlm/qmlm.py` & `qlatent-1.0.1/qlatent/qmlm/qmlm.py`

 * *Files identical despite different names*

### Comparing `qlatent-1.0.0/qlatent/qmnli/qmnli.py` & `qlatent-1.0.1/qlatent/qmnli/qmnli.py`

 * *Files identical despite different names*

### Comparing `qlatent-1.0.0/qlatent/qmnli/utils.py` & `qlatent-1.0.1/qlatent/qmnli/utils.py`

 * *Files identical despite different names*

