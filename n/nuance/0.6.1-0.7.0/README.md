# Comparing `tmp/nuance-0.6.1.tar.gz` & `tmp/nuance-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuance-0.6.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nuance-0.6.1.tar` & `nuance-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,58 @@
--rw-r--r--   0        0        0     1097 2024-05-20 23:14:43.037973 nuance-0.6.1/LICENSE
--rw-r--r--   0        0        0     1492 2024-05-20 23:14:43.037973 nuance-0.6.1/README.md
--rw-r--r--   0        0        0      254 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/__init__.py
--rw-r--r--   0        0        0     9245 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/combined.py
--rw-r--r--   0        0        0     1815 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/core.py
--rw-r--r--   0        0        0     1811 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/kernels.py
--rw-r--r--   0        0        0    17920 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/nuance.py
--rw-r--r--   0        0        0     4988 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/search_data.py
--rw-r--r--   0        0        0     7156 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/star.py
--rw-r--r--   0        0        0     6403 2024-05-20 23:14:43.057973 nuance-0.6.1/nuance/utils.py
--rw-r--r--   0        0        0      814 2024-05-20 23:14:43.061973 nuance-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 nuance-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nuance-0.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 nuance-0.7.0/.zenodo.json
+-rw-r--r--   0        0        0   275647 2020-02-02 00:00:00.000000 nuance-0.7.0/poetry.lock
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 nuance-0.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 nuance-0.7.0/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/examples.md
+-rw-r--r--   0        0        0   443507 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/illustrations.afdesign
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0    80334 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/nuance.afdesign
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/readme_quick.ipynb
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/box.png
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0    49748 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/illu.png
+-rw-r--r--   0        0        0    52919 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/illu_readme.png
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/logo.png
+-rw-r--r--   0        0        0    26544 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/nuance.svg
+-rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/star.png
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/style.css
+-rw-r--r--   0        0        0    22236 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_static/wire.png
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_templates/class.rst
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/_templates/navbar-logo.html
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/markdown/API.md
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/markdown/hardware.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/markdown/how.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/markdown/install.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/markdown/tutorials.md
+-rw-r--r--   0        0        0   151726 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/combined.ipynb
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/gp.ipynb
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/lc_prep.ipynb
+-rw-r--r--   0        0        0   415496 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/motivation.ipynb
+-rw-r--r--   0        0        0   191292 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/multi.ipynb
+-rw-r--r--   0        0        0    99429 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/periodic.ipynb
+-rw-r--r--   0        0        0   230454 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/single.ipynb
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/star.ipynb
+-rw-r--r--   0        0        0    72592 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/templates.ipynb
+-rw-r--r--   0        0        0   143699 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/tutorials/GP_optimization.ipynb
+-rw-r--r--   0        0        0   450889 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/tutorials/exocomet.ipynb
+-rw-r--r--   0        0        0   183985 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/tutorials/ground_based.ipynb
+-rw-r--r--   0        0        0   206986 2020-02-02 00:00:00.000000 nuance-0.7.0/docs/notebooks/tutorials/tess_search.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/__init__.py
+-rw-r--r--   0        0        0     9245 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/combined.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/core.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/kernels.py
+-rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/nuance.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/search_data.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/star.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 nuance-0.7.0/nuance/utils.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nuance-0.7.0/tests/test_devices.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nuance-0.7.0/tests/test_full.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nuance-0.7.0/tests/test_units.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 nuance-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nuance-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 nuance-0.7.0/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 nuance-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nuance-0.7.0/PKG-INFO
```

### Comparing `nuance-0.6.1/LICENSE` & `nuance-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuance-0.6.1/README.md` & `nuance-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # nuance
-Efficient detection of planets transiting active stars
+Efficient detection of planets transiting quiet or active stars
 
 <p align="center">
     <img src="docs/_static/illu_readme.png" height="350" style="margin:50px">
 </p>
 
 *nuance* uses linear models and Gaussian processes (using the [JAX](https://github.com/google/jax)-based [tinygp](https://github.com/dfm/tinygp)) to simultaneously **search for planetary transits while modeling correlated noises** (e.g. stellar variability) in a tractable way. See [the paper](https://arxiv.org/abs/2402.06835) for more details.
 
 When to use *nuance*?
 - To detect single or periodic transits
 - When correlated noises are present in the data (e.g. stellar variability or instrumental systematics)
 - For space-based or sparse ground-based observations
 - To effectively find transits in light curves from multiple instruments
+- To use GPUs for fast transit searches
 
 Documentation at [nuance.readthedocs.io](https://nuance.readthedocs.io)
 
 ## Example
 
 ```python
 from nuance import Nuance, utils
```

### Comparing `nuance-0.6.1/nuance/combined.py` & `nuance-0.7.0/nuance/combined.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.1/nuance/core.py` & `nuance-0.7.0/nuance/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import partial
 
 import jax
 import jax.numpy as jnp
+import jaxopt
 
 
-def eval_model(flux, X, gp):
+def solve(flux, X, gp):
     Liy = gp.solver.solve_triangular(flux)
     LiX = gp.solver.solve_triangular(X.T)
 
     @jax.jit
     def function(m):
         Xm = jnp.vstack([X, m])
         Lim = gp.solver.solve_triangular(m)
@@ -18,14 +19,44 @@
         w = jnp.linalg.lstsq(LimX2, LiXmT @ Liy)[0]
         v = jnp.linalg.inv(LimX2)
         return gp.log_probability(flux - w @ Xm), w, v
 
     return function
 
 
+def gp_model(x, y, build_gp, X=None):
+
+    if X is None:
+        X = jnp.atleast_2d(jnp.ones_like(x))
+
+    @jax.jit
+    def nll_w(params):
+        gp = build_gp(params, x)
+        Liy = gp.solver.solve_triangular(y)
+        LiX = gp.solver.solve_triangular(X.T)
+        LiXT = LiX.T
+        LiX2 = LiXT @ LiX
+        w = jnp.linalg.lstsq(LiX2, LiXT @ Liy)[0]
+        nll = -gp.log_probability(y - w @ X)
+        return nll, w
+
+    @jax.jit
+    def nll(params):
+        return nll_w(params)[0]
+
+    @jax.jit
+    def mu(params):
+        gp = build_gp(params, x)
+        _, w = nll_w(params)
+        cond_gp = gp.condition(y - w @ X, x).gp
+        return cond_gp.loc + w @ X
+
+    return mu, nll
+
+
 def transit_protopapas(t, t0, D, P=1e15, c=12):
     _t = P * jnp.sin(jnp.pi * (t - t0) / P) / (jnp.pi * D)
     return -0.5 * jnp.tanh(c * (_t + 1 / 2)) + 0.5 * jnp.tanh(c * (_t - 1 / 2))
 
 
 def transit_box(time, t0, D, P=1e15):
     return -((jnp.abs(time - t0) % P) < D / 2).astype(float)
```

### Comparing `nuance-0.6.1/nuance/kernels.py` & `nuance-0.7.0/nuance/kernels.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.1/nuance/nuance.py` & `nuance-0.7.0/nuance/nuance.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             kernel = kernels.quasisep.Exp(1e12)
 
             self.gp = GaussianProcess(
                 kernel, self.time, diag=self.error**2, mean=self.mean
             )
 
         if self.compute:
-            self.eval_model = jax.jit(core.eval_model(self.flux, self.X, self.gp))
+            self._solve = jax.jit(core.solve(self.flux, self.X, self.gp))
 
         self.search_data = None
 
     def __repr__(self):
         noise = (
             f"kernel={self.gp.kernel}"
             if self.error is None
@@ -107,28 +107,28 @@
     def searched(self):
         """Whether the linear search has been performed."""
         return self.search_data is not None
 
     @property
     def time_span(self):
         """Time span"""
-        return np.max(self.time) - np.min(self.time)
+        return np.ptp(self.time)
 
     @property
     def ll0(self) -> float:
         """Log-likelihood of data without model.
 
         Returns
         -------
         float
         """
-        return self.eval_model(np.zeros_like(self.time))[0].__array__()
+        return self._solve(np.zeros_like(self.time))[0].__array__()
 
     def _models(self, m):
-        _, w, _ = self.eval_model(m)
+        _, w, _ = self._solve(m)
         mean = w[0:-1] @ self.X
         signal = m * w[-1]
 
         @jax.jit
         def gp_mean():
             return self.gp.condition(self.flux - mean - signal).gp.mean
 
@@ -152,58 +152,18 @@
         tuple
             A tuple containing three functions:
 
             - :code:`optimize`: a function that optimizes the GP model.
             - :code:`mu`: a function that returns the mean of the GP model (jax.jit-compiled).
             - :code:`nll`: a function that returns the negative log-likelihood of the GP model (jax.jit-compiled).
         """
-        if mask is None:
-            mask = np.ones_like(self.time).astype(bool)
-
-        masked_x = self.time[mask]
-        masked_y = self.flux[mask]
-        masked_X = self.X[:, mask]
-
-        @jax.jit
-        def nll_w(params):
-            gp = build_gp(params, masked_x)
-            Liy = gp.solver.solve_triangular(masked_y)
-            LiX = gp.solver.solve_triangular(masked_X.T)
-            LiXT = LiX.T
-            LiX2 = LiXT @ LiX
-            w = jnp.linalg.lstsq(LiX2, LiXT @ Liy)[0]
-            nll = -gp.log_probability(masked_y - w @ masked_X)
-            return nll, w
-
-        @jax.jit
-        def nll(params):
-            return nll_w(params)[0]
-
-        @jax.jit
-        def mu(params):
-            gp = build_gp(params, masked_x)
-            _, w = nll_w(params)
-            cond_gp = gp.condition(masked_y - w @ masked_X, self.time).gp
-            return cond_gp.loc + w @ self.X
-
-        def optimize(init_params, param_names=None):
-            def inner(theta, *args, **kwargs):
-                params = dict(init_params, **theta)
-                return nll(params, *args, **kwargs)
-
-            param_names = (
-                list(init_params.keys()) if param_names is None else param_names
-            )
-            start = {k: init_params[k] for k in param_names}
-
-            solver = jaxopt.ScipyMinimize(fun=inner)
-            soln = solver.run(start)
-            print(soln.state)
-
-            return dict(init_params, **soln.params)
+        mu, nll = core.gp_model(
+            self.time[mask], self.flux[mask], build_gp, X=self.X[:, None]
+        )
+        optimize = partial(utils.minimize, nll)
 
         return optimize, mu, nll
 
     def mu(self, time=None):
         """
         Computes the mean model of the GP.
 
@@ -218,15 +178,15 @@
         """
         if time is None:
             time = self.time
 
         @jax.jit
         def _mu():
             gp = self.gp
-            _, w, _ = self.eval_model(np.zeros_like(time))
+            _, w, _ = self._solve(np.zeros_like(time))
             w = w[0:-1]
             cond_gp = gp.condition(self.flux - w @ self.X, time).gp
             return cond_gp.loc + w @ self.X
 
         return _mu()
 
     def models(self, t0: float = None, D: float = None, P: float = 1e15):
@@ -283,15 +243,15 @@
 
         Returns
         -------
         list
             (w, v): linear coefficients and their covariance matrix
         """
         m = self.model(self.time, t0, D, P)
-        _, w, v = self.eval_model(m)
+        _, w, v = self._solve(m)
         return w, v
 
     def depth(self, t0: float, D: float, P: float = None):
         """Depth linearly solved for epoch `t0` and duration `D` (and period `P` for a periodic model).
 
         Parameters
         ----------
@@ -362,49 +322,50 @@
         None
         """
         assert backend in [None, "cpu", "gpu"], "backend must be 'cpu' or 'gpu'"
 
         if backend is None:
             backend = jax.default_backend()
 
+        if batch_size is None:
+            batch_size = {"cpu": DEVICES_COUNT, "gpu": 1000}[backend]
+
+        @jax.jit
+        def solve(t0, D):
+            m = self.model(self.time, t0, D)
+            ll, w, v = self._solve(m)
+            return jnp.array([w[-1], v[-1, -1], ll])
+
         if backend == "cpu":
-            eval_t0_Ds_function = core.pmap_cpus
-            if batch_size is None:
-                batch_size = DEVICES_COUNT
-
-        elif backend == "gpu":
-            eval_t0_Ds_function = core.vmap_gpu
-            if batch_size is None:
-                batch_size = 1000
-
-        eval_t0s_Ds = eval_t0_Ds_function(self.eval_model, self.model, self.time)
-
-        batches_n = int(np.ceil(len(t0s) / batch_size))
-        padded_t0s = np.pad(t0s, pad_width=[0, batches_n * batch_size - len(t0s)])
-        batched_t0s = np.array(np.array_split(padded_t0s, batches_n))
-
-        ll = np.zeros((len(padded_t0s), len(Ds)))
-        depths = ll.copy()
-        vars = ll.copy()
-        depths = ll.copy()
-
-        _progress = lambda x: (tqdm(x) if progress else x)
-
-        for i, t0 in enumerate(_progress(batched_t0s)):
-            _depths, _vars, _ll = eval_t0s_Ds(t0, Ds)
-            depths[i * batch_size : (i + 1) * batch_size, :] = _depths.T
-            vars[i * batch_size : (i + 1) * batch_size, :] = _vars.T
-            ll[i * batch_size : (i + 1) * batch_size, :] = _ll.T
-
-        depths = np.array(depths[0 : len(t0s), :])
-        vars = np.array(vars[0 : len(t0s), :])
-        ll = np.array(ll[0 : len(t0s), :])
+            solve_batch = jax.pmap(
+                jax.vmap(solve, in_axes=(None, 0)), in_axes=(0, None)
+            )
+        else:
+            solve_batch = jax.vmap(
+                jax.vmap(solve, in_axes=(None, 0)), in_axes=(0, None)
+            )
+
+        t0s_padded = np.pad(t0s, [0, batch_size - (len(t0s) % batch_size) % batch_size])
+        t0s_batches = np.reshape(
+            t0s_padded, (len(t0s_padded) // batch_size, batch_size)
+        )
+
+        _progress = lambda x: (tqdm(x, unit_scale=batch_size) if progress else x)
+
+        results = []
+
+        for t0_batch in _progress(t0s_batches):
+            results.append(solve_batch(t0_batch, Ds))
+
+        depths, vars, ll = np.transpose(results, axes=[3, 0, 1, 2]).reshape(
+            (3, len(t0s_padded), len(Ds))
+        )[:, 0 : len(t0s), :]
 
         if positive:
-            ll0 = self.eval_model(np.zeros_like(self.time))[0]
+            ll0 = self._solve(np.zeros_like(self.time))[0]
             ll[depths < 0] = ll0
 
         vars[~np.isfinite(vars)] = 1e25
 
         self.search_data = SearchData(
             t0s=t0s, Ds=Ds, ll=ll, z=depths, vz=vars, ll0=self.ll0
         )
@@ -542,34 +503,30 @@
             The loaded object.
         """
         return cls(**pickle.load(open(filename, "rb")))
 
     def mask_flares(self, build_gp=None, init=None, window=20, sigma=5, iterations=3):
         # for now
         assert build_gp is not None and init is not None
-        mask = np.ones_like(self.time).astype(bool)
 
-        if build_gp is not None:
-            optimize, mu, nll = self.gp_optimization(build_gp)
-            opt = init.copy()
+        flare_mask = np.ones_like(self.time).astype(bool)
+        mu, nll = utils.minimize(self.time, self.flux, build_gp, X=self.X)
 
         for _ in range(iterations):
-            residuals = self.flux - mu(opt)
-            mask[residuals > sigma * np.std(residuals[mask])] = False
-            mask = np.roll(minimum_filter1d(mask, window), shift=window // 3)
-
-            if build_gp is not None:
-                optimize, mu, _ = self.gp_optimization(build_gp, mask)
-                opt = optimize(init)
+            residuals = self.flux - mu(gp_params)
+            flare_mask = flare_mask & utils.sigma_clip_mask(
+                residuals, sigma=sigma, window=window
+            )
+            gp_params = utils.minimize(nll, gp_params)
 
         new_nu = Nuance(
-            time=self.time[mask],
-            flux=self.flux[mask],
-            X=self.X[:, mask],
-            gp=build_gp(opt, self.time[mask]),
+            time=self.time[flare_mask],
+            flux=self.flux[flare_mask],
+            X=self.X[:, flare_mask],
+            gp=build_gp(gp_params, self.time[flare_mask]),
             compute=True,
         )
 
         return new_nu
 
 
 def _search(p):
```

### Comparing `nuance-0.6.1/nuance/search_data.py` & `nuance-0.7.0/nuance/search_data.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.1/nuance/star.py` & `nuance-0.7.0/nuance/star.py`

 * *Files identical despite different names*

### Comparing `nuance-0.6.1/nuance/utils.py` & `nuance-0.7.0/nuance/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import jax
-import matplotlib.pyplot as plt
+import jaxopt
 import numpy as np
 import tinygp
+from scipy.ndimage import minimum_filter1d
 
 from nuance import core
 from nuance.core import transit_protopapas
 
 
 def interp_split_times(time, p, dphi=0.01):
     tmax, tmin = np.max(time), np.min(time)
@@ -102,14 +103,16 @@
     Parameters
     ----------
     nu : _type_
         _description_
     search : _type_
         _description_
     """
+    import matplotlib.pyplot as plt
+
     t0, D, P = search.best
 
     plt.subplot(2, 2, (1, 3))
     plt.plot(search.periods, search.Q_snr)
     plt.title(f"{P:.5f} days")
 
     mean, astro, noise = nu.models(t0, D, P)
@@ -226,7 +229,65 @@
         "transits": transits,
         "variabilities": variabilities,
         "systematics": systematics,
         "transit_params": true,
     }
 
     return observations, signals
+
+
+def minimize(fun, init_params, param_names=None):
+    """Minimize a function using jaxopt.ScipyMinimize
+
+    Parameters
+    ----------
+    fun : callable
+        the function to minimize of the form fun(params: dict) -> float
+    init_params : dict
+        initial parameters
+    param_names : list, optional
+        list of parameters to optimize, all others being fixed,
+        by default None
+
+    Returns
+    -------
+    dict
+        optimized parameters
+    """
+
+    def inner(theta, *args, **kwargs):
+        params = dict(init_params, **theta)
+        return fun(params, *args, **kwargs)
+
+    param_names = list(init_params.keys()) if param_names is None else param_names
+    start = {k: init_params[k] for k in param_names}
+
+    solver = jaxopt.ScipyMinimize(fun=inner)
+    soln = solver.run(start)
+
+    return dict(init_params, **soln.params)
+
+
+def sigma_clip_mask(residuals, sigma=5, window=20):
+    """Returns a masked of the sigma clipped data. The mask is set
+        to false on the +/-{windows} data points around the sigma
+        clipped residuals, i.e. code:`residuals > sigma * std(residuals)`.
+
+    Parameters
+    ----------
+    residuals : array
+        Data to sigma clip.
+    sigma : int, optional
+        Sigma clipping standard deviation, by default 5.
+    window : int, optional
+        The window of points around which mask is set to False if
+        a data point is sigma clipped, by default 20
+
+    Returns
+    -------
+    array
+        boolean mask of sigma clipped values (i.e :code:`<std(residuals)`).
+    """
+    mask = np.ones_like(residuals, dtype=bool)
+    mask[residuals > sigma * np.std(residuals)] = False
+    mask = np.roll(minimum_filter1d(mask, window), shift=window // 3)
+    return mask
```

