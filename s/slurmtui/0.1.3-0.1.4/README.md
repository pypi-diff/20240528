# Comparing `tmp/slurmtui-0.1.3.tar.gz` & `tmp/slurmtui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmtui-0.1.3.tar", last modified: Thu Jan 11 15:09:55 2024, max compression
+gzip compressed data, was "slurmtui-0.1.4.tar", last modified: Tue May 28 18:26:21 2024, max compression
```

## Comparing `slurmtui-0.1.3.tar` & `slurmtui-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:55.979315 slurmtui-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-11 15:09:44.000000 slurmtui-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-11 15:09:55.979315 slurmtui-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-11 15:09:44.000000 slurmtui-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 15:09:55.979315 slurmtui-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-11 15:09:44.000000 slurmtui-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:55.975315 slurmtui-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:55.979315 slurmtui-0.1.3/src/slurmtui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:44.000000 slurmtui-0.1.3/src/slurmtui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:55.979315 slurmtui-0.1.3/src/slurmtui/css/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-11 15:09:44.000000 slurmtui-0.1.3/src/slurmtui/css/slurmtui.css
--rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-01-11 15:09:44.000000 slurmtui-0.1.3/src/slurmtui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-01-11 15:09:44.000000 slurmtui-0.1.3/src/slurmtui/slurm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-11 15:09:44.000000 slurmtui-0.1.3/src/slurmtui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:09:55.979315 slurmtui-0.1.3/src/slurmtui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-11 15:09:55.000000 slurmtui-0.1.3/src/slurmtui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:21.595602 slurmtui-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 18:26:15.000000 slurmtui-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-28 18:26:21.595602 slurmtui-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-28 18:26:15.000000 slurmtui-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:26:21.595602 slurmtui-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-28 18:26:15.000000 slurmtui-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:21.591602 slurmtui-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:21.591602 slurmtui-0.1.4/src/slurmtui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:15.000000 slurmtui-0.1.4/src/slurmtui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:21.591602 slurmtui-0.1.4/src/slurmtui/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 18:26:15.000000 slurmtui-0.1.4/src/slurmtui/css/slurmtui.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-28 18:26:15.000000 slurmtui-0.1.4/src/slurmtui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-28 18:26:15.000000 slurmtui-0.1.4/src/slurmtui/slurm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 18:26:15.000000 slurmtui-0.1.4/src/slurmtui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:26:21.595602 slurmtui-0.1.4/src/slurmtui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 18:26:21.000000 slurmtui-0.1.4/src/slurmtui.egg-info/top_level.txt
```

### Comparing `slurmtui-0.1.3/LICENSE` & `slurmtui-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.3/PKG-INFO` & `slurmtui-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmtui
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Terminal UI (TUI) for Slurm
 Home-page: https://github.com/WissamAntoun/SlurmTUI
 Author: Wissam Antoun
 Author-email: wissam.antoun@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `slurmtui-0.1.3/README.md` & `slurmtui-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.3/setup.py` & `slurmtui-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = f.read()
 
     return long_description
 
 
 setup(
     name="slurmtui",
-    version="0.1.3",
+    version="0.1.4",
     author="Wissam Antoun",
     author_email="wissam.antoun@gmail.com",
     description="A simple Terminal UI (TUI) for Slurm",
     long_description=get_long_description().replace(
         "./img/screenshot.png",
         "https://raw.githubusercontent.com/WissamAntoun/SlurmTUI/main/img/screenshot.png",
     ),
```

### Comparing `slurmtui-0.1.3/src/slurmtui/css/slurmtui.css` & `slurmtui-0.1.4/src/slurmtui/css/slurmtui.css`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.3/src/slurmtui/main.py` & `slurmtui-0.1.4/src/slurmtui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                 str(
                     v["array_job_id"]["number"]
                     if v["array_job_id"]["set"] and v["array_job_id"]["number"] != 0
                     else ""
                 ),
                 str(v["array_task_id"]["number"] if v["array_task_id"]["set"] else ""),
                 str(v["name"])[0:50],
-                str(v["job_resources"].get("nodes", ""))[0:50],
+                str(v["job_resources"].get("nodes", ""))[0:25],
                 str(v["partition"]),
                 str(
                     datetime.datetime.fromtimestamp(
                         v["start_time"] if v["start_time"] else v["submit_time"]
                     )
                 ),
                 time_remaining_string,
@@ -424,36 +424,33 @@
 
     def _delete_job(self, selected_job: Dict[str, Any], delete_array=False) -> None:
         if delete_array:
             self.jobs_to_be_deleted.extend(
                 [
                     job["job_id"]
                     for job in self.running_jobs_dict.values()
-                    if job["array_id"] == selected_job["array_id"]
+                    if job["array_job_id"]["number"] == selected_job["array_job_id"]["number"]
                 ]
             )
         else:
             self.jobs_to_be_deleted.append(selected_job["job_id"])
         if not self.mock:
             if delete_array:
                 os.system(f"scancel --array {selected_job['array_id']}")
             else:
                 os.system(f"scancel {selected_job['job_id']}")
 
     def _check_job_is_array(self, selected_job: Dict[str, Any]) -> bool:
         """Check if the selected job is an array job."""
+
         if selected_job["array_job_id"]["number"] == 0:
             return False
-        elif selected_job["array_job_id"] > 1:
+        elif selected_job["array_job_id"]["number"] > 1:
             return True
 
-        for job in self.running_jobs_dict.values():
-            if job["array_id"] == selected_job["array_id"] and job["array_index"] > 1:
-                return True
-
         return False
 
     def action_delete(self) -> None:
         """Delete the job."""
         if self._check_no_jobs():
             return
```

### Comparing `slurmtui-0.1.3/src/slurmtui/slurm_utils.py` & `slurmtui-0.1.4/src/slurmtui/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.3/src/slurmtui.egg-info/PKG-INFO` & `slurmtui-0.1.4/src/slurmtui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmtui
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Terminal UI (TUI) for Slurm
 Home-page: https://github.com/WissamAntoun/SlurmTUI
 Author: Wissam Antoun
 Author-email: wissam.antoun@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

