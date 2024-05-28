# Comparing `tmp/levy_stable_jax-0.2.0.tar.gz` & `tmp/levy_stable_jax-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levy_stable_jax-0.2.0.tar", max compression
+gzip compressed data, was "levy_stable_jax-0.2.1.tar", max compression
```

## Comparing `levy_stable_jax-0.2.0.tar` & `levy_stable_jax-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-10-22 07:47:03.747679 levy_stable_jax-0.2.0/LICENSE
--rw-r--r--   0        0        0     1259 2024-05-03 14:16:08.822396 levy_stable_jax-0.2.0/README.md
--rw-r--r--   0        0        0     2994 2024-05-08 15:39:39.030808 levy_stable_jax-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      352 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/__init__.py
--rw-r--r--   0        0        0      708 2024-04-24 12:12:58.006634 levy_stable_jax-0.2.0/src/levy_stable_jax/_cache.py
--rw-r--r--   0        0        0     4270 2024-05-03 11:58:27.607858 levy_stable_jax-0.2.0/src/levy_stable_jax/_generate_data.py
--rw-r--r--   0        0        0      975 2024-05-03 13:51:24.346392 levy_stable_jax-0.2.0/src/levy_stable_jax/_interp.py
--rw-r--r--   0        0        0      559 2024-05-03 13:29:34.962247 levy_stable_jax-0.2.0/src/levy_stable_jax/_typing.py
--rw-r--r--   0        0        0     7703 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/_utils.py
--rw-r--r--   0        0        0    16921 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/distribution.py
--rw-r--r--   0        0        0     4633 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/estimation.py
--rw-r--r--   0        0        0  6464128 2024-05-03 13:29:34.994248 levy_stable_jax-0.2.0/src/levy_stable_jax/logpdf.npy
--rw-r--r--   0        0        0     6195 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/pymc.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 levy_stable_jax-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 07:08:26.556737 levy_stable_jax-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1259 2024-05-06 07:08:26.556737 levy_stable_jax-0.2.1/README.md
+-rw-r--r--   0        0        0     3119 2024-05-28 08:25:14.917881 levy_stable_jax-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-05-28 05:00:01.237655 levy_stable_jax-0.2.1/src/levy_stable_jax/__init__.py
+-rw-r--r--   0        0        0      708 2024-05-06 07:08:26.576737 levy_stable_jax-0.2.1/src/levy_stable_jax/_cache.py
+-rw-r--r--   0        0        0     4421 2024-05-28 08:25:14.917881 levy_stable_jax-0.2.1/src/levy_stable_jax/_generate_data.py
+-rw-r--r--   0        0        0      983 2024-05-28 08:25:14.917881 levy_stable_jax-0.2.1/src/levy_stable_jax/_interp.py
+-rw-r--r--   0        0        0      559 2024-05-06 07:08:26.576737 levy_stable_jax-0.2.1/src/levy_stable_jax/_typing.py
+-rw-r--r--   0        0        0     7757 2024-05-28 08:25:14.917881 levy_stable_jax-0.2.1/src/levy_stable_jax/_utils.py
+-rw-r--r--   0        0        0    17164 2024-05-28 08:25:14.921881 levy_stable_jax-0.2.1/src/levy_stable_jax/distribution.py
+-rw-r--r--   0        0        0     4830 2024-05-28 08:25:14.921881 levy_stable_jax-0.2.1/src/levy_stable_jax/estimation.py
+-rw-r--r--   0        0        0  6464128 2024-05-16 20:42:31.194455 levy_stable_jax-0.2.1/src/levy_stable_jax/logpdf.npy
+-rw-r--r--   0        0        0     6540 2024-05-28 08:25:14.921881 levy_stable_jax-0.2.1/src/levy_stable_jax/pymc.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 levy_stable_jax-0.2.1/PKG-INFO
```

### Comparing `levy_stable_jax-0.2.0/LICENSE` & `levy_stable_jax-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.2.0/README.md` & `levy_stable_jax-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.2.0/pyproject.toml` & `levy_stable_jax-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [project]
 name = "levy-stable-jax"
-version = "0.2.0"
+# RELEASE
+version = "0.2.1"
 authors = [
     {name = "Tim Hunter", email = "tjhunter@cs.stanford.edu"},
 ]
 license = { text = "Apache 2 License" }
 description = "Implementation of the Lévy stable distributions for Jax."
 readme = "README.md"
 requires-python = ">=3.9"
