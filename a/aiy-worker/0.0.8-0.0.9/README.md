# Comparing `tmp/aiy_worker-0.0.8.tar.gz` & `tmp/aiy_worker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiy_worker-0.0.8.tar", last modified: Sun May 26 13:00:12 2024, max compression
+gzip compressed data, was "aiy_worker-0.0.9.tar", last modified: Sun May 26 13:12:02 2024, max compression
```

## Comparing `aiy_worker-0.0.8.tar` & `aiy_worker-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:00:12.209813 aiy_worker-0.0.8/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 13:00:12.209341 aiy_worker-0.0.8/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.8/README.md
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:00:12.206174 aiy_worker-0.0.8/aiy_worker/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.8/aiy_worker/__init__.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     2223 2024-05-26 12:59:33.000000 aiy_worker-0.0.8/aiy_worker/types.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.8/aiy_worker/utils.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     6872 2024-05-26 07:26:56.000000 aiy_worker-0.0.8/aiy_worker/worker.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)    10768 2024-05-25 11:19:01.000000 aiy_worker-0.0.8/aiy_worker/ws_client.py
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:00:12.208799 aiy_worker-0.0.8/aiy_worker.egg-info/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 13:00:12.000000 aiy_worker-0.0.8/aiy_worker.egg-info/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-05-26 13:00:12.000000 aiy_worker-0.0.8/aiy_worker.egg-info/SOURCES.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-05-26 13:00:12.000000 aiy_worker-0.0.8/aiy_worker.egg-info/dependency_links.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-05-26 13:00:12.000000 aiy_worker-0.0.8/aiy_worker.egg-info/requires.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-05-26 13:00:12.000000 aiy_worker-0.0.8/aiy_worker.egg-info/top_level.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-05-26 13:00:12.209907 aiy_worker-0.0.8/setup.cfg
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-05-26 12:59:45.000000 aiy_worker-0.0.8/setup.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:12:02.792845 aiy_worker-0.0.9/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 13:12:02.792283 aiy_worker-0.0.9/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.9/README.md
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:12:02.788632 aiy_worker-0.0.9/aiy_worker/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.9/aiy_worker/__init__.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     2223 2024-05-26 12:59:33.000000 aiy_worker-0.0.9/aiy_worker/types.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.9/aiy_worker/utils.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     6874 2024-05-26 13:11:59.000000 aiy_worker-0.0.9/aiy_worker/worker.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)    10768 2024-05-25 11:19:01.000000 aiy_worker-0.0.9/aiy_worker/ws_client.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 13:12:02.791638 aiy_worker-0.0.9/aiy_worker.egg-info/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 13:12:02.000000 aiy_worker-0.0.9/aiy_worker.egg-info/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-05-26 13:12:02.000000 aiy_worker-0.0.9/aiy_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-05-26 13:12:02.000000 aiy_worker-0.0.9/aiy_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-05-26 13:12:02.000000 aiy_worker-0.0.9/aiy_worker.egg-info/requires.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-05-26 13:12:02.000000 aiy_worker-0.0.9/aiy_worker.egg-info/top_level.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-05-26 13:12:02.793027 aiy_worker-0.0.9/setup.cfg
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-05-26 13:11:51.000000 aiy_worker-0.0.9/setup.py
```

### Comparing `aiy_worker-0.0.8/aiy_worker/types.py` & `aiy_worker-0.0.9/aiy_worker/types.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.8/aiy_worker/utils.py` & `aiy_worker-0.0.9/aiy_worker/utils.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.8/aiy_worker/worker.py` & `aiy_worker-0.0.9/aiy_worker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     self.set_progress(task, progress)
                 import threading
                 t = threading.Thread(target=received, args=(task,))
                 t.start()
                 logger.info("Start to generate image")
                 if task.kind == TaskKind.TEXT_TO_IMAGE:
                     images = self.on_task(task, _set_progress)
-                if task.kind == TaskKind.CANNY:
+                elif task.kind == TaskKind.CANNY:
                     images = self.on_canny_task(task, _set_progress)
                 else:
                     raise Exception('Task kind is NONE')
                 # 等待 submit 成功
                 t.join()
                 logger.info(f"Execute task successfully")       
                 with timer('handle image[0]'):
```

### Comparing `aiy_worker-0.0.8/aiy_worker/ws_client.py` & `aiy_worker-0.0.9/aiy_worker/ws_client.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.8/setup.py` & `aiy_worker-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if os.path.exists("requirements.txt"):
     install_requires = [i for i in io.open("requirements.txt").read().split("\n") if i]
 else:
     install_requires = []
 print(install_requires)
 setuptools.setup(
     name="aiy_worker",
-    version="0.0.8",
+    version="0.0.9",
     author="zgljl2012",
     # license = 'MIT License',
     # author_email="pengshiyuyx@gmail.com",
     description="aiy worker",
     long_description=long_description,
     # long_description_content_type="text/x-rst",
     # url="https://github.com/mouday/chinesename",
```

