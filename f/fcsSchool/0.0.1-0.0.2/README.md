# Comparing `tmp/fcsschool-0.0.1.tar.gz` & `tmp/fcsschool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcsschool-0.0.1.tar", last modified: Sun May 26 12:14:07 2024, max compression
+gzip compressed data, was "fcsschool-0.0.2.tar", last modified: Tue May 28 15:48:04 2024, max compression
```

## Comparing `fcsschool-0.0.1.tar` & `fcsschool-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-26 12:14:07.365558 fcsschool-0.0.1/
--rw-r--r--   0 ananta    (1000) ananta    (1000)      502 2024-05-26 12:14:07.365558 fcsschool-0.0.1/PKG-INFO
--rw-rw-r--   0 ananta    (1000) ananta    (1000)       43 2024-05-26 12:03:25.000000 fcsschool-0.0.1/README.txt
-drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-26 12:14:07.361558 fcsschool-0.0.1/fcsSchool/
--rw-r--r--   0 ananta    (1000) ananta    (1000)      250 2024-05-26 12:01:52.000000 fcsschool-0.0.1/fcsSchool/__init__.py
-drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-26 12:14:07.365558 fcsschool-0.0.1/fcsSchool.egg-info/
--rw-r--r--   0 ananta    (1000) ananta    (1000)      502 2024-05-26 12:14:03.000000 fcsschool-0.0.1/fcsSchool.egg-info/PKG-INFO
--rw-rw-r--   0 ananta    (1000) ananta    (1000)      173 2024-05-26 12:14:06.000000 fcsschool-0.0.1/fcsSchool.egg-info/SOURCES.txt
--rw-rw-r--   0 ananta    (1000) ananta    (1000)        1 2024-05-26 12:14:03.000000 fcsschool-0.0.1/fcsSchool.egg-info/dependency_links.txt
--rw-rw-r--   0 ananta    (1000) ananta    (1000)       10 2024-05-26 12:14:03.000000 fcsschool-0.0.1/fcsSchool.egg-info/top_level.txt
--rw-rw-r--   0 ananta    (1000) ananta    (1000)       38 2024-05-26 12:14:07.365558 fcsschool-0.0.1/setup.cfg
--rw-rw-rw-   0 ananta    (1000) ananta    (1000)      787 2024-05-26 12:13:55.000000 fcsschool-0.0.1/setup.py
+drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-28 15:48:03.997052 fcsschool-0.0.2/
+-rw-r--r--   0 ananta    (1000) ananta    (1000)      540 2024-05-28 15:48:03.997052 fcsschool-0.0.2/PKG-INFO
+-rw-rw-r--   0 ananta    (1000) ananta    (1000)       81 2024-05-28 15:45:54.000000 fcsschool-0.0.2/README.txt
+drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-28 15:48:03.993052 fcsschool-0.0.2/fcsSchool/
+-rw-r--r--   0 ananta    (1000) ananta    (1000)      344 2024-05-28 15:44:57.000000 fcsschool-0.0.2/fcsSchool/__init__.py
+drwxrwxr-x   0 ananta    (1000) ananta    (1000)        0 2024-05-28 15:48:03.997052 fcsschool-0.0.2/fcsSchool.egg-info/
+-rw-r--r--   0 ananta    (1000) ananta    (1000)      540 2024-05-28 15:48:00.000000 fcsschool-0.0.2/fcsSchool.egg-info/PKG-INFO
+-rw-rw-r--   0 ananta    (1000) ananta    (1000)      173 2024-05-28 15:48:03.000000 fcsschool-0.0.2/fcsSchool.egg-info/SOURCES.txt
+-rw-rw-r--   0 ananta    (1000) ananta    (1000)        1 2024-05-28 15:48:00.000000 fcsschool-0.0.2/fcsSchool.egg-info/dependency_links.txt
+-rw-rw-r--   0 ananta    (1000) ananta    (1000)       10 2024-05-28 15:48:00.000000 fcsschool-0.0.2/fcsSchool.egg-info/top_level.txt
+-rw-rw-r--   0 ananta    (1000) ananta    (1000)       38 2024-05-28 15:48:03.997052 fcsschool-0.0.2/setup.cfg
+-rw-rw-rw-   0 ananta    (1000) ananta    (1000)      787 2024-05-28 15:45:17.000000 fcsschool-0.0.2/setup.py
```

### Comparing `fcsschool-0.0.1/setup.py` & `fcsschool-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='fcsSchool',
-    version='0.0.1',
+    version='0.0.2',
     description='A very basic description',
     long_description=open('README.txt').read(),
     url='',  # Replace with a valid URL or remove this line if not available
     author='A K Ghosh',
     author_email='anantafcs@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

