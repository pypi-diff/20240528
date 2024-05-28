# Comparing `tmp/louvainsplit-0.2.0.2.tar.gz` & `tmp/louvainsplit-0.2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "louvainsplit-0.2.0.2.tar", last modified: Mon May 27 01:43:06 2024, max compression
+gzip compressed data, was "louvainsplit-0.2.0.3.tar", last modified: Tue May 28 15:00:40 2024, max compression
```

## Comparing `louvainsplit-0.2.0.2.tar` & `louvainsplit-0.2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.786962 louvainsplit-0.2.0.2/
--rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.2.0.2/LICENCE
--rw-rw-rw-   0        0        0     5295 2024-05-27 01:43:06.784960 louvainsplit-0.2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4402 2024-05-27 01:41:51.000000 louvainsplit-0.2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.744962 louvainsplit-0.2.0.2/louvainsplit/
--rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.2.0.2/louvainsplit/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.2.0.2/louvainsplit/feature_extraction.py
--rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.2.0.2/louvainsplit/louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.782975 louvainsplit-0.2.0.2/louvainsplit/tests/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.2.0.2/louvainsplit/tests/__init__.py
--rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.2.0.2/louvainsplit/tests/test_louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.783961 louvainsplit-0.2.0.2/louvainsplit.egg-info/
--rw-rw-rw-   0        0        0     5295 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 01:43:06.786962 louvainsplit-0.2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1231 2024-05-27 01:42:08.000000 louvainsplit-0.2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:00:40.799829 louvainsplit-0.2.0.3/
+-rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.2.0.3/LICENCE
+-rw-rw-rw-   0        0        0     5426 2024-05-28 15:00:40.797829 louvainsplit-0.2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4533 2024-05-28 15:00:27.000000 louvainsplit-0.2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 15:00:40.735834 louvainsplit-0.2.0.3/louvainsplit/
+-rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.2.0.3/louvainsplit/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.2.0.3/louvainsplit/feature_extraction.py
+-rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.2.0.3/louvainsplit/louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:00:40.795827 louvainsplit-0.2.0.3/louvainsplit/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.2.0.3/louvainsplit/tests/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.2.0.3/louvainsplit/tests/test_louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:00:40.796832 louvainsplit-0.2.0.3/louvainsplit.egg-info/
+-rw-rw-rw-   0        0        0     5426 2024-05-28 15:00:40.000000 louvainsplit-0.2.0.3/louvainsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-28 15:00:40.000000 louvainsplit-0.2.0.3/louvainsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 15:00:40.000000 louvainsplit-0.2.0.3/louvainsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-28 15:00:40.000000 louvainsplit-0.2.0.3/louvainsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 15:00:40.000000 louvainsplit-0.2.0.3/louvainsplit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 15:00:40.799829 louvainsplit-0.2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2024-05-28 14:13:34.000000 louvainsplit-0.2.0.3/setup.py
```

### Comparing `louvainsplit-0.2.0.2/LICENCE` & `louvainsplit-0.2.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.2/PKG-INFO` & `louvainsplit-0.2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: louvainsplit
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: Efficient graph partitioning using LouvainSplit algorithm
 Home-page: https://github.com/mehrdaddjavadi/louvainsplit
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -18,17 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: torch
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: python-louvain
 
