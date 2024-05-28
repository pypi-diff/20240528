# Comparing `tmp/KeyboardPaster-0.1.5.tar.gz` & `tmp/KeyboardPaster-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyboardPaster-0.1.5.tar", last modified: Tue May  9 11:21:57 2023, max compression
+gzip compressed data, was "KeyboardPaster-0.1.6.tar", last modified: Tue May  9 14:06:49 2023, max compression
```

## Comparing `KeyboardPaster-0.1.5.tar` & `KeyboardPaster-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.465831 KeyboardPaster-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.457325 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1040 2023-05-09 11:21:57.465332 KeyboardPaster-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.463330 KeyboardPaster-0.1.5/keyboardpaster/
--rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.5/keyboardpaster/__init__.py
--rw-rw-rw-   0        0        0     3485 2023-05-09 11:08:22.000000 KeyboardPaster-0.1.5/keyboardpaster/app.py
--rw-rw-rw-   0        0        0    10577 2023-05-09 10:59:43.000000 KeyboardPaster-0.1.5/keyboardpaster/keyboard_layout_detector.py
--rw-rw-rw-   0        0        0      552 2023-05-09 08:59:34.000000 KeyboardPaster-0.1.5/keyboardpaster/keyboardpaster.kv
--rw-rw-rw-   0        0        0       42 2023-05-09 11:21:57.465831 KeyboardPaster-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1411 2023-05-09 11:20:04.000000 KeyboardPaster-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:06:49.522362 KeyboardPaster-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-05-09 14:06:49.512854 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 14:06:49.000000 KeyboardPaster-0.1.6/KeyboardPaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-09 14:06:49.521360 KeyboardPaster-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 14:06:49.519359 KeyboardPaster-0.1.6/keyboardpaster/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.6/keyboardpaster/__init__.py
+-rw-rw-rw-   0        0        0     5209 2023-05-09 14:05:10.000000 KeyboardPaster-0.1.6/keyboardpaster/app.py
+-rw-rw-rw-   0        0        0    10577 2023-05-09 10:59:43.000000 KeyboardPaster-0.1.6/keyboardpaster/keyboard_layout_detector.py
+-rw-rw-rw-   0        0        0     2185 2023-05-09 14:03:00.000000 KeyboardPaster-0.1.6/keyboardpaster/keyboardpaster_app.kv
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:06:49.522362 KeyboardPaster-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-05-09 12:56:48.000000 KeyboardPaster-0.1.6/setup.py
```

### Comparing `KeyboardPaster-0.1.5/KeyboardPaster.egg-info/PKG-INFO` & `KeyboardPaster-0.1.6/KeyboardPaster.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.5/PKG-INFO` & `KeyboardPaster-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.5/keyboardpaster/keyboard_layout_detector.py` & `KeyboardPaster-0.1.6/keyboardpaster/keyboard_layout_detector.py`

 * *Files identical despite different names*

### Comparing `KeyboardPaster-0.1.5/setup.py` & `KeyboardPaster-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KeyboardPaster",
-    version="0.1.5",
+    version="0.1.6",
     author="Brian Knutsson",
     author_email="development@knutsson.it",
     description="A Python package to type text using the keyboard module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KnutssonDevelopment/KeyboardPaster",
     packages=find_packages(),
     package_data={
-        "keyboardpaster": ["keyboardpaster.kv"],
+        "keyboardpaster": ["keyboardpaster_app.kv"],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.10",
     install_requires=[
-        "keyboard",
+        "pynput",
         "kivy",
         "kivymd",
     ],
     extras_require={
         "windows": ["pywin32"],
         "linux": ["setuptools"],
         "macos": ["setuptools"],
```

