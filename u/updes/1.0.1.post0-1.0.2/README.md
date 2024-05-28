# Comparing `tmp/updes-1.0.1.post0.tar.gz` & `tmp/updes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "updes-1.0.1.post0.tar", last modified: Thu Apr 18 13:16:46 2024, max compression
+gzip compressed data, was "updes-1.0.2.tar", last modified: Tue May 28 08:36:43 2024, max compression
```

## Comparing `updes-1.0.1.post0.tar` & `updes-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:16:46.979137 updes-1.0.1.post0/
--rw-r--r--   0 ddrous     (501) staff       (20)    18092 2024-04-15 09:28:58.000000 updes-1.0.1.post0/LICENSE
--rw-r--r--   0 ddrous     (501) staff       (20)     3701 2024-04-18 13:16:46.978913 updes-1.0.1.post0/PKG-INFO
--rw-r--r--   0 ddrous     (501) staff       (20)     3753 2024-04-18 12:57:50.000000 updes-1.0.1.post0/README.md
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:16:46.976516 updes-1.0.1.post0/docs/
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:16:46.977688 updes-1.0.1.post0/docs/assets/
--rw-r--r--   0 ddrous     (501) staff       (20)     3089 2024-04-18 13:04:46.000000 updes-1.0.1.post0/docs/assets/README_PyPI.md
--rw-r--r--   0 ddrous     (501) staff       (20)      651 2024-04-18 13:14:55.000000 updes-1.0.1.post0/pyproject.toml
--rw-r--r--   0 ddrous     (501) staff       (20)       38 2024-04-18 13:16:46.979186 updes-1.0.1.post0/setup.cfg
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:16:46.978536 updes-1.0.1.post0/updes.egg-info/
--rw-r--r--   0 ddrous     (501) staff       (20)     3701 2024-04-18 13:16:46.000000 updes-1.0.1.post0/updes.egg-info/PKG-INFO
--rw-r--r--   0 ddrous     (501) staff       (20)      203 2024-04-18 13:16:46.000000 updes-1.0.1.post0/updes.egg-info/SOURCES.txt
--rw-r--r--   0 ddrous     (501) staff       (20)        1 2024-04-18 13:16:46.000000 updes-1.0.1.post0/updes.egg-info/dependency_links.txt
--rw-r--r--   0 ddrous     (501) staff       (20)       94 2024-04-18 13:16:46.000000 updes-1.0.1.post0/updes.egg-info/requires.txt
--rw-r--r--   0 ddrous     (501) staff       (20)        6 2024-04-18 13:16:46.000000 updes-1.0.1.post0/updes.egg-info/top_level.txt
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-05-28 08:36:43.783002 updes-1.0.2/
+-rw-r--r--   0 ddrous     (501) staff       (20)    18092 2024-04-15 09:28:58.000000 updes-1.0.2/LICENSE
+-rw-r--r--   0 ddrous     (501) staff       (20)     3726 2024-05-28 08:36:43.782775 updes-1.0.2/PKG-INFO
+-rw-r--r--   0 ddrous     (501) staff       (20)     4410 2024-05-28 08:27:24.000000 updes-1.0.2/README.md
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-05-28 08:36:43.780408 updes-1.0.2/docs/
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-05-28 08:36:43.781575 updes-1.0.2/docs/assets/
+-rw-r--r--   0 ddrous     (501) staff       (20)     3098 2024-05-28 08:27:24.000000 updes-1.0.2/docs/assets/README_PyPI.md
+-rw-r--r--   0 ddrous     (501) staff       (20)      660 2024-05-28 08:34:08.000000 updes-1.0.2/pyproject.toml
+-rw-r--r--   0 ddrous     (501) staff       (20)       38 2024-05-28 08:36:43.783044 updes-1.0.2/setup.cfg
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-05-28 08:36:43.782371 updes-1.0.2/updes.egg-info/
+-rw-r--r--   0 ddrous     (501) staff       (20)     3726 2024-05-28 08:36:43.000000 updes-1.0.2/updes.egg-info/PKG-INFO
+-rw-r--r--   0 ddrous     (501) staff       (20)      203 2024-05-28 08:36:43.000000 updes-1.0.2/updes.egg-info/SOURCES.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)        1 2024-05-28 08:36:43.000000 updes-1.0.2/updes.egg-info/dependency_links.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)      101 2024-05-28 08:36:43.000000 updes-1.0.2/updes.egg-info/requires.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)        6 2024-05-28 08:36:43.000000 updes-1.0.2/updes.egg-info/top_level.txt
```

### Comparing `updes-1.0.1.post0/LICENSE` & `updes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `updes-1.0.1.post0/PKG-INFO` & `updes-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: updes
-Version: 1.0.1.post0
+Version: 1.0.2
 Summary: Universal Partial Differential Equations Simulator
 Author-email: Roussel Desmond Nzoyem <desmond.ngueguin@gmail.com>
 Keywords: differentiable-programming,radial-basis-function,meshfree,optimisation,differentiable-physics,PDEs
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.3.4
+Requires-Dist: lineax
 Requires-Dist: gmsh
 Requires-Dist: pytest
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: seaborn
 Provides-Extra: dev
 Requires-Dist: pyvista[trame]; extra == "dev"
@@ -31,15 +32,15 @@
 - Support for Dirichlet, Neumann, Robin, and Periodic boundary conditions
 - Automatic generation of normals from 2D GMSH meshes
 
 𝕌pdes in incredibly extendable, with additional features added frequently.
 
 
 ## Getting started
-The package is available on PyPi. You can install it with
+The package is available on PyPI. You can install it with
 ```
 pip install updes
 ```
 
 The example below illustrates how to solve the Laplace equation with Dirichlet and Neumann boundary conditions:
 ```python
 import updes
