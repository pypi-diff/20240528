# Comparing `tmp/django_oauth_emailbackend-0.1.1.tar.gz` & `tmp/django_oauth_emailbackend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_emailbackend-0.1.1.tar", last modified: Tue May 28 07:28:51 2024, max compression
+gzip compressed data, was "django_oauth_emailbackend-0.1.2.tar", last modified: Tue May 28 08:01:33 2024, max compression
```

## Comparing `django_oauth_emailbackend-0.1.1.tar` & `django_oauth_emailbackend-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.211050 django_oauth_emailbackend-0.1.1/
--rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 07:28:48.000000 django_oauth_emailbackend-0.1.1/LICENSE
--rw-r--r--   0 odop       (501) staff       (20)     3567 2024-05-28 07:28:51.210854 django_oauth_emailbackend-0.1.1/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 07:28:48.000000 django_oauth_emailbackend-0.1.1/README.md
--rw-r--r--   0 odop       (501) staff       (20)     1046 2024-05-28 07:28:48.000000 django_oauth_emailbackend-0.1.1/pyproject.toml
--rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 07:28:51.211087 django_oauth_emailbackend-0.1.1/setup.cfg
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.207213 django_oauth_emailbackend-0.1.1/src/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.210649 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/
--rw-r--r--   0 odop       (501) staff       (20)     3567 2024-05-28 07:28:51.000000 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)      891 2024-05-28 07:28:51.000000 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/SOURCES.txt
--rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 07:28:51.000000 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/dependency_links.txt
--rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 07:28:51.000000 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/requires.txt
--rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 07:28:51.000000 django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/top_level.txt
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.209866 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/admin.py
--rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/apps.py
--rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/backends.py
--rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/forms.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.207335 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/management/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.209994 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/management/commands/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/management/commands/__init__.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.210217 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/migrations/
--rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/migrations/0001_initial.py
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/migrations/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7583 2024-05-28 06:13:36.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/models.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 07:28:51.210449 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/providers/
--rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/providers/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/providers/gmail.py
--rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/tasks.py
--rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/tests.py
--rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/urls.py
--rw-r--r--   0 odop       (501) staff       (20)     8192 2024-04-05 06:47:31.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/utils.py
--rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/views.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334816 django_oauth_emailbackend-0.1.2/
+-rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/LICENSE
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:01:33.334626 django_oauth_emailbackend-0.1.2/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/README.md
+-rw-r--r--   0 odop       (501) staff       (20)     1001 2024-05-28 08:01:30.000000 django_oauth_emailbackend-0.1.2/pyproject.toml
+-rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 08:01:33.334852 django_oauth_emailbackend-0.1.2/setup.cfg
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.330702 django_oauth_emailbackend-0.1.2/src/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334412 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/
+-rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)      891 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/requires.txt
+-rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 08:01:33.000000 django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/top_level.txt
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333549 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     4925 2024-04-05 06:47:05.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/admin.py
+-rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/apps.py
+-rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/backends.py
+-rw-r--r--   0 odop       (501) staff       (20)     1642 2024-03-29 04:43:53.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/forms.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.330831 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333680 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/commands/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/management/commands/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.333936 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/
+-rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/0001_initial.py
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7628 2024-05-28 08:01:12.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/models.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 08:01:33.334197 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/
+-rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/gmail.py
+-rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tasks.py
+-rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tests.py
+-rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/urls.py
+-rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/utils.py
+-rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/views.py
```

### Comparing `django_oauth_emailbackend-0.1.1/LICENSE` & `django_oauth_emailbackend-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/PKG-INFO` & `django_oauth_emailbackend-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
```

### Comparing `django_oauth_emailbackend-0.1.1/README.md` & `django_oauth_emailbackend-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/pyproject.toml` & `django_oauth_emailbackend-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [project]
 name = "django-oauth-emailbackend"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sun-Yeon Lee", email="odop@youhasoft.com" },
 ]
 description = "Django emailbackend with Celery that using IMAP and google OAuth api"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
```

### Comparing `django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/PKG-INFO` & `django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django emailbackend with Celery that using IMAP and google OAuth api
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
```

### Comparing `django_oauth_emailbackend-0.1.1/src/django_oauth_emailbackend.egg-info/SOURCES.txt` & `django_oauth_emailbackend-0.1.2/src/django_oauth_emailbackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/admin.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/admin.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/apps.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/apps.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/backends.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/backends.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/forms.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/forms.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/migrations/0001_initial.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/models.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     instance.site.save()
 pre_save.connect(__clear_site_cache, sender=EmailClient)
 
 
 
 class SendHistory(models.Model):
     message_id = models.CharField(max_length=100, editable=False)
-    site = models.ForeignKey(Site, on_delete=models.CASCADE)
+    site = models.ForeignKey(Site, on_delete=models.CASCADE, related_name='emailbackend_sendhistory_set')
     recipients = models.CharField('수신자들', max_length=1200, null=True, blank=True)
     
     subject = models.CharField('제목', max_length=200, null=True)
     raw = models.TextField('메시지 원본', null=True, blank=True)
     
     arranged_time = models.DateTimeField("예약시간", auto_now_add=True)
     sent_time = models.DateTimeField("발송 완료시간", null=True, blank=True)
```

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/providers/__init__.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/providers/gmail.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/providers/gmail.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/tasks.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/utils.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,17 @@
         obj.mark(success, error_message, retry_count)
         
     except Exception as e:
         print(e)
         # Send error message using user's os system email
         # send_system_email(subject, body)
 
-def add_send_history(message_id, site: Site, message: Optional[EmailMessage | Message], using='default', success=None, **kwargs) -> Optional[ Type[T]]: 
+# python 3.9 compatibility
+# def add_send_history(message_id, site: Site, message: Optional[EmailMessage | Message], using='default', success=None, **kwargs) -> Optional[ Type[T]]: 
+def add_send_history(message_id, site: Site, message, using='default', success=None, **kwargs) -> Optional[ Type[T]]: 
     """ 발송히스토리를 생성한다. """
     from .models import SendHistory 
     try:
         message_id = _strip_message_id(message_id)
 
         obj, created = SendHistory.objects.using(using).get_or_create(
                     message_id=message_id,
```

### Comparing `django_oauth_emailbackend-0.1.1/src/oauth_emailbackend/views.py` & `django_oauth_emailbackend-0.1.2/src/oauth_emailbackend/views.py`

 * *Files identical despite different names*

