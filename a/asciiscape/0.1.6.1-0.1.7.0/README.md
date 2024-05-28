# Comparing `tmp/asciiscape-0.1.6.1.tar.gz` & `tmp/asciiscape-0.1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciiscape-0.1.6.1.tar", max compression
+gzip compressed data, was "asciiscape-0.1.7.0.tar", max compression
```

## Comparing `asciiscape-0.1.6.1.tar` & `asciiscape-0.1.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.6.1/asciiscape/__init__.py
--rw-r--r--   0        0        0      654 2024-05-28 04:12:13.050449 asciiscape-0.1.6.1/asciiscape/__main__.py
--rw-r--r--   0        0        0     4410 2024-05-28 04:10:11.855019 asciiscape-0.1.6.1/asciiscape/console.py
--rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.6.1/asciiscape/imgUtils.py
--rw-r--r--   0        0        0      498 2024-05-28 04:19:53.479265 asciiscape-0.1.6.1/pyproject.toml
--rw-r--r--   0        0        0      274 2024-05-28 04:19:45.904447 asciiscape-0.1.6.1/README.md
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 asciiscape-0.1.6.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.7.0/asciiscape/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-28 04:12:13.050449 asciiscape-0.1.7.0/asciiscape/__main__.py
+-rw-r--r--   0        0        0     4414 2024-05-28 04:58:15.046752 asciiscape-0.1.7.0/asciiscape/console.py
+-rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.7.0/asciiscape/imgUtils.py
+-rw-r--r--   0        0        0      498 2024-05-28 05:00:10.436433 asciiscape-0.1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      274 2024-05-28 04:19:45.904447 asciiscape-0.1.7.0/README.md
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 asciiscape-0.1.7.0/PKG-INFO
```

### Comparing `asciiscape-0.1.6.1/asciiscape/__main__.py` & `asciiscape-0.1.7.0/asciiscape/__main__.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.6.1/asciiscape/console.py` & `asciiscape-0.1.7.0/asciiscape/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         brailleImageArray, brailleImageRGB=iu.imgToAsciiBraille(resizedImageArray, threshold)
         brailleShape=brailleImageArray.shape
         for i in range(brailleShape[0]):
             for j in range(brailleShape[1]):
                 console.print(brailleImageArray[i][j][0], end="")
             print("")
             
-    elif charset=="big" and color==color:
+    elif charset=="big" and color=="color":
         asciiImageArray=iu.imgToAsciiBig(resizedImageArray)
         shape=asciiImageArray.shape
         for i in range(shape[0]):
             for j in range(shape[1]):
                 console.print(asciiImageArray[i][j], end="", style=f"rgb({resizedImageArray[i][j][0]},{resizedImageArray[i][j][1]},{resizedImageArray[i][j][2]})")
             print()
     
@@ -63,15 +63,15 @@
         asciiImageArray=iu.imgToAsciiBig(resizedImageArray)
         shape=asciiImageArray.shape
         for i in range(shape[0]):
             for j in range(shape[1]):
                 console.print(asciiImageArray[i][j], end="")
             print()
             
-    elif charset=="small" and color==color:
+    elif charset=="small" and color=="color":
         asciiImageArray=iu.imgToAsciiSmall(resizedImageArray)
         shape=asciiImageArray.shape
         for i in range(shape[0]):
             for j in range(shape[1]):
                 console.print(asciiImageArray[i][j], end="", style=f"rgb({resizedImageArray[i][j][0]},{resizedImageArray[i][j][1]},{resizedImageArray[i][j][2]})")
             print()
```

### Comparing `asciiscape-0.1.6.1/asciiscape/imgUtils.py` & `asciiscape-0.1.7.0/asciiscape/imgUtils.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.6.1/PKG-INFO` & `asciiscape-0.1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asciiscape
-Version: 0.1.6.1
+Version: 0.1.7.0
 Summary: A simple CLI Python tool for converting image to ASCII textpe
 Author: Lucca Chiguti
 Author-email: luccachbusiness@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

