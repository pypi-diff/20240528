# Comparing `tmp/crunchstat_summary-2.7.3.tar.gz` & `tmp/crunchstat_summary-2.7.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunchstat_summary-2.7.3.tar", last modified: Tue May 28 13:36:15 2024, max compression
+gzip compressed data, was "crunchstat_summary-2.7.3rc2.tar", last modified: Tue May 28 17:54:39 2024, max compression
```

## Comparing `crunchstat_summary-2.7.3.tar` & `crunchstat_summary-2.7.3rc2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:15.167348 crunchstat_summary-2.7.3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      226 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      377 2024-05-28 13:36:15.167348 crunchstat_summary-2.7.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      130 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/README.rst
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/agpl-3.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:15.139345 crunchstat_summary-2.7.3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      475 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/bin/crunchstat-summary
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:15.139345 crunchstat_summary-2.7.3/crunchstat_summary/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      255 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-05-28 13:36:14.000000 crunchstat_summary-2.7.3/crunchstat_summary/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3720 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/command.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3017 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/dygraphs.js
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1754 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/dygraphs.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3380 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/reader.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31405 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/summarizer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8454 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/synchronizer.js
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2131 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/crunchstat_summary/webchart.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 13:36:15.167348 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      377 2024-05-28 13:36:14.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      618 2024-05-28 13:36:15.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 13:36:14.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2021-06-03 18:28:10.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       29 2024-05-28 13:36:14.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       19 2024-05-28 13:36:14.000000 crunchstat_summary-2.7.3/crunchstat_summary.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 13:36:15.167348 crunchstat_summary-2.7.3/setup.cfg
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1558 2024-05-28 13:36:08.000000 crunchstat_summary-2.7.3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      226 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      130 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/README.rst
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/agpl-3.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      475 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/bin/crunchstat-summary
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/crunchstat_summary/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      255 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3720 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/command.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3017 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/dygraphs.js
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1754 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/dygraphs.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3380 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/reader.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31405 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/summarizer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8454 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/synchronizer.js
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2131 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary/webchart.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      618 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2021-06-03 18:28:10.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       32 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       19 2024-05-28 17:54:39.000000 crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-05-28 17:54:39.695756 crunchstat_summary-2.7.3rc2/setup.cfg
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1558 2024-05-28 17:54:35.000000 crunchstat_summary-2.7.3rc2/setup.py
```

### Comparing `crunchstat_summary-2.7.3/agpl-3.0.txt` & `crunchstat_summary-2.7.3rc2/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/arvados_version.py` & `crunchstat_summary-2.7.3rc2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/command.py` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/command.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/dygraphs.js` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/dygraphs.js`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/dygraphs.py` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/dygraphs.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/reader.py` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/reader.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/summarizer.py` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/synchronizer.js` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/synchronizer.js`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary/webchart.py` & `crunchstat_summary-2.7.3rc2/crunchstat_summary/webchart.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/crunchstat_summary.egg-info/SOURCES.txt` & `crunchstat_summary-2.7.3rc2/crunchstat_summary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.7.3/setup.py` & `crunchstat_summary-2.7.3rc2/setup.py`

 * *Files identical despite different names*

