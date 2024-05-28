# Comparing `tmp/django_eztaskmanager-0.3.1.tar.gz` & `tmp/django_eztaskmanager-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eztaskmanager-0.3.1.tar", max compression
+gzip compressed data, was "django_eztaskmanager-0.3.7.tar", max compression
```

## Comparing `django_eztaskmanager-0.3.1.tar` & `django_eztaskmanager-0.3.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      381 2024-04-09 14:45:55.746954 django_eztaskmanager-0.3.1/AUTHORS.md
--rw-r--r--   0        0        0    34283 2024-04-09 14:45:55.746954 django_eztaskmanager-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     8084 2024-04-09 14:45:55.746954 django_eztaskmanager-0.3.1/README.md
--rw-r--r--   0        0        0      265 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/__init__.py
--rw-r--r--   0        0        0    14211 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/admin.py
--rw-r--r--   0        0        0     1445 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/__init__.py
--rw-r--r--   0        0        0      185 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/commands/__init__.py
--rw-r--r--   0        0        0     1008 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/commands/collectcommands.py
--rw-r--r--   0        0        0     1096 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_command.py
--rw-r--r--   0        0        0     1887 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_livelogging_command.py
--rw-r--r--   0        0        0     1722 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_logging_command.py
--rw-r--r--   0        0        0     4929 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/0001_initial.py
--rw-r--r--   0        0        0      473 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/0002_task_scheduled_job_id.py
--rw-r--r--   0        0        0      653 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py
--rw-r--r--   0        0        0        0 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/__init__.py
--rw-r--r--   0        0        0     5437 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14196 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/models.py
--rw-r--r--   0        0        0     3598 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/services/__init__.py
--rw-r--r--   0        0        0     2965 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/services/logger.py
--rw-r--r--   0        0        0     5546 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/services/notifications.py
--rw-r--r--   0        0        0     6057 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/services/queues.py
--rw-r--r--   0        0        0     2281 2024-04-09 14:45:55.758954 django_eztaskmanager-0.3.1/eztaskmanager/settings.py
--rw-r--r--   0        0        0      362 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/img/iconfinder_ic_wrap_text.png
--rw-r--r--   0        0        0      278 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/img/icons8-double-down-32.png
--rw-r--r--   0        0        0      175 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/img/icons8-new-document-32.png
--rw-r--r--   0        0        0    46173 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/js/axios.js
--rw-r--r--   0        0        0    19574 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/js/linkify.min.js
--rw-r--r--   0        0        0     3029 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/js/menu_filter_collapse.js
--rw-r--r--   0        0        0   342146 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/static/js/vue.js
--rw-r--r--   0        0        0      305 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/templates/admin/appcommand_changeform.html
--rw-r--r--   0        0        0      289 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/templates/admin/custom_changeform.html
--rw-r--r--   0        0        0     3854 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/templates/admin/edit_inline/tabular_reports.html
--rw-r--r--   0        0        0    12853 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/templates/live_log_viewer.html
--rw-r--r--   0        0        0      286 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/templates/log_viewer.html
--rw-r--r--   0        0        0    16778 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/tests/test_admin.py
--rw-r--r--   0        0        0     1825 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/tests/test_logger.py
--rw-r--r--   0        0        0     8604 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/tests/test_models.py
--rw-r--r--   0        0        0    19344 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/tests/test_services.py
--rw-r--r--   0        0        0     8064 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/tests/test_views.py
--rw-r--r--   0        0        0      504 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/urls.py
--rw-r--r--   0        0        0     4018 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/eztaskmanager/views.py
--rw-r--r--   0        0        0     2369 2024-04-09 14:45:55.762954 django_eztaskmanager-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10210 1970-01-01 00:00:00.000000 django_eztaskmanager-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/AUTHORS.md
+-rw-r--r--   0        0        0    34283 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/LICENSE.md
+-rw-r--r--   0        0        0     8084 2024-05-28 14:29:04.795775 django_eztaskmanager-0.3.7/README.md
+-rw-r--r--   0        0        0      265 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/__init__.py
+-rw-r--r--   0        0        0    14211 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/admin.py
+-rw-r--r--   0        0        0     1445 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/apps.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/collectcommands.py
+-rw-r--r--   0        0        0     1096 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_command.py
+-rw-r--r--   0        0        0     1887 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_livelogging_command.py
+-rw-r--r--   0        0        0     1722 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_logging_command.py
+-rw-r--r--   0        0        0     4929 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0001_initial.py
+-rw-r--r--   0        0        0      473 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0002_task_scheduled_job_id.py
+-rw-r--r--   0        0        0      653 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__init__.py
+-rw-r--r--   0        0        0     5437 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14196 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/models.py
+-rw-r--r--   0        0        0     3598 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/__init__.py
+-rw-r--r--   0        0        0     2965 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/logger.py
+-rw-r--r--   0        0        0     5546 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/notifications.py
+-rw-r--r--   0        0        0     6930 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/services/queues.py
+-rw-r--r--   0        0        0     2281 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/settings.py
+-rw-r--r--   0        0        0      362 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/iconfinder_ic_wrap_text.png
+-rw-r--r--   0        0        0      278 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/icons8-double-down-32.png
+-rw-r--r--   0        0        0      175 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/img/icons8-new-document-32.png
+-rw-r--r--   0        0        0    46173 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/axios.js
+-rw-r--r--   0        0        0    19574 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/linkify.min.js
+-rw-r--r--   0        0        0     3029 2024-05-28 14:29:04.811775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/menu_filter_collapse.js
+-rw-r--r--   0        0        0   342146 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/static/js/vue.js
+-rw-r--r--   0        0        0      305 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/appcommand_changeform.html
+-rw-r--r--   0        0        0      289 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/custom_changeform.html
+-rw-r--r--   0        0        0     3854 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/edit_inline/tabular_reports.html
+-rw-r--r--   0        0        0    12853 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/live_log_viewer.html
+-rw-r--r--   0        0        0      286 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/templates/log_viewer.html
+-rw-r--r--   0        0        0    16778 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_admin.py
+-rw-r--r--   0        0        0     1825 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_logger.py
+-rw-r--r--   0        0        0     8604 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_models.py
+-rw-r--r--   0        0        0    20709 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_services.py
+-rw-r--r--   0        0        0     8064 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/tests/test_views.py
+-rw-r--r--   0        0        0      504 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/urls.py
+-rw-r--r--   0        0        0     4018 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/eztaskmanager/views.py
+-rw-r--r--   0        0        0     2369 2024-05-28 14:29:04.815775 django_eztaskmanager-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    10210 1970-01-01 00:00:00.000000 django_eztaskmanager-0.3.7/PKG-INFO
```

### Comparing `django_eztaskmanager-0.3.1/LICENSE.md` & `django_eztaskmanager-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/README.md` & `django_eztaskmanager-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/admin.py` & `django_eztaskmanager-0.3.7/eztaskmanager/admin.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/apps.py` & `django_eztaskmanager-0.3.7/eztaskmanager/apps.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/management/commands/collectcommands.py` & `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/collectcommands.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_command.py` & `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_livelogging_command.py` & `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_livelogging_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/management/commands/test_logging_command.py` & `django_eztaskmanager-0.3.7/eztaskmanager/management/commands/test_logging_command.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/migrations/0001_initial.py` & `django_eztaskmanager-0.3.7/eztaskmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py` & `django_eztaskmanager-0.3.7/eztaskmanager/migrations/0003_alter_task_cached_next_ride_alter_task_scheduling.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django_eztaskmanager-0.3.7/eztaskmanager/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/models.py` & `django_eztaskmanager-0.3.7/eztaskmanager/models.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/services/__init__.py` & `django_eztaskmanager-0.3.7/eztaskmanager/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/services/logger.py` & `django_eztaskmanager-0.3.7/eztaskmanager/services/logger.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/services/notifications.py` & `django_eztaskmanager-0.3.7/eztaskmanager/services/notifications.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/services/queues.py` & `django_eztaskmanager-0.3.7/eztaskmanager/services/queues.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 - RQTaskQueueService implements the service with Redis Queue.
 - CeleryTaskQueueService implements the service with Celery (TBD)
 """
 import datetime
 from abc import ABC, abstractmethod
 
-import django_rq
-from celery import Celery, shared_task
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
-from eztaskmanager.models import Task
 from eztaskmanager.settings import EZTASKMANAGER_QUEUE_SERVICE_TYPE
+from ..models import Task
 
 
 class TaskQueueService(ABC):
     """Abstract base class for managing task queues."""
 
     @abstractmethod
     def add(self, task):  # pragma: no cover
@@ -29,150 +27,170 @@
 
     @abstractmethod
     def remove(self, task):  # pragma: no cover
         """To be implemented in concrete subclasses."""
         pass
 
 
-def get_task_service():
-    """Fetch the correct queue service, based on settings."""
-    if EZTASKMANAGER_QUEUE_SERVICE_TYPE == 'RQ':
-        return RQTaskQueueService()
-    else:
-        return CeleryTaskQueueService()
-
-
 class TaskQueueException(Exception):
     """Dedicated exception for TaskQueue classes."""
 
     pass
 
 
-class RQTaskQueueService(TaskQueueService):
-    """
-    A subclass of TaskQueueService that manages tasks using RQ (Redis Queue).
-
-    Attributes:
-        queue (Queue): The default RQ queue.
+# conditional import
+try:
+    import django_rq
 