@@ -42,15 +43,15 @@
 Homepage = "https://github.com/tjhunter/levy-stable-jax"
 Documentation = "https://github.com/tjhunter/levy-stable-jax"
 Repository = "https://github.com/tjhunter/levy-stable-jax"
 
 [tool.poetry]
 packages = [{include = "levy_stable_jax", from="src"}]
 name = "levy-stable-jax"
-version = "0.2.0"
+version = "0.2.1" # RELEASE
 authors = ["Tim Hunter <tjhunter@cs.stanford.edu>"]
 description = "Implementation of the Lévy alpha-stable distributions for Jax."
 readme = "README.md"
 license = "Apache 2.0"
 homepage = "https://github.com/tjhunter/levy-stable-jax"
 documentation = "https://levy-stable-jax.readthedocs.io/en/latest/"
 repository = "https://github.com/tjhunter/levy-stable-jax"
@@ -80,15 +81,15 @@
 sphinx-rtd-theme = "^2.0.0"
 mkdocs-material = "^9.5.19"
 mkdocstrings = {extras = ["python"], version = "^0.24.3"}
 pytkdocs = {version = "^0.16.1", extras = ["numpy-style"]}
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
-mypy = "^1.9.0"
+mypy = "1.10.0"
 ruff = "^0.4.1"
 hypothesis = "^6.100.1"
 pytest = "^8.1.1"
 absl-py = "^2.1.0"
 scikit-learn = "^1.4.2"
 # Interactive sessions
 jupyter = "^1.0.0"
@@ -105,14 +106,21 @@
 testpaths = [
     "tests",
 ]
 pythonpath = [
     "src",
 ]
 
