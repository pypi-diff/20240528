# Comparing `tmp/django_superapp-1.0.7.tar.gz` & `tmp/django_superapp-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_superapp-1.0.7.tar", last modified: Tue May 21 17:36:34 2024, max compression
+gzip compressed data, was "django_superapp-1.0.8.tar", last modified: Tue May 28 10:16:31 2024, max compression
```

## Comparing `django_superapp-1.0.7.tar` & `django_superapp-1.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.302111 django_superapp-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 17:36:24.000000 django_superapp-1.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-21 17:36:34.302111 django_superapp-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 17:36:24.000000 django_superapp-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 17:36:24.000000 django_superapp-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 17:36:34.302111 django_superapp-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-21 17:36:24.000000 django_superapp-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.294111 django_superapp-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.298111 django_superapp-1.0.7/src/django_superapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.298111 django_superapp-1.0.7/src/django_superapp/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/db_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.298111 django_superapp-1.0.7/src/django_superapp/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.298111 django_superapp-1.0.7/src/django_superapp/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/management/commands/list_all_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/management/commands/list_all_urls_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/management/commands/truncate_all_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.298111 django_superapp-1.0.7/src/django_superapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1267 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/sites.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-21 17:36:24.000000 django_superapp-1.0.7/src/django_superapp/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:34.302111 django_superapp-1.0.7/src/django_superapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 17:36:34.000000 django_superapp-1.0.7/src/django_superapp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 10:16:21.000000 django_superapp-1.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 10:16:31.369929 django_superapp-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-28 10:16:21.000000 django_superapp-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 10:16:21.000000 django_superapp-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 10:16:31.369929 django_superapp-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-28 10:16:21.000000 django_superapp-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.365929 django_superapp-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/db_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/management/commands/list_all_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/management/commands/list_all_urls_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/management/commands/truncate_all_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1267 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1590 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-28 10:16:21.000000 django_superapp-1.0.8/src/django_superapp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:16:31.369929 django_superapp-1.0.8/src/django_superapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 10:16:31.000000 django_superapp-1.0.8/src/django_superapp.egg-info/top_level.txt
```

### Comparing `django_superapp-1.0.7/LICENSE.md` & `django_superapp-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/PKG-INFO` & `django_superapp-1.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_superapp
-Version: 1.0.7
+Version: 1.0.8
 Summary: Build your startup's product faster.
 Home-page: https://github.com/django-superapp/django-superapp
 Author: Django SuperApp
 Author-email: django-superapp@bringes.io
 License: MIT
 Project-URL: Bug Reports, https://github.com/django-superapp/django-superapp/issues
 Project-URL: Source, https://github.com/django-superapp/django-superapp
@@ -36,22 +36,30 @@
 Requires-Dist: django-admin-confirm>=1.0.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: copier>=9.2.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=2.7.1
 
 # Django SuperApp
