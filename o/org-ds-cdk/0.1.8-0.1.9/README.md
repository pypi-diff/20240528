# Comparing `tmp/org-ds-cdk-0.1.8.tar.gz` & `tmp/org-ds-cdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "org-ds-cdk-0.1.8.tar", last modified: Mon May 27 07:49:20 2024, max compression
+gzip compressed data, was "org-ds-cdk-0.1.9.tar", last modified: Tue May 28 09:19:00 2024, max compression
```

## Comparing `org-ds-cdk-0.1.8.tar` & `org-ds-cdk-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 07:49:20.624907 org-ds-cdk-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-05-27 07:49:20.624907 org-ds-cdk-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2024-05-27 06:48:38.000000 org-ds-cdk-0.1.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-27 07:49:20.624907 org-ds-cdk-0.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      629 2024-05-27 07:49:10.000000 org-ds-cdk-0.1.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-28 09:19:00.377019 org-ds-cdk-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-05-28 09:19:00.377019 org-ds-cdk-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2024-05-27 06:48:38.000000 org-ds-cdk-0.1.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-28 09:19:00.377019 org-ds-cdk-0.1.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      629 2024-05-28 09:18:49.000000 org-ds-cdk-0.1.9/setup.py
```

### Comparing `org-ds-cdk-0.1.8/PKG-INFO` & `org-ds-cdk-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: org-ds-cdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: DS Organization CDK Constructs
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Building and Publishing CDK Constructs to PyPi
```

### Comparing `org-ds-cdk-0.1.8/README.md` & `org-ds-cdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `org-ds-cdk-0.1.8/setup.py` & `org-ds-cdk-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='org-ds-cdk',
-    version='0.1.08',
+    version='0.1.09',
     description='DS Organization CDK Constructs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages('../cdk_main'),
     package_dir={'': '../cdk_main'},
     install_requires=[
-        'aws-cdk-lib==2.142.0',
+        'aws-cdk-lib==2.143.0',
         'constructs>=10.0.0'
     ],
 )
```

