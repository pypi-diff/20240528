# Comparing `tmp/mate_cxinsys-1.0.2.tar.gz` & `tmp/mate_cxinsys-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mate_cxinsys-1.0.2.tar", last modified: Tue May 28 07:23:03 2024, max compression
+gzip compressed data, was "mate_cxinsys-1.0.3.tar", last modified: Tue May 28 08:26:10 2024, max compression
```

## Comparing `mate_cxinsys-1.0.2.tar` & `mate_cxinsys-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.899990 mate_cxinsys-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 07:23:03.899990 mate_cxinsys-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.895990 mate_cxinsys-1.0.2/mate/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.895990 mate_cxinsys-1.0.2/mate/array/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23087 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/array/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.895990 mate_cxinsys-1.0.2/mate/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/matelightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.895990 mate_cxinsys-1.0.2/mate/transferentropy/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/transferentropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/transferentropy/telightning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/transferentropy/transferentropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.895990 mate_cxinsys-1.0.2/mate/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 07:22:55.000000 mate_cxinsys-1.0.2/mate/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:23:03.899990 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/mate_cxinsys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:23:03.899990 mate_cxinsys-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 07:23:03.000000 mate_cxinsys-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.750234 mate_cxinsys-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 08:26:10.750234 mate_cxinsys-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.746234 mate_cxinsys-1.0.3/mate/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.746234 mate_cxinsys-1.0.3/mate/array/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/array/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.746234 mate_cxinsys-1.0.3/mate/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/matelightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.746234 mate_cxinsys-1.0.3/mate/transferentropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/transferentropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/transferentropy/telightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/transferentropy/transferentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.746234 mate_cxinsys-1.0.3/mate/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 08:25:58.000000 mate_cxinsys-1.0.3/mate/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:26:10.750234 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/mate_cxinsys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:26:10.750234 mate_cxinsys-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 08:26:10.000000 mate_cxinsys-1.0.3/setup.py
```

### Comparing `mate_cxinsys-1.0.2/LICENSE` & `mate_cxinsys-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/PKG-INFO` & `mate_cxinsys-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mate-cxinsys
-Version: 1.0.2
+Version: 1.0.3
 Summary: MATE
 Home-page: https://github.com/cxinsys/mate
 Author: Complex Intelligent Systems Laboratory (CISLAB)
 Author-email: daewon4you@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mate_cxinsys-1.0.2/README.md` & `mate_cxinsys-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/mate/array/module.py` & `mate_cxinsys-1.0.3/mate/array/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -348,65 +348,21 @@
     def concatenate(self, *args, **kwargs):
         return jnp.concatenate(*args, **kwargs)
 
     def stack(self, *args, **kwargs):
         return jnp.stack(*args, **kwargs)
 
     def unique(self, array, return_counts=False, axis=None):
-        if axis is None:
-            return jnp.unique(array, return_counts=return_counts)
-        else:
-            if len(array.shape) != 2:
-                raise ValueError("Input array must be 2D")
-            # s = time.time()
-            sortarr = array[self.lexsort(array.T[::-1])]
-            # print(time.time() - s)
-            mask = jnp.empty(array.shape[0], dtype=bool)
-            # mask[0] = True
-            mask = mask.at[0].set(True)
-            # mask[1:] = jnp.any(sortarr[1:] != sortarr[:-1], axis=1)
-            mask = mask.at[1:].set(jnp.any(sortarr[1:] != sortarr[:-1], axis=1))
-
-            ret = sortarr[mask]
-            if not return_counts:
-                return ret
-
-            ret = ret,
-            if return_counts:
-                nonzero = jnp.nonzero(mask)[0]
-                idx = jnp.empty((nonzero.size + 1,), nonzero.dtype)
-                # idx[:-1] = nonzero
-                idx = idx.at[:-1].set(nonzero)
-                # idx[-1] = mask.size
-                idx = idx.at[-1].set(mask.size)
-                ret += idx[1:] - idx[:-1],
-                # print(time.time() - s)
-
-
-            return ret
-        # return jnp.unique(*args, **kwargs)
+        return jnp.unique(*args, **kwargs)
 
     def zeros(self, *args, **kwargs):
         return jnp.zeros(*args, **kwargs)
 
