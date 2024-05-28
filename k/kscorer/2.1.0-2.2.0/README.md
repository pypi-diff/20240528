# Comparing `tmp/kscorer-2.1.0.tar.gz` & `tmp/kscorer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscorer-2.1.0.tar", last modified: Fri Oct 27 13:01:32 2023, max compression
+gzip compressed data, was "kscorer-2.2.0.tar", last modified: Tue May 28 08:16:09 2024, max compression
```

## Comparing `kscorer-2.1.0.tar` & `kscorer-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 13:01:32.006479 kscorer-2.1.0/
--rw-rw-rw-   0        0        0    35823 2023-09-21 07:31:18.000000 kscorer-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    45595 2023-10-27 13:01:32.004479 kscorer-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3569 2023-10-27 12:59:23.000000 kscorer-2.1.0/README.md
--rw-rw-rw-   0        0        0     1451 2023-10-27 13:01:12.000000 kscorer-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-27 13:01:32.006479 kscorer-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-27 13:01:31.987951 kscorer-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-10-27 13:01:31.996175 kscorer-2.1.0/src/kscorer/
--rw-rw-rw-   0        0        0       23 2023-10-27 13:01:12.000000 kscorer-2.1.0/src/kscorer/__init__.py
--rw-rw-rw-   0        0        0    12214 2023-10-27 12:59:46.000000 kscorer-2.1.0/src/kscorer/kscorer.py
--rw-rw-rw-   0        0        0     2454 2023-10-25 08:54:44.000000 kscorer-2.1.0/src/kscorer/pmixin.py
-drwxrwxrwx   0        0        0        0 2023-10-27 13:01:32.002477 kscorer-2.1.0/src/kscorer.egg-info/
--rw-rw-rw-   0        0        0    45595 2023-10-27 13:01:31.000000 kscorer-2.1.0/src/kscorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-10-27 13:01:31.000000 kscorer-2.1.0/src/kscorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 13:01:31.000000 kscorer-2.1.0/src/kscorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-10-27 13:01:31.000000 kscorer-2.1.0/src/kscorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-27 13:01:31.000000 kscorer-2.1.0/src/kscorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 08:16:09.819154 kscorer-2.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-09-21 07:31:18.000000 kscorer-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    45900 2024-05-28 08:16:09.817154 kscorer-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3817 2023-11-06 21:29:59.000000 kscorer-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1601 2024-05-28 08:15:45.000000 kscorer-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:16:09.819154 kscorer-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 08:16:09.793152 kscorer-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:16:09.803154 kscorer-2.2.0/src/kscorer/
+-rw-rw-rw-   0        0        0       23 2024-05-28 08:15:45.000000 kscorer-2.2.0/src/kscorer/__init__.py
+-rw-rw-rw-   0        0        0    12502 2024-05-28 07:40:14.000000 kscorer-2.2.0/src/kscorer/kscorer.py
+-rw-rw-rw-   0        0        0     2454 2023-10-25 08:54:44.000000 kscorer-2.2.0/src/kscorer/pmixin.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:16:09.815156 kscorer-2.2.0/src/kscorer.egg-info/
+-rw-rw-rw-   0        0        0    45900 2024-05-28 08:16:09.000000 kscorer-2.2.0/src/kscorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-28 08:16:09.000000 kscorer-2.2.0/src/kscorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:16:09.000000 kscorer-2.2.0/src/kscorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-28 08:16:09.000000 kscorer-2.2.0/src/kscorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-28 08:16:09.000000 kscorer-2.2.0/src/kscorer.egg-info/top_level.txt
```

### Comparing `kscorer-2.1.0/LICENSE` & `kscorer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kscorer-2.1.0/PKG-INFO` & `kscorer-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscorer
-Version: 2.1.0
+Version: 2.2.0
 Summary: Auto-select optimal K-means clusters with advanced scoring
 Author-email: Volodymyr Holomb <wldmrgml@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,14 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Source, https://github.com/woldemarg/kscorer
