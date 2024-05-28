# Comparing `tmp/django_post_deploy-2.4.3.tar.gz` & `tmp/django_post_deploy-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_post_deploy-2.4.3.tar", last modified: Thu May 23 14:44:48 2024, max compression
+gzip compressed data, was "django_post_deploy-2.4.4.tar", last modified: Tue May 28 07:25:22 2024, max compression
```

## Comparing `django_post_deploy-2.4.3.tar` & `django_post_deploy-2.4.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.588364 django_post_deploy-2.4.3/
--rw-r--r--   0 erlend     (501) staff       (20)      237 2024-05-22 13:15:43.000000 django_post_deploy-2.4.3/MANIFEST.in
--rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-23 14:44:48.588315 django_post_deploy-2.4.3/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)     5701 2024-05-22 13:17:21.000000 django_post_deploy-2.4.3/README.md
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.588114 django_post_deploy-2.4.3/django_post_deploy.egg-info/
--rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-23 14:44:48.000000 django_post_deploy-2.4.3/django_post_deploy.egg-info/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)      935 2024-05-23 14:44:48.000000 django_post_deploy-2.4.3/django_post_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 erlend     (501) staff       (20)        1 2024-05-23 14:44:48.000000 django_post_deploy-2.4.3/django_post_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 erlend     (501) staff       (20)        7 2024-05-23 14:44:48.000000 django_post_deploy-2.4.3/django_post_deploy.egg-info/requires.txt
--rw-r--r--   0 erlend     (501) staff       (20)       12 2024-05-23 14:44:48.000000 django_post_deploy-2.4.3/django_post_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.585926 django_post_deploy-2.4.3/post_deploy/
--rw-r--r--   0 erlend     (501) staff       (20)    20137 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/LICENSE.txt
--rw-r--r--   0 erlend     (501) staff       (20)      121 2024-05-22 14:17:09.000000 django_post_deploy-2.4.3/post_deploy/README.md
--rw-r--r--   0 erlend     (501) staff       (20)       82 2024-05-23 14:42:29.000000 django_post_deploy-2.4.3/post_deploy/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)       56 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/errors.py
--rw-r--r--   0 erlend     (501) staff       (20)     2120 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/local_utils.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.583124 django_post_deploy-2.4.3/post_deploy/management/
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.586012 django_post_deploy-2.4.3/post_deploy/management/commands/
--rw-r--r--   0 erlend     (501) staff       (20)     6666 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/management/commands/deploy.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.586701 django_post_deploy-2.4.3/post_deploy/migrations/
--rw-r--r--   0 erlend     (501) staff       (20)     1123 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/migrations/0001_initial.py
--rw-r--r--   0 erlend     (501) staff       (20)     1871 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/migrations/0002_postdeploylog.py
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/migrations/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     4533 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/models.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.586776 django_post_deploy-2.4.3/post_deploy/plugins/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/plugins/__init__.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.586992 django_post_deploy-2.4.3/post_deploy/plugins/context/
--rw-r--r--   0 erlend     (501) staff       (20)      280 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/plugins/context/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)      439 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/plugins/context/tenant.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.587214 django_post_deploy-2.4.3/post_deploy/plugins/scheduler/
--rw-r--r--   0 erlend     (501) staff       (20)      291 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/plugins/scheduler/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     1311 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/plugins/scheduler/celery.py
--rw-r--r--   0 erlend     (501) staff       (20)      369 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/tasks.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 14:44:48.587787 django_post_deploy-2.4.3/post_deploy/tests/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/tests/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     2472 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/tests/test_decorator.py
--rw-r--r--   0 erlend     (501) staff       (20)     5323 2024-05-22 12:55:59.000000 django_post_deploy-2.4.3/post_deploy/tests/test_log_queryset.py
--rw-r--r--   0 erlend     (501) staff       (20)     7172 2024-05-22 13:04:35.000000 django_post_deploy-2.4.3/post_deploy/tests/test_management_command.py
--rw-r--r--   0 erlend     (501) staff       (20)     2246 2024-05-23 14:44:03.000000 django_post_deploy-2.4.3/post_deploy/utils.py
--rw-r--r--   0 erlend     (501) staff       (20)       76 2024-05-23 14:44:48.588569 django_post_deploy-2.4.3/setup.cfg
--rw-r--r--   0 erlend     (501) staff       (20)     1045 2024-05-22 14:15:07.000000 django_post_deploy-2.4.3/setup.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.613390 django_post_deploy-2.4.4/
+-rw-r--r--   0 erlend     (501) staff       (20)      237 2024-05-22 13:15:43.000000 django_post_deploy-2.4.4/MANIFEST.in
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-28 07:25:22.613325 django_post_deploy-2.4.4/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)     5701 2024-05-22 13:17:21.000000 django_post_deploy-2.4.4/README.md
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.613103 django_post_deploy-2.4.4/django_post_deploy.egg-info/
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-28 07:25:22.000000 django_post_deploy-2.4.4/django_post_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)      935 2024-05-28 07:25:22.000000 django_post_deploy-2.4.4/django_post_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        1 2024-05-28 07:25:22.000000 django_post_deploy-2.4.4/django_post_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        7 2024-05-28 07:25:22.000000 django_post_deploy-2.4.4/django_post_deploy.egg-info/requires.txt
+-rw-r--r--   0 erlend     (501) staff       (20)       12 2024-05-28 07:25:22.000000 django_post_deploy-2.4.4/django_post_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.611512 django_post_deploy-2.4.4/post_deploy/
+-rw-r--r--   0 erlend     (501) staff       (20)    20137 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/LICENSE.txt
+-rw-r--r--   0 erlend     (501) staff       (20)      121 2024-05-22 14:17:09.000000 django_post_deploy-2.4.4/post_deploy/README.md
+-rw-r--r--   0 erlend     (501) staff       (20)       82 2024-05-28 07:22:34.000000 django_post_deploy-2.4.4/post_deploy/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)       56 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/errors.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2120 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/local_utils.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.609623 django_post_deploy-2.4.4/post_deploy/management/
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.611608 django_post_deploy-2.4.4/post_deploy/management/commands/
+-rw-r--r--   0 erlend     (501) staff       (20)     6643 2024-05-28 07:21:43.000000 django_post_deploy-2.4.4/post_deploy/management/commands/deploy.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.611914 django_post_deploy-2.4.4/post_deploy/migrations/
+-rw-r--r--   0 erlend     (501) staff       (20)     1123 2024-05-22 13:04:35.000000 django_post_deploy-2.4.4/post_deploy/migrations/0001_initial.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1871 2024-05-22 13:04:35.000000 django_post_deploy-2.4.4/post_deploy/migrations/0002_postdeploylog.py
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/migrations/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     4533 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/models.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.612005 django_post_deploy-2.4.4/post_deploy/plugins/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/plugins/__init__.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.612194 django_post_deploy-2.4.4/post_deploy/plugins/context/
+-rw-r--r--   0 erlend     (501) staff       (20)      280 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/plugins/context/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)      439 2024-05-22 13:04:35.000000 django_post_deploy-2.4.4/post_deploy/plugins/context/tenant.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.612415 django_post_deploy-2.4.4/post_deploy/plugins/scheduler/
+-rw-r--r--   0 erlend     (501) staff       (20)      291 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/plugins/scheduler/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1311 2024-05-22 13:04:35.000000 django_post_deploy-2.4.4/post_deploy/plugins/scheduler/celery.py
+-rw-r--r--   0 erlend     (501) staff       (20)      369 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/tasks.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-28 07:25:22.612902 django_post_deploy-2.4.4/post_deploy/tests/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/tests/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2472 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/tests/test_decorator.py
+-rw-r--r--   0 erlend     (501) staff       (20)     5323 2024-05-22 12:55:59.000000 django_post_deploy-2.4.4/post_deploy/tests/test_log_queryset.py
+-rw-r--r--   0 erlend     (501) staff       (20)     7172 2024-05-22 13:04:35.000000 django_post_deploy-2.4.4/post_deploy/tests/test_management_command.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2269 2024-05-28 07:24:09.000000 django_post_deploy-2.4.4/post_deploy/utils.py
+-rw-r--r--   0 erlend     (501) staff       (20)       76 2024-05-28 07:25:22.613619 django_post_deploy-2.4.4/setup.cfg
+-rw-r--r--   0 erlend     (501) staff       (20)     1045 2024-05-22 14:15:07.000000 django_post_deploy-2.4.4/setup.py
```

### Comparing `django_post_deploy-2.4.3/PKG-INFO` & `django_post_deploy-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django_post_deploy
-Version: 2.4.3
+Version: 2.4.4
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.3.tar.gz
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.4.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
 Keywords: Django,Deployment,Management,CLI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django_post_deploy-2.4.3/README.md` & `django_post_deploy-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/django_post_deploy.egg-info/PKG-INFO` & `django_post_deploy-2.4.4/django_post_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-post-deploy