@@ -74,15 +75,15 @@
 cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution")
 ```
 
 𝕌pdes can handle much complicated cases with little to no modifications to the code above. Check out further notebooks and scripts in the [documentation](https://ddrous.github.io/Updes/) and the folder [`demos`](./demos)!
 
 
 ## Dependencies
-- **Core**: JAX - GMSH - Matplotlib - Seaborn - Scikit-Learn
+- **Core**: JAX - GMSH - Lineax - Matplotlib - Seaborn - Scikit-Learn
 - **Optional**: PyVista - FFMPEG - QuartoDoc
 
 See the `pyproject.toml` file the specific versions of the dependencies.
 
 
 ## Cite us !
 If you use this software, please cite us with the following BibTeX entry:
```

### Comparing `updes-1.0.1.post0/README.md` & `updes-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # 𝕌pdes
 
 𝕌pdes is a general-purpose library for mesh-free PDE simulation and control. There is no faster way to explore the realm of PDEs !
 
 <table>
   <tr>
     <th><img src="docs/assets/laplace.png" width="180"></th>
-    <th><img src="docs/assets/advection_diffusion.gif" width="350"></th>
-    <th><img src="docs/assets/burgers_u.gif" width="188"></th>
+    <th><img src="docs/assets/adv_diff_periodic.gif" width="350"></th>
+    <!-- <th><img src="docs/assets/burgers_u.gif" width="188"></th> -->
+    <th><img src="docs/assets/ns_norm.gif" width="150"></th>
   </tr>
 </table>
 
 
 ## Features
 𝕌pdes leverages Radial Basis Functions (RBFs) and JAX to provide the following features:
 - User-centric design: no need to re-implement a solver for each new PDE
 - Lightning fast mesh-free simulation via Radial Basis Functions
 - Robust differentiable simulation via JAX, and portable across CPU, GPU, and TPU
 - Support for Dirichlet, Neumann, Robin, and Periodic boundary conditions
 - Automatic generation of normals from 2D GMSH meshes
 
-𝕌pdes in incredibly extendable, with additional features added frequently.
+𝕌pdes is easily extendable, with additional features added frequently.
 
 
 ## Getting started
-The package is available on PyPi. You can install it with
+The package is available on PyPI. You can install it with
 ```
 pip install updes
 ```
 
 The example below illustrates how to solve the Laplace equation with Dirichlet and Neumann boundary conditions:
+<p align="center">
+<img src="docs/assets/LaplacePDE.png" width="250">
+</p>
+
 ```python
 import updes
 import jax.numpy as jnp
 
 # Create a mesh-free cloud of points on a unit square
 facet_types={"South":"n", "West":"d", "North":"d", "East":"d"}
 cloud = updes.SquareCloud(Nx=30, Ny=20, facet_types=facet_types)
@@ -58,36 +63,37 @@
                     rbf=updes.polyharmonic,
                     max_degree=1)
 
 # Visualize the solution
 cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution")
 ```
 