-    Methods:
-        - add(task, at=None): Enqueues a task to be executed either immediately or at a specific time.
-        - remove(task): Cancels a task if it is currently in the queue.
+    class RQTaskQueueService(TaskQueueService):
+        """
+        A subclass of TaskQueueService that manages tasks using RQ (Redis Queue).
 
-    """
+        Attributes:
+            queue (Queue): The default RQ queue.
 
-    def __init__(self):
-        self.queue = django_rq.get_queue('default')
-        self.scheduler = django_rq.get_scheduler('default', interval=60)
+        Methods:
+            - add(task, at=None): Enqueues a task to be executed either immediately or at a specific time.
+            - remove(task): Cancels a task if it is currently in the queue.
 
-    def add(self, task: Task):
         """
-        Add the task to the Redis queue.
 
-        Args:
-            task: The task to be added.
+        def __init__(self):
+            self.queue = django_rq.get_queue('default')
+            self.scheduler = django_rq.get_scheduler('default', interval=60)
+
+        def add(self, task: Task):
+            """
+            Add the task to the Redis queue.
+
+            Args:
+                task: The task to be added.
+
+            Returns:
+                The job created for the task, either scheduled or enqueued for immediate execution.
+
+            Raises:
+                 Exception: If there is an error while launching the task.
+
+            """
+            from eztaskmanager.services import run_management_command
+
+            if task.scheduling and task.scheduling_utc < timezone.now():
+                raise TaskQueueException(_("It is not possible to schedule tasks in the past"))
+
+            try:
+                if task.scheduling:
+                    if task.is_periodic:
+                        # schedule execution at a point in time, with periodicity
+                        rq_job = self.scheduler.schedule(
+                            task.scheduling_utc,
+                            run_management_command, [task.id],
+                            interval=task.interval_in_seconds,
+                            result_ttl=int(1.5 * task.interval_in_seconds)
+                        )
+                    else:
+                        # schedule execution at a point in time, with periodicity
+                        rq_job = self.scheduler.enqueue_at(
+                            task.scheduling_utc,
+                            run_management_command, task.id
+                        )
+                    task.scheduled_job_id = rq_job.id
+                    task.status = Task.STATUS_SCHEDULED
+                    job_id, task.cached_next_ride = self.fetch_job_with_next_time(task)
+                    task.save()
+                else:
+                    # enqueue for immediate execution
+                    rq_job = self.queue.enqueue(run_management_command, task.id)
+                return rq_job
+            except Exception as e:
+                raise TaskQueueException(_(f"Failed to add task: {e}")) from e
+
+        def fetch_job_with_next_time(self, task):
+            """Fetch the next job in the queue, with its execution time."""
+            try:
+                job_id, next_time = next(
+                    (j, next_time) for j, next_time in self.scheduler.get_jobs(with_times=True)
+                    if j.id == task.scheduled_job_id
+                )
+                next_time = timezone.make_aware(next_time, timezone=timezone.timezone.utc)
+                return job_id, next_time
+            except StopIteration:
+                return None, None
+
+        def remove(self, task):
+            """Remove the job from the queue and updates the tasks' values."""
+            job, next_time = self.fetch_job_with_next_time(task)
+
+            if job:
+                self.scheduler.cancel(job)
+                task.scheduled_job_id = None
+                task.cached_next_ride = None
+                task.status = Task.STATUS_IDLE
+                task.save()
 
