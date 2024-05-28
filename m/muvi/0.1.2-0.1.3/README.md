# Comparing `tmp/muvi-0.1.2.tar.gz` & `tmp/muvi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muvi-0.1.2.tar", max compression
+gzip compressed data, was "muvi-0.1.3.tar", max compression
```

## Comparing `muvi-0.1.2.tar` & `muvi-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1515 2023-01-23 16:36:17.349155 muvi-0.1.2/LICENSE
--rw-r--r--   0        0        0     4733 2023-10-24 14:53:35.030001 muvi-0.1.2/README.md
--rwxr-xr-x   0        0        0      582 2024-05-26 20:36:44.623539 muvi-0.1.2/muvi/__init__.py
--rwxr-xr-x   0        0        0      424 2024-05-26 20:36:44.626371 muvi-0.1.2/muvi/core/__init__.py
--rwxr-xr-x   0        0        0     9150 2024-05-26 20:36:44.628594 muvi-0.1.2/muvi/core/callbacks.py
--rwxr-xr-x   0        0        0     1817 2024-05-26 20:36:44.630678 muvi-0.1.2/muvi/core/early_stopping.py
--rwxr-xr-x   0        0        0      394 2024-05-09 18:16:27.710380 muvi-0.1.2/muvi/core/gpu.py
--rwxr-xr-x   0        0        0     3941 2024-05-26 20:36:44.632935 muvi-0.1.2/muvi/core/index.py
--rwxr-xr-x   0        0        0    71140 2024-05-26 20:36:44.634969 muvi-0.1.2/muvi/core/models.py
--rwxr-xr-x   0        0        0    21949 2024-05-26 20:36:44.638061 muvi-0.1.2/muvi/core/synthetic.py
--rwxr-xr-x   0        0        0      285 2024-05-09 18:15:08.122336 muvi-0.1.2/muvi/log.conf
--rwxr-xr-x   0        0        0      108 2024-05-09 18:17:03.362634 muvi-0.1.2/muvi/tools/__init__.py
--rwxr-xr-x   0        0        0     3719 2024-05-26 20:36:44.642634 muvi-0.1.2/muvi/tools/cache.py
--rw-r--r--   0        0        0     4358 2024-05-09 18:17:21.029149 muvi-0.1.2/muvi/tools/external.py
--rwxr-xr-x   0        0        0    22083 2024-05-26 20:36:44.645212 muvi-0.1.2/muvi/tools/feature_sets.py
--rwxr-xr-x   0        0        0    34430 2024-05-26 20:36:44.647589 muvi-0.1.2/muvi/tools/plotting.py
--rw-r--r--   0        0        0    30931 2024-05-26 20:36:44.648921 muvi-0.1.2/muvi/tools/utils.py
--rwxr-xr-x   0        0        0     2789 2024-05-26 20:36:44.656677 muvi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 muvi-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1515 2023-01-23 16:36:17.349155 muvi-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4733 2023-10-24 14:53:35.030001 muvi-0.1.3/README.md
+-rwxr-xr-x   0        0        0      582 2024-05-26 20:36:44.623539 muvi-0.1.3/muvi/__init__.py
+-rwxr-xr-x   0        0        0      424 2024-05-26 20:36:44.626371 muvi-0.1.3/muvi/core/__init__.py
+-rwxr-xr-x   0        0        0     9150 2024-05-26 20:36:44.628594 muvi-0.1.3/muvi/core/callbacks.py
+-rwxr-xr-x   0        0        0     1817 2024-05-26 20:36:44.630678 muvi-0.1.3/muvi/core/early_stopping.py
+-rwxr-xr-x   0        0        0      394 2024-05-09 18:16:27.710380 muvi-0.1.3/muvi/core/gpu.py
+-rwxr-xr-x   0        0        0     3941 2024-05-26 20:36:44.632935 muvi-0.1.3/muvi/core/index.py
+-rwxr-xr-x   0        0        0    71416 2024-05-28 10:03:40.444017 muvi-0.1.3/muvi/core/models.py
+-rwxr-xr-x   0        0        0    21949 2024-05-26 20:36:44.638061 muvi-0.1.3/muvi/core/synthetic.py
+-rwxr-xr-x   0        0        0      285 2024-05-09 18:15:08.122336 muvi-0.1.3/muvi/log.conf
+-rwxr-xr-x   0        0        0      108 2024-05-09 18:17:03.362634 muvi-0.1.3/muvi/tools/__init__.py
+-rwxr-xr-x   0        0        0     3719 2024-05-26 20:36:44.642634 muvi-0.1.3/muvi/tools/cache.py
+-rw-r--r--   0        0        0     4358 2024-05-09 18:17:21.029149 muvi-0.1.3/muvi/tools/external.py
+-rwxr-xr-x   0        0        0    22083 2024-05-26 20:36:44.645212 muvi-0.1.3/muvi/tools/feature_sets.py
+-rwxr-xr-x   0        0        0    34430 2024-05-26 20:36:44.647589 muvi-0.1.3/muvi/tools/plotting.py
+-rw-r--r--   0        0        0    30931 2024-05-26 20:36:44.648921 muvi-0.1.3/muvi/tools/utils.py
+-rwxr-xr-x   0        0        0     2806 2024-05-28 10:05:33.750520 muvi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 muvi-0.1.3/PKG-INFO
```

### Comparing `muvi-0.1.2/LICENSE` & `muvi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/README.md` & `muvi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/__init__.py` & `muvi-0.1.3/muvi/__init__.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/core/callbacks.py` & `muvi-0.1.3/muvi/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/core/early_stopping.py` & `muvi-0.1.3/muvi/core/early_stopping.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/core/index.py` & `muvi-0.1.3/muvi/core/index.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/core/models.py` & `muvi-0.1.3/muvi/core/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,20 @@
             logger.warning("Making index unique.")
             idx = _make_index_unique(idx)
         return idx
 
     def _normalize_observations(self):
         logger.info("Normalizing observations.")
         for vn, obs in self.observations.items():
