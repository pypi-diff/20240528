# Comparing `tmp/django_eztaskmanager-0.3.7.tar.gz` & `tmp/django_eztaskmanager-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eztaskmanager-0.3.7.tar", max compression
+gzip compressed data, was "django_eztaskmanager-0.3.8.tar", max compression
```

## Comparing `django_eztaskmanager-0.3.7.tar` & `django_eztaskmanager-0.3.8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      381 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/AUTHORS.md
--rw-r--r--   0        0        0    34283 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/LICENSE.md
--rw-r--r--   0        0        0     8084 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/README.md
--rw-r--r--   0        0        0      265 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/__init__.py
--rw-r--r--   0        0        0    14211 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/admin.py
--rw-r--r--   0        0        0     1445 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/apps.py
--rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/__init__.py
--rw-r--r--   0        0        0      185 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/collectcommands.py
--rw-r--r--   0        0        0     1096 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_command.py
--rw-r--r--   0        0        0     1887 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_livelogging_command.py
--rw-r--r--   0        0        0     1722 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_logging_command.py
--rw-r--r--   0        0        0     4929 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0001_initial.py
--rw-r--r--   0        0        0      473 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0002_task_scheduled_job_id.py
--rw-r--r--   0        0        0      653 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py
--rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__init__.py
--rw-r--r--   0        0        0     5437 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14196 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/models.py
--rw-r--r--   0        0        0     3598 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/__init__.py
--rw-r--r--   0        0        0     2965 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/logger.py
--rw-r--r--   0        0        0     5546 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/notifications.py
--rw-r--r--   0        0        0     6930 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/queues.py
--rw-r--r--   0        0        0     2281 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/settings.py
--rw-r--r--   0        0        0      362 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/iconfinder_ic_wrap_text.png
--rw-r--r--   0        0        0      278 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/icons8-double-down-32.png
--rw-r--r--   0        0        0      175 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/icons8-new-document-32.png
--rw-r--r--   0        0        0    46173 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/axios.js
--rw-r--r--   0        0        0    19574 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/linkify.min.js
--rw-r--r--   0        0        0     3029 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/menu_filter_collapse.js
--rw-r--r--   0        0        0   342146 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/vue.js
--rw-r--r--   0        0        0      305 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/appcommand_changeform.html
--rw-r--r--   0        0        0      289 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/custom_changeform.html
--rw-r--r--   0        0        0     3854 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/edit_inline/tabular_reports.html
--rw-r--r--   0        0        0    12853 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/live_log_viewer.html
--rw-r--r--   0        0        0      286 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/log_viewer.html
--rw-r--r--   0        0        0    16778 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_admin.py
--rw-r--r--   0        0        0     1825 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_logger.py
--rw-r--r--   0        0        0     8604 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_models.py
--rw-r--r--   0        0        0    20709 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_services.py
--rw-r--r--   0        0        0     8064 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_views.py
--rw-r--r--   0        0        0      504 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/urls.py
--rw-r--r--   0        0        0     4018 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/views.py
--rw-r--r--   0        0        0     2369 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    10210 1970-01-01 00:00:00.000000 django_eztaskmanager-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-05-28 15:34:00.658754 django_eztaskmanager-0.3.8/AUTHORS.md
+-rw-r--r--   0        0        0    34283 2024-05-28 15:34:00.658754 django_eztaskmanager-0.3.8/LICENSE.md
+-rw-r--r--   0        0        0     8084 2024-05-28 15:34:00.658754 django_eztaskmanager-0.3.8/README.md
+-rw-r--r--   0        0        0      265 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/__init__.py
+-rw-r--r--   0        0        0    14211 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/admin.py
+-rw-r--r--   0        0        0     1445 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/apps.py
+-rw-r--r--   0        0        0     5004 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/commands/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/commands/collectcommands.py
+-rw-r--r--   0        0        0     1096 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_command.py
+-rw-r--r--   0        0        0     1887 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_livelogging_command.py
+-rw-r--r--   0        0        0     1722 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_logging_command.py
+-rw-r--r--   0        0        0     4929 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/0001_initial.py
+-rw-r--r--   0        0        0      473 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/0002_task_scheduled_job_id.py
+-rw-r--r--   0        0        0      653 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/__init__.py
+-rw-r--r--   0        0        0     5437 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14196 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/models.py
+-rw-r--r--   0        0        0     3598 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/services/__init__.py
+-rw-r--r--   0        0        0     2965 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/services/logger.py
+-rw-r--r--   0        0        0     5546 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/services/notifications.py
+-rw-r--r--   0        0        0     6930 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/services/queues.py
+-rw-r--r--   0        0        0     2281 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/settings.py
+-rw-r--r--   0        0        0      362 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/img/iconfinder_ic_wrap_text.png
+-rw-r--r--   0        0        0      278 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/img/icons8-double-down-32.png
+-rw-r--r--   0        0        0      175 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/img/icons8-new-document-32.png
+-rw-r--r--   0        0        0    46173 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/js/axios.js
+-rw-r--r--   0        0        0    19574 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/js/linkify.min.js
+-rw-r--r--   0        0        0     3029 2024-05-28 15:34:00.674754 django_eztaskmanager-0.3.8/eztaskmanager/static/js/menu_filter_collapse.js
+-rw-r--r--   0        0        0   342146 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/static/js/vue.js
+-rw-r--r--   0        0        0      305 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/templates/admin/appcommand_changeform.html
+-rw-r--r--   0        0        0      289 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/templates/admin/custom_changeform.html
+-rw-r--r--   0        0        0     3854 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/templates/admin/edit_inline/tabular_reports.html
+-rw-r--r--   0        0        0    12853 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/templates/live_log_viewer.html
+-rw-r--r--   0        0        0      286 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/templates/log_viewer.html
+-rw-r--r--   0        0        0    16778 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/tests/test_admin.py
+-rw-r--r--   0        0        0     1825 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/tests/test_logger.py
+-rw-r--r--   0        0        0     8604 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/tests/test_models.py
+-rw-r--r--   0        0        0    20709 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/tests/test_services.py
+-rw-r--r--   0        0        0     8064 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/tests/test_views.py
+-rw-r--r--   0        0        0      504 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/urls.py
+-rw-r--r--   0        0        0     4018 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/eztaskmanager/views.py
+-rw-r--r--   0        0        0     2369 2024-05-28 15:34:00.678754 django_eztaskmanager-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    10210 1970-01-01 00:00:00.000000 django_eztaskmanager-0.3.8/PKG-INFO
```

### Comparing `django_eztaskmanager-0.3.7/LICENSE.md` & `django_eztaskmanager-0.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/README.md` & `django_eztaskmanager-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/admin.py` & `django_eztaskmanager-0.3.8/eztaskmanager/admin.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/apps.py` & `django_eztaskmanager-0.3.8/eztaskmanager/apps.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/collectcommands.py` & `django_eztaskmanager-0.3.8/eztaskmanager/management/commands/collectcommands.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_command.py` & `django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_livelogging_command.py` & `django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_livelogging_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_logging_command.py` & `django_eztaskmanager-0.3.8/eztaskmanager/management/commands/test_logging_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/migrations/0001_initial.py` & `django_eztaskmanager-0.3.8/eztaskmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py` & `django_eztaskmanager-0.3.8/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django_eztaskmanager-0.3.8/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/models.py` & `django_eztaskmanager-0.3.8/eztaskmanager/models.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/services/__init__.py` & `django_eztaskmanager-0.3.8/eztaskmanager/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/services/logger.py` & `django_eztaskmanager-0.3.8/eztaskmanager/services/logger.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/services/notifications.py` & `django_eztaskmanager-0.3.8/eztaskmanager/services/notifications.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/services/queues.py` & `django_eztaskmanager-0.3.8/eztaskmanager/services/queues.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/settings.py` & `django_eztaskmanager-0.3.8/eztaskmanager/settings.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/static/js/axios.js` & `django_eztaskmanager-0.3.8/eztaskmanager/static/js/axios.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/static/js/linkify.min.js` & `django_eztaskmanager-0.3.8/eztaskmanager/static/js/linkify.min.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/static/js/menu_filter_collapse.js` & `django_eztaskmanager-0.3.8/eztaskmanager/static/js/menu_filter_collapse.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/static/js/vue.js` & `django_eztaskmanager-0.3.8/eztaskmanager/static/js/vue.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/edit_inline/tabular_reports.html` & `django_eztaskmanager-0.3.8/eztaskmanager/templates/admin/edit_inline/tabular_reports.html`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/templates/live_log_viewer.html` & `django_eztaskmanager-0.3.8/eztaskmanager/templates/live_log_viewer.html`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_admin.py` & `django_eztaskmanager-0.3.8/eztaskmanager/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_logger.py` & `django_eztaskmanager-0.3.8/eztaskmanager/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_models.py` & `django_eztaskmanager-0.3.8/eztaskmanager/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_services.py` & `django_eztaskmanager-0.3.8/eztaskmanager/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_views.py` & `django_eztaskmanager-0.3.8/eztaskmanager/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/eztaskmanager/views.py` & `django_eztaskmanager-0.3.8/eztaskmanager/views.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.7/pyproject.toml` & `django_eztaskmanager-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-eztaskmanager"
-version = "0.3.7"
+version = "0.3.8"
 packages = [{include = "eztaskmanager"}]
 description = "Django application that allows the management of scheduled, long, asynchronous tasks."
 license = "MIT License"
 authors = ["Guglielmo Celata <guglielmo@openpolis.it>"]
 readme = "README.md"
 homepage = "https://github.com/openpolis/django-eztaskmanager.git"
 repository = "https://github.com/openpolis/django-eztaskmanager.git"
```

### Comparing `django_eztaskmanager-0.3.7/PKG-INFO` & `django_eztaskmanager-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eztaskmanager
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django application that allows the management of scheduled, long, asynchronous tasks.
 Home-page: https://github.com/openpolis/django-eztaskmanager.git
 License: MIT
 Keywords: async,cron,django,commands,manager,queues,task,timer,scheduling,rq,celery
 Author: Guglielmo Celata
 Author-email: guglielmo@openpolis.it
 Requires-Python: >=3.10
```