+Project-URL: Home, https://github.com/woldemarg/kscorer
 Project-URL: Author, https://www.linkedin.com/in/vholomb
 Keywords: visualization,analysis,clustering
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
@@ -693,14 +694,17 @@
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: seaborn>=0.12
 Requires-Dist: tqdm>=4.66.1
 
 KScorer: Auto-select optimal K-means clusters with advanced scoring
 
 ### Basic Usage
+
+> LIVE demo-notebook is [here](https://jovian.com/wldmrgml/kscorer-demo)
+
 #### Load Modules
 ```python
 In [1]: import numpy as np
    ...: import pandas as pd
    ...: from sklearn import datasets
    ...: from sklearn.metrics import balanced_accuracy_score
    ...: from sklearn.model_selection import train_test_split
@@ -739,23 +743,24 @@
 #### Confusion Matrix
 ```python
 In [8]: labels_mtx = (pd.Series(y_train)
    ...:               .groupby([labels, y_train])
    ...:               .count()
    ...:               .unstack()
    ...:               .fillna(0))
-   ...: # match arbitrary labely to ground-truth labels
+   ...: # match arbitrary labels to ground-truth labels
    ...: order = []
    ...: 
    ...: for i, r in labels_mtx.iterrows():
    ...:     left = [x for x in np.unique(y_train) if x not in order]
    ...:     order.append(r.iloc[left].idxmax())
    ...: 
    ...: confusion_mtx = labels_mtx[order]
    ...: confusion_mtx
+Out[8]:
 ```
 |   	| 5     	| 9    	| 4     	| 2     	| 0     	| 6     	| 1    	| 7     	| 8    	| 3    	|
 |---	|-------	|------	|-------	|-------	|-------	|-------	|------	|-------	|------	|------	|
 | 0 	| 124.0 	| 5.0  	| 1.0   	| 0.0   	| 0.0   	| 0.0   	| 2.0  	| 7.0   	| 4.0  	| 2.0  	|
 | 1 	| 12.0  	| 95.0 	| 0.0   	| 0.0   	| 0.0   	| 0.0   	| 0.0  	| 0.0   	| 9.0  	| 90.0 	|
 | 2 	| 2.0   	| 0.0  	| 122.0 	| 0.0   	| 1.0   	| 2.0   	| 0.0  	| 1.0   	| 0.0  	| 0.0  	|
 | 3 	| 0.0   	| 0.0  	| 0.0   	| 108.0 	| 0.0   	| 0.0   	| 22.0 	| 0.0   	| 1.0  	| 20.0 	|
@@ -780,11 +785,13 @@
 ```
 ```python
 In [12]: balanced_accuracy_score(y_test, y_unseen)  # unseen data
 Out[12]: 0.646615365026082
 ```
 ___
 
-#### ToDo:
-- apply power-transform before initial scaling-
+### ToDo:
+- consider applying power-transform before initial scaling
 - consider [pyckmeans](https://pypi.org/project/pyckmeans)
 - consider [pyxmeans](https://github.com/mynameisfiber/pyxmeans)
+- consider [spherecluster](https://github.com/jasonlaska/spherecluster)
+- consider [benchmark testing](https://stackoverflow.com/a/53343336/6025592)
```

### Comparing `kscorer-2.1.0/README.md` & `kscorer-2.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 KScorer: Auto-select optimal K-means clusters with advanced scoring
 
 ### Basic Usage
+
+> LIVE demo-notebook is [here](https://jovian.com/wldmrgml/kscorer-demo)
+
 #### Load Modules
 ```python
 In [1]: import numpy as np
    ...: import pandas as pd
    ...: from sklearn import datasets
    ...: from sklearn.metrics import balanced_accuracy_score
    ...: from sklearn.model_selection import train_test_split
@@ -43,23 +46,24 @@
 #### Confusion Matrix
 ```python
 In [8]: labels_mtx = (pd.Series(y_train)
    ...:               .groupby([labels, y_train])
    ...:               .count()
    ...:               .unstack()
    ...:               .fillna(0))
-   ...: # match arbitrary labely to ground-truth labels
+   ...: # match arbitrary labels to ground-truth labels
    ...: order = []
    ...: 
    ...: for i, r in labels_mtx.iterrows():
    ...:     left = [x for x in np.unique(y_train) if x not in order]
    ...:     order.append(r.iloc[left].idxmax())
    ...: 
    ...: confusion_mtx = labels_mtx[order]
    ...: confusion_mtx
+Out[8]:
 ```
 |   	| 5     	| 9    	| 4     	| 2     	| 0     	| 6     	| 1    	| 7     	| 8    	| 3    	|
 |---	|-------	|------	|-------	|-------	|-------	|-------	|------	|-------	|------	|------	|
 | 0 	| 124.0 	| 5.0  	| 1.0   	| 0.0   	| 0.0   	| 0.0   	| 2.0  	| 7.0   	| 4.0  	| 2.0  	|
 | 1 	| 12.0  	| 95.0 	| 0.0   	| 0.0   	| 0.0   	| 0.0   	| 0.0  	| 0.0   	| 9.0  	| 90.0 	|
 | 2 	| 2.0   	| 0.0  	| 122.0 	| 0.0   	| 1.0   	| 2.0   	| 0.0  	| 1.0   	| 0.0  	| 0.0  	|
 | 3 	| 0.0   	| 0.0  	| 0.0   	| 108.0 	| 0.0   	| 0.0   	| 22.0 	| 0.0   	| 1.0  	| 20.0 	|
@@ -84,11 +88,13 @@
 ```
 ```python
 In [12]: balanced_accuracy_score(y_test, y_unseen)  # unseen data
 Out[12]: 0.646615365026082
 ```
 ___
 
-#### ToDo:
-- apply power-transform before initial scaling-
+### ToDo:
+- consider applying power-transform before initial scaling
 - consider [pyckmeans](https://pypi.org/project/pyckmeans)
-- consider [pyxmeans](https://github.com/mynameisfiber/pyxmeans)
+- consider [pyxmeans](https://github.com/mynameisfiber/pyxmeans)
+- consider [spherecluster](https://github.com/jasonlaska/spherecluster)
+- consider [benchmark testing](https://stackoverflow.com/a/53343336/6025592)
```

### Comparing `kscorer-2.1.0/src/kscorer/kscorer.py` & `kscorer-2.2.0/src/kscorer/kscorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self.peak_scores_ = None
         self.ranked_ = None
         self.scores_ = None
         self.scaler_before_pca = None
         self.pca = None
         self.scaler_after_pca = None
         self.res_ = None
+        self.feature_names_in_ = None
 
     @staticmethod
     def _find_knee(*args):
 
         # https://pypi.org/project/kneefinder/
         # https://github.com/arvkevi/kneed
 
@@ -285,15 +286,17 @@
         return X_scaled
 
     def fit(self,
             data: np.array,
             *args,
             **kwargs):
 
-        data = data.values if isinstance(data, pd.DataFrame) else data
+        if isinstance(data, pd.DataFrame):
+            self.feature_names_in_ = data.columns.to_list()
+            data = data.values
 
         sample = data[next(self._cv_gen(data, self.random_state))]
 
         # https://scikit-learn.org/stable/auto_examples/preprocessing/plot_scaling_importance.html
         preferred_scaling, n_components = self._choose_scaler_and_pca(sample)
 
         data_scaled = self._fit_scaler_and_pca(
@@ -385,14 +388,16 @@
         data = data.values if isinstance(data, pd.DataFrame) else data
 
         n_clusters = n_clusters if n_clusters else self.optimal_
 
         if n_clusters:
 
             # https://datascience.stackexchange.com/a/36003/101016
+            # https://medium.com/ai-for-real/relationship-between-cosine-similarity-and-euclidean-distance-7e283a277dff
+            # https://stats.stackexchange.com/q/146221/363056
             X_scaled = normalize(
                 self.scaler_after_pca.transform(
                     self.pca.transform(
                         self.scaler_before_pca.transform(
                             data))))
 
             res = self.kmeans_clustering(
```

### Comparing `kscorer-2.1.0/src/kscorer/pmixin.py` & `kscorer-2.2.0/src/kscorer/pmixin.py`

 * *Files identical despite different names*

### Comparing `kscorer-2.1.0/src/kscorer.egg-info/PKG-INFO` & `kscorer-2.2.0/src/kscorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscorer
-Version: 2.1.0
+Version: 2.2.0
 Summary: Auto-select optimal K-means clusters with advanced scoring
 Author-email: Volodymyr Holomb <wldmrgml@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,14 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Source, https://github.com/woldemarg/kscorer
+Project-URL: Home, https://github.com/woldemarg/kscorer
 Project-URL: Author, https://www.linkedin.com/in/vholomb
 Keywords: visualization,analysis,clustering
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
@@ -693,14 +694,17 @@
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: seaborn>=0.12
 Requires-Dist: tqdm>=4.66.1
 
 KScorer: Auto-select optimal K-means clusters with advanced scoring
 
 ### Basic Usage
+
+> LIVE demo-notebook is [here](https://jovian.com/wldmrgml/kscorer-demo)
+
 #### Load Modules
 ```python
 In [1]: import numpy as np
    ...: import pandas as pd
    ...: from sklearn import datasets
    ...: from sklearn.metrics import balanced_accuracy_score
    ...: from sklearn.model_selection import train_test_split
@@ -739,23 +743,24 @@
 #### Confusion Matrix
 ```python
 In [8]: labels_mtx = (pd.Series(y_train)
    ...:               .groupby([labels, y_train])
    ...:               .count()
    ...:               .unstack()
    ...:               .fillna(0))
-   ...: # match arbitrary labely to ground-truth labels
+   ...: # match arbitrary labels to ground-truth labels
    ...: order = []
    ...: 
    ...: for i, r in labels_mtx.iterrows():
    ...:     left = [x for x in np.unique(y_train) if x not in order]
    ...:     order.append(r.iloc[left].idxmax())
    ...: 
    ...: confusion_mtx = labels_mtx[order]
    ...: confusion_mtx
+Out[8]:
 ```
 |   	| 5     	| 9    	| 4     	| 2     	| 0     	| 6     	| 1    	| 7     	| 8    	| 3    	|
 |---	|-------	|------	|-------	|-------	|-------	|-------	|------	|-------	|------	|------	|
 | 0 	| 124.0 	| 5.0  	| 1.0   	| 0.0   	| 0.0   	| 0.0   	| 2.0  	| 7.0   	| 4.0  	| 2.0  	|
 | 1 	| 12.0  	| 95.0 	| 0.0   	| 0.0   	| 0.0   	| 0.0   	| 0.0  	| 0.0   	| 9.0  	| 90.0 	|
 | 2 	| 2.0   	| 0.0  	| 122.0 	| 0.0   	| 1.0   	| 2.0   	| 0.0  	| 1.0   	| 0.0  	| 0.0  	|
 | 3 	| 0.0   	| 0.0  	| 0.0   	| 108.0 	| 0.0   	| 0.0   	| 22.0 	| 0.0   	| 1.0  	| 20.0 	|
@@ -780,11 +785,13 @@
 ```
 ```python
 In [12]: balanced_accuracy_score(y_test, y_unseen)  # unseen data
 Out[12]: 0.646615365026082
 ```
 ___
 
-#### ToDo:
-- apply power-transform before initial scaling-
+### ToDo:
+- consider applying power-transform before initial scaling
 - consider [pyckmeans](https://pypi.org/project/pyckmeans)
 - consider [pyxmeans](https://github.com/mynameisfiber/pyxmeans)
+- consider [spherecluster](https://github.com/jasonlaska/spherecluster)
+- consider [benchmark testing](https://stackoverflow.com/a/53343336/6025592)
```