-        Returns:
-            The job created for the task, either scheduled or enqueued for immediate execution.
+    available_service = RQTaskQueueService
 
-        Raises:
-             Exception: If there is an error while launching the task.
+except ImportError:
+    try:
+        from celery import Celery, shared_task
 
-        """
-        from eztaskmanager.services import run_management_command
 
-        if task.scheduling and task.scheduling_utc < timezone.now():
-            raise TaskQueueException(_("It is not possible to schedule tasks in the past"))
+        class CeleryTaskQueueService(TaskQueueService):
+            """A subclass of TaskQueueService that manages tasks using Celery."""
 
-        try:
-            if task.scheduling:
-                if task.is_periodic:
-                    # schedule execution at a point in time, with periodicity
-                    rq_job = self.scheduler.schedule(
-                        task.scheduling_utc,
-                        run_management_command, [task.id],
-                        interval=task.interval_in_seconds,
-                        result_ttl=int(1.5 * task.interval_in_seconds)
-                    )
-                else:
-                    # schedule execution at a point in time, with periodicity
-                    rq_job = self.scheduler.enqueue_at(
-                        task.scheduling_utc,
-                        run_management_command, task.id
-                    )
-                task.scheduled_job_id = rq_job.id
-                task.status = Task.STATUS_SCHEDULED
-                job_id, task.cached_next_ride = self.fetch_job_with_next_time(task)
-                task.save()
-            else:
-                # enqueue for immediate execution
-                rq_job = self.queue.enqueue(run_management_command, task.id)
-            return rq_job
-        except Exception as e:
-            raise TaskQueueException(_(f"Failed to add task: {e}")) from e
-
-    def fetch_job_with_next_time(self, task):
-        """Fetch the next job in the queue, with its execution time."""
-        try:
-            job_id, next_time = next(
-                (j, next_time) for j, next_time in self.scheduler.get_jobs(with_times=True)
-                if j.id == task.scheduled_job_id
-            )
-            next_time = timezone.make_aware(next_time, timezone=timezone.timezone.utc)
-            return job_id, next_time
-        except StopIteration:
-            return None, None
-
-    def remove(self, task):
-        """Remove the job from the queue and updates the tasks' values."""
-        job, next_time = self.fetch_job_with_next_time(task)
-
-        if job:
-            self.scheduler.cancel(job)
-            task.scheduled_job_id = None
-            task.cached_next_ride = None
-            task.status = Task.STATUS_IDLE
-            task.save()
-
-
-@shared_task
-def execute_management_command(task):
-    """Wrap the management command executor for Celery."""
-    from eztaskmanager.services import run_management_command
-
-    return run_management_command(task)
-
-
-class CeleryTaskQueueService(TaskQueueService):
-    """A subclass of TaskQueueService that manages tasks using Celery."""
-
-    def __init__(self):
-        self.app = Celery(
-            'tasks',
-            broker='redis://redis:6379/1', backend='redis://redis:6379:2'
-        )
-
-    def add(self, task: Task):
-        """Add a task to the Celery queue."""
-        try:
-            if task.scheduling:
-                delay = task.scheduling - datetime.datetime.now()
-                self.app.send_task(
-                    'eztaskmanager.services.queues.execute_management_command',
-                    args=[task],
-                    countdown=delay.total_seconds()
+            def __init__(self):
+                self.app = Celery(
+                    'tasks',
+                    broker='redis://redis:6379/1', backend='redis://redis:6379:2'
                 )
-            else:
-                self.app.send_task('eztaskmanager.services.queues.execute_management_command', args=[task])
 
-            return True
-        except Exception as e:
-            print(f"Error while launching task: {e}")
-
-    def remove(self, task):
-        """Remove a job from the Celery queue."""
-        try:
-            # With Celery, it's not straightforward to remove a task from the queue
-            # The recommended way to stop a task is to revoke it
-            self.app.control.revoke(task.id)
-        except Exception as e:
-            print(f"Error while halting task: {e}")
+            def add(self, task: Task):
+                """Add a task to the Celery queue."""
+                try:
+                    if task.scheduling:
+                        delay = task.scheduling - datetime.datetime.now()
+                        self.app.send_task(
+                            'eztaskmanager.services.queues.execute_management_command',
+                            args=[task],
+                            countdown=delay.total_seconds()
+                        )
+                    else:
+                        self.app.send_task('eztaskmanager.services.queues.execute_management_command', args=[task])
+
+                    return True
+                except Exception as e:
+                    print(f"Error while launching task: {e}")
+
+            def remove(self, task):
+                """Remove a job from the Celery queue."""
+                try:
+                    # With Celery, it's not straightforward to remove a task from the queue
+                    # The recommended way to stop a task is to revoke it
+                    self.app.control.revoke(task.id)
+                except Exception as e:
+                    print(f"Error while halting task: {e}")
+
+
+        @shared_task
+        def execute_management_command(task):
+            """Wrap the management command executor for Celery."""
+            from eztaskmanager.services import run_management_command
+
+            return run_management_command(task)
+
+
+        available_service = CeleryTaskQueueService
+
+    except ImportError:
+        raise ImportError("Both django_rq and Celery packages are not installed.")
+
+
+def get_task_service():
+    """Fetch the correct queue service, based on settings."""
+    if EZTASKMANAGER_QUEUE_SERVICE_TYPE == 'RQ' or available_service == RQTaskQueueService:
+        return RQTaskQueueService()
+    else:
+        return CeleryTaskQueueService()
+
+
+
+
```

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/settings.py` & `django_eztaskmanager-0.3.7/eztaskmanager/settings.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/static/js/axios.js` & `django_eztaskmanager-0.3.7/eztaskmanager/static/js/axios.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/static/js/linkify.min.js` & `django_eztaskmanager-0.3.7/eztaskmanager/static/js/linkify.min.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/static/js/menu_filter_collapse.js` & `django_eztaskmanager-0.3.7/eztaskmanager/static/js/menu_filter_collapse.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/static/js/vue.js` & `django_eztaskmanager-0.3.7/eztaskmanager/static/js/vue.js`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/templates/admin/edit_inline/tabular_reports.html` & `django_eztaskmanager-0.3.7/eztaskmanager/templates/admin/edit_inline/tabular_reports.html`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/templates/live_log_viewer.html` & `django_eztaskmanager-0.3.7/eztaskmanager/templates/live_log_viewer.html`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/tests/test_admin.py` & `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/tests/test_logger.py` & `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/tests/test_models.py` & `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/tests/test_services.py` & `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,284 +6,304 @@
 from django.urls import reverse
 from django.utils import timezone
 
 import eztaskmanager
 from eztaskmanager.models import Task, LaunchReport
 from eztaskmanager.services.notifications import SlackNotificationHandler, LEVEL_MAPPING, MESSAGES, \
     EmailNotificationHandler, get_base_url, emit_notifications
-from eztaskmanager.services.queues import RQTaskQueueService, get_task_service, \
-    CeleryTaskQueueService, TaskQueueException
+
+from eztaskmanager.services.queues import get_task_service, TaskQueueException
+tsq_imported_module = None
+try:
+    from eztaskmanager.services.queues import RQTaskQueueService
+    tsq_imported_module = 'rq'
+except ImportError:
+    try:
+        from eztaskmanager.services.queues import CeleryTaskQueueService
+        tsq_imported_module = 'celery'
+    except ImportError:
+        raise ImportError('Could not import a TaskQueueService: celery or django-rq must be installed')
 
 
 class GetTaskServiceTest(TestCase):
 
     @patch('django_rq.get_queue', return_value=MagicMock())
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.queues.EZTASKMANAGER_QUEUE_SERVICE_TYPE', new='RQ')
     def test_get_task_service_with_rq(self, mock_get_scheduler, mock_get_queue):
         """
         Test get_task_service function for 'RQ' service type
         """
-        service = get_task_service()
+        if tsq_imported_module == 'rq':
+            service = get_task_service()
 
-        # Assert that RQTaskQueueService instance is returned when 'RQ' is the type
-        self.assertIsInstance(service, RQTaskQueueService)
+            # Assert that RQTaskQueueService instance is returned when 'RQ' is the type
+            self.assertIsInstance(service, RQTaskQueueService)
 
-        mock_get_queue.assert_called_once_with('default')
-        mock_get_scheduler.assert_called_once_with('default', interval=60)
-        self.assertIsInstance(
-            service.queue, MagicMock
-        )
-        self.assertIsInstance(
-            service.scheduler, MagicMock
-        )
+            mock_get_queue.assert_called_once_with('default')
+            mock_get_scheduler.assert_called_once_with('default', interval=60)
+            self.assertIsInstance(
+                service.queue, MagicMock
+            )
+            self.assertIsInstance(
+                service.scheduler, MagicMock
+            )
 
     @patch('eztaskmanager.services.queues.EZTASKMANAGER_QUEUE_SERVICE_TYPE', new='Celery')
     def test_get_task_service_with_celery(self):
         """
         Test get_task_service function for non 'RQ' service type
         """
-        service = get_task_service()
+        if tsq_imported_module == 'celery':
+            service = get_task_service()
 
-        # Assert that CeleryTaskQueueService instance is returned when type is not 'RQ'
-        self.assertIsInstance(service, CeleryTaskQueueService)
+            # Assert that CeleryTaskQueueService instance is returned when type is not 'RQ'
+            self.assertIsInstance(service, CeleryTaskQueueService)
 
 
 class TestRQTaskQueueService(TestCase):
 
     @patch('django_rq.get_queue', return_value=MagicMock())
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.run_management_command')
     @patch('eztaskmanager.services.queues.RQTaskQueueService.fetch_job_with_next_time')
     def test_add_non_periodic_task(
             self,
             mock_fetch_job_with_next_time, mock_run_management_command,
             mock_get_scheduler, mock_get_queue
     ):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
+        if tsq_imported_module == 'rq':
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock Task instance
+            mock_task = MagicMock()
+            mock_task.scheduling = (datetime.now() + timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
+            mock_task.scheduling_utc = timezone.make_aware(
+                datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
+            )
+            mock_task.interval_in_seconds = None
+            mock_task.is_periodic = False
+            mock_task.id = 1
+
+            # mock fetch_job_with_next_time to return a demonstration value
+            mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
+
+            # mock run_management_command to return a demonstration value
+            mock_run_management_command.return_value = 'Demo Value'
+
+            # determine the return value of scheduler.schedule and queue.enqueue
+            mock_rq_enqueued_job = MagicMock(id='001-002-003-004')
+            service.scheduler.enqueue_at.return_value = mock_rq_enqueued_job
+
+            # Call the method
+            service.add(mock_task)
 
-        # Create a mock Task instance
-        mock_task = MagicMock()
-        mock_task.scheduling = (datetime.now() + timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
-        mock_task.scheduling_utc = timezone.make_aware(
-            datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
-        )
-        mock_task.interval_in_seconds = None
-        mock_task.is_periodic = False
-        mock_task.id = 1
-
-        # mock fetch_job_with_next_time to return a demonstration value
-        mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
-
-        # mock run_management_command to return a demonstration value
-        mock_run_management_command.return_value = 'Demo Value'
-
-        # determine the return value of scheduler.schedule and queue.enqueue
-        mock_rq_enqueued_job = MagicMock(id='001-002-003-004')
-        service.scheduler.enqueue_at.return_value = mock_rq_enqueued_job
-
-        # Call the method
-        service.add(mock_task)
-
-        # Assert the methods were called with the right parameters
-        service.scheduler.enqueue_at.assert_called_once_with(
-            mock_task.scheduling_utc,
-            mock_run_management_command, mock_task.id
-        )
-
-        # Assert that the task has been assigned the correct attributes
-        self.assertEqual(mock_task.scheduled_job_id, mock_rq_enqueued_job.id)
-        self.assertEqual(mock_task.status, Task.STATUS_SCHEDULED)
-        self.assertEqual(mock_task.cached_next_ride, mock_fetch_job_with_next_time.return_value[1])
-
-        # If the task does not contain the schedule attribute, the queue.enqueue method should be called
-        mock_task.scheduling = None
-        service.add(mock_task)
-        service.queue.enqueue.assert_called_once_with(mock_run_management_command, mock_task.id)
+            # Assert the methods were called with the right parameters
+            service.scheduler.enqueue_at.assert_called_once_with(
+                mock_task.scheduling_utc,
+                mock_run_management_command, mock_task.id
+            )
+
+            # Assert that the task has been assigned the correct attributes
+            self.assertEqual(mock_task.scheduled_job_id, mock_rq_enqueued_job.id)
+            self.assertEqual(mock_task.status, Task.STATUS_SCHEDULED)
+            self.assertEqual(mock_task.cached_next_ride, mock_fetch_job_with_next_time.return_value[1])
+
+            # If the task does not contain the schedule attribute, the queue.enqueue method should be called
+            mock_task.scheduling = None
+            service.add(mock_task)
+            service.queue.enqueue.assert_called_once_with(mock_run_management_command, mock_task.id)
 
     @patch('django_rq.get_queue', return_value=MagicMock())
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.run_management_command')
     @patch('eztaskmanager.services.queues.RQTaskQueueService.fetch_job_with_next_time')
     def test_add_periodic_task(
             self,
             mock_fetch_job_with_next_time, mock_run_management_command,
             mock_get_scheduler, mock_get_queue
     ):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
+        if tsq_imported_module == 'rq':
+
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock Task instance
+            mock_task = MagicMock()
+            mock_task.scheduling = (datetime.now() + timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
+            mock_task.scheduling_utc = timezone.make_aware(
+                datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
+            )
+            mock_task.interval_in_seconds = 86400
+            mock_task.is_periodic = True
+            mock_task.id = 1
+
+            # mock fetch_job_with_next_time to return a demonstration value
+            mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
+
+            # mock run_management_command to return a demonstration value
+            mock_run_management_command.return_value = 'Demo Value'
+
+            # determine the return value of scheduler.schedule and queue.enqueue
+            mock_rq_scheduled_job = MagicMock(id='001-001-001-001')
+            mock_rq_enqueued_job = MagicMock(id='002-002-002-002')
+            service.scheduler.schedule.return_value = mock_rq_scheduled_job
+            service.queue.enqueue.return_value = mock_rq_enqueued_job
+
+            # Call the method
+            service.add(mock_task)
 
-        # Create a mock Task instance
-        mock_task = MagicMock()
-        mock_task.scheduling = (datetime.now() + timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
-        mock_task.scheduling_utc = timezone.make_aware(
-            datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
-        )
-        mock_task.interval_in_seconds = 86400
-        mock_task.is_periodic = True
-        mock_task.id = 1
-
-        # mock fetch_job_with_next_time to return a demonstration value
-        mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
-
-        # mock run_management_command to return a demonstration value
-        mock_run_management_command.return_value = 'Demo Value'
-
-        # determine the return value of scheduler.schedule and queue.enqueue
-        mock_rq_scheduled_job = MagicMock(id='001-001-001-001')
-        mock_rq_enqueued_job = MagicMock(id='002-002-002-002')
-        service.scheduler.schedule.return_value = mock_rq_scheduled_job
-        service.queue.enqueue.return_value = mock_rq_enqueued_job
-
-        # Call the method
-        service.add(mock_task)
-
-        # Assert the methods were called with the right parameters
-        service.scheduler.schedule.assert_called_once_with(
-            mock_task.scheduling_utc,
-            mock_run_management_command, [mock_task.id],
-            interval=mock_task.interval_in_seconds,
-            result_ttl=int(1.5 * mock_task.interval_in_seconds)
-        )
-
-        # Assert that the task has been assigned the correct attributes
-        self.assertEqual(mock_task.scheduled_job_id, mock_rq_scheduled_job.id)
-        self.assertEqual(mock_task.status, Task.STATUS_SCHEDULED)
-        self.assertEqual(mock_task.cached_next_ride, mock_fetch_job_with_next_time.return_value[1])
-
-        # If the task does not contain the schedule attribute, the queue.enqueue method should be called
-        mock_task.scheduling = False
-        service.add(mock_task)
-        service.queue.enqueue.assert_called_once_with(mock_run_management_command, mock_task.id)
+            # Assert the methods were called with the right parameters
+            service.scheduler.schedule.assert_called_once_with(
+                mock_task.scheduling_utc,
+                mock_run_management_command, [mock_task.id],
+                interval=mock_task.interval_in_seconds,
+                result_ttl=int(1.5 * mock_task.interval_in_seconds)
+            )
+
+            # Assert that the task has been assigned the correct attributes
+            self.assertEqual(mock_task.scheduled_job_id, mock_rq_scheduled_job.id)
+            self.assertEqual(mock_task.status, Task.STATUS_SCHEDULED)
+            self.assertEqual(mock_task.cached_next_ride, mock_fetch_job_with_next_time.return_value[1])
+
+            # If the task does not contain the schedule attribute, the queue.enqueue method should be called
+            mock_task.scheduling = False
+            service.add(mock_task)
+            service.queue.enqueue.assert_called_once_with(mock_run_management_command, mock_task.id)
 
     @patch('django_rq.get_queue', return_value=MagicMock())
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.run_management_command')
     @patch('eztaskmanager.services.queues.RQTaskQueueService.fetch_job_with_next_time')
     def test_add_with_exception(
             self,
             mock_fetch_job_with_next_time, mock_run_management_command,
             mock_get_scheduler, mock_get_queue
     ):
-        # Setup
-        service = RQTaskQueueService()
-        mock_task = MagicMock()
-        mock_task.scheduling = (datetime.now() - timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
-        mock_task.scheduling_utc = timezone.make_aware(
-            datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
-        )
-        mock_run_management_command.return_value = 'Demo Value'
-        mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
-
-        # Call the method and assert it raises the expected exception
-        with self.assertRaises(TaskQueueException) as context:
-            service.add(mock_task)
+        if tsq_imported_module == 'rq':
+            # Setup
+            service = RQTaskQueueService()
+            mock_task = MagicMock()
+            mock_task.scheduling = (datetime.now() - timedelta(days=5)).strftime("%Y-%m-%d %H:%M:%S")
+            mock_task.scheduling_utc = timezone.make_aware(
+                datetime.strptime(mock_task.scheduling, "%Y-%m-%d %H:%M:%S")
+            )
+            mock_run_management_command.return_value = 'Demo Value'
+            mock_fetch_job_with_next_time.return_value = ('Demo Ride', 'Demo time')
+
+            # Call the method and assert it raises the expected exception
+            with self.assertRaises(TaskQueueException) as context:
+                service.add(mock_task)
 
-        # Assert the exception message is as expected
-        self.assertTrue('It is not possible to schedule tasks in the past' in str(context.exception))
+            # Assert the exception message is as expected
+            self.assertTrue('It is not possible to schedule tasks in the past' in str(context.exception))
 
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.queues.RQTaskQueueService.fetch_job_with_next_time')
     def test_remove(self, mock_fetch_job_with_next_time, mock_get_scheduler):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
-
-        # Create a mock Task instance
-        mock_task = MagicMock()
-        mock_task.id = 1
-        mock_task.scheduled_job_id = 'job-id'
-
-        mock_job = MagicMock(id='job-id')
-        mock_fetch_job_with_next_time.return_value = (mock_job, 'next_time')
-
-        # Call the method
-        service.remove(mock_task)
-
-        # Assert the methods were called with the right parameters
-        mock_fetch_job_with_next_time.assert_called_once_with(mock_task)
-
-        # Assert the methods were called with the right parameters
-        service.scheduler.cancel.assert_called_once_with(mock_job)
-
-        # Assert the task attributes are correctly updated
-        self.assertEqual(mock_task.scheduled_job_id, None)
-        self.assertEqual(mock_task.cached_next_ride, None)
-        self.assertEqual(mock_task.status, Task.STATUS_IDLE)
-        mock_task.save.assert_called_once()
+        if tsq_imported_module == 'rq':
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock Task instance
+            mock_task = MagicMock()
+            mock_task.id = 1
+            mock_task.scheduled_job_id = 'job-id'
+
+            mock_job = MagicMock(id='job-id')
+            mock_fetch_job_with_next_time.return_value = (mock_job, 'next_time')
+
+            # Call the method
+            service.remove(mock_task)
+
+            # Assert the methods were called with the right parameters
+            mock_fetch_job_with_next_time.assert_called_once_with(mock_task)
+
+            # Assert the methods were called with the right parameters
+            service.scheduler.cancel.assert_called_once_with(mock_job)
+
+            # Assert the task attributes are correctly updated
+            self.assertEqual(mock_task.scheduled_job_id, None)
+            self.assertEqual(mock_task.cached_next_ride, None)
+            self.assertEqual(mock_task.status, Task.STATUS_IDLE)
+            mock_task.save.assert_called_once()
 
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     @patch('eztaskmanager.services.queues.RQTaskQueueService.fetch_job_with_next_time')
     def test_remove_non_existing_job(self, mock_fetch_job_with_next_time, mock_get_scheduler):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
-
-        # Create a mock Task instance
-        mock_task = MagicMock()
-        mock_task.scheduled_job_id = None
-        mock_task.cached_next_ride = None
-        mock_task.status = Task.STATUS_SCHEDULED
-
-        # mock the return value of fetch_job_with_next_time
-        mock_fetch_job_with_next_time.return_value = (None, None)
-
-        # Call the method
-        service.remove(mock_task)
-
-        # Assert the methods were called with the right parameters
-        mock_fetch_job_with_next_time.assert_called_once_with(mock_task)
-
-        # Assert scheduler.cancel was not called
-        service.scheduler.cancel.assert_not_called()
-
-        # Assert the task attributes were not updated
-        assert not mock_task.scheduled_job_id
-        assert not mock_task.cached_next_ride
-        assert not mock_task.status == Task.STATUS_IDLE
-        mock_task.save.assert_not_called()
+        if tsq_imported_module == 'rq':
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock Task instance
+            mock_task = MagicMock()
+            mock_task.scheduled_job_id = None
+            mock_task.cached_next_ride = None
+            mock_task.status = Task.STATUS_SCHEDULED
+
+            # mock the return value of fetch_job_with_next_time
+            mock_fetch_job_with_next_time.return_value = (None, None)
+
+            # Call the method
+            service.remove(mock_task)
+
+            # Assert the methods were called with the right parameters
+            mock_fetch_job_with_next_time.assert_called_once_with(mock_task)
+
+            # Assert scheduler.cancel was not called
+            service.scheduler.cancel.assert_not_called()
+
+            # Assert the task attributes were not updated
+            assert not mock_task.scheduled_job_id
+            assert not mock_task.cached_next_ride
+            assert not mock_task.status == Task.STATUS_IDLE
+            mock_task.save.assert_not_called()
 
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     def test_fetch_job_with_next_time_job_exists(self, mock_get_scheduler):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
-
-        # Create a mock task
-        mock_task = MagicMock()
-        mock_task.scheduled_job_id = 'job-id'
-
-        # mock the return value of scheduler.get_jobs
-        mock_job = MagicMock(id='job-id')
-        next_time = datetime.now() + timedelta(days=1)
-        service.scheduler.get_jobs.return_value = [(mock_job, next_time)]
-
-        # Call the method
-        job, next_run_time = service.fetch_job_with_next_time(mock_task)
-
-        # Assert the method returns the correct job and next_time
-        self.assertEqual(job, mock_job)
-        self.assertEqual(next_run_time, timezone.make_aware(next_time, timezone=timezone.timezone.utc))
+        if tsq_imported_module == 'rq':
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock task
+            mock_task = MagicMock()
+            mock_task.scheduled_job_id = 'job-id'
+
+            # mock the return value of scheduler.get_jobs
+            mock_job = MagicMock(id='job-id')
+            next_time = datetime.now() + timedelta(days=1)
+            service.scheduler.get_jobs.return_value = [(mock_job, next_time)]
+
+            # Call the method
+            job, next_run_time = service.fetch_job_with_next_time(mock_task)
+
+            # Assert the method returns the correct job and next_time
+            self.assertEqual(job, mock_job)
+            self.assertEqual(next_run_time, timezone.make_aware(next_time, timezone=timezone.timezone.utc))
 
     @patch('django_rq.get_scheduler', return_value=MagicMock())
     def test_fetch_job_with_next_time_job_not_exists(self, mock_scheduler):
-        # Create the instance of the RQTaskQueueService
-        service = RQTaskQueueService()
-
-        # Create a mock task
-        mock_task = MagicMock()
-        mock_task.scheduled_job_id = 'job_id'
-
-        # mock the return value of scheduler.get_jobs
-        mock_scheduler.get_jobs.return_value = [(MagicMock(id='other_job_id'), 'next_time')]
-
-        # Call the method
-        job, next_time = service.fetch_job_with_next_time(mock_task)
-
-        # Assert the method returns None, None if the job is not found
-        self.assertEqual(job, None)
-        self.assertEqual(next_time, None)
+        if tsq_imported_module == 'rq':
+            # Create the instance of the RQTaskQueueService
+            service = RQTaskQueueService()
+
+            # Create a mock task
+            mock_task = MagicMock()
+            mock_task.scheduled_job_id = 'job_id'
+
+            # mock the return value of scheduler.get_jobs
+            mock_scheduler.get_jobs.return_value = [(MagicMock(id='other_job_id'), 'next_time')]
+
+            # Call the method
+            job, next_time = service.fetch_job_with_next_time(mock_task)
+
+            # Assert the method returns None, None if the job is not found
+            self.assertEqual(job, None)
+            self.assertEqual(next_time, None)
 
 
 class TestSlackNotificationHandler(TestCase):
 
     @patch('slack_sdk.WebClient')
     def test_init(self, mock_webclient):
         # Setup
```

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/tests/test_views.py` & `django_eztaskmanager-0.3.7/eztaskmanager/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/eztaskmanager/views.py` & `django_eztaskmanager-0.3.7/eztaskmanager/views.py`

 * *Files identical despite different names*

### Comparing `django_eztaskmanager-0.3.1/pyproject.toml` & `django_eztaskmanager-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-eztaskmanager"
-version = "0.3.1"
+version = "0.3.7"
 packages = [{include = "eztaskmanager"}]
 description = "Django application that allows the management of scheduled, long, asynchronous tasks."
 license = "MIT License"
 authors = ["Guglielmo Celata <guglielmo@openpolis.it>"]
 readme = "README.md"
 homepage = "https://github.com/openpolis/django-eztaskmanager.git"
 repository = "https://github.com/openpolis/django-eztaskmanager.git"
```

### Comparing `django_eztaskmanager-0.3.1/PKG-INFO` & `django_eztaskmanager-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eztaskmanager
-Version: 0.3.1
+Version: 0.3.7
 Summary: Django application that allows the management of scheduled, long, asynchronous tasks.
 Home-page: https://github.com/openpolis/django-eztaskmanager.git
 License: MIT
 Keywords: async,cron,django,commands,manager,queues,task,timer,scheduling,rq,celery
 Author: Guglielmo Celata
 Author-email: guglielmo@openpolis.it
 Requires-Python: >=3.10
```