+[tool.mypy]
+strict = true
+
+[[tool.mypy.overrides]]
+module = "levy_stable_jax.pymc"
+ignore_errors = true
+
 
 [tool.coverage.run]
 source = ["src"]
 
 [tool.ruff]
 
 line-length = 100
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/_cache.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/_cache.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/_generate_data.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/_generate_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+from numpy.typing import NDArray
+from typing import Any
 from scipy.stats import levy_stable as sp_levy_stable  # type: ignore
 import scipy.interpolate  # type: ignore
 import logging
 import os
 
 from .distribution import (
     TAB_X_CUTOFF,
@@ -19,15 +21,15 @@
 
 _logger = logging.getLogger(__name__)
 
 _THRESH_D2 = 1.0
 _KINK_DELTA = 1e-1
 
 
-def make_data_files():
+def make_data_files() -> None:
     """
     Generates the lookup tables.
 
     This is based on the pylevy's code,
     but it uses instead the scipy implementation
     of the Levy distribution.
     - Some of the values are inaccurate and lead to oscillatory behaviour
@@ -53,26 +55,28 @@
                 )
     ROOT = os.path.dirname(os.path.abspath(__file__))
     path = os.path.join(ROOT, "logpdf.npy")
     _logger.info(f"Saving logpdf to {path}")
     np.save(path, logpdf)
 
 
-def _is_kink(z):
+def _is_kink(z: NDArray[Any]) -> NDArray[Any]:
     before = np.array(z)
     before[:-1] = z[1:]
     after = np.array(z)
     after[1:] = z[:-1]
     epsi = _KINK_DELTA
     return ((z > before + epsi) & (z > after + epsi)) | (
         (z < before - epsi) & (z < after - epsi)
     )
 
 
-def _gen_clean_vals(alpha, beta, xs, dx):
+def _gen_clean_vals(
+    alpha: float, beta: float, xs: NDArray[Any], dx: float
+) -> NDArray[Any]:
     """
     Generates the values for the logpdf using scipy's code, and perform various
     checks.
 
     The code from scipy has a number of bugs which this function corrects.
     - for beta close to 1/-1, the values are incorrect in the tail.
     - for some values close to the mode, one value may be jumping far.
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/_interp.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/_interp.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     points: has shape [n,m] where n is the number of points and m is the len of the
      shape of the grid
     grid: has shape Y
     lower, upper: have shape (m,) where m is the len of the shape of the grid
     """
     grid_shape = jnp.array(jnp.shape(grid))
     points_ = (points - lower) * ((grid_shape - 1) / (upper - lower))
-    res = jsp.ndimage.map_coordinates(grid, points_.T, order=1, mode="nearest")  # type: ignore
+    res: JArray = jsp.ndimage.map_coordinates(grid, points_.T, order=1, mode="nearest")  # type: ignore
     # The +- infinity values trigger NaN in the jax interpolation code.
     res = jnp.where(jnp.isnan(res), -jnp.inf, res)
     return res
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/_typing.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/_typing.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/_utils.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Tuple, Union, Sequence
+from typing import Tuple, Any, Union, Sequence, Generator
 from scipy.stats import levy_stable as sp_levy_stable  # type: ignore
 from contextlib import contextmanager
 from jax import Array as JArray
 import jax.numpy as jnp
 
 from ._typing import Params, Param
 
 
 @contextmanager
-def set_stable(p: Param):
+def set_stable(p: Param) -> Generator[Any, Any, Any]:
     """
     Manages the parametrization of scipy's levy_stable distribution.
 
     Since the parametrization of scipy is at the module level, this function
     provides a way to temporarily change the parametrization of the distribution.
 
     Example:
@@ -65,15 +65,15 @@
 
     Returns:
         (loc, scale) in the requested parametrization.
     """
 
     # For now, we only need to shift the location. The conversion of the scale
     # will only be needed for N2/N3 parametrization.
-    def _phi():
+    def _phi() -> JArray:
         return jnp.tan(jnp.pi * alpha / 2)
 
     if param_from == param_to:
         return (loc, scale)
     # All N0 -> Nx
     if param_from == Params.N0:
         if param_to == Params.N1:
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/distribution.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Univariate stable distribution by John Nolan, 2020.
 
 """
 
 from __future__ import annotations  # for the | syntax.
 
 from math import pi as PI
-from typing import Tuple, List, Sequence
+from typing import Tuple, List, Sequence, no_type_check
 
 import jax
 import jax.numpy as jnp
 from jax import Array as JArray
 import jax.scipy.special as jax_special
 from jax import lax
 import numpy as np
@@ -64,15 +64,15 @@
 
 def _log_tail_gaussian(x: JArray) -> JArray:
     """
     Distribution in the gaussian regime (alpha = 2)
     """
     # When alpha = 2, the Levy-stable distribution is equal to a
     # Gaussian distribution with scale = 2
-    return -0.25 * jnp.square(x) - jnp.log(2 * PI) / 2 - np.log(2.0) / 2
+    return -0.25 * jnp.square(x) - jnp.log(2 * PI) / 2 - np.log(2.0) / 2  # type:ignore
 
 
 INPUT_TYPE = npt.ArrayLike | JArray
 
 
 def pdf(
     x: INPUT_TYPE,
@@ -81,27 +81,26 @@
     loc: INPUT_TYPE = 0.0,
     scale: INPUT_TYPE = 1.0,
     param: Param = Params.N0,
 ) -> JArray | float:
     """
     The probability density function for the Levy-Stable distribution.
 
-    Parameters:
-
-    - x: the values at which to evaluate the PDF
-    - alpha: the alpha parameter of the distribution
-    - beta: the beta parameter of the distribution
-    - loc: the location parameter of the distribution
-        (default 0.0, meaning depends on the parametrization)
-    - scale: the scale parameter of the distribution
-        (default 1.0, meaning depends on the parametrization)
-    - param: the parametrization of the distribution
+    Args:
+        x: the values at which to evaluate the PDF
+        alpha: the alpha parameter of the distribution
+        beta: the beta parameter of the distribution
+        loc: the location parameter of the distribution
+            (default 0.0, meaning depends on the parametrization)
+        scale: the scale parameter of the distribution
+            (default 1.0, meaning depends on the parametrization)
+        param: the parametrization of the distribution
 
     Returns:
-    - the value of the PDF at the given point(s)
+        the value of the PDF at the given point(s)
 
     Examples:
 
     Evaluation of the unit Levy-stable distribution at 0.0, with alpha=1.5, beta=0.0.
     ```py
     >>> pdf(0.0, 1.5, 0.0) # doctest: +ELLIPSIS
     0.28568...
@@ -129,24 +128,23 @@
     loc: INPUT_TYPE = 0.0,
     scale: INPUT_TYPE = 1.0,
     param: Param = Params.N0,
 ) -> JArray | float:
     """
     The probability density function for the Levy-Stable distribution.
 
-    Parameters:
-
-    - x: the values at which to evaluate the PDF
-    - alpha: the alpha parameter of the distribution
-    - beta: the beta parameter of the distribution
-    - loc: the location parameter of the distribution
-        (default 0.0, meaning depends on the parametrization)
-    - scale: the scale parameter of the distribution
-        (default 1.0, meaning depends on the parametrization)
-    - param: the parametrization of the distribution (see Params)
+    Args:
+        x: the values at which to evaluate the PDF
+        alpha: the alpha parameter of the distribution
+        beta: the beta parameter of the distribution
+        loc: the location parameter of the distribution
+            (default 0.0, meaning depends on the parametrization)
+        scale: the scale parameter of the distribution
+            (default 1.0, meaning depends on the parametrization)
+        param: the parametrization of the distribution (see Params)
 
     Examples:
 
     ```py
     >>> logpdf(0.0, 1.5, 0.0, 1.0) # doctest: +ELLIPSIS
     -1.603550...
 
@@ -164,15 +162,15 @@
         res = res.item()
     return res
 
 
 def rvs(
     alpha: INPUT_TYPE,
     beta: INPUT_TYPE,
-    prng: jax.random.PRNGKey,
+    prng: jax.typing.ArrayLike,
     loc: INPUT_TYPE = 0.0,
     scale: INPUT_TYPE = 1.0,
     shape: Shape = (),
     param: Param = Params.N0,
 ) -> JArray:
     """
     Generate random samples from the Levy-Stable distribution.
@@ -197,26 +195,28 @@
     >>> rvs(alpha=1.5, beta=0.0, loc=0.0, scale=1.0, param=Params.N1,
     ...  shape=(10,), prng=prng) # doctest: +ELLIPSIS
     Array([-0.750..., -0.495..., ...], ...)
 
     ```
     """
     # The sampling algorithm is for N1 parametrization.
-    unit_n1 = _sample_unit_n1(alpha, beta, prng, shape)
-    return _values_n1_to_param(alpha, beta, unit_n1, loc, scale, param)
+    unit_n1 = _sample_unit_n1(jnp.asarray(alpha), jnp.asarray(beta), prng, shape)
+    return _values_n1_to_param(alpha, beta, unit_n1, loc, scale, param)  # type:ignore
 
 
+# This function seems to make mypy freeze.
+@no_type_check
 def _values_n1_to_param(
     alpha: INPUT_TYPE,
     beta: INPUT_TYPE,
     values: INPUT_TYPE,
     loc: INPUT_TYPE,
     scale: INPUT_TYPE,
     to_param: Param,
-) -> Tuple[JArray, JArray]:
+) -> JArray:
     """
     Takes values in the unit N1 parametrization and shifts them to the requested parametrization.
 
     Valid for all alpha.
     """
     # TODO: merge with utils.scale?
     if to_param == Params.N0:
@@ -306,15 +306,15 @@
 
 
 def _logpdf_unit(x: JArray, alpha: JArray, beta: JArray) -> JArray:
     """ """
     cutoff_min = -TAB_X_CUTOFF
     cutoff_max = TAB_X_CUTOFF
 
-    def return_interp(x_, alpha_, beta_):
+    def return_interp(x_: JArray, alpha_: JArray, beta_: JArray) -> JArray:
         # For all values in the interior, use interpolation.
         # For everything else, use the tail approximation function.
 
         # tail values and interpolation values are used the following:
         # - tail values are always used for |x| > TAB_X_CUTOFF
         # - for some special cases (beta ~ +- 1, alpha ~ 2) either the
         #    tail or the interpolation values are used.
@@ -361,15 +361,15 @@
                 # Heuristic to  blend tail and interp
                 blend,
                 interp_vals,
             ),
             tail_vals,
         )
 
-    def check_tail(x_, alpha_, beta_) -> JArray:
+    def check_tail(x_: JArray, alpha_: JArray, beta_: JArray) -> JArray:
         # This function should just apply to tail values.
 
         # Flip all x to positive and switch the sign of beta.
         # This uses the symmetry properties of the Levy-stable distribution.
         beta_ = jnp.where(x_ < 0, -beta_, beta_)
         x_ = jnp.maximum(
             jnp.abs(x_), X_TAIL_CUTOFF
@@ -377,15 +377,15 @@
 
         return jnp.where(
             beta_ <= BETA_EXP_CUTOFF,
             _log_tail_exp_pos_n1(_n0_to_n1_unit(x_, alpha_, beta_), alpha_),
             check_tail_inner_pos(x_, alpha_, jnp.maximum(beta_, BETA_EXP_CUTOFF)),
         )
 
-    def check_tail_inner_pos(x_, alpha_, beta_) -> JArray:
+    def check_tail_inner_pos(x_: JArray, alpha_: JArray, beta_: JArray) -> JArray:
         # Builds tail in the standard case, and applies corrections if the tail is close to
         # boundaries.
         # Assumes that x > 1, beta < 1, alpha < 2
 
         zeros = jnp.zeros_like(x_)
         ninfs = jnp.ones_like(x_) * (-np.inf)
 
@@ -453,15 +453,15 @@
 def _canonicalize_input(arrays: List[npt.ArrayLike]) -> Tuple[List[JArray], bool]:
     """
     Given a set of various sorts of inputs, returns a list of 1d arrays that all have the
      same lengths.
     """
     # TODO: use primitives in numpy to achieve the same result
 
-    def _can_elt(t) -> JArray:
+    def _can_elt(t: npt.ArrayLike) -> JArray:
         arr = jnp.asarray(t)
         if arr.ndim == 0:
             arr = arr[jnp.newaxis]
         if arr.ndim > 1:
             raise Exception(
                 f"Input should be scalar or 1d array, one array has dim {arr.ndim}"
             )
@@ -486,15 +486,15 @@
             return jnp.tile(arr, max_len)
         raise AssertionError(f"Size mismatch: {arr.shape} vs {max_len}")
 
     return [_check_size(arr) for arr in arrs], False
 
 
 def _sample_unit_n1(
-    alpha: JArray, beta: JArray, prng: jax.random.PRNGKey, shape: Shape
+    alpha: JArray, beta: JArray, prng: jax.typing.ArrayLike, shape: Shape
 ) -> JArray:
     """
     Sample from the unit Levy-stable distribution in the N1 parametrization.
 
     This implementation only support alpha != 1, it will diverge or return NaNs for alpha == 1.
 
     Algorithm based on Nolan (2020), Theorem 1.3
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/estimation.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/estimation.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Different algorithms to estimate the parameters of a stable distribution.
 
 These algorithms should be all considered as experimental and not part 
 of the standard API: their interface is not likely to change but 
 they may not be as numerically stable.
 """
 
-from typing import Optional
+from typing import Optional, Tuple
 
 import jax.numpy as jnp
 from jax import Array as JArray
 import jaxopt  # type: ignore
 import scipy.stats._levy_stable  # type: ignore
 
-from .distribution import logpdf, Params, Param
+from .distribution import logpdf
 from ._utils import param_convert
+from ._typing import Param, Params
 
 
 def fit_quantiles(samples: JArray, param: Param) -> JArray:
     """
     A rough approximation of the distribution parameters based on quantiles.
 
     For now, it is just wrapping the scipy code.
@@ -50,15 +51,15 @@
 
 def fit_ll(
     samples: JArray,
     param: Param,
     weights: Optional[JArray] = None,
     alpha: Optional[float] = None,
     beta: Optional[float] = None,
-):
+) -> JArray:
     """
     Maximum likelihood evaluation for univariate Lévy-Stable distributions.
 
     Args:
         param: the parametrization of the returned distribution
         samples: a 1-d array with the observed samples.
         weights: optional, the weights on each of the samples.
@@ -76,40 +77,40 @@
 
     The first value is alpha, then beta, then the location parameter and then
      the scale parameter.
     """
     assert samples.ndim == 1, samples
     assert samples.size > 4, samples.size
 
