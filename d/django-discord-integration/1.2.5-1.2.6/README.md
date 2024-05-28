# Comparing `tmp/django-discord-integration-1.2.5.tar.gz` & `tmp/django-discord-integration-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-discord-integration-1.2.5.tar", last modified: Tue Jan  3 20:49:28 2023, max compression
+gzip compressed data, was "dist/django-discord-integration-1.2.6.tar", last modified: Tue May 28 17:20:08 2024, max compression
```

## Comparing `django-discord-integration-1.2.5.tar` & `django-discord-integration-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 evanzhang  (1000) evanzhang  (1000)        0 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)    34520 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/LICENSE
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     2344 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/PKG-INFO
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     1320 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/README.md
-drwxr-xr-x   0 evanzhang  (1000) evanzhang  (1000)        0 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/discord_integration/
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)       73 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/__init__.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)      269 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/admin.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)      265 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/apps.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     4476 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/log.py
-drwxr-xr-x   0 evanzhang  (1000) evanzhang  (1000)        0 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/discord_integration/migrations/
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     1029 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/migrations/0001_initial.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)      758 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/migrations/0002_auto_20200412_1649.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)      553 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/migrations/0003_discordintegration_name.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)        0 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/migrations/__init__.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     1054 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/models.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)       26 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/tests.py
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)       26 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/discord_integration/views.py
-drwxr-xr-x   0 evanzhang  (1000) evanzhang  (1000)        0 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/django_discord_integration.egg-info/
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     2344 2023-01-03 20:49:28.000000 django-discord-integration-1.2.5/django_discord_integration.egg-info/PKG-INFO
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)      641 2023-01-03 20:49:28.000000 django-discord-integration-1.2.5/django_discord_integration.egg-info/SOURCES.txt
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)        1 2023-01-03 20:49:28.000000 django-discord-integration-1.2.5/django_discord_integration.egg-info/dependency_links.txt
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)       20 2023-01-03 20:49:28.000000 django-discord-integration-1.2.5/django_discord_integration.egg-info/top_level.txt
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)       38 2023-01-03 20:49:28.180054 django-discord-integration-1.2.5/setup.cfg
--rw-r--r--   0 evanzhang  (1000) evanzhang  (1000)     1219 2023-01-03 20:49:18.000000 django-discord-integration-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/discord_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/discord_integration/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0002_auto_20200412_1649.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/0003_discordintegration_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/discord_integration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/django_discord_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:20:08.000000 django-discord-integration-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:20:01.000000 django-discord-integration-1.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-discord-integration-1.2.5/PKG-INFO` & `django-discord-integration-1.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,59 @@
 Metadata-Version: 2.1
 Name: django-discord-integration
-Version: 1.2.5
+Version: 1.2.6
 Summary: Discord integration for Django, supporting error reporting via webhooks.
 Home-page: https://github.com/Ninjaclasher/django-discord-integration
 Author: Evan Zhang
+License: UNKNOWN
+Description: # Django Discord Integration
+        
+        Discord integration for Django, supporting error reporting via webhooks.
+        
+        This app comes with two message handlers: `DiscordMessageHandler` and `SimpleDiscordMessageHandler`. `DiscordMessageHandler` sends all the information related to the message, such as a traceback if there is one, while the `SimpleDiscordMessageHandler` only sends the title.
+        
+        ## Installation
+        ```bash
+        $ pip install django-discord-integration
+        ```
+        
+        In your `settings.py`, add the following:
+        ```python
+        INSTALLED_APPS = (
+            'discord_integration',
+            ...
+        )
+        ```
+        
+        Next, migrate the database:
+        ```
+        $ python manage.py migrate
+        ```
+        
+        Finally, create a Discord integration object in the Django admin site. Set the Discord webhook URL as well as the bot username and avatar URL if necessary. You can create multiple objects to direct different logs to different channels. The default object should the name `default`.
+        
+        
+        ## Sample Logging Configuration
+        
+        ```python
+        LOGGING = {
+            'handlers': {
+                'discord_integration': {
+                    'level': 'ERROR',
+                    'class': 'discord_integration.log.DiscordMessageHandler',
+                    'model_name': 'default',  # OPTIONAL: specify a name to use a different integration configuration.
+                },
+            },
+            'loggers': {
+                'handlers': ['discord_integration'],
+            },
+        }
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
@@ -15,52 +61,7 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Django Discord Integration
-
-Discord integration for Django, supporting error reporting via webhooks.
-
-This app comes with two message handlers: `DiscordMessageHandler` and `SimpleDiscordMessageHandler`. `DiscordMessageHandler` sends all the information related to the message, such as a traceback if there is one, while the `SimpleDiscordMessageHandler` only sends the title.
-
-## Installation
-```bash
-$ pip install django-discord-integration
-```
-
-In your `settings.py`, add the following:
-```python
-INSTALLED_APPS = (
-    'discord_integration',
-    ...
-)
-```
-
-Next, migrate the database:
-```
-$ python manage.py migrate
-```
-
-Finally, create a Discord integration object in the Django admin site. Set the Discord webhook URL as well as the bot username and avatar URL if necessary. You can create multiple objects to direct different logs to different channels. The default object should the name `default`.
-
-
-## Sample Logging Configuration
-
-```python
-LOGGING = {
-    'handlers': {
-        'discord_integration': {
-            'level': 'ERROR',
-            'class': 'discord_integration.log.DiscordMessageHandler',
-            'model_name': 'default',  # OPTIONAL: specify a name to use a different integration configuration.
-        },
-    },
-    'loggers': {
-        'handlers': ['discord_integration'],
-    },
-}
-```
```

