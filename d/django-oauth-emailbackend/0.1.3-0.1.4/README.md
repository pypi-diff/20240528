# Comparing `tmp/django_oauth_emailbackend-0.1.3.tar.gz` & `tmp/django_oauth_emailbackend-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_emailbackend-0.1.3.tar", last modified: Tue May 28 08:07:56 2024, max compression
+gzip compressed data, was "django_oauth_emailbackend-0.1.4.tar", last modified: Tue May 28 10:09:22 2024, max compression
```

## Comparing `django_oauth_emailbackend-0.1.3.tar` & `django_oauth_emailbackend-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148684 django_oauth_emailbackend-0.1.3/
--rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/LICENSE
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:07:56.148483 django_oauth_emailbackend-0.1.3/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/README.md
--rw-r--r--   0 odop       (501) staff       (20)     1001 2024-05-28 08:07:53.000000 django_oauth_emailbackend-0.1.3/pyproject.toml
--rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 08:07:56.148720 django_oauth_emailbackend-0.1.3/setup.cfg
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.144392 django_oauth_emailbackend-0.1.3/src/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148270 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)      891 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/SOURCES.txt
--rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/dependency_links.txt
--rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/requires.txt
--rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 08:07:56.000000 django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/top_level.txt
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147271 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/admin.py
--rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/apps.py
--rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/backends.py
--rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/forms.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.144523 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147525 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/commands/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/management/commands/__init__.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.147833 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/
--rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/0001_initial.py
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7628 2024-05-28 08:01:12.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/models.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:07:56.148081 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/
--rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/gmail.py
--rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tasks.py
--rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tests.py
--rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/urls.py
--rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/utils.py
--rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/views.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.095867 django_oauth_emailbackend-0.1.4/
+-rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 10:09:18.000000 django_oauth_emailbackend-0.1.4/LICENSE
+-rw-r--r--   0 odop       (501) staff       (20)      142 2024-05-28 10:09:18.000000 django_oauth_emailbackend-0.1.4/MANIFEST.in
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 10:09:22.095674 django_oauth_emailbackend-0.1.4/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 10:09:18.000000 django_oauth_emailbackend-0.1.4/README.md
+-rw-r--r--   0 odop       (501) staff       (20)     1002 2024-05-28 10:09:18.000000 django_oauth_emailbackend-0.1.4/pyproject.toml
+-rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 10:09:22.095913 django_oauth_emailbackend-0.1.4/setup.cfg
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.090940 django_oauth_emailbackend-0.1.4/src/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.095431 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 10:09:22.000000 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     1135 2024-05-28 10:09:22.000000 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 10:09:22.000000 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 10:09:22.000000 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/requires.txt
+-rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 10:09:22.000000 django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/top_level.txt
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.094287 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/admin.py
+-rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/apps.py
+-rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/backends.py
+-rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/forms.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.094401 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/management/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 09:55:42.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/management/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.094490 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/management/commands/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/management/commands/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.094740 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/migrations/
+-rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/migrations/0001_initial.py
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/migrations/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7628 2024-05-28 08:01:12.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/models.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.094981 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/providers/
+-rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/providers/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/providers/gmail.py
+-rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/tasks.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.091493 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.091378 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/admin/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.091429 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/admin/oauth_emailbackend/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.095127 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/
+-rw-r--r--   0 odop       (501) staff       (20)     3957 2024-04-05 05:22:12.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 10:09:22.095263 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)     3101 2024-04-05 06:19:46.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/templates/oauth_emailbackend/callback.html
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 10:06:11.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/test.html
+-rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/tests.py
+-rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/urls.py
+-rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/utils.py
+-rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/views.py
```

### Comparing `django_oauth_emailbackend-0.1.3/LICENSE` & `django_oauth_emailbackend-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/PKG-INFO` & `django_oauth_emailbackend-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django_oauth_emailbackend-0.1.3/README.md` & `django_oauth_emailbackend-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/pyproject.toml` & `django_oauth_emailbackend-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-oauth-emailbackend"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Sun-Yeon Lee", email="odop@youhasoft.com" },
 ]
 description = "Django emailbackend with Celery that using IMAP and google OAuth api"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -25,11 +25,11 @@
   'google-api-core',
   'google-api-python-client',
   'google-auth',
   'google-auth-oauthlib',
   'google-auth-httplib2',
 ]
 
-
 [project.urls]
 Homepage = "https://github.com/youhasoft/django-oauth-emailbackend"
-Issues = "https://github.com/youhasoft/django-oauth-emailbackend/issues"
+Issues = "https://github.com/youhasoft/django-oauth-emailbackend/issues"
+
```

### Comparing `django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/PKG-INFO` & `django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django_oauth_emailbackend-0.1.3/src/django_oauth_emailbackend.egg-info/SOURCES.txt` & `django_oauth_emailbackend-0.1.4/src/django_oauth_emailbackend.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/django_oauth_emailbackend.egg-info/PKG-INFO
 src/django_oauth_emailbackend.egg-info/SOURCES.txt
 src/django_oauth_emailbackend.egg-info/dependency_links.txt
 src/django_oauth_emailbackend.egg-info/requires.txt
 src/django_oauth_emailbackend.egg-info/top_level.txt
 src/oauth_emailbackend/__init__.py
 src/oauth_emailbackend/admin.py
 src/oauth_emailbackend/apps.py
 src/oauth_emailbackend/backends.py
 src/oauth_emailbackend/forms.py
 src/oauth_emailbackend/models.py
 src/oauth_emailbackend/tasks.py
+src/oauth_emailbackend/test.html
 src/oauth_emailbackend/tests.py
 src/oauth_emailbackend/urls.py
 src/oauth_emailbackend/utils.py
 src/oauth_emailbackend/views.py
+src/oauth_emailbackend/management/__init__.py
 src/oauth_emailbackend/management/commands/__init__.py
 src/oauth_emailbackend/migrations/0001_initial.py
 src/oauth_emailbackend/migrations/__init__.py
 src/oauth_emailbackend/providers/__init__.py
-src/oauth_emailbackend/providers/gmail.py
+src/oauth_emailbackend/providers/gmail.py
+src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html
+src/oauth_emailbackend/templates/oauth_emailbackend/callback.html
```

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/admin.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/admin.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/apps.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/apps.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/backends.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/backends.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/forms.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/forms.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/migrations/0001_initial.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/models.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/models.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/__init__.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/providers/gmail.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/providers/gmail.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/tasks.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/utils.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/utils.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.3/src/oauth_emailbackend/views.py` & `django_oauth_emailbackend-0.1.4/src/oauth_emailbackend/views.py`

 * *Files identical despite different names*