-Version: 2.4.3
+Version: 2.4.4
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.3.tar.gz
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.4.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
 Keywords: Django,Deployment,Management,CLI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django_post_deploy-2.4.3/django_post_deploy.egg-info/SOURCES.txt` & `django_post_deploy-2.4.4/django_post_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/LICENSE.txt` & `django_post_deploy-2.4.4/post_deploy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/local_utils.py` & `django_post_deploy-2.4.4/post_deploy/local_utils.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/management/commands/deploy.py` & `django_post_deploy-2.4.4/post_deploy/management/commands/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.core.management.base import BaseCommand
 from django.utils import timezone
 from django.utils.timezone import get_current_timezone as ltz
 
 from post_deploy.local_utils import (get_context_manager,
-                                     get_scheduler_manager, initialize_actions,
+                                     initialize_actions,
                                      model_ok)
 from post_deploy.models import PostDeployLog
 from post_deploy.utils import run_task
 
 
 def strftime(datetime: timezone.datetime):
     return datetime.astimezone(ltz()).strftime("%Y-%m-%d %H:%M")
```

### Comparing `django_post_deploy-2.4.3/post_deploy/migrations/0001_initial.py` & `django_post_deploy-2.4.4/post_deploy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/migrations/0002_postdeploylog.py` & `django_post_deploy-2.4.4/post_deploy/migrations/0002_postdeploylog.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/models.py` & `django_post_deploy-2.4.4/post_deploy/models.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/plugins/scheduler/celery.py` & `django_post_deploy-2.4.4/post_deploy/plugins/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/tests/test_decorator.py` & `django_post_deploy-2.4.4/post_deploy/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/tests/test_log_queryset.py` & `django_post_deploy-2.4.4/post_deploy/tests/test_log_queryset.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/tests/test_management_command.py` & `django_post_deploy-2.4.4/post_deploy/tests/test_management_command.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.3/post_deploy/utils.py` & `django_post_deploy-2.4.4/post_deploy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     actions = initialize_actions()
     for import_name in actions.keys():
         PostDeployLog.objects.skip_action(import_name, reason)
 
 
 def run_task(import_name):
     from django.utils.translation import gettext as _
-    from post_deploy.local_utils import get_context_manager
+    from post_deploy.local_utils import get_context_manager, get_scheduler_manager
     from post_deploy.models import PostDeployLog
     assert not PostDeployLog.objects.is_running(import_name), _("Task is already running")
 
     context_manager = get_context_manager(None)
     action_log = PostDeployLog.objects.register_action(import_name)
     task_id = get_scheduler_manager().schedule([action_log], context_manager.default_parameters())
     PostDeployLog.objects.filter(import_name=import_name).update(task_id=task_id)
```

### Comparing `django_post_deploy-2.4.3/setup.py` & `django_post_deploy-2.4.4/setup.py`

 * *Files identical despite different names*

