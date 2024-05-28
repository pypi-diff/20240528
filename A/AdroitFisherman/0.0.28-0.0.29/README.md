# Comparing `tmp/AdroitFisherman-0.0.28.tar.gz` & `tmp/AdroitFisherman-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.28.tar", last modified: Sun May 26 11:35:53 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.29.tar", last modified: Tue May 28 13:24:41 2024, max compression
```

## Comparing `AdroitFisherman-0.0.28.tar` & `AdroitFisherman-0.0.29.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.933450 AdroitFisherman-0.0.28/
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.840915 AdroitFisherman-0.0.28/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.894552 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/
--rw-rw-rw-   0        0        0      707 2024-05-26 11:34:28.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/Base64Util.py
--rw-rw-rw-   0        0        0     1034 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/CircularSingleLinkedList.py
--rw-rw-rw-   0        0        0     1174 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/DoubleLinkedList.py
--rw-rw-rw-   0        0        0      860 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SequentialList.py
--rw-rw-rw-   0        0        0     1000 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SingleLinkedList.py
--rw-rw-rw-   0        0        0     1039 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
--rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.897546 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/__pycache__/
--rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
--rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.28/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.28/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.898541 AdroitFisherman-0.0.28/AdroitFisherman/__pycache__/
--rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.28/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.932482 AdroitFisherman-0.0.28/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      588 2024-05-26 02:00:28.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/Base64Util.c
--rw-rw-rw-   0        0        0     6779 2024-05-26 11:05:55.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/Base64Util.h
--rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/CircularSingleLinkedList.c
--rw-rw-rw-   0        0        0     8594 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/CircularSingleLinkedList.h
--rw-rw-rw-   0        0        0     1103 2024-05-11 09:23:06.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/DoubleLinkedList.c
--rw-rw-rw-   0        0        0     9854 2024-05-11 09:37:50.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/DoubleLinkedList.h
--rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5179 2024-05-11 09:55:01.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SeqList.h
--rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedList.c
--rw-rw-rw-   0        0        0     8383 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedList.h
--rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
--rw-rw-rw-   0        0        0     9370 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
-drwxrwxrwx   0        0        0        0 2024-05-26 11:35:53.853880 AdroitFisherman-0.0.28/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-05-26 11:35:53.000000 AdroitFisherman-0.0.28/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1556 2024-05-26 11:35:53.000000 AdroitFisherman-0.0.28/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:35:53.000000 AdroitFisherman-0.0.28/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-26 11:35:53.000000 AdroitFisherman-0.0.28/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.28/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-05-26 11:35:53.934467 AdroitFisherman-0.0.28/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-26 11:35:48.000000 AdroitFisherman-0.0.28/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 11:35:53.935474 AdroitFisherman-0.0.28/setup.cfg
--rw-rw-rw-   0        0        0     1886 2024-05-26 11:32:05.000000 AdroitFisherman-0.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.520698 AdroitFisherman-0.0.29/
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.410991 AdroitFisherman-0.0.29/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.480804 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0      707 2024-05-26 11:34:28.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/Base64Util.py
+-rw-rw-rw-   0        0        0     1034 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/CircularSingleLinkedList.py
+-rw-rw-rw-   0        0        0     1174 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/DoubleLinkedList.py
+-rw-rw-rw-   0        0        0      860 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0     1000 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0     1039 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.483797 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
+-rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.29/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.484794 AdroitFisherman-0.0.29/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.29/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.519700 AdroitFisherman-0.0.29/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      588 2024-05-26 02:00:28.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.c
+-rw-rw-rw-   0        0        0     6747 2024-05-28 13:24:34.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.h
+-rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.c
+-rw-rw-rw-   0        0        0     8594 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.h
+-rw-rw-rw-   0        0        0     1103 2024-05-11 09:23:06.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.c
+-rw-rw-rw-   0        0        0     9854 2024-05-11 09:37:50.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.h
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5179 2024-05-11 09:55:01.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8383 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.h
+-rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+-rw-rw-rw-   0        0        0     9370 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
+drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.426947 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.29/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-05-28 13:24:41.520698 AdroitFisherman-0.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-26 11:35:48.000000 AdroitFisherman-0.0.29/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:24:41.521695 AdroitFisherman-0.0.29/setup.cfg
+-rw-rw-rw-   0        0        0     1886 2024-05-28 13:24:34.000000 AdroitFisherman-0.0.29/setup.py
```

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/Base64Util.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/Base64Util.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/CircularSingleLinkedList.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/CircularSingleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/DoubleLinkedList.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/DoubleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SequentialList.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SequentialList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SingleLinkedList.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc` & `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/Base64Util.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/Base64Util.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.h`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,14 @@
 			if(temp==0)
 			{
 			    self->data[i]=0;
 			}
 			self->data[counter++] = temp;
 		}
 		self->data[counter] = '\0';
-		printf("\n%s\n",self->data);
 		PyObject* result = Py_BuildValue("y",self->data);
 		Py_INCREF(result);
 		return result;
 	}
 }
 static PyObject* GetEncryptData(Base64block* self)
 {
```

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/CircularSingleLinkedList.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/CircularSingleLinkedList.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/DoubleLinkedList.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/DoubleLinkedList.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedList.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedList.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h` & `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.29/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.28
+Version: 0.0.29
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.28/AdroitFisherman.egg-info/SOURCES.txt` & `AdroitFisherman-0.0.29/AdroitFisherman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.28/PKG-INFO` & `AdroitFisherman-0.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.28
+Version: 0.0.29
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.28/setup.py` & `AdroitFisherman-0.0.29/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SingleLinkedListWithoutHeadNode=Extension("AdroitFisherman.SingleLinkedListWithoutHeadNode",sources=['AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c'])
 CircularSingleLinkedList=Extension("AdroitFisherman.CircularSingleLinkedList",sources=['AdroitFisherman/includes/CircularSingleLinkedList.c'])
 DoubleLinkedList=Extension("AdroitFisherman.DoubleLinkedList",sources=['AdroitFisherman/includes/DoubleLinkedList.c'])
 Base64=Extension("AdroitFisherman.Base64Utility",sources=['AdroitFisherman/includes/Base64Util.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.28",
+    version="0.0.29",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
```

