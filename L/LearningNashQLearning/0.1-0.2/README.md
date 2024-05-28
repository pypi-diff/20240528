# Comparing `tmp/LearningNashQLearning-0.1.tar.gz` & `tmp/LearningNashQLearning-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LearningNashQLearning-0.1.tar", last modified: Tue May 28 09:08:39 2024, max compression
+gzip compressed data, was "LearningNashQLearning-0.2.tar", last modified: Tue May 28 10:12:38 2024, max compression
```

## Comparing `LearningNashQLearning-0.1.tar` & `LearningNashQLearning-0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:08:39.993071 LearningNashQLearning-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-28 09:08:39.960249 LearningNashQLearning-0.1/LearningNashQLearning/
-drwxrwxrwx   0        0        0        0 2024-05-28 09:08:39.979291 LearningNashQLearning-0.1/LearningNashQLearning/Model/
--rw-rw-rw-   0        0        0      888 2024-05-28 08:48:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/Model/Agent.py
--rw-rw-rw-   0        0        0    11859 2024-05-28 08:48:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/Model/Environment.py
--rw-rw-rw-   0        0        0     1232 2024-05-28 08:48:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/Model/History.py
--rw-rw-rw-   0        0        0    27051 2024-05-28 08:48:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/Model/NashQLearning.py
--rw-rw-rw-   0        0        0        0 2024-05-25 16:18:54.000000 LearningNashQLearning-0.1/LearningNashQLearning/Model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:08:39.993071 LearningNashQLearning-0.1/LearningNashQLearning/View/
--rw-rw-rw-   0        0        0     3964 2024-05-25 16:38:41.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/EnvGraphDisplay.py
--rw-rw-rw-   0        0        0    18670 2024-05-25 17:54:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/FinalDisplay.py
--rw-rw-rw-   0        0        0    14709 2024-05-25 16:33:28.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/GameEditor.py
--rw-rw-rw-   0        0        0     3457 2024-05-25 16:32:45.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/GraphClass.py
--rw-rw-rw-   0        0        0    11881 2024-05-28 08:48:57.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/PresetGames.py
--rw-rw-rw-   0        0        0        0 2024-05-25 16:35:10.000000 LearningNashQLearning-0.1/LearningNashQLearning/View/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-25 16:35:28.000000 LearningNashQLearning-0.1/LearningNashQLearning/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:08:39.979291 LearningNashQLearning-0.1/LearningNashQLearning.egg-info/
--rw-rw-rw-   0        0        0       66 2024-05-28 09:08:39.000000 LearningNashQLearning-0.1/LearningNashQLearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2024-05-28 09:08:39.000000 LearningNashQLearning-0.1/LearningNashQLearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:08:39.000000 LearningNashQLearning-0.1/LearningNashQLearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-28 09:08:39.000000 LearningNashQLearning-0.1/LearningNashQLearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2024-05-28 09:08:39.993071 LearningNashQLearning-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-28 09:08:39.993071 LearningNashQLearning-0.1/setup.cfg
--rw-rw-rw-   0        0        0      175 2024-05-25 16:23:24.000000 LearningNashQLearning-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:12:38.277996 LearningNashQLearning-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:12:38.245844 LearningNashQLearning-0.2/LearningNashQLearning/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:12:38.277996 LearningNashQLearning-0.2/LearningNashQLearning/Model/
+-rw-rw-rw-   0        0        0      888 2024-05-28 08:48:57.000000 LearningNashQLearning-0.2/LearningNashQLearning/Model/Agent.py
+-rw-rw-rw-   0        0        0    11859 2024-05-28 08:48:57.000000 LearningNashQLearning-0.2/LearningNashQLearning/Model/Environment.py
+-rw-rw-rw-   0        0        0     1232 2024-05-28 08:48:57.000000 LearningNashQLearning-0.2/LearningNashQLearning/Model/History.py
+-rw-rw-rw-   0        0        0    19290 2024-05-28 09:30:41.000000 LearningNashQLearning-0.2/LearningNashQLearning/Model/NashQLearning.py
+-rw-rw-rw-   0        0        0        0 2024-05-25 16:18:54.000000 LearningNashQLearning-0.2/LearningNashQLearning/Model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:12:38.277996 LearningNashQLearning-0.2/LearningNashQLearning/View/
+-rw-rw-rw-   0        0        0     3964 2024-05-25 16:38:41.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/EnvGraphDisplay.py
+-rw-rw-rw-   0        0        0    18670 2024-05-25 17:54:57.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/FinalDisplay.py
+-rw-rw-rw-   0        0        0    14709 2024-05-25 16:33:28.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/GameEditor.py
+-rw-rw-rw-   0        0        0     3457 2024-05-25 16:32:45.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/GraphClass.py
+-rw-rw-rw-   0        0        0     7825 2024-05-28 09:09:57.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/NashQLearningWidgets.py
+-rw-rw-rw-   0        0        0    11881 2024-05-28 09:30:52.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/PresetGames.py
+-rw-rw-rw-   0        0        0        0 2024-05-25 16:35:10.000000 LearningNashQLearning-0.2/LearningNashQLearning/View/__init__.py
+-rw-rw-rw-   0        0        0       43 2024-05-25 16:35:28.000000 LearningNashQLearning-0.2/LearningNashQLearning/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:12:38.261484 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-05-28 10:12:38.000000 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2024-05-28 10:12:38.000000 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 10:12:38.000000 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-28 10:12:38.000000 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-28 10:12:38.000000 LearningNashQLearning-0.2/LearningNashQLearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      423 2024-05-28 10:12:38.277996 LearningNashQLearning-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-04-15 18:26:09.000000 LearningNashQLearning-0.2/README.md
+-rw-rw-rw-   0        0        0      698 2024-05-28 10:11:45.000000 LearningNashQLearning-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 10:12:38.277996 LearningNashQLearning-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-05-28 10:11:36.000000 LearningNashQLearning-0.2/setup.py
```

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/Model/Agent.py` & `LearningNashQLearning-0.2/LearningNashQLearning/Model/Agent.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/Model/Environment.py` & `LearningNashQLearning-0.2/LearningNashQLearning/Model/Environment.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/Model/History.py` & `LearningNashQLearning-0.2/LearningNashQLearning/Model/History.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/View/EnvGraphDisplay.py` & `LearningNashQLearning-0.2/LearningNashQLearning/View/EnvGraphDisplay.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/View/FinalDisplay.py` & `LearningNashQLearning-0.2/LearningNashQLearning/View/FinalDisplay.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/View/GameEditor.py` & `LearningNashQLearning-0.2/LearningNashQLearning/View/GameEditor.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/View/GraphClass.py` & `LearningNashQLearning-0.2/LearningNashQLearning/View/GraphClass.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning/View/PresetGames.py` & `LearningNashQLearning-0.2/LearningNashQLearning/View/PresetGames.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         ################Game 2####################
         games[2].setPossibleActions(np.array([2, 2]))
 
         games[2].setTransition((0, 0), 0, 1)
         games[2].setPayoff((0, 0), np.array([1,1]))
 
         games[2].setTransition((0, 1), 1, 1)
-        games[2].setPayoff((0, 1), np.array([-1,-2]))
+        games[2].setPayoff((0, 1), np.array([-2,-1]))
 
         games[2].setTransition((1, 0), 2, 1)
         games[2].setPayoff((1, 0), np.array([0,-2]))
 
         games[2].setTransition((1, 1), 2, 1)
         games[2].setPayoff((1, 1), np.array([0,-1]))
 
@@ -323,11 +323,11 @@
         games[3].setTransition((0, 0), 0, 1)
         games[3].setPayoff((0, 0), np.array([1,1]))
 
         games[3].setTransition((0, 1), 3, 1)
         games[3].setPayoff((0, 1), np.array([-2,0]))
 
         games[3].setTransition((1, 0), 1, 1)
-        games[3].setPayoff((1, 0), np.array([-2,-1]))
+        games[3].setPayoff((1, 0), np.array([-1,-2]))
 
         games[3].setTransition((1, 1), 3, 1)
         games[3].setPayoff((1, 1), np.array([-1,0]))
```

### Comparing `LearningNashQLearning-0.1/LearningNashQLearning.egg-info/SOURCES.txt` & `LearningNashQLearning-0.2/LearningNashQLearning.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+README.md
+pyproject.toml
 setup.py
 LearningNashQLearning/__init__.py
 LearningNashQLearning.egg-info/PKG-INFO
 LearningNashQLearning.egg-info/SOURCES.txt
 LearningNashQLearning.egg-info/dependency_links.txt
+LearningNashQLearning.egg-info/requires.txt
 LearningNashQLearning.egg-info/top_level.txt
 LearningNashQLearning/Model/Agent.py
 LearningNashQLearning/Model/Environment.py
 LearningNashQLearning/Model/History.py
 LearningNashQLearning/Model/NashQLearning.py
 LearningNashQLearning/Model/__init__.py
 LearningNashQLearning/View/EnvGraphDisplay.py
 LearningNashQLearning/View/FinalDisplay.py
 LearningNashQLearning/View/GameEditor.py
 LearningNashQLearning/View/GraphClass.py
+LearningNashQLearning/View/NashQLearningWidgets.py
 LearningNashQLearning/View/PresetGames.py
 LearningNashQLearning/View/__init__.py
```

