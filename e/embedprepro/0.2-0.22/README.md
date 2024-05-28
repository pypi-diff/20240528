# Comparing `tmp/embedprepro-0.2.tar.gz` & `tmp/embedprepro-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedprepro-0.2.tar", last modified: Sun May 26 15:29:49 2024, max compression
+gzip compressed data, was "embedprepro-0.22.tar", last modified: Tue May 28 14:39:34 2024, max compression
```

## Comparing `embedprepro-0.2.tar` & `embedprepro-0.22.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.363268 embedprepro-0.2/
--rw-r--r--   0 eier       (501) staff       (20)     5473 2024-05-26 15:29:49.362603 embedprepro-0.2/PKG-INFO
--rw-r--r--   0 eier       (501) staff       (20)     5379 2024-05-26 15:22:25.000000 embedprepro-0.2/README.md
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.353047 embedprepro-0.2/embedprepro.egg-info/
--rw-r--r--   0 eier       (501) staff       (20)     5473 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/PKG-INFO
--rw-r--r--   0 eier       (501) staff       (20)      435 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/SOURCES.txt
--rw-r--r--   0 eier       (501) staff       (20)        1 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/dependency_links.txt
--rw-r--r--   0 eier       (501) staff       (20)       54 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/entry_points.txt
--rw-r--r--   0 eier       (501) staff       (20)      769 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/requires.txt
--rw-r--r--   0 eier       (501) staff       (20)       14 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/top_level.txt
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.361388 embedprepro-0.2/preprocessing/
--rw-r--r--   0 eier       (501) staff       (20)        0 2024-05-25 20:53:37.000000 embedprepro-0.2/preprocessing/__init__.py
--rw-r--r--   0 eier       (501) staff       (20)     8560 2024-05-25 22:54:06.000000 embedprepro-0.2/preprocessing/agglomerative_clustering.py
--rw-r--r--   0 eier       (501) staff       (20)     6168 2024-05-26 12:50:08.000000 embedprepro-0.2/preprocessing/cli.py
--rw-r--r--   0 eier       (501) staff       (20)     8067 2024-05-25 23:33:31.000000 embedprepro-0.2/preprocessing/dimensionality_reduction.py
--rw-r--r--   0 eier       (501) staff       (20)     2028 2024-05-25 13:21:15.000000 embedprepro-0.2/preprocessing/embedding_service.py
--rw-r--r--   0 eier       (501) staff       (20)     3509 2024-05-26 12:37:01.000000 embedprepro-0.2/preprocessing/visualization_service.py
--rw-r--r--   0 eier       (501) staff       (20)       38 2024-05-26 15:29:49.363479 embedprepro-0.2/setup.cfg
--rw-r--r--   0 eier       (501) staff       (20)     1633 2024-05-26 15:29:00.000000 embedprepro-0.2/setup.py
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-28 14:39:34.538496 embedprepro-0.22/
+-rw-r--r--   0 eier       (501) staff       (20)     5803 2024-05-28 14:39:34.537627 embedprepro-0.22/PKG-INFO
+-rw-r--r--   0 eier       (501) staff       (20)     5603 2024-05-28 14:30:40.000000 embedprepro-0.22/README.md
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-28 14:39:34.524664 embedprepro-0.22/embedprepro.egg-info/
+-rw-r--r--   0 eier       (501) staff       (20)     5803 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/PKG-INFO
+-rw-r--r--   0 eier       (501) staff       (20)      435 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/SOURCES.txt
+-rw-r--r--   0 eier       (501) staff       (20)        1 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/dependency_links.txt
+-rw-r--r--   0 eier       (501) staff       (20)       54 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/entry_points.txt
+-rw-r--r--   0 eier       (501) staff       (20)      154 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/requires.txt
+-rw-r--r--   0 eier       (501) staff       (20)       14 2024-05-28 14:39:34.000000 embedprepro-0.22/embedprepro.egg-info/top_level.txt
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-28 14:39:34.536355 embedprepro-0.22/preprocessing/
+-rw-r--r--   0 eier       (501) staff       (20)        0 2024-05-25 20:53:37.000000 embedprepro-0.22/preprocessing/__init__.py
+-rw-r--r--   0 eier       (501) staff       (20)     8560 2024-05-25 22:54:06.000000 embedprepro-0.22/preprocessing/agglomerative_clustering.py
+-rw-r--r--   0 eier       (501) staff       (20)     6169 2024-05-26 22:01:12.000000 embedprepro-0.22/preprocessing/cli.py
+-rw-r--r--   0 eier       (501) staff       (20)     8067 2024-05-25 23:33:31.000000 embedprepro-0.22/preprocessing/dimensionality_reduction.py
+-rw-r--r--   0 eier       (501) staff       (20)     2028 2024-05-25 13:21:15.000000 embedprepro-0.22/preprocessing/embedding_service.py
+-rw-r--r--   0 eier       (501) staff       (20)     3509 2024-05-26 12:37:01.000000 embedprepro-0.22/preprocessing/visualization_service.py
+-rw-r--r--   0 eier       (501) staff       (20)       38 2024-05-28 14:39:34.538708 embedprepro-0.22/setup.cfg
+-rw-r--r--   0 eier       (501) staff       (20)      734 2024-05-28 14:38:41.000000 embedprepro-0.22/setup.py
```

### Comparing `embedprepro-0.2/PKG-INFO` & `embedprepro-0.22/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 Metadata-Version: 2.1
 Name: embedprepro
