# Comparing `tmp/django_oauth_emailbackend-0.1.2.tar.gz` & `tmp/django_oauth_emailbackend-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_emailbackend-0.1.2.tar", last modified: Tue May 28 08:01:33 2024, max compression
+gzip compressed data, was "django_oauth_emailbackend-0.1.3.tar", last modified: Tue May 28 08:07:56 2024, max compression
```

## Comparing `django_oauth_emailbackend-0.1.2.tar` & `django_oauth_emailbackend-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334816 django_oauth_emailbackend-0.1.2/
--rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/LICENSE
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:01:33.334626 django_oauth_emailbackend-0.1.2/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/README.md
--rw-r--r--   0 odop       (501) staff       (20)     1001 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/pyproject.toml
--rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 08:01:33.334852 django_oauth_emailbackend-0.1.2/setup.cfg
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.330702 django_oauth_emailbackend-0.1.2/src/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334412 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)      891 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/SOURCES.txt
--rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/dependency_links.txt
--rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/requires.txt
--rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/top_level.txt
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333549 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/admin.py
--rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/apps.py
--rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/backends.py
--rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/forms.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.330831 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333680 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/commands/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/commands/__init__.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333936 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/
--rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/0001_initial.py
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7628 2024-05-28 08:01:12.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/models.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334197 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/
--rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/gmail.py
--rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tasks.py
--rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tests.py
--rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/urls.py
--rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/utils.py
--rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/views.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148684 django_oauth_emailbackend-0.1.3/
+-rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/LICENSE
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:07:56.148483 django_oauth_emailbackend-0.1.3/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/README.md
+-rw-r--r--   0 odop       (501) staff       (20)     1001 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/pyproject.toml
+-rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 08:07:56.148720 django_oauth_emailbackend-0.1.3/setup.cfg
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.144392 django_oauth_emailbackend-0.1.3/src/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148270 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)      891 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/requires.txt
+-rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/top_level.txt
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147271 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/admin.py
+-rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/apps.py
+-rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/backends.py
+-rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/forms.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.144523 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147525 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/commands/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/commands/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147833 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/
+-rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/0001_initial.py
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7628 2024-05-28 08:01:12.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/models.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148081 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/
+-rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/gmail.py
+-rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tasks.py
+-rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tests.py
+-rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/urls.py
+-rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/utils.py
+-rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/views.py
```

### Comparing `django_oauth_emailbackend-0.1.2/LICENSE` & `django_oauth_emailbackend-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/PKG-INFO` & `django_oauth_emailbackend-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 5.0
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>3.2.8
 Requires-Dist: celery>5.2
 Requires-Dist: google-api-core
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth
```

### Comparing `django_oauth_emailbackend-0.1.2/README.md` & `django_oauth_emailbackend-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/pyproject.toml` & `django_oauth_emailbackend-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "django-oauth-emailbackend"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Sun-Yeon Lee", email="odop@youhasoft.com" },
 ]
 description = "Django emailbackend with Celery that using IMAP and google OAuth api"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/PKG-INFO` & `django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 5.0
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>3.2.8
 Requires-Dist: celery>5.2
 Requires-Dist: google-api-core
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth
```

### Comparing `django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/SOURCES.txt` & `django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/admin.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/admin.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/apps.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/apps.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/backends.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/backends.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/forms.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/forms.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/0001_initial.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/models.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/models.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/__init__.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/gmail.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/gmail.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tasks.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/utils.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/utils.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/views.py` & `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/views.py`

 * *Files identical despite different names*