+SuperApp is a framework on top of Django, designed to accelerate the development of software projects for startups. It incorporates all the powerful features of Django, plus additional tools to seamlessly integrate various applications.
+
+![django-superapp-demo](https://django-superapp.bringes.io/assets/docs/admin-portal/admin-portal.svg "Django SuperApp")
 
 ### Getting Started
 ```bash
 pipx install django_superapp
-django_superapp create-project test_project
-cd test_project
-django_superapp add-app --app-name sample_app
+django_superapp create-project --project-template default ./my_superapp
+cd my_superapp
+django_superapp create-app --app-template sample_app
+make setup-sample-env
+make start-docker
 ```
 
+### Documentation
+For a more detailed documentation, visit [https://django-superapp.bringes.io](https://django-superapp.bringes.io).
+
 ### Development
 ```bash
 make install-requirements
 make install
 make release
 ```
```

### Comparing `django_superapp-1.0.7/setup.py` & `django_superapp-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/autocomplete.py` & `django_superapp-1.0.8/src/django_superapp/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/cli/main.py` & `django_superapp-1.0.8/src/django_superapp/cli/main.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/decorators.py` & `django_superapp-1.0.8/src/django_superapp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/forms.py` & `django_superapp-1.0.8/src/django_superapp/forms.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/helpers.py` & `django_superapp-1.0.8/src/django_superapp/helpers.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/management/commands/list_all_urls_patterns.py` & `django_superapp-1.0.8/src/django_superapp/management/commands/list_all_urls_patterns.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/management/commands/truncate_all_models.py` & `django_superapp-1.0.8/src/django_superapp/management/commands/truncate_all_models.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/settings.py` & `django_superapp-1.0.8/src/django_superapp/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import importlib
+import logging
 import pkgutil
 
 from django.urls import reverse_lazy
 from django.templatetags.static import static
 from django.utils.translation import gettext_lazy as _
 
+logger = logging.getLogger(__name__)
+
 
 def extend_superapp_settings(main_settings, package):
     for importer, modname, ispkg in pkgutil.iter_modules(package.__path__):
         submodule_name = f"{package.__name__}.{modname}.settings"
 
         try:
             settings_module = importlib.import_module(submodule_name)
-        except ModuleNotFoundError:
+        except ModuleNotFoundError as e:
+            logger.warning(e)
             continue
 
         if hasattr(settings_module, "extend_superapp_settings"):
             settings_module.extend_superapp_settings(main_settings)
 
 
 def extend_with_superapp_settings(main_settings, superapp_apps):
     main_settings.update({
         'LOGIN_URL': "admin:login",
         'LOGIN_REDIRECT_URL': reverse_lazy("admin:index"),
     })
     main_settings['INSTALLED_APPS'] = [
-        'admin_confirm',
-        'unfold',
-        "unfold.contrib.filters",
-        "unfold.contrib.import_export",
-        "unfold.contrib.guardian",
-        "unfold.contrib.simple_history",
-        "unfold.contrib.forms",
-    ] + main_settings['INSTALLED_APPS']
+                                          'admin_confirm',
+                                          'unfold',
+                                          "unfold.contrib.filters",
+                                          "unfold.contrib.import_export",
+                                          "unfold.contrib.guardian",
+                                          "unfold.contrib.simple_history",
+                                          "unfold.contrib.forms",
+                                      ] + main_settings['INSTALLED_APPS']
 
     main_settings['UNFOLD'] = {
         "SITE_HEADER": _("SuperApp Demo"),
         "SITE_TITLE": _("SuperApp Demo"),
         "SITE_SYMBOL": "settings",
         "SHOW_HISTORY": False,
         "STYLES": [],
```

### Comparing `django_superapp-1.0.7/src/django_superapp/sites.py` & `django_superapp-1.0.8/src/django_superapp/sites.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/types.py` & `django_superapp-1.0.8/src/django_superapp/types.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp/urls.py` & `django_superapp-1.0.8/src/django_superapp/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import importlib
+import logging
 import pkgutil
 
 from django.urls import path
 
+logger = logging.getLogger(__name__)
+
 def extend_superapp_urlpatterns(main_urlpatterns, package):
     for importer, modname, ispkg in pkgutil.iter_modules(package.__path__):
         submodule_name = f"{package.__name__}.{modname}.urls"
 
         try:
             urls_module = importlib.import_module(submodule_name)
-        except ModuleNotFoundError:
-            # TODO: when the submodule has a not found exception, we shouldn't raise this exception
+        except ModuleNotFoundError as e:
+            logger.warning(e)
             continue
 
         if hasattr(urls_module, "extend_superapp_urlpatterns"):
             urls_module.extend_superapp_urlpatterns(main_urlpatterns)
 
 
 def extend_superapp_admin_urlpatterns(main_admin_urlpatterns, package):
     for importer, modname, ispkg in pkgutil.iter_modules(package.__path__):
         submodule_name = f"{package.__name__}.{modname}.urls"
 
         try:
             urls_module = importlib.import_module(submodule_name)
-        except ModuleNotFoundError:
+        except ModuleNotFoundError as e:
+            logger.warning(e)
             continue
 
         if hasattr(urls_module, "extend_superapp_admin_urlpatterns"):
             urls_module.extend_superapp_admin_urlpatterns(main_admin_urlpatterns)
 
 
 main_admin_urlpatterns = []
```

### Comparing `django_superapp-1.0.7/src/django_superapp/widgets.py` & `django_superapp-1.0.8/src/django_superapp/widgets.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.7/src/django_superapp.egg-info/PKG-INFO` & `django_superapp-1.0.8/src/django_superapp.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_superapp
-Version: 1.0.7
+Version: 1.0.8
 Summary: Build your startup's product faster.
 Home-page: https://github.com/django-superapp/django-superapp
 Author: Django SuperApp
 Author-email: django-superapp@bringes.io
 License: MIT
 Project-URL: Bug Reports, https://github.com/django-superapp/django-superapp/issues
 Project-URL: Source, https://github.com/django-superapp/django-superapp
@@ -36,22 +36,30 @@
 Requires-Dist: django-admin-confirm>=1.0.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: copier>=9.2.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=2.7.1
 
 # Django SuperApp
+SuperApp is a framework on top of Django, designed to accelerate the development of software projects for startups. It incorporates all the powerful features of Django, plus additional tools to seamlessly integrate various applications.
+
+![django-superapp-demo](https://django-superapp.bringes.io/assets/docs/admin-portal/admin-portal.svg "Django SuperApp")
 
 ### Getting Started
 ```bash
 pipx install django_superapp
-django_superapp create-project test_project
-cd test_project
-django_superapp add-app --app-name sample_app
+django_superapp create-project --project-template default ./my_superapp
+cd my_superapp
+django_superapp create-app --app-template sample_app
+make setup-sample-env
+make start-docker
 ```
 
+### Documentation
+For a more detailed documentation, visit [https://django-superapp.bringes.io](https://django-superapp.bringes.io).
+
 ### Development
 ```bash
 make install-requirements
 make install
 make release
 ```
```

### Comparing `django_superapp-1.0.7/src/django_superapp.egg-info/SOURCES.txt` & `django_superapp-1.0.8/src/django_superapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