-𝕌pdes can handle much complicated cases with little to no modifications to the code above. Check out further notebooks and scripts in the documentation and the folder [`demos`](./demos)!
+𝕌pdes can handle much complicated cases with little modifications to the code above. Check out the [documentation](https://ddrous.github.io/Updes/) and Python interactive notebooks in the [`demos`](./demos) folder !
 
 
 
 
 ## To-Dos
-- Logo, contributors guide, and developer documentation
-- Better introductory examples and user documentation for outreach:
-    - Integration with Neural Networks and Equinox
+1. Logo, contributors guide, and developer documentation
+2. Improved ill-conditioned linear systems for RBF-FD (i.e. `support_size != "max"`)
+2. More introductory examples in the documentation :
+    - Integration with neural networks and [Equinox](https://github.com/patrick-kidger/equinox)
     - Non-linear and multi-dimensional PDEs
     - Adjoint schemes for fluid flows
-- Better point generation with accurate geometry and normals: 
+3. Better point generation with accurate geometry and normals: 
     - USD format
-    - Gmsh tutorial
-- Add support for 3D radial basis functions
+    - GMSH tutorial
+4. Support for 3D radial basis functions
 
 We welcome contributions from the community. Please feel free to open an issue or a pull request.
 
 
 ## Dependencies
-- **Core**: JAX - GMSH - Matplotlib - Seaborn - Scikit-Learn
-- **Optional**: PyVista - FFMPEG - QuartoDoc
+- **Core**: [JAX](https://github.com/google/jax) - [GMSH](https://pypi.org/project/gmsh/) - [Lineax](https://github.com/patrick-kidger/lineax) - [Matplotlib](https://github.com/matplotlib/matplotlib) - [Seaborn](https://github.com/mwaskom/seaborn) - [Scikit-Learn](https://github.com/scikit-learn/scikit-learn)
+- **Optional**: [PyVista](https://github.com/pyvista/pyvista) - [FFMPEG](https://github.com/kkroening/ffmpeg-python) - [QuartoDoc](https://github.com/machow/quartodoc/)
 
 See the `pyproject.toml` file the specific versions of the dependencies.
 
 
 ## Cite us !
 If you use this software, please cite us with the following BibTeX entry:
 ```
```

### Comparing `updes-1.0.1.post0/docs/assets/README_PyPI.md` & `updes-1.0.2/docs/assets/README_PyPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - Support for Dirichlet, Neumann, Robin, and Periodic boundary conditions
 - Automatic generation of normals from 2D GMSH meshes
 
 𝕌pdes in incredibly extendable, with additional features added frequently.
 
 
 ## Getting started
-The package is available on PyPi. You can install it with
+The package is available on PyPI. You can install it with
 ```
 pip install updes
 ```
 
 The example below illustrates how to solve the Laplace equation with Dirichlet and Neumann boundary conditions:
 ```python
 import updes
@@ -56,15 +56,15 @@
 cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution")
 ```
 
 𝕌pdes can handle much complicated cases with little to no modifications to the code above. Check out further notebooks and scripts in the [documentation](https://ddrous.github.io/Updes/) and the folder [`demos`](./demos)!
 
 
 ## Dependencies
-- **Core**: JAX - GMSH - Matplotlib - Seaborn - Scikit-Learn
+- **Core**: JAX - GMSH - Lineax - Matplotlib - Seaborn - Scikit-Learn
 - **Optional**: PyVista - FFMPEG - QuartoDoc
 
 See the `pyproject.toml` file the specific versions of the dependencies.
 
 
 ## Cite us !
 If you use this software, please cite us with the following BibTeX entry:
```

### Comparing `updes-1.0.1.post0/pyproject.toml` & `updes-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "updes"
 description = "Universal Partial Differential Equations Simulator"
-version = "1.0.1.post"
+version = "1.0.2"
 readme = "docs/assets/README_PyPI.md"
 authors = [
     { name = "Roussel Desmond Nzoyem", email = "desmond.ngueguin@gmail.com" }
 ]
 keywords = [
     "differentiable-programming",
     "radial-basis-function",
@@ -13,14 +13,15 @@
     "optimisation",
     "differentiable-physics",
     "PDEs",
 ]
 
 dependencies = [
     "jax >= 0.3.4",
+    "lineax",
     "gmsh",
     "pytest",
     "matplotlib>=3.4.0",
     "scikit-learn",
     "seaborn",
 ]
```

### Comparing `updes-1.0.1.post0/updes.egg-info/PKG-INFO` & `updes-1.0.2/updes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: updes
-Version: 1.0.1.post0
+Version: 1.0.2
 Summary: Universal Partial Differential Equations Simulator
 Author-email: Roussel Desmond Nzoyem <desmond.ngueguin@gmail.com>
 Keywords: differentiable-programming,radial-basis-function,meshfree,optimisation,differentiable-physics,PDEs
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.3.4
+Requires-Dist: lineax
 Requires-Dist: gmsh
 Requires-Dist: pytest
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: scikit-learn
 Requires-Dist: seaborn
 Provides-Extra: dev
 Requires-Dist: pyvista[trame]; extra == "dev"
@@ -31,15 +32,15 @@
 - Support for Dirichlet, Neumann, Robin, and Periodic boundary conditions
 - Automatic generation of normals from 2D GMSH meshes
 
 𝕌pdes in incredibly extendable, with additional features added frequently.
 
 
 ## Getting started
-The package is available on PyPi. You can install it with
+The package is available on PyPI. You can install it with
 ```
 pip install updes
 ```
 
 The example below illustrates how to solve the Laplace equation with Dirichlet and Neumann boundary conditions:
 ```python
 import updes
@@ -74,15 +75,15 @@
 cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution")
 ```
 
 𝕌pdes can handle much complicated cases with little to no modifications to the code above. Check out further notebooks and scripts in the [documentation](https://ddrous.github.io/Updes/) and the folder [`demos`](./demos)!
 
 
 ## Dependencies
-- **Core**: JAX - GMSH - Matplotlib - Seaborn - Scikit-Learn
+- **Core**: JAX - GMSH - Lineax - Matplotlib - Seaborn - Scikit-Learn
 - **Optional**: PyVista - FFMPEG - QuartoDoc
 
 See the `pyproject.toml` file the specific versions of the dependencies.
 
 
 ## Cite us !
 If you use this software, please cite us with the following BibTeX entry:
```

