# Comparing `tmp/cvprocessor-1.0.5.tar.gz` & `tmp/cvprocessor-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-1.0.5.tar", last modified: Sat May 25 01:48:55 2024, max compression
+gzip compressed data, was "cvprocessor-1.0.6.tar", last modified: Tue May 28 07:45:41 2024, max compression
```

## Comparing `cvprocessor-1.0.5.tar` & `cvprocessor-1.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.936982 cvprocessor-1.0.5/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-1.0.5/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-25 01:48:55.936514 cvprocessor-1.0.5/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-1.0.5/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-25 01:46:39.000000 cvprocessor-1.0.5/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-25 01:48:55.937062 cvprocessor-1.0.5/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.910177 cvprocessor-1.0.5/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.927315 cvprocessor-1.0.5/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-1.0.5/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     4365 2024-05-21 06:21:00.000000 cvprocessor-1.0.5/src/cvprocessor/authors.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.929999 cvprocessor-1.0.5/src/cvprocessor/contact/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:11:09.000000 cvprocessor-1.0.5/src/cvprocessor/contact/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     3497 2024-05-21 02:03:19.000000 cvprocessor-1.0.5/src/cvprocessor/contact/contact.py
--rw-r--r--   0 fernando   (501) staff       (20)     7749 2024-05-20 00:37:00.000000 cvprocessor-1.0.5/src/cvprocessor/cv.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.930795 cvprocessor-1.0.5/src/cvprocessor/date/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-18 23:14:35.000000 cvprocessor-1.0.5/src/cvprocessor/date/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     3445 2024-05-19 09:59:29.000000 cvprocessor-1.0.5/src/cvprocessor/date/date.py
--rw-r--r--   0 fernando   (501) staff       (20)     3179 2024-05-19 22:43:58.000000 cvprocessor-1.0.5/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     3281 2024-05-25 01:46:30.000000 cvprocessor-1.0.5/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3232 2024-05-19 23:43:56.000000 cvprocessor-1.0.5/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3301 2024-05-19 02:18:35.000000 cvprocessor-1.0.5/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-1.0.5/src/cvprocessor/intro.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.932009 cvprocessor-1.0.5/src/cvprocessor/links/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 22:55:50.000000 cvprocessor-1.0.5/src/cvprocessor/links/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     2957 2024-05-21 01:29:26.000000 cvprocessor-1.0.5/src/cvprocessor/links/links.py
--rw-r--r--   0 fernando   (501) staff       (20)     1534 2024-05-19 10:04:27.000000 cvprocessor-1.0.5/src/cvprocessor/memberships.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.932868 cvprocessor-1.0.5/src/cvprocessor/name/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-19 02:13:29.000000 cvprocessor-1.0.5/src/cvprocessor/name/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)      937 2024-05-19 02:16:28.000000 cvprocessor-1.0.5/src/cvprocessor/name/name.py
--rw-r--r--   0 fernando   (501) staff       (20)     2568 2024-05-19 02:27:08.000000 cvprocessor-1.0.5/src/cvprocessor/news.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.933698 cvprocessor-1.0.5/src/cvprocessor/personal/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-21 06:20:45.000000 cvprocessor-1.0.5/src/cvprocessor/personal/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     1532 2024-05-21 06:20:48.000000 cvprocessor-1.0.5/src/cvprocessor/personal/personal.py
--rw-r--r--   0 fernando   (501) staff       (20)    13642 2024-05-21 06:24:08.000000 cvprocessor-1.0.5/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1623 2024-05-20 03:02:34.000000 cvprocessor-1.0.5/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1491 2024-05-19 08:07:27.000000 cvprocessor-1.0.5/src/cvprocessor/research_interests.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.934984 cvprocessor-1.0.5/src/cvprocessor/security/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:18:52.000000 cvprocessor-1.0.5/src/cvprocessor/security/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     1021 2024-05-17 23:21:12.000000 cvprocessor-1.0.5/src/cvprocessor/security/security.py
--rw-r--r--   0 fernando   (501) staff       (20)     2110 2024-05-20 02:54:45.000000 cvprocessor-1.0.5/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2982 2024-05-20 02:08:33.000000 cvprocessor-1.0.5/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     3484 2024-05-19 22:06:55.000000 cvprocessor-1.0.5/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3048 2024-05-20 01:46:13.000000 cvprocessor-1.0.5/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     2577 2024-05-20 01:38:33.000000 cvprocessor-1.0.5/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-25 01:48:55.935832 cvprocessor-1.0.5/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-25 01:48:55.000000 cvprocessor-1.0.5/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1153 2024-05-25 01:48:55.000000 cvprocessor-1.0.5/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-25 01:48:55.000000 cvprocessor-1.0.5/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-25 01:48:55.000000 cvprocessor-1.0.5/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-25 01:48:55.000000 cvprocessor-1.0.5/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.114687 cvprocessor-1.0.6/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-1.0.6/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-28 07:45:41.114077 cvprocessor-1.0.6/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-1.0.6/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-28 07:44:08.000000 cvprocessor-1.0.6/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-28 07:45:41.114783 cvprocessor-1.0.6/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.077881 cvprocessor-1.0.6/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.099779 cvprocessor-1.0.6/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-1.0.6/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4365 2024-05-21 06:21:00.000000 cvprocessor-1.0.6/src/cvprocessor/authors.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.105483 cvprocessor-1.0.6/src/cvprocessor/contact/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:11:09.000000 cvprocessor-1.0.6/src/cvprocessor/contact/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3497 2024-05-21 02:03:19.000000 cvprocessor-1.0.6/src/cvprocessor/contact/contact.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7749 2024-05-20 00:37:00.000000 cvprocessor-1.0.6/src/cvprocessor/cv.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.106843 cvprocessor-1.0.6/src/cvprocessor/date/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-18 23:14:35.000000 cvprocessor-1.0.6/src/cvprocessor/date/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3445 2024-05-19 09:59:29.000000 cvprocessor-1.0.6/src/cvprocessor/date/date.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3179 2024-05-19 22:43:58.000000 cvprocessor-1.0.6/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3281 2024-05-25 01:46:30.000000 cvprocessor-1.0.6/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3232 2024-05-19 23:43:56.000000 cvprocessor-1.0.6/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3301 2024-05-19 02:18:35.000000 cvprocessor-1.0.6/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-1.0.6/src/cvprocessor/intro.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.108555 cvprocessor-1.0.6/src/cvprocessor/links/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 22:55:50.000000 cvprocessor-1.0.6/src/cvprocessor/links/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2977 2024-05-28 07:43:49.000000 cvprocessor-1.0.6/src/cvprocessor/links/links.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1534 2024-05-19 10:04:27.000000 cvprocessor-1.0.6/src/cvprocessor/memberships.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.109875 cvprocessor-1.0.6/src/cvprocessor/name/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-19 02:13:29.000000 cvprocessor-1.0.6/src/cvprocessor/name/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)      937 2024-05-19 02:16:28.000000 cvprocessor-1.0.6/src/cvprocessor/name/name.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2568 2024-05-19 02:27:08.000000 cvprocessor-1.0.6/src/cvprocessor/news.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.111163 cvprocessor-1.0.6/src/cvprocessor/personal/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-21 06:20:45.000000 cvprocessor-1.0.6/src/cvprocessor/personal/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1532 2024-05-21 06:20:48.000000 cvprocessor-1.0.6/src/cvprocessor/personal/personal.py
+-rw-r--r--   0 fernando   (501) staff       (20)    13642 2024-05-21 06:24:08.000000 cvprocessor-1.0.6/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1623 2024-05-20 03:02:34.000000 cvprocessor-1.0.6/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1491 2024-05-19 08:07:27.000000 cvprocessor-1.0.6/src/cvprocessor/research_interests.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.112474 cvprocessor-1.0.6/src/cvprocessor/security/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:18:52.000000 cvprocessor-1.0.6/src/cvprocessor/security/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1021 2024-05-17 23:21:12.000000 cvprocessor-1.0.6/src/cvprocessor/security/security.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2110 2024-05-20 02:54:45.000000 cvprocessor-1.0.6/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2982 2024-05-20 02:08:33.000000 cvprocessor-1.0.6/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3484 2024-05-19 22:06:55.000000 cvprocessor-1.0.6/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3048 2024-05-20 01:46:13.000000 cvprocessor-1.0.6/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2577 2024-05-20 01:38:33.000000 cvprocessor-1.0.6/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-28 07:45:41.113456 cvprocessor-1.0.6/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-28 07:45:41.000000 cvprocessor-1.0.6/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1153 2024-05-28 07:45:41.000000 cvprocessor-1.0.6/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-28 07:45:41.000000 cvprocessor-1.0.6/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-28 07:45:41.000000 cvprocessor-1.0.6/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-28 07:45:41.000000 cvprocessor-1.0.6/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-1.0.5/LICENSE` & `cvprocessor-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/PKG-INFO` & `cvprocessor-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 1.0.5
+Version: 1.0.6
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-1.0.5/README.md` & `cvprocessor-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/pyproject.toml` & `cvprocessor-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-1.0.5/src/cvprocessor/authors.py` & `cvprocessor-1.0.6/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/contact/contact.py` & `cvprocessor-1.0.6/src/cvprocessor/contact/contact.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/cv.py` & `cvprocessor-1.0.6/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/date/date.py` & `cvprocessor-1.0.6/src/cvprocessor/date/date.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/education.py` & `cvprocessor-1.0.6/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/experience.py` & `cvprocessor-1.0.6/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/grants_awards.py` & `cvprocessor-1.0.6/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/institutes.py` & `cvprocessor-1.0.6/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/intro.py` & `cvprocessor-1.0.6/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/links/links.py` & `cvprocessor-1.0.6/src/cvprocessor/links/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 
 link_types = {
     "website": "Website",
     "linkedin": "LinkedIn",
     "preprint": "Preprint",
     "pdf": "PDF",
+    "demo": "Demo",
     "code": "Code",
     "github": "GitHub",
     "twitter": "Twitter",
     "facebook": "Facebook",
     "instagram": "Instagram",
     "youtube": "YouTube",
     "slideshare": "SlideShare",
```

### Comparing `cvprocessor-1.0.5/src/cvprocessor/memberships.py` & `cvprocessor-1.0.6/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/name/name.py` & `cvprocessor-1.0.6/src/cvprocessor/name/name.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/news.py` & `cvprocessor-1.0.6/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/personal/personal.py` & `cvprocessor-1.0.6/src/cvprocessor/personal/personal.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/publications.py` & `cvprocessor-1.0.6/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/references.py` & `cvprocessor-1.0.6/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/research_interests.py` & `cvprocessor-1.0.6/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/security/security.py` & `cvprocessor-1.0.6/src/cvprocessor/security/security.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/service.py` & `cvprocessor-1.0.6/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/skills.py` & `cvprocessor-1.0.6/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/software.py` & `cvprocessor-1.0.6/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/supervision.py` & `cvprocessor-1.0.6/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor/teaching.py` & `cvprocessor-1.0.6/src/cvprocessor/teaching.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-1.0.5/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-1.0.6/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 1.0.5
+Version: 1.0.6
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-1.0.5/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-1.0.6/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