+            if self.likelihoods[vn] == "bernoulli":
+                logger.info(
+                    f"Skipping normalization for view `{vn}` with a Bernoulli"
+                    " likelihood."
+                )
+                continue
             if self.nmf[vn]:
                 logger.info(f"Setting min value of view `{vn}` to 0.")
                 obs -= np.nanmin(obs, axis=0)
             else:
                 logger.info(f"Centering features of view `{vn}`.")
                 obs -= np.nanmean(obs, axis=0)
             global_std = np.nanstd(obs)
@@ -662,15 +668,17 @@
         self.n_dense_factors = n_dense_factors
         return prior_masks, prior_scales
 
     def _setup_likelihoods(self, likelihoods):
         if likelihoods is None:
             likelihoods = ["normal" for _ in range(self.n_views)]
         if isinstance(likelihoods, list):
-            likelihoods = {self.view_names[m]: ll for m, ll in enumerate(likelihoods)}
+            likelihoods = {
+                self.view_names[m]: ll.lower() for m, ll in enumerate(likelihoods)
+            }
         likelihoods = {vn: likelihoods.get(vn, "normal") for vn in self.view_names}
         logger.info(f"Likelihoods set to `{likelihoods}`.")
         return likelihoods
 
     def _setup_nmf(self, nmf):
         if nmf is None:
             nmf = [False for _ in range(self.n_views)]
```

### Comparing `muvi-0.1.2/muvi/core/synthetic.py` & `muvi-0.1.3/muvi/core/synthetic.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/tools/cache.py` & `muvi-0.1.3/muvi/tools/cache.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/tools/external.py` & `muvi-0.1.3/muvi/tools/external.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/tools/feature_sets.py` & `muvi-0.1.3/muvi/tools/feature_sets.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/tools/plotting.py` & `muvi-0.1.3/muvi/tools/plotting.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/muvi/tools/utils.py` & `muvi-0.1.3/muvi/tools/utils.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.2/pyproject.toml` & `muvi-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muvi"
-version = "0.1.2"
+version = "0.1.3"
 description = "MuVI: A multi-view latent variable model with domain-informed structured sparsity for integrating noisy feature sets."
 readme = "README.md"
 authors = ["Arber Qoku <arber.qoku@dkfz-heidelberg.com>"]
 homepage = "https://github.com/MLO-lab/MuVI"
 repository = "https://github.com/MLO-lab/MuVI"
 keywords = ["multi-view", "multi-omics", "feature sets", "latent variable model", "structured sparsity", "variational inference", "single-cell"]
 
@@ -34,14 +34,15 @@
 leidenalg = "^0.10.2"
 tensordict = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "2.20.0"
 jupyter = "^1.0.0"
 ipython = "^8.10.0"
+twine = "^5.1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-cov = "^4.0"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.1.0"
```

### Comparing `muvi-0.1.2/PKG-INFO` & `muvi-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muvi
-Version: 0.1.2
+Version: 0.1.3
 Summary: MuVI: A multi-view latent variable model with domain-informed structured sparsity for integrating noisy feature sets.
 Home-page: https://github.com/MLO-lab/MuVI
 Keywords: multi-view,multi-omics,feature sets,latent variable model,structured sparsity,variational inference,single-cell
 Author: Arber Qoku
 Author-email: arber.qoku@dkfz-heidelberg.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
```

