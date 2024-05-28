# Comparing `tmp/tabswitcher-0.1.2.tar.gz` & `tmp/tabswitcher-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.2.tar", last modified: Mon May 27 22:40:00 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.3.tar", last modified: Mon May 27 22:50:41 2024, max compression
```

## Comparing `tabswitcher-0.1.2.tar` & `tabswitcher-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:40:00.361276 tabswitcher-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-27 22:40:00.361276 tabswitcher-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:40:00.361276 tabswitcher-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:40:00.353276 tabswitcher-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:40:00.357276 tabswitcher-0.1.2/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:40:00.357276 tabswitcher-0.1.2/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:39:56.000000 tabswitcher-0.1.2/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:40:00.361276 tabswitcher-0.1.2/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:40:00.000000 tabswitcher-0.1.2/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:50:41.658604 tabswitcher-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-27 22:50:41.658604 tabswitcher-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:50:41.658604 tabswitcher-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:50:41.650604 tabswitcher-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:50:41.654604 tabswitcher-0.1.3/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:50:41.658604 tabswitcher-0.1.3/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:50:37.000000 tabswitcher-0.1.3/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:50:41.658604 tabswitcher-0.1.3/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:50:41.000000 tabswitcher-0.1.3/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.2/LICENCE` & `tabswitcher-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/PKG-INFO` & `tabswitcher-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.2/README.md` & `tabswitcher-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/setup.py` & `tabswitcher-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.2',
+    version='0.1.3',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.1.2/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.3/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.3/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/Settings.py` & `tabswitcher-0.1.3/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/Tab.py` & `tabswitcher-0.1.3/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/TabList.py` & `tabswitcher-0.1.3/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.3/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/__main__.py` & `tabswitcher-0.1.3/src/tabswitcher/__main__.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/actions.py` & `tabswitcher-0.1.3/src/tabswitcher/actions.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.3/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/assets/install.bat` & `tabswitcher-0.1.3/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.3/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.3/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/brotab.py` & `tabswitcher-0.1.3/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/colors.py` & `tabswitcher-0.1.3/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.3/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.3/src/tabswitcher/loadBookmarks.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.3/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.3/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.2/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.3/tabswitcher.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.2/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.3/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