-    def _unpack(theta):
+    def _unpack(theta: JArray) -> Tuple[JArray, JArray, JArray, JArray]:
         idx = 0
         if alpha is None:
             alpha_ = theta[idx]
             idx += 1
         else:
-            alpha_ = alpha
+            alpha_ = jnp.asarray(alpha)
         if beta is None:
             beta_ = theta[idx]
             idx += 1
         else:
-            beta_ = beta
+            beta_ = jnp.asarray(beta)
         loc_ = theta[idx]
         scale_ = theta[idx + 1]
         return (alpha_, beta_, loc_, scale_)
 
-    def _pack(alpha_, beta_, loc_, scale_):
+    def _pack(alpha_: JArray, beta_: JArray, loc_: JArray, scale_: JArray) -> JArray:
         vals = [
             [alpha_] if alpha is None else [],
             [beta_] if beta is None else [],
             [loc_],
             [scale_],
         ]
         return jnp.array([x for val in vals for x in val])
 
-    def _log_likelikhood_n0(theta):
+    def _log_likelikhood_n0(theta: JArray) -> JArray:
         (alpha_, beta_, loc_, scale_) = _unpack(theta)
         logs = logpdf(
             samples, alpha=alpha_, beta=beta_, loc=loc_, scale=scale_, param=Params.N0
         )
         if weights is None:
             res = -jnp.mean(logs)
         else:
