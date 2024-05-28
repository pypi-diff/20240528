# Comparing `tmp/aic_tools_pinecone-1.0.1.tar.gz` & `tmp/aic_tools_pinecone-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aic_tools_pinecone-1.0.1.tar", last modified: Fri Apr 12 20:56:48 2024, max compression
+gzip compressed data, was "aic_tools_pinecone-1.0.2.tar", last modified: Tue May 28 01:33:57 2024, max compression
```

## Comparing `aic_tools_pinecone-1.0.1.tar` & `aic_tools_pinecone-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-12 20:56:48.367818 aic_tools_pinecone-1.0.1/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      336 2024-04-12 20:56:48.367612 aic_tools_pinecone-1.0.1/PKG-INFO
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-12 20:56:48.366584 aic_tools_pinecone-1.0.1/aic_tools_pinecone/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3191 2024-04-12 20:54:54.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone/__init__.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-12 20:56:48.367394 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      336 2024-04-12 20:56:48.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      248 2024-04-12 20:56:48.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-12 20:56:48.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       62 2024-04-12 20:56:48.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       19 2024-04-12 20:56:48.000000 aic_tools_pinecone-1.0.1/aic_tools_pinecone.egg-info/top_level.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-12 20:56:48.367863 aic_tools_pinecone-1.0.1/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      738 2024-04-12 20:56:31.000000 aic_tools_pinecone-1.0.1/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-05-28 01:33:57.966701 aic_tools_pinecone-1.0.2/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      338 2024-05-28 01:33:57.966486 aic_tools_pinecone-1.0.2/PKG-INFO
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-05-28 01:33:57.965473 aic_tools_pinecone-1.0.2/aic_tools_pinecone/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3191 2024-04-12 23:35:00.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone/__init__.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-05-28 01:33:57.966260 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      338 2024-05-28 01:33:57.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      248 2024-05-28 01:33:57.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-05-28 01:33:57.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       64 2024-05-28 01:33:57.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       19 2024-05-28 01:33:57.000000 aic_tools_pinecone-1.0.2/aic_tools_pinecone.egg-info/top_level.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-05-28 01:33:57.966741 aic_tools_pinecone-1.0.2/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      738 2024-05-28 01:33:36.000000 aic_tools_pinecone-1.0.2/setup.py
```

### Comparing `aic_tools_pinecone-1.0.1/aic_tools_pinecone/__init__.py` & `aic_tools_pinecone-1.0.2/aic_tools_pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `aic_tools_pinecone-1.0.1/setup.py` & `aic_tools_pinecone-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='aic_tools_pinecone',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     description='Pinecone tools for AI Characters',
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
     install_requires=install_requires
```

