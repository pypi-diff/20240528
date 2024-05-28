# Comparing `tmp/torchret-0.1.1.tar.gz` & `tmp/torchret-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchret-0.1.1.tar", last modified: Sun May 26 18:16:03 2024, max compression
+gzip compressed data, was "torchret-0.1.2.tar", last modified: Tue May 28 18:33:47 2024, max compression
```

## Comparing `torchret-0.1.1.tar` & `torchret-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-26 18:16:03.277233 torchret-0.1.1/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-26 18:16:03.277074 torchret-0.1.1/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-26 18:16:03.277303 torchret-0.1.1/setup.cfg
--rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-26 18:14:31.000000 torchret-0.1.1/setup.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-26 18:16:03.275892 torchret-0.1.1/torchret/
--rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.1.1/torchret/__init__.py
--rw-r--r--   0 parth      (501) staff       (20)    11951 2024-05-26 04:16:16.000000 torchret-0.1.1/torchret/model.py
--rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.1.1/torchret/utils.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-26 18:16:03.276839 torchret-0.1.1/torchret.egg-info/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-26 18:16:03.000000 torchret-0.1.1/torchret.egg-info/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-26 18:16:03.000000 torchret-0.1.1/torchret.egg-info/SOURCES.txt
--rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-26 18:16:03.000000 torchret-0.1.1/torchret.egg-info/dependency_links.txt
--rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-26 18:16:03.000000 torchret-0.1.1/torchret.egg-info/requires.txt
--rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-26 18:16:03.000000 torchret-0.1.1/torchret.egg-info/top_level.txt
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-28 18:33:47.593080 torchret-0.1.2/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-28 18:33:47.592877 torchret-0.1.2/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-28 18:33:47.593160 torchret-0.1.2/setup.cfg
+-rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-28 18:33:26.000000 torchret-0.1.2/setup.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-28 18:33:47.591542 torchret-0.1.2/torchret/
+-rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.1.2/torchret/__init__.py
+-rw-r--r--   0 parth      (501) staff       (20)    11959 2024-05-28 18:32:26.000000 torchret-0.1.2/torchret/model.py
+-rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.1.2/torchret/utils.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-28 18:33:47.592587 torchret-0.1.2/torchret.egg-info/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-28 18:33:47.000000 torchret-0.1.2/torchret.egg-info/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-28 18:33:47.000000 torchret-0.1.2/torchret.egg-info/SOURCES.txt
+-rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-28 18:33:47.000000 torchret-0.1.2/torchret.egg-info/dependency_links.txt
+-rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-28 18:33:47.000000 torchret-0.1.2/torchret.egg-info/requires.txt
+-rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-28 18:33:47.000000 torchret-0.1.2/torchret.egg-info/top_level.txt
```

### Comparing `torchret-0.1.1/setup.py` & `torchret-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 
 setup(
     name="torchret",
     description="",
     long_description="",
-    version = '0.1.1',
+    version = '0.1.2',
     long_description_content_type="text/markdown",
     author="Parth Dhameliya",
     url="https://github.com/parthdhameliya7",
     license="Apache License 2.0",
     packages=find_packages(),
     include_package_data=True,
     platforms=["linux", "unix"],
```

### Comparing `torchret-0.1.1/torchret/model.py` & `torchret-0.1.2/torchret/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,19 +141,19 @@
             tracker.set_postfix(epoch = self.current_epoch, loss='%.6f' %float(losses.avg), stage="train", current_lr = self.optimizer.param_groups[0]['lr'], **monitor)
             self.current_train_step += 1
 
         if self.swa_training is True:
             if self.current_epoch + 1 >= self.swa_start:
                 self.swa_model.update_parameters(self)
             else:
-                if self.scheduler is True:
+                if self.scheduler is not None:
                     if self.step_scheduler_after == 'epoch':
                         self.scheduler.step()
         else:
-            if self.scheduler is True:
+            if self.scheduler is not None:
                 if self.step_scheduler_after == 'epoch':
                     self.scheduler.step()
         tracker.close()
         if self.logger is True:
             self.train_one_epoch_logs(losses.avg, monitor)
         return losses.avg, monitor
```

### Comparing `torchret-0.1.1/torchret/utils.py` & `torchret-0.1.2/torchret/utils.py`

 * *Files identical despite different names*