-Version: 0.2
+Version: 0.22
+Home-page: https://github.com/Elma-dev/embedprepro-lib.git/
+Author-email: elmajjodi.abdeljalil@gmail.com
 Description-Content-Type: text/markdown
 
 # Library
 <p align="center">
-    <img src="https://github.com/Elma-dev/embedprepro-lib/assets/67378945/eac85a48-54ed-4e90-8ce4-faddf1c2a7a2" width="250" height="250">
+    <img src="images/logo.png" width="250" height="250">
     
 </p>
 
 `embedprepro` is a command-line tool designed for text analysis tasks, including embedding, clustering, dimensionality reduction, and visualization. This tool leverages various machine learning and data processing techniques to provide a comprehensive solution for text data analysis.
+<p align="center">
+    <img src="images/img.png">
+</p>
 
-![image](https://github.com/Elma-dev/embedprepro-lib/assets/67378945/766c902d-9281-4baa-8996-10c9b3cd5df9)
+## Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Command-line Interface](#command-line-interface)
+    - [Embedding](#embedding)
+    - [Dimensionality Reduction](#dimensionality-reduction)
+    - [Clustering](#clustering)
+    - [Visualization](#visualization)
+  - [Importing in Your Project](#python-project)
 
 # **Installation**
 
 You can install the package directly using pip:
 
 ```
-!pip install -U embedprepro==0.1
+!pip install -U embedprepro
 ```
 
 If you prefer to install the package from the source, clone the repository and install it using pip:
 
 ```
-
-git clone https://github.com/
+git clone https://github.com/Elma-dev/embedprepro-lib.git
 cd text_analysis_cli
 pip install .
 ```
 
 # **Usage**
 
 ## **Command-line Interface**
```

### Comparing `embedprepro-0.2/README.md` & `embedprepro-0.22/embedprepro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,48 @@
+Metadata-Version: 2.1
+Name: embedprepro
+Version: 0.22
+Home-page: https://github.com/Elma-dev/embedprepro-lib.git/
+Author-email: elmajjodi.abdeljalil@gmail.com
+Description-Content-Type: text/markdown
+
 # Library
 <p align="center">
-    <img src="https://github.com/Elma-dev/embedprepro-lib/assets/67378945/eac85a48-54ed-4e90-8ce4-faddf1c2a7a2" width="250" height="250">
+    <img src="images/logo.png" width="250" height="250">
     
 </p>
 
 `embedprepro` is a command-line tool designed for text analysis tasks, including embedding, clustering, dimensionality reduction, and visualization. This tool leverages various machine learning and data processing techniques to provide a comprehensive solution for text data analysis.
+<p align="center">
+    <img src="images/img.png">
+</p>
 
-![image](https://github.com/Elma-dev/embedprepro-lib/assets/67378945/766c902d-9281-4baa-8996-10c9b3cd5df9)
+## Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Command-line Interface](#command-line-interface)
+    - [Embedding](#embedding)
+    - [Dimensionality Reduction](#dimensionality-reduction)
+    - [Clustering](#clustering)
+    - [Visualization](#visualization)
+  - [Importing in Your Project](#python-project)
 
 # **Installation**
 
 You can install the package directly using pip:
 
 ```
-!pip install -U embedprepro==0.1
+!pip install -U embedprepro
 ```
 
 If you prefer to install the package from the source, clone the repository and install it using pip:
 
 ```
-
-git clone https://github.com/
+git clone https://github.com/Elma-dev/embedprepro-lib.git
 cd text_analysis_cli
 pip install .
 ```
 
 # **Usage**
 
 ## **Command-line Interface**
```

### Comparing `embedprepro-0.2/embedprepro.egg-info/PKG-INFO` & `embedprepro-0.22/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-Metadata-Version: 2.1
-Name: embedprepro
-Version: 0.2
-Description-Content-Type: text/markdown
-
 # Library
 <p align="center">
-    <img src="https://github.com/Elma-dev/embedprepro-lib/assets/67378945/eac85a48-54ed-4e90-8ce4-faddf1c2a7a2" width="250" height="250">
+    <img src="images/logo.png" width="250" height="250">
     
 </p>
 
 `embedprepro` is a command-line tool designed for text analysis tasks, including embedding, clustering, dimensionality reduction, and visualization. This tool leverages various machine learning and data processing techniques to provide a comprehensive solution for text data analysis.
+<p align="center">
+    <img src="images/img.png">
+</p>
 
-![image](https://github.com/Elma-dev/embedprepro-lib/assets/67378945/766c902d-9281-4baa-8996-10c9b3cd5df9)
+## Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Command-line Interface](#command-line-interface)
+    - [Embedding](#embedding)
+    - [Dimensionality Reduction](#dimensionality-reduction)
+    - [Clustering](#clustering)
+    - [Visualization](#visualization)
+  - [Importing in Your Project](#python-project)
 
 # **Installation**
 
 You can install the package directly using pip:
 
 ```
-!pip install -U embedprepro==0.1
+!pip install -U embedprepro
 ```
 
 If you prefer to install the package from the source, clone the repository and install it using pip:
 
 ```
-
-git clone https://github.com/
+git clone https://github.com/Elma-dev/embedprepro-lib.git
 cd text_analysis_cli
 pip install .
 ```
 
 # **Usage**
 
 ## **Command-line Interface**
```

### Comparing `embedprepro-0.2/preprocessing/agglomerative_clustering.py` & `embedprepro-0.22/preprocessing/agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.2/preprocessing/cli.py` & `embedprepro-0.22/preprocessing/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,9 @@
     if zi==-1:
         visualizer.plot_2d(clusters=np.load(clusters_data, allow_pickle=True))
     else:
         visualizer.plot_3d(clusters=np.load(clusters_data,allow_pickle=True))
 
 
 if __name__ == "__main__":
+
     cli()
```

### Comparing `embedprepro-0.2/preprocessing/dimensionality_reduction.py` & `embedprepro-0.22/preprocessing/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.2/preprocessing/embedding_service.py` & `embedprepro-0.22/preprocessing/embedding_service.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.2/preprocessing/visualization_service.py` & `embedprepro-0.22/preprocessing/visualization_service.py`

 * *Files identical despite different names*

