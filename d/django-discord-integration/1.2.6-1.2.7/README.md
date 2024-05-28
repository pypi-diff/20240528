# Comparing `tmp/django-discord-integration-1.2.6.tar.gz` & `tmp/django-discord-integration-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-discord-integration-1.2.6.tar", last modified: Tue May 28 17:20:08 2024, max compression
+gzip compressed data, was "dist/django-discord-integration-1.2.7.tar", last modified: Tue May 28 17:23:43 2024, max compression
```

## Comparing `django-discord-integration-1.2.6.tar` & `django-discord-integration-1.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/discord_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/discord_integration/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0002_auto_20200412_1649.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0003_discordintegration_name.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/discord_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/discord_integration/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/migrations/0002_auto_20200412_1649.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/migrations/0003_discordintegration_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/discord_integration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/django_discord_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/django_discord_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/django_discord_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/django_discord_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/django_discord_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:23:43.000000 django-discord-integration-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:23:36.000000 django-discord-integration-1.2.7/setup.py
```

### Comparing `django-discord-integration-1.2.6/PKG-INFO` & `django-discord-integration-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-discord-integration
-Version: 1.2.6
+Version: 1.2.7
 Summary: Discord integration for Django, supporting error reporting via webhooks.
 Home-page: https://github.com/Ninjaclasher/django-discord-integration
 Author: Evan Zhang
 License: UNKNOWN
 Description: # Django Discord Integration
         
         Discord integration for Django, supporting error reporting via webhooks.
```

### Comparing `django-discord-integration-1.2.6/README.md` & `django-discord-integration-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/discord_integration/log.py` & `django-discord-integration-1.2.7/discord_integration/log.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/discord_integration/migrations/0001_initial.py` & `django-discord-integration-1.2.7/discord_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/discord_integration/migrations/0002_auto_20200412_1649.py` & `django-discord-integration-1.2.7/discord_integration/migrations/0002_auto_20200412_1649.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/discord_integration/migrations/0003_discordintegration_name.py` & `django-discord-integration-1.2.7/discord_integration/migrations/0003_discordintegration_name.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/discord_integration/models.py` & `django-discord-integration-1.2.7/discord_integration/models.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/django_discord_integration.egg-info/PKG-INFO` & `django-discord-integration-1.2.7/django_discord_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-discord-integration
-Version: 1.2.6
+Version: 1.2.7
 Summary: Discord integration for Django, supporting error reporting via webhooks.
 Home-page: https://github.com/Ninjaclasher/django-discord-integration
 Author: Evan Zhang
 License: UNKNOWN
 Description: # Django Discord Integration
         
         Discord integration for Django, supporting error reporting via webhooks.
```

### Comparing `django-discord-integration-1.2.6/django_discord_integration.egg-info/SOURCES.txt` & `django-discord-integration-1.2.7/django_discord_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.6/setup.py` & `django-discord-integration-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='django-discord-integration',
-    version='1.2.6',
+    version='1.2.7',
     author='Evan Zhang',
     install_requires=[],
     description='Discord integration for Django, supporting error reporting via webhooks.',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/Ninjaclasher/django-discord-integration',
     packages=find_packages(),
```

