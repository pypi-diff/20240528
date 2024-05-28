# Comparing `tmp/bpetokenizer-1.0.1.tar.gz` & `tmp/bpetokenizer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpetokenizer-1.0.1.tar", last modified: Mon May 27 18:18:56 2024, max compression
+gzip compressed data, was "bpetokenizer-1.0.2.tar", last modified: Mon May 27 20:35:18 2024, max compression
```

## Comparing `bpetokenizer-1.0.1.tar` & `bpetokenizer-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.909775 bpetokenizer-1.0.1/
--rw-rw-rw-   0        0        0     5787 2024-05-27 18:18:56.907666 bpetokenizer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5181 2024-05-27 17:12:12.000000 bpetokenizer-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.905480 bpetokenizer-1.0.1/bpetokenizer.egg-info/
--rw-rw-rw-   0        0        0     5787 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 18:18:56.909775 bpetokenizer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1169 2024-05-27 17:19:44.000000 bpetokenizer-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.903436 bpetokenizer-1.0.1/tests/
--rw-rw-rw-   0        0        0      945 2024-05-27 07:10:18.000000 bpetokenizer-1.0.1/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:35:18.203131 bpetokenizer-1.0.2/
+-rw-rw-rw-   0        0        0     5787 2024-05-27 20:35:18.201036 bpetokenizer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5181 2024-05-27 17:12:12.000000 bpetokenizer-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:35:18.129070 bpetokenizer-1.0.2/bpetokenizer/
+-rw-rw-rw-   0        0        0       98 2024-05-27 09:23:45.000000 bpetokenizer-1.0.2/bpetokenizer/__init__.py
+-rw-rw-rw-   0        0        0     6817 2024-05-27 11:15:13.000000 bpetokenizer-1.0.2/bpetokenizer/base.py
+-rw-rw-rw-   0        0        0     5579 2024-05-27 16:21:16.000000 bpetokenizer-1.0.2/bpetokenizer/tokenizer.py
+-rw-rw-rw-   0        0        0       21 2024-05-27 20:35:01.000000 bpetokenizer-1.0.2/bpetokenizer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:35:18.198934 bpetokenizer-1.0.2/bpetokenizer.egg-info/
+-rw-rw-rw-   0        0        0     5787 2024-05-27 20:35:17.000000 bpetokenizer-1.0.2/bpetokenizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-27 20:35:17.000000 bpetokenizer-1.0.2/bpetokenizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:35:17.000000 bpetokenizer-1.0.2/bpetokenizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-27 20:35:17.000000 bpetokenizer-1.0.2/bpetokenizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 20:35:17.000000 bpetokenizer-1.0.2/bpetokenizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:35:18.203131 bpetokenizer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-27 20:33:55.000000 bpetokenizer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:35:18.190501 bpetokenizer-1.0.2/tests/
+-rw-rw-rw-   0        0        0      945 2024-05-27 07:10:18.000000 bpetokenizer-1.0.2/tests/test_tokenizer.py
```

### Comparing `bpetokenizer-1.0.1/PKG-INFO` & `bpetokenizer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpetokenizer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Byte Pair Encoding Tokenizer with special tokens and regex pattern
 Home-page: https://github.com/Hk669/bpetokenizer
 Author: Hrushikesh Dokala
 Author-email: hrushi669@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bpetokenizer-1.0.1/README.md` & `bpetokenizer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bpetokenizer-1.0.1/bpetokenizer.egg-info/PKG-INFO` & `bpetokenizer-1.0.2/bpetokenizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpetokenizer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Byte Pair Encoding Tokenizer with special tokens and regex pattern
 Home-page: https://github.com/Hk669/bpetokenizer
 Author: Hrushikesh Dokala
 Author-email: hrushi669@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bpetokenizer-1.0.1/setup.py` & `bpetokenizer-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     description="Byte Pair Encoding Tokenizer with special tokens and regex pattern",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hk669/bpetokenizer",
     author="Hrushikesh Dokala",
     author_email="hrushi669@gmail.com",
     license="MIT",
-    package_dir={"bpetokenizer": "bpetokenizer"},
-    packages=find_packages(where="bpetokenizer"),
+    packages=find_packages(include=["bpetokenizer"]),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=["regex"],
     extras_require={
```

### Comparing `bpetokenizer-1.0.1/tests/test_tokenizer.py` & `bpetokenizer-1.0.2/tests/test_tokenizer.py`

 * *Files identical despite different names*

