# Comparing `tmp/dataset_iterator-0.4.5.tar.gz` & `tmp/dataset_iterator-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.5.tar", last modified: Wed May 22 20:42:17 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.6.tar", last modified: Tue May 28 09:01:23 2024, max compression
```

## Comparing `dataset_iterator-0.4.5.tar` & `dataset_iterator-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.423889 dataset_iterator-0.4.5/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.423889 dataset_iterator-0.4.5/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22252 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/keras_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    57911 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/ordered_enqueuer_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:42:17.000000 dataset_iterator-0.4.5/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:42:17.427888 dataset_iterator-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-22 20:42:14.000000 dataset_iterator-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:01:23.759174 dataset_iterator-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-28 09:01:23.755174 dataset_iterator-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:01:23.755174 dataset_iterator-0.4.6/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:01:23.755174 dataset_iterator-0.4.6/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22252 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/keras_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57911 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:01:23.755174 dataset_iterator-0.4.6/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-28 09:01:23.000000 dataset_iterator-0.4.6/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 09:01:23.000000 dataset_iterator-0.4.6/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:01:23.000000 dataset_iterator-0.4.6/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 09:01:23.000000 dataset_iterator-0.4.6/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:01:23.000000 dataset_iterator-0.4.6/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:01:23.759174 dataset_iterator-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-28 09:01:20.000000 dataset_iterator-0.4.6/setup.py
```

### Comparing `dataset_iterator-0.4.5/LICENSE.txt` & `dataset_iterator-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/PKG-INFO` & `dataset_iterator-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.5
+Version: 0.4.6
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.6/dataset_iterator-0.4.6.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.5/README.md` & `dataset_iterator-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/__init__.py` & `dataset_iterator-0.4.6/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.6/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.6/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.6/dataset_iterator/hard_sample_mining.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,30 @@
             self.iterator.enable_random_transforms(self.data_aug_param)
         self.iterator.close()
 
     def need_compute(self, epoch):
         return epoch + 1 + self.start_epoch >= self.start_from_epoch and (self.period == 1 or (epoch + 1 + self.start_epoch - self.start_from_epoch) % self.period == 0)
 
     def on_epoch_begin(self, epoch, logs=None):
-        if self.proba_per_metric is not None or self.need_compute(epoch):
+        if self.n_metrics > 1 or self.need_compute(epoch):
             self.wait_for_me.clear()  # will lock
 
     def on_epoch_end(self, epoch, logs=None):
         if self.need_compute(epoch):
             self.target_iterator.close()
             self.iterator.open()
             metrics = self.compute_metrics()
             self.iterator.close()
             self.target_iterator.open()
             first = self.proba_per_metric is None
             self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
             self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
             if first and self.n_metrics > self.period:
                 warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
-        if self.proba_per_metric is not None:
+        if self.proba_per_metric is not None and not self.wait_for_me.is_set():
             if len(self.proba_per_metric.shape) == 2:
                 self.metric_idx = (self.metric_idx + 1) % self.n_metrics
                 proba = self.proba_per_metric[self.metric_idx]
             else:
                 proba = self.proba_per_metric
             self.target_iterator.set_index_probability(proba)
             self.wait_for_me.set()  # release lock
@@ -131,17 +131,18 @@
     return proba
 
 def get_index_probability(metrics, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, verbose:int=1):
     if len(metrics.shape) == 1:
         return get_index_probability_1d(metrics, enrich_factor=enrich_factor, quantile_max=quantile_max, quantile_min=quantile_min, verbose=verbose)
     probas_per_metric = [get_index_probability_1d(metrics[:, i], enrich_factor=enrich_factor, quantile_max=quantile_max, quantile_min=quantile_min, verbose=verbose) for i in range(metrics.shape[1])]
     probas_per_metric = np.stack(probas_per_metric, axis=0)
-    #proba = np.max(probas_per_metric, axis=0)
-    #proba /= np.sum(proba)
-    return probas_per_metric
+    #return probas_per_metric
+    proba = np.mean(probas_per_metric, axis=0)
+    return proba / np.sum(proba)
+
 
 def compute_metrics(iterator, predict_function, metrics_function, disable_augmentation:bool=True, disable_channel_postprocessing:bool=False, workers:int=None, verbose:int=1):
     iterator.open()
     data_aug_param = iterator.disable_random_transforms(disable_augmentation, disable_channel_postprocessing)
     simple_iterator = SimpleIterator(iterator)
     batch_size = iterator.get_batch_size()
     n_batches = len(simple_iterator)
```

### Comparing `dataset_iterator-0.4.5/dataset_iterator/helpers.py` & `dataset_iterator-0.4.6/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.6/dataset_iterator/image_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.6/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/keras_callbacks.py` & `dataset_iterator-0.4.6/dataset_iterator/keras_callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,51 +13,65 @@
                  **kwargs):
         super().__init__(filepath, **kwargs)
         self.n_retry = n_retry
         self.sleep_time = sleep_time
         self._alternative_path = False
 
     def _save_model(self, epoch, batch, logs):
