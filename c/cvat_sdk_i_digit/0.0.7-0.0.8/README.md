# Comparing `tmp/cvat_sdk_i_digit-0.0.7.tar.gz` & `tmp/cvat_sdk_i_digit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk_i_digit-0.0.7.tar", last modified: Thu May 23 14:42:39 2024, max compression
+gzip compressed data, was "cvat_sdk_i_digit-0.0.8.tar", last modified: Tue May 28 07:43:36 2024, max compression
```

## Comparing `cvat_sdk_i_digit-0.0.7.tar` & `cvat_sdk_i_digit-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-05-23 02:59:28.391193 cvat_sdk_i_digit-0.0.7/LICENSE
--rw-r--r--   0        0        0     1599 2024-05-23 03:50:28.062949 cvat_sdk_i_digit-0.0.7/README.md
--rw-r--r--   0        0        0     1599 2024-05-23 03:50:28.062949 cvat_sdk_i_digit-0.0.7/README.md
--rw-r--r--   0        0        0      679 2024-05-23 14:42:39.691025 cvat_sdk_i_digit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 11:19:44.471973 cvat_sdk_i_digit-0.0.7/src/cvat_sdk_i_digit/__init__.py
--rw-r--r--   0        0        0     6031 2024-05-23 03:06:00.080006 cvat_sdk_i_digit-0.0.7/src/cvat_sdk_i_digit/config.py
--rw-r--r--   0        0        0     3586 2024-05-23 13:34:20.264919 cvat_sdk_i_digit-0.0.7/src/cvat_sdk_i_digit/cvat_api.py
--rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 cvat_sdk_i_digit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 02:59:28.391193 cvat_sdk_i_digit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1599 2024-05-23 03:50:28.062949 cvat_sdk_i_digit-0.0.8/README.md
+-rw-r--r--   0        0        0     1599 2024-05-23 03:50:28.062949 cvat_sdk_i_digit-0.0.8/README.md
+-rw-r--r--   0        0        0      679 2024-05-28 07:43:36.350901 cvat_sdk_i_digit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 11:19:44.471973 cvat_sdk_i_digit-0.0.8/src/cvat_sdk_i_digit/__init__.py
+-rw-r--r--   0        0        0     6031 2024-05-23 03:06:00.080006 cvat_sdk_i_digit-0.0.8/src/cvat_sdk_i_digit/config.py
+-rw-r--r--   0        0        0     4002 2024-05-28 07:42:07.910203 cvat_sdk_i_digit-0.0.8/src/cvat_sdk_i_digit/cvat_api.py
+-rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 cvat_sdk_i_digit-0.0.8/PKG-INFO
```

### Comparing `cvat_sdk_i_digit-0.0.7/LICENSE` & `cvat_sdk_i_digit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.7/README.md` & `cvat_sdk_i_digit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.7/pyproject.toml` & `cvat_sdk_i_digit-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cvat_sdk_i_digit"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = [
     { name = "Шумелев Дмитрий Игоревич", email = "cmit.dima@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "cvat-sdk>=2.13.0",
```

### Comparing `cvat_sdk_i_digit-0.0.7/src/cvat_sdk_i_digit/config.py` & `cvat_sdk_i_digit-0.0.8/src/cvat_sdk_i_digit/config.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk_i_digit-0.0.7/src/cvat_sdk_i_digit/cvat_api.py` & `cvat_sdk_i_digit-0.0.8/src/cvat_sdk_i_digit/cvat_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,59 +5,68 @@
 from pydantic import BaseModel, computed_field
 from typing import Any
 from cvat_sdk.core.proxies.tasks import Task
 from cvat_sdk.core.proxies.projects import Project
 
 
 class Settings(BaseModel):
-    host: str = "localhost:8080"
+    host: str = "localhost"
+    port: int = 8080
     username: str = ''
     password: str = ''
 
     @computed_field
     @property
     def credentials(self) -> tuple:
         return (self.username, self.password)
 
 
 class Cvat:
     def __init__(self, settings: Settings) -> None:
         self.settings = settings
 
     def get_all_project(self) -> list[Project]:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.projects.list()
 
     def get_all_tasks(self) -> list[Task]:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.tasks.list()
 
     def get_all_task_from_project(self, id_project: int) -> list[Task]:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             tasks = client.projects.retrieve(id_project).get_tasks()
             return tasks
 
     def get_project(self, id_project: int) -> Project:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.projects.retrieve(id_project)
 
     def get_task(self, id_task: int) -> Task:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.tasks.retrieve(id_task)
 
     def create_project(self, project_spec: dict = project_spec) -> Project:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.projects.create(spec=project_spec)
 
     def create_tasks(self, task_spec: dict, resources: Any) -> Task:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             return client.tasks.create_from_data(spec=task_spec, resource_type=ResourceType.LOCAL, resources=resources)
 
     def dowload_dataset(self, task_id: int, path_file_save: Path) -> None:
-        with make_client(host=self.settings.host, credentials=self.settings.credentials) as client:
+        with make_client(host=self.settings.host, port=self.settings.port,
+                         credentials=self.settings.credentials) as client:
             task = client.tasks.retrieve(task_id)
             task.export_dataset(filename=path_file_save, format_name="CVAT for images 1.1", include_images=True)
 
 
 if __name__ == "__main__":
     settings = Settings()
     cvat = Cvat(settings)
```

### Comparing `cvat_sdk_i_digit-0.0.7/PKG-INFO` & `cvat_sdk_i_digit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk_i_digit
-Version: 0.0.7
+Version: 0.0.8
 Author-Email: =?utf-8?b?0KjRg9C80LXQu9C10LIg0JTQvNC40YLRgNC40Lkg0JjQs9C+0YDQtdCy0LjRhw==?= <cmit.dima@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: cvat-sdk>=2.13.0
 Requires-Dist: pydantic-settings>=2.0.2
 Requires-Dist: passlib>=1.7.4
 Requires-Dist: pandas>=2.2.2
 Description-Content-Type: text/markdown
```