@@ -122,15 +123,15 @@
     # Get a crude start
     # TODO: this is not using the weights
     # All the work is done in the N0 parametrization.
     start = fit_quantiles(samples, Params.N0)
     theta_start = _pack(*start)
 
     # Build the bounds for the solver:
-    def _bounds():
+    def _bounds() -> Tuple[JArray, JArray]:
         lower = []
         upper = []
         idx = 0
         if alpha is None:
             lower.append(1.1)
             upper.append(2.0)
             idx += 1
```

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/logpdf.npy` & `levy_stable_jax-0.2.1/src/levy_stable_jax/logpdf.npy`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.2.0/src/levy_stable_jax/pymc.py` & `levy_stable_jax-0.2.1/src/levy_stable_jax/pymc.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 # https://www.pymc.io/projects/examples/en/2022.12.0/howto/custom_distribution.html
 
 
 import jax.numpy as jnp
 import numpy as np
 import jax
 import pytensor.tensor as pt
-from pytensor.graph import Apply, Op
-from pytensor.link.jax.dispatch import jax_funcify
+from pytensor.graph import Apply, Op  # type: ignore
+from pytensor.link.jax.dispatch import jax_funcify  # type: ignore
 import pymc as pm  # type: ignore
 
-from .distribution import logpdf as levy_stable_logpdf
-from .distribution import Params
+from .distribution import logpdf as levy_stable_logpdf, rvs as ls_rvs
+from ._typing import Params
 
 __all__ = ["LevyStableN0"]
 
 
 def LevyStableN0(name, alpha, beta, loc, scale, observed=None):
     """
     A Lévy-stable distribution. The parametrization follows the "0" notation
     from Nolan (2022). It is also known as the "S0" parametrization in scipy.
 
     Args:
-        alpha: the stability parameter. Must be in (1.1, 2].
-        beta: the skewness parameter. Must be in [-1, 1].
-        loc: the location parameter (delta in Nolan's notation).
-        scale: the scale parameter (gamma in Nolan's notation).
+        alpha(tensor): the stability parameter. Must be in (1.1, 2].
+        beta(tensor): the skewness parameter. Must be in [-1, 1].
+        loc(tensor): the location parameter (delta in Nolan's notation).
+        scale(tensor): the scale parameter (gamma in Nolan's notation).
 
     This distribution is explicitly implemented and parametrized for the N0
     parametrization, because the N1 parametrization is not continuous
     for alpha close to 1, and is not recommended in general for numerical work.
     Use the `shift_scale` function if you wish to convert to other parametrizations.
 
     **Practical tips**
@@ -67,23 +67,33 @@
     I have found that tune=6000 really helps further convergence.
 
     Since all the code is implemented in JAX, a JAX-based sampler will be much faster.
     It is recommended to use `pymc.sampling_jax.sample_numpyro_nuts`
 
     TODO: turn into a proper distribution.
 
-    TODO: add a sampler.
-
-
     """
     return pm.CustomDist(
-        name, alpha, beta, loc, scale, logp=_levy_stable_logp_op, observed=observed
+        name,
+        alpha,
+        beta,
+        loc,
+        scale,
+        logp=_levy_stable_logp_op,
+        random=_sample,
+        observed=observed,
     )
 
 
+def _sample(alpha, beta, loc, scale, rng, size):
+    # TODO: unsure if this is a good idea to hardcode the PRNG here.
+    prng = jax.random.PRNGKey(1)
+    return ls_rvs(alpha, beta, prng, loc, scale, size, param=Params.N0)
+
+
 def _logp_sum_n0(x, alpha, beta, loc, scale):
     # TODO: it should already return a scalar, but currently returning a vector
     return jnp.sum(levy_stable_logpdf(x, alpha, beta, loc, scale, Params.N0))
 
 
 _jit_logp_n0 = jax.jit(_logp_sum_n0)
 _jit_logp_n0_grad = jax.jit(jax.grad(_logp_sum_n0, argnums=list(range(5))))
```

### Comparing `levy_stable_jax-0.2.0/PKG-INFO` & `levy_stable_jax-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: levy-stable-jax
-Version: 0.2.0
+Version: 0.2.1
 Summary: Implementation of the Lévy alpha-stable distributions for Jax.
 Home-page: https://github.com/tjhunter/levy-stable-jax
 License: Apache 2.0
 Keywords: levy,stable,jax,probability,statistics
 Author: Tim Hunter
 Author-email: tjhunter@cs.stanford.edu
 Requires-Python: >=3.10,<3.13
```