-        for i in range(self.n_retry):
-            if i>1:
-                print(f"save_model: start of for loop: {i + 1}/{self.n_retry}")
-            try:
-                path = self._get_file_path(epoch, batch, logs)
-                tmp_path = self._tmp_path(path)
-                #print(f"save_model: try {i + 1}/{self.n_retry}, path: {path} temp path: {tmp_path}", flush=True)
-                if os.path.exists(path): # move file before saving
-                    os.rename(path, tmp_path)
-                    #print(f"moved: {path} to {tmp_path}", flush=True)
-                if i == self.n_retry - 1:
-                    self._alternative_path = True
-                super()._save_model(epoch, batch, logs)
-                #print(f"saved epoch: {epoch}", flush=True)
+        if isinstance(self.save_freq, int) or self.epochs_since_last_save >= self.period:
+            for i in range(self.n_retry):
                 if i>1:
-                    print(f"model saved after retrying: {i+1}/{self.n_retry}", flush=True)
-            except BlockingIOError as error:
-                print(f"Error saving weights: {error}. Retry: {i+1}/{self.n_retry}", flush=True)
-                time.sleep(self.sleep_time)  # wait for X seconds before trying to save again
-                print(f"slept: {self.sleep_time}s")
-                os.remove(self._get_file_path(epoch, batch, logs))
-                print(f"file {self._get_file_path(epoch, batch, logs)} removed")
-                self._alternative_path = False
-            else:
-                self._alternative_path = False
-                if os.path.exists(tmp_path):
-                    os.remove(tmp_path)
-                return
-            print(f"save_model: end of for loop: {i+1}/{self.n_retry}")
+                    print(f"save_model: start of for loop: {i + 1}/{self.n_retry}")
+                try:
+                    self._alternative_path = False
+                    path = self._get_file_path(epoch, batch, logs)
+                    tmp_path = self._tmp_path(path)
+                    self._alternative_path = True
+                    super()._save_model(epoch, batch, logs) # save to tmp path
+                    self._alternative_path = False
+                    #print(f"save_model: try {i + 1}/{self.n_retry}, path: {path} temp path: {tmp_path}", flush=True)
+                    if os.path.exists(tmp_path):  # move tmp file to new file
+                        if os.path.exists(path):
+                            os.remove(path)
+                        os.rename(tmp_path, path)
+                        #print(f"moved: {path} to {tmp_path}", flush=True)
+                    if i == self.n_retry - 1:
+                        self._alternative_path = True
+                    super()._save_model(epoch, batch, logs)
+                    #print(f"saved epoch: {epoch}", flush=True)
+                except BlockingIOError as error:
+                    print(f"Error saving weights: {error}. Retry: {i+1}/{self.n_retry}", flush=True)
+                    time.sleep(self.sleep_time)  # wait for X seconds before trying to save again
+                    print(f"slept: {self.sleep_time}s")
+                    os.remove(self._get_file_path(epoch, batch, logs))
+                    print(f"file {self._get_file_path(epoch, batch, logs)} removed")
+                    self._alternative_path = False
+                else:
+                    self._alternative_path = False
+                    tmp = os.path.exists(tmp_path)
+                    main = os.path.exists(path)
+                    if main and tmp:
+                        os.remove(tmp_path)
+                        return
+                    elif main:
+                        return
+                    elif tmp and not main and i == self.n_retry-1:
+                        os.rename(tmp_path, path)
+                        print(f"model could not be saved at {self._get_file_path(epoch, batch, logs)} after {self.n_retry} retry, restoring temp file", flush=True)
+                        return
+                    time.sleep(self.sleep_time)
+                print(f"save_model: end of for loop: {i+1}/{self.n_retry}", flush=True)
 
         # 21:45:07.667:   File "h5py/h5f.pyx", line 126, in h5py.h5f.create
         # 21:45:07.667: BlockingIOError: [Errno 11] Unable to create file (unable to lock file, errno = 11, error message = 'Resource temporarily unavailable')
 
     def _get_file_path(self, epoch, batch, logs):
         path = super()._get_file_path(epoch, batch, logs)
         if self._alternative_path:
-            path = self._tmp_path(path)
+            return self._tmp_path(path)
         return path
 
     def _tmp_path(self, path):
         split = os.path.splitext(path)
         return split[0] + "_tmp" + split[1]
```

### Comparing `dataset_iterator-0.4.5/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.6/dataset_iterator/multichannel_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/ordered_enqueuer_cf.py` & `dataset_iterator-0.4.6/dataset_iterator/ordered_enqueuer_cf.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.6/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/shared_memory.py` & `dataset_iterator-0.4.6/dataset_iterator/shared_memory.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.6/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.6/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator/utils.py` & `dataset_iterator-0.4.6/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.6/dataset_iterator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.5
+Version: 0.4.6
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.6/dataset_iterator-0.4.6.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.5/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.6/dataset_iterator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.5/setup.py` & `dataset_iterator-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.5",
+    version="0.4.6",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.5/dataset_iterator-0.4.5.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.6/dataset_iterator-0.4.6.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