-    # def lexsort(self, *args, **kwargs):
-    #     return jnp.lexsort(*args, **kwargs)
-
-    def lexsort(self, keys, axis=-1):
-        if len(keys.shape) < 2:
-            raise ValueError(f"keys must be at least 2 dimensional, but {len(keys.shape)=}.")
-        if len(keys) == 0:
-            raise ValueError(f"Must have at least 1 key, but {len(keys)=}.")
-
-        idx = jnp.argsort(keys[0])
-        for k in keys[1:]:
-            # idx = idx.index_select(dim, k.index_select(dim, idx).argsort(dim=dim, stable=True))
-            idx = jnp.take(idx, jnp.argsort(jnp.take(k, idx, axis=axis), axis=axis), axis=axis)
-
-        return idx
+    def lexsort(self, *args, **kwargs):
+        return jnp.lexsort(*args, **kwargs)
 
     def arange(self, *args, **kwargs):
         return device_put(jnp.arange(*args, **kwargs), jax.devices()[self.device_id])
 
     def multiply(self, *args, **kwargs):
         return jnp.multiply(*args, **kwargs)
```

### Comparing `mate_cxinsys-1.0.2/mate/dataset/dataset.py` & `mate_cxinsys-1.0.3/mate/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/mate/mate.py` & `mate_cxinsys-1.0.3/mate/mate.py`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/mate/matelightning.py` & `mate_cxinsys-1.0.3/mate/matelightning.py`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/mate/transferentropy/telightning.py` & `mate_cxinsys-1.0.3/mate/transferentropy/telightning.py`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/mate/transferentropy/transferentropy.py` & `mate_cxinsys-1.0.3/mate/transferentropy/transferentropy.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 
         self._shm_name = shm_name
         self._result_matrix = result_matrix
         self._sem = sem
 
         self._dt = dt
 
-        self.fpath_log = osp.join('./', 'elapsed_time_per_task.csv')
-
-        if not osp.exists(self.fpath_log):
-            with open(self.fpath_log, 'w') as f:
-                f.write("Task, " \
-                        "Elapsed time \n")
+        # self.fpath_log = osp.join('./', 'elapsed_time_per_task.csv')
+        #
+        # if not osp.exists(self.fpath_log):
+        #     with open(self.fpath_log, 'w') as f:
+        #         f.write("Task, " \
+        #                 "Elapsed time \n")
 
     @property
     def am(self):
         return self._am
 
     def solve(self,
               batch_size=None,
@@ -157,18 +157,18 @@
                                   axis=3)
 
 
             t_vals = self.am.transpose(vals, axes=(2, 0, 1, 3))
 
             pair_vals = self.am.concatenate((tile_inds_pair[:, None], self.am.reshape(t_vals, (-1, 3))), axis=1)
 
-            stime_imaginary = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Preprocess, " \
-                        f"{stime_imaginary - stime_preproc} \n")
+            # stime_imaginary = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Preprocess, " \
+            #             f"{stime_imaginary - stime_preproc} \n")
 
             # 허수 제거
             n_bins = self.am.array(n_bins, dtype=n_bins.dtype)
             n_bins = self.am.take(n_bins, t_pairs, axis=0)
             n_bins = self.am.repeat(n_bins, (len_time - 1))
             n_bins = self.am.tile(n_bins, bin_arrs.shape[-1])
 
@@ -184,18 +184,18 @@
             )
 
             left_inds = self.am.where(left_bools)[0]
 
             pair_vals = self.am.take(pair_vals, left_inds, axis=0)
             # 허수 제거
 
-            stime_unique = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Remove imaginary, " \
-                        f"{stime_unique - stime_imaginary} \n")
+            # stime_unique = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Remove imaginary, " \
+            #             f"{stime_unique - stime_imaginary} \n")
 
             uvals_xt1_xt_yt, cnts_xt1_xt_yt = self.am.unique(pair_vals, return_counts=True, axis=0)
 
             uvals_xt1_xt, cnts_xt1_xt = self.am.unique(pair_vals[:, :-1], return_counts=True, axis=0)
             uvals_xt_yt, cnts_xt_yt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2, 3]), axis=1),
                                                      return_counts=True, axis=0)
             uvals_xt, cnts_xt = self.am.unique(self.am.take(pair_vals, self.am.array([0, 2]), axis=1), return_counts=True,
@@ -205,75 +205,75 @@
             subuvals_xt_yt, n_subuvals_xt_yt = self.am.unique(self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2, 3]), axis=1), return_counts=True, axis=0)
             subuvals_xt, n_subuvals_xt = self.am.unique(self.am.take(uvals_xt1_xt_yt, self.am.array([0, 2]), axis=1), return_counts=True, axis=0)
 
             # s_time = time.time()
             # tmp_cnts_xt1_xt = self.am.concatenate([self.am.broadcast_to(cnt, self.am.take(n_subuvals_xt1_xt, i).item()) for i, cnt in enumerate(cnts_xt1_xt)])
             # print(time.time() - s_time)
 
-            stime_repeat1 = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Uniques, " \
-                        f"{stime_repeat1 - stime_unique} \n")
+            # stime_repeat1 = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Uniques, " \
+            #             f"{stime_repeat1 - stime_unique} \n")
             cnts_xt1_xt = self.am.repeat(cnts_xt1_xt, n_subuvals_xt1_xt)
 
-            stime_repeat2 = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Repeat1, " \
-                        f"{stime_repeat2 - stime_repeat1} \n")
+            # stime_repeat2 = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Repeat1, " \
+            #             f"{stime_repeat2 - stime_repeat1} \n")
             cnts_xt_yt = self.am.repeat(cnts_xt_yt, n_subuvals_xt_yt)
 
-            stime_sort1 = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Repeat2, " \
-                        f"{stime_sort1 - stime_repeat2} \n")
+            # stime_sort1 = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Repeat2, " \
+            #             f"{stime_sort1 - stime_repeat2} \n")
             ind_xt_yt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([3, 2, 0]), axis=1).T)
             ind2ori_xt_yt = self.am.argsort(ind_xt_yt)
             cnts_xt_yt = self.am.take(cnts_xt_yt, ind2ori_xt_yt)
 
-            stime_repeat3 = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Sort1, " \
-                        f"{stime_repeat3 - stime_sort1} \n")
+            # stime_repeat3 = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Sort1, " \
+            #             f"{stime_repeat3 - stime_sort1} \n")
             cnts_xt = self.am.repeat(cnts_xt, n_subuvals_xt)
 
-            stime_sort2 = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Repeat3, " \
-                        f"{stime_sort2 - stime_repeat3} \n")
+            # stime_sort2 = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Repeat3, " \
+            #             f"{stime_sort2 - stime_repeat3} \n")
             ind_xt = self.am.lexsort(self.am.take(uvals_xt1_xt_yt, self.am.array([2, 0]), axis=1).T)
             ind2ori_xt = self.am.argsort(ind_xt)
             cnts_xt = self.am.take(cnts_xt, ind2ori_xt)
 
-            stime_te = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Sort2, " \
-                        f"{stime_te - stime_sort2} \n")
+            # stime_te = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Sort2, " \
+            #             f"{stime_te - stime_sort2} \n")
             # TE
             p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1) * bin_arrs.shape[-1])
             # p_xt1_xt_yt = self.am.divide(cnts_xt1_xt_yt, (len_time - 1))
 
             numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
             denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
             fraction = self.am.divide(numer, denom)
             log_val = self.am.log2(fraction)
             entropies = self.am.multiply(p_xt1_xt_yt, log_val)
 
-            stime_bincount = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("TE, " \
-                        f"{stime_bincount - stime_te} \n")
+            # stime_bincount = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("TE, " \
+            #             f"{stime_bincount - stime_te} \n")
             uvals_tot, n_subuvals_tot = self.am.unique(uvals_xt1_xt_yt[:, 0], return_counts=True)
             final_bins = self.am.repeat(uvals_tot, n_subuvals_tot)
             final_bins = self.am.astype(x=final_bins, dtype='int32')
             entropy_final = self.am.bincount(final_bins, weights=entropies)
 
-            etime = time.time()
-            with open(self.fpath_log, 'a') as f:
-                f.write("Bincount, " \
-                        f"{etime - stime_bincount} \n")
+            # etime = time.time()
+            # with open(self.fpath_log, 'a') as f:
+            #     f.write("Bincount, " \
+            #             f"{etime - stime_bincount} \n")
 
             # # LocalTE
             # numer = self.am.multiply(cnts_xt1_xt_yt, cnts_xt)
             # denom = self.am.multiply(cnts_xt1_xt, cnts_xt_yt)
             # fraction = self.am.divide(numer, denom)
             # log_val = self.am.log2(fraction)
             #
```

### Comparing `mate_cxinsys-1.0.2/mate_cxinsys.egg-info/PKG-INFO` & `mate_cxinsys-1.0.3/mate_cxinsys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mate-cxinsys
-Version: 1.0.2
+Version: 1.0.3
 Summary: MATE
 Home-page: https://github.com/cxinsys/mate
 Author: Complex Intelligent Systems Laboratory (CISLAB)
 Author-email: daewon4you@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mate_cxinsys-1.0.2/mate_cxinsys.egg-info/SOURCES.txt` & `mate_cxinsys-1.0.3/mate_cxinsys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mate_cxinsys-1.0.2/setup.py` & `mate_cxinsys-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='mate-cxinsys',
-      version='1.0.2',
+      version='1.0.3',
       description='MATE',
       url='https://github.com/cxinsys/mate',
       author='Complex Intelligent Systems Laboratory (CISLAB)',
       author_email='daewon4you@gmail.com',
       license='BSD-3-Clause',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
```