### Comparing `django-discord-integration-1.2.5/README.md` & `django-discord-integration-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.5/discord_integration/log.py` & `django-discord-integration-1.2.6/discord_integration/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import traceback
 from logging import LogRecord
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Tuple
 from urllib import request
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.log import AdminEmailHandler
+from django_stubs_ext import StrOrPromise
 from urllib3 import encode_multipart_formdata
 
 __all__ = ['DiscordMessageHandler', 'SimpleDiscordMessageHandler']
 
 
 MESSAGE_LIMIT: int = getattr(settings, 'DISCORD_MESSAGE_LIMIT', 4000)
 BOT_USERNAME: Optional[str] = getattr(settings, 'DISCORD_BOT_USERNAME', None)
@@ -45,21 +46,24 @@
         if avatar_url and 'avatar_url' not in message:
             message['avatar_url'] = avatar_url
 
         files = []
         if full_message:
             files.append(('full_message.txt', full_message, 'text/plain'))
 
-        data = {
-            'payload_json': ('', json.dumps(message), 'application/json'),
+        data: Dict[str, Tuple[Optional[str], str, str]] = {
+            'payload_json': (None, json.dumps(message), 'application/json'),
         }
         for i, file in enumerate(files):
             data['files[{}]'.format(i)] = file
 
-        body, header = encode_multipart_formdata(data)
+        # We want to pass in None for the filename, but for some reason the
+        # typing here doesn't allow that even though the underlying code
+        # supports it. Ignore the type error for now.
+        body, header = encode_multipart_formdata(data)  # type: ignore[arg-type]
 
         req = request.Request(
             self.model.webhook_url,
             data=body,
             headers={'User-Agent': 'Python/3', 'Content-Type': header},
         )
         request.urlopen(req)
@@ -105,26 +109,26 @@
 
     def emit(self, record: LogRecord) -> None:
         self.__level = record.levelname
         self.__request_uri = self._get_raw_insecure_uri(record)
         self.__traceback = self._get_traceback(record)
         return super().emit(record)
 
-    def send_mail(self, subject: str, message: str, *args: Any, **kwargs: Any) -> None:
+    def send_mail(self, subject: StrOrPromise, message: StrOrPromise, *args: Any, **kwargs: Any) -> None:
         webhook = DiscordWebhook(self.model_name)
 
         webhook.message(
             {
                 'embeds': [{
-                    'title': webhook.escape(subject),
+                    'title': webhook.escape(str(subject)),
                     'url': self.__request_uri,
                     'description': webhook.format_codeblock(self.__traceback[:MESSAGE_LIMIT], 'py'),
                     'color': COLORS.get(self.__level, 0xeee),
                 }],
             },
-            full_message=message,
+            full_message=str(message),
         )
 
 
 class SimpleDiscordMessageHandler(DiscordMessageHandler):
-    def send_mail(self, subject: str, message: str, *args: Any, **kwargs: Any) -> None:
+    def send_mail(self, subject: StrOrPromise, message: StrOrPromise, *args: Any, **kwargs: Any) -> None:
         super().send_mail(subject, '', *args, **kwargs)
```

### Comparing `django-discord-integration-1.2.5/discord_integration/migrations/0001_initial.py` & `django-discord-integration-1.2.6/discord_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.5/discord_integration/migrations/0002_auto_20200412_1649.py` & `django-discord-integration-1.2.6/discord_integration/migrations/0002_auto_20200412_1649.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.5/discord_integration/migrations/0003_discordintegration_name.py` & `django-discord-integration-1.2.6/discord_integration/migrations/0003_discordintegration_name.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.5/discord_integration/models.py` & `django-discord-integration-1.2.6/discord_integration/models.py`

 * *Files identical despite different names*

### Comparing `django-discord-integration-1.2.5/django_discord_integration.egg-info/PKG-INFO` & `django-discord-integration-1.2.6/django_discord_integration.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,59 @@
 Metadata-Version: 2.1
 Name: django-discord-integration
-Version: 1.2.5
+Version: 1.2.6
 Summary: Discord integration for Django, supporting error reporting via webhooks.
 Home-page: https://github.com/Ninjaclasher/django-discord-integration
 Author: Evan Zhang
+License: UNKNOWN
+Description: # Django Discord Integration
+        
+        Discord integration for Django, supporting error reporting via webhooks.
+        
+        This app comes with two message handlers: `DiscordMessageHandler` and `SimpleDiscordMessageHandler`. `DiscordMessageHandler` sends all the information related to the message, such as a traceback if there is one, while the `SimpleDiscordMessageHandler` only sends the title.
+        
+        ## Installation
+        ```bash
+        $ pip install django-discord-integration
+        ```
+        
+        In your `settings.py`, add the following:
+        ```python
+        INSTALLED_APPS = (
+            'discord_integration',
+            ...
+        )
+        ```
+        
+        Next, migrate the database:
+        ```
+        $ python manage.py migrate
+        ```
+        
+        Finally, create a Discord integration object in the Django admin site. Set the Discord webhook URL as well as the bot username and avatar URL if necessary. You can create multiple objects to direct different logs to different channels. The default object should the name `default`.
+        
+        
+        ## Sample Logging Configuration
+        
+        ```python
+        LOGGING = {
+            'handlers': {
+                'discord_integration': {
+                    'level': 'ERROR',
+                    'class': 'discord_integration.log.DiscordMessageHandler',
+                    'model_name': 'default',  # OPTIONAL: specify a name to use a different integration configuration.
+                },
+            },
+            'loggers': {
+                'handlers': ['discord_integration'],
+            },
+        }
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
@@ -15,52 +61,7 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Django Discord Integration
-
-Discord integration for Django, supporting error reporting via webhooks.
-
-This app comes with two message handlers: `DiscordMessageHandler` and `SimpleDiscordMessageHandler`. `DiscordMessageHandler` sends all the information related to the message, such as a traceback if there is one, while the `SimpleDiscordMessageHandler` only sends the title.
-
-## Installation
-```bash
-$ pip install django-discord-integration
-```
-
-In your `settings.py`, add the following:
-```python
-INSTALLED_APPS = (
-    'discord_integration',
-    ...
-)
-```
-
-Next, migrate the database:
-```
-$ python manage.py migrate
-```
-
-Finally, create a Discord integration object in the Django admin site. Set the Discord webhook URL as well as the bot username and avatar URL if necessary. You can create multiple objects to direct different logs to different channels. The default object should the name `default`.
-
-
-## Sample Logging Configuration
-
-```python
-LOGGING = {
-    'handlers': {
-        'discord_integration': {
-            'level': 'ERROR',
-            'class': 'discord_integration.log.DiscordMessageHandler',
-            'model_name': 'default',  # OPTIONAL: specify a name to use a different integration configuration.
-        },
-    },
-    'loggers': {
-        'handlers': ['discord_integration'],
-    },
-}
-```
```

### Comparing `django-discord-integration-1.2.5/django_discord_integration.egg-info/SOURCES.txt` & `django-discord-integration-1.2.6/django_discord_integration.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 discord_integration/__init__.py
 discord_integration/admin.py
 discord_integration/apps.py
 discord_integration/log.py
 discord_integration/models.py
```

### Comparing `django-discord-integration-1.2.5/setup.py` & `django-discord-integration-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='django-discord-integration',
-    version='1.2.5',
+    version='1.2.6',
     author='Evan Zhang',
     install_requires=[],
     description='Discord integration for Django, supporting error reporting via webhooks.',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/Ninjaclasher/django-discord-integration',
     packages=find_packages(),
```

