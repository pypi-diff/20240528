# Comparing `tmp/slurmray-3.6.1.tar.gz` & `tmp/slurmray-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmray-3.6.1.tar", max compression
+gzip compressed data, was "slurmray-3.6.2.tar", max compression
```

## Comparing `slurmray-3.6.1.tar` & `slurmray-3.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-11-03 09:04:55.530868 slurmray-3.6.1/LICENSE
--rw-r--r--   0        0        0     2572 2024-05-24 09:50:27.907919 slurmray-3.6.1/README.md
--rw-r--r--   0        0        0      751 2024-05-24 16:48:26.492424 slurmray-3.6.1/pyproject.toml
--rw-r--r--   0        0        0    23452 2024-05-24 16:47:54.742431 slurmray-3.6.1/slurmray/RayLauncher.py
--rw-r--r--   0        0        0        0 2023-11-03 09:04:55.530868 slurmray-3.6.1/slurmray/__init__.py
--rw-r--r--   0        0        0     2273 2023-11-03 09:04:55.530868 slurmray-3.6.1/slurmray/assets/sbatch_template.sh
--rw-r--r--   0        0        0     1506 2024-05-24 10:21:10.257516 slurmray-3.6.1/slurmray/assets/slurmray_server.sh
--rw-r--r--   0        0        0      461 2024-05-24 16:30:31.132660 slurmray-3.6.1/slurmray/assets/slurmray_server_template.py
--rw-r--r--   0        0        0      597 2023-12-05 14:46:52.657175 slurmray-3.6.1/slurmray/assets/spython_template.py
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 slurmray-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-03 09:04:55.530868 slurmray-3.6.2/LICENSE
+-rw-r--r--   0        0        0     2572 2024-05-24 09:50:27.907919 slurmray-3.6.2/README.md
+-rw-r--r--   0        0        0      734 2024-05-28 17:47:52.599423 slurmray-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0    23483 2024-05-24 16:53:39.542357 slurmray-3.6.2/slurmray/RayLauncher.py
+-rw-r--r--   0        0        0        0 2023-11-03 09:04:55.530868 slurmray-3.6.2/slurmray/__init__.py
+-rw-r--r--   0        0        0     2273 2023-11-03 09:04:55.530868 slurmray-3.6.2/slurmray/assets/sbatch_template.sh
+-rw-r--r--   0        0        0     1506 2024-05-24 10:21:10.257516 slurmray-3.6.2/slurmray/assets/slurmray_server.sh
+-rw-r--r--   0        0        0      461 2024-05-24 16:30:31.132660 slurmray-3.6.2/slurmray/assets/slurmray_server_template.py
+-rw-r--r--   0        0        0      597 2023-12-05 14:46:52.657175 slurmray-3.6.2/slurmray/assets/spython_template.py
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 slurmray-3.6.2/PKG-INFO
```

### Comparing `slurmray-3.6.1/LICENSE` & `slurmray-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmray-3.6.1/README.md` & `slurmray-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `slurmray-3.6.1/pyproject.toml` & `slurmray-3.6.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "slurmray"
-version = "3.6.1"
+version = "3.6.2"
 description = "SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. "
 authors = ["Henri Jamet <henri.jamet@unil.ch>"]
 license = "Apache License"
 homepage = "https://henri-jamet.vercel.app/"
 documentation = "https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dill = "^0.3.7"
 ray = {extras = ["data", "serve", "train", "tune"], version = "^2.7.1"}
 pdoc3 = "^0.10.0"
 paramiko = "^3.3.1"
-torch = "^2.1.1"
 pip-chill = "^1.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.26.0"
 
 [build-system]
```

### Comparing `slurmray-3.6.1/slurmray/RayLauncher.py` & `slurmray-3.6.2/slurmray/RayLauncher.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
                 if time.time() - start_time > 60:
                     start_time = time.time()
                     print("Update time: {}".format(time.strftime("%H:%M:%S")))
 
                 if current_queue is None or current_queue != to_queue:
                     current_queue = to_queue
                     with open(queue_log_file, "w") as f:
-                        text = "Current queue:\n"
+                        text = f"Current queue ({time.strftime('%H:%M:%S')}):\n"
                         format_row = "{:>30}" * (len(current_queue[0]))
                         for user, status, nodes, node_list in current_queue:
                             text += (
                                 format_row.format(user, status, nodes, node_list) + "\n"
                             )
                         text += "\n"
                         f.write(text)
```

### Comparing `slurmray-3.6.1/slurmray/assets/sbatch_template.sh` & `slurmray-3.6.2/slurmray/assets/sbatch_template.sh`

 * *Files identical despite different names*

### Comparing `slurmray-3.6.1/slurmray/assets/slurmray_server.sh` & `slurmray-3.6.2/slurmray/assets/slurmray_server.sh`

 * *Files identical despite different names*

### Comparing `slurmray-3.6.1/slurmray/assets/spython_template.py` & `slurmray-3.6.2/slurmray/assets/spython_template.py`

 * *Files identical despite different names*

### Comparing `slurmray-3.6.1/PKG-INFO` & `slurmray-3.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmray
-Version: 3.6.1
+Version: 3.6.2
 Summary: SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. 
 Home-page: https://henri-jamet.vercel.app/
 License: Apache License
 Author: Henri Jamet
 Author-email: henri.jamet@unil.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: paramiko (>=3.3.1,<4.0.0)
 Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
 Requires-Dist: pip-chill (>=1.0.3,<2.0.0)
 Requires-Dist: ray[data,serve,train,tune] (>=2.7.1,<3.0.0)
-Requires-Dist: torch (>=2.1.1,<3.0.0)
 Project-URL: Documentation, https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/
 Description-Content-Type: text/markdown
 
 # SLURM_RAY
 
 👉[Full documentation](https://www.henri-jamet.com/docs/slurmray/slurm-ray/)
```