+![LouvainSplit Logo](https://github.com/mehrdaddjavadi/louvainsplit/blob/master/logo.jpg)
+
 # LouvainSplit
 
-LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi.
+LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi, Hossein Aghighi and Mohsen Azadbakht.
 
 ## Abstract
 
 Graph partitioning is essential for uncovering cohesive communities within complex networks. This paper introduces LouvainSplit, an innovative algorithm designed to enhance graph partitioning efficiency and accuracy. LouvainSplit leverages advanced techniques in feature representation, community detection, and evaluation, providing a robust framework for addressing challenges inherent in graph partitioning tasks across diverse domains. At its core, LouvainSplit utilizes a feature pyramid representation approach to extract both basic and summary features from input graphs at multiple granularity levels. This methodology ensures a subtle evaluation of graph data by capturing fundamental graph information alongside intricate structural patterns, thus offering a comprehensive representation of underlying community structures. A key innovation of our approach is the integration of the Louvain algorithm, renowned for its efficacy in community detection. By leveraging pairwise cosine similarities computed from node feature vectors, the Louvain algorithm optimizes modularity iteratively, effectively partitioning graphs into cohesive communities. This iterative process facilitates the identification of significant network structures within complex networks, providing valuable insights into their organizational dynamics. To comprehensively evaluate LouvainSplit's performance, we integrated diverse graph partitioning algorithms, including PyMetis, Genetic Algorithm (GA), DBSCAN, KMeans, OPTICS, and spectral clustering to evaluate the effectiveness of LouvainSplit and using popular evaluation metrics across diverse benchmarks spanning various domains and graphs. The results demonstrate LouvainSplit's superiority in terms of recall score, modularity, and scalability compared to existing methods. Moreover, LouvainSplit maintains competitive average runtime values, ensuring efficient processing even with large-scale datasets.
 
 DOI: [10.21203/rs.3.rs-4301602/v1](https://doi.org/10.21203/rs.3.rs-4301602/v1)
```

### Comparing `louvainsplit-0.2.0.2/README.md` & `louvainsplit-0.2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+![LouvainSplit Logo](https://github.com/mehrdaddjavadi/louvainsplit/blob/master/logo.jpg)
+
 # LouvainSplit
 
-LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi.
+LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi, Hossein Aghighi and Mohsen Azadbakht.
 
 ## Abstract
 
 Graph partitioning is essential for uncovering cohesive communities within complex networks. This paper introduces LouvainSplit, an innovative algorithm designed to enhance graph partitioning efficiency and accuracy. LouvainSplit leverages advanced techniques in feature representation, community detection, and evaluation, providing a robust framework for addressing challenges inherent in graph partitioning tasks across diverse domains. At its core, LouvainSplit utilizes a feature pyramid representation approach to extract both basic and summary features from input graphs at multiple granularity levels. This methodology ensures a subtle evaluation of graph data by capturing fundamental graph information alongside intricate structural patterns, thus offering a comprehensive representation of underlying community structures. A key innovation of our approach is the integration of the Louvain algorithm, renowned for its efficacy in community detection. By leveraging pairwise cosine similarities computed from node feature vectors, the Louvain algorithm optimizes modularity iteratively, effectively partitioning graphs into cohesive communities. This iterative process facilitates the identification of significant network structures within complex networks, providing valuable insights into their organizational dynamics. To comprehensively evaluate LouvainSplit's performance, we integrated diverse graph partitioning algorithms, including PyMetis, Genetic Algorithm (GA), DBSCAN, KMeans, OPTICS, and spectral clustering to evaluate the effectiveness of LouvainSplit and using popular evaluation metrics across diverse benchmarks spanning various domains and graphs. The results demonstrate LouvainSplit's superiority in terms of recall score, modularity, and scalability compared to existing methods. Moreover, LouvainSplit maintains competitive average runtime values, ensuring efficient processing even with large-scale datasets.
 
 DOI: [10.21203/rs.3.rs-4301602/v1](https://doi.org/10.21203/rs.3.rs-4301602/v1)
```

### Comparing `louvainsplit-0.2.0.2/louvainsplit/feature_extraction.py` & `louvainsplit-0.2.0.3/louvainsplit/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.2/louvainsplit/louvain_algorithm.py` & `louvainsplit-0.2.0.3/louvainsplit/louvain_algorithm.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.2/louvainsplit/tests/test_louvain_algorithm.py` & `louvainsplit-0.2.0.3/louvainsplit/tests/test_louvain_algorithm.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.2/louvainsplit.egg-info/PKG-INFO` & `louvainsplit-0.2.0.3/louvainsplit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: louvainsplit
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: Efficient graph partitioning using LouvainSplit algorithm
 Home-page: https://github.com/mehrdaddjavadi/louvainsplit
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -18,17 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: torch
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: python-louvain
 
+![LouvainSplit Logo](https://github.com/mehrdaddjavadi/louvainsplit/blob/master/logo.jpg)
+
 # LouvainSplit
 
-LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi.
+LouvainSplit is a Python package for efficient graph partitioning using the LouvainSplit algorithm, based on the paper by Mehrdad Javadi, Hossein Aghighi and Mohsen Azadbakht.
 
 ## Abstract
 
 Graph partitioning is essential for uncovering cohesive communities within complex networks. This paper introduces LouvainSplit, an innovative algorithm designed to enhance graph partitioning efficiency and accuracy. LouvainSplit leverages advanced techniques in feature representation, community detection, and evaluation, providing a robust framework for addressing challenges inherent in graph partitioning tasks across diverse domains. At its core, LouvainSplit utilizes a feature pyramid representation approach to extract both basic and summary features from input graphs at multiple granularity levels. This methodology ensures a subtle evaluation of graph data by capturing fundamental graph information alongside intricate structural patterns, thus offering a comprehensive representation of underlying community structures. A key innovation of our approach is the integration of the Louvain algorithm, renowned for its efficacy in community detection. By leveraging pairwise cosine similarities computed from node feature vectors, the Louvain algorithm optimizes modularity iteratively, effectively partitioning graphs into cohesive communities. This iterative process facilitates the identification of significant network structures within complex networks, providing valuable insights into their organizational dynamics. To comprehensively evaluate LouvainSplit's performance, we integrated diverse graph partitioning algorithms, including PyMetis, Genetic Algorithm (GA), DBSCAN, KMeans, OPTICS, and spectral clustering to evaluate the effectiveness of LouvainSplit and using popular evaluation metrics across diverse benchmarks spanning various domains and graphs. The results demonstrate LouvainSplit's superiority in terms of recall score, modularity, and scalability compared to existing methods. Moreover, LouvainSplit maintains competitive average runtime values, ensuring efficient processing even with large-scale datasets.
 
 DOI: [10.21203/rs.3.rs-4301602/v1](https://doi.org/10.21203/rs.3.rs-4301602/v1)
```

### Comparing `louvainsplit-0.2.0.2/setup.py` & `louvainsplit-0.2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='louvainsplit',
-    version='0.2.0.2',
+    version='0.2.0.3',
     description='Efficient graph partitioning using LouvainSplit algorithm',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Mehrdad Javadi',
     author_email='mehrdaddjavadi@gmail.com',
     url='https://github.com/mehrdaddjavadi/louvainsplit',
     packages=find_packages(),
```

