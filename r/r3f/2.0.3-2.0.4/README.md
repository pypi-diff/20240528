# Comparing `tmp/r3f-2.0.3.tar.gz` & `tmp/r3f-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3f-2.0.3.tar", last modified: Tue Apr 16 02:54:55 2024, max compression
+gzip compressed data, was "r3f-2.0.4.tar", last modified: Tue May 28 16:17:50 2024, max compression
```

## Comparing `r3f-2.0.3.tar` & `r3f-2.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.713215 r3f-2.0.3/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.3/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-04-16 02:54:55.713159 r3f-2.0.3/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.3/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.3/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2024-04-16 02:54:55.713438 r3f-2.0.3/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.710770 r3f-2.0.3/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.711910 r3f-2.0.3/src/r3f/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.3/src/r3f/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)   101759 2024-04-12 15:53:17.000000 r3f-2.0.3/src/r3f/r3f.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19785 2023-12-14 19:22:14.000000 r3f-2.0.3/src/r3f/test_r3f.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.713000 r3f-2.0.3/src/r3f.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.670345 r3f-2.0.4/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.4/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-28 16:17:50.670288 r3f-2.0.4/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.4/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.4/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2024-05-28 16:17:50.670578 r3f-2.0.4/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.668245 r3f-2.0.4/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.669360 r3f-2.0.4/src/r3f/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.4/src/r3f/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)   102708 2024-05-28 16:08:59.000000 r3f-2.0.4/src/r3f/r3f.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19909 2024-05-28 16:07:59.000000 r3f-2.0.4/src/r3f/test_r3f.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.670111 r3f-2.0.4/src/r3f.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/top_level.txt
```

### Comparing `r3f-2.0.3/LICENSE.txt` & `r3f-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `r3f-2.0.3/PKG-INFO` & `r3f-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.3
+Version: 2.0.4
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `r3f-2.0.3/README.md` & `r3f-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `r3f-2.0.3/setup.cfg` & `r3f-2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = r3f
-version = 2.0.3
+version = 2.0.4
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for three-dimensional, reference-frame conversions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/r3f
 classifiers =
```

### Comparing `r3f-2.0.3/src/r3f/r3f.py` & `r3f-2.0.4/src/r3f/r3f.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,19 +109,20 @@
 not conform to the ideal type and shape. Generally, the allowed types are int,
 float, list, and np.ndarray.
 --------------------------------------------------------------------------------
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-04-12"
+__date__ = "2024-05-28"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
+import math
 import numpy as np
 
 # WGS84 constants (IS-GPS-200M and NIMA TR8350.2)
 A_E = 6378137.0             # Earth's semi-major axis (m) (p. 109)
 F_E = 298.257223563         # Earth's flattening constant (NIMA)
 B_E = 6356752.314245        # Earth's semi-minor axis (m) A_E*(1 - 1/F_E)
 E2 = 6.694379990141317e-3   # Earth's eccentricity squared (ND) (derived)
@@ -1121,43 +1122,58 @@
     """
 
     # Check input.
     if isinstance(C, (list, tuple)):
         C = np.array(C)
     s = np.pi/180 if degs else 1.0
 
-    # Parse out the elements of the DCM that are needed.
     if C.ndim == 2:
+        # Parse out the elements of the DCM that are needed.
         c11 = C[0, 0]
         c33 = C[2, 2]
         c12 = C[0, 1]
         c13 = C[0, 2]
         c23 = C[1, 2]
+
+        # Get roll.
+        rpy = np.zeros(3)
+        rpy[0] = math.atan2(c23, c33)
+
+        # Get pitch.
+        sp = -c13
+        pa = math.asin(sp)
+        nm = math.sqrt(c11**2 + c12**2 + c23**2 + c33**2)
+        pb = math.acos(nm/math.sqrt(2))
+        rpy[1] = (1.0 - abs(sp))*pa + sp*pb
+
+        # Get yaw.
+        rpy[2] = math.atan2(c12, c11)
     else:
+        # Parse out the elements of the DCM that are needed.
         c11 = C[:, 0, 0]
         c33 = C[:, 2, 2]
         c12 = C[:, 0, 1]
         c13 = C[:, 0, 2]
         c23 = C[:, 1, 2]
 
-    # Get roll.
-    r = np.arctan2(c23, c33)
+        # Get roll.
+        r = np.arctan2(c23, c33)
 
-    # Get pitch.
-    sp = -c13
-    pa = np.arcsin(sp)
-    nm = np.sqrt(c11**2 + c12**2 + c23**2 + c33**2)
-    pb = np.arccos(nm/np.sqrt(2))
-    p = (1.0 - np.abs(sp))*pa + sp*pb
+        # Get pitch.
+        sp = -c13
+        pa = np.arcsin(sp)
+        nm = np.sqrt(c11**2 + c12**2 + c23**2 + c33**2)
+        pb = np.arccos(nm/np.sqrt(2))
+        p = (1.0 - np.abs(sp))*pa + sp*pb
 
-    # Get yaw.
-    y = np.arctan2(c12, c11)
+        # Get yaw.
+        y = np.arctan2(c12, c11)
 
-    # Build the output.
-    rpy = np.array([r, p ,y])/s
+        # Build the output.
+        rpy = np.array([r, p ,y])/s
 
     return rpy
 
 
 def rpy_to_dcm(rpy, degs=False):
     """
     Convert roll, pitch, and yaw Euler angles to a direction cosine matrix that
@@ -1200,83 +1216,102 @@
     trs = (rpy.ndim == 2 and rpy.shape[0] != 3)
     s = np.pi/180 if degs else 1.0
 
     # Tranpose.
     if trs:
         rpy = rpy.T
 
-    # Get the cosine and sine functions.
-    cr = np.cos(s*rpy[0])
-    sr = np.sin(s*rpy[0])
-    cp = np.cos(s*rpy[1])
-    sp = np.sin(s*rpy[1])
-    cy = np.cos(s*rpy[2])
-    sy = np.sin(s*rpy[2])
-
-    # Build the output matrix.
     if rpy.ndim == 1:
+        # Get the cosine and sine functions.
+        r, p, y = rpy
+        cr = math.cos(s*r)
+        sr = math.sin(s*r)
+        cp = math.cos(s*p)
+        sp = math.sin(s*p)
+        cy = math.cos(s*y)
+        sy = math.sin(s*y)
+
+        # Build the output matrix.
         C = np.array([
             [            cp*cy,             cp*sy,   -sp],
             [-cr*sy + sr*sp*cy,  cr*cy + sr*sp*sy, sr*cp],
             [ sr*sy + cr*sp*cy, -sr*cy + cr*sp*sy, cr*cp]])
     else:
+        # Get the cosine and sine functions.
+        cr = np.cos(s*rpy[0])
+        sr = np.sin(s*rpy[0])
+        cp = np.cos(s*rpy[1])
+        sp = np.sin(s*rpy[1])
+        cy = np.cos(s*rpy[2])
+        sy = np.sin(s*rpy[2])
+
+        # Build the output matrix.
         C = np.zeros((rpy.shape[1], 3, 3))
         C[:, 0, 0] = cp*cy
         C[:, 0, 1] = cp*sy
         C[:, 0, 2] = -sp
         C[:, 1, 0] = -cr*sy + sr*sp*cy
         C[:, 1, 1] = cr*cy + sr*sp*sy
         C[:, 1, 2] = sr*cp
         C[:, 2, 0] = sr*sy + cr*sp*cy
         C[:, 2, 1] = -sr*cy + cr*sp*sy
         C[:, 2, 2] = cr*cp
 
     return C
 
 
-def rot(ang, ax=2, degs=False):
+def rot(ang, ax=None, degs=False):
     """
     Build a three-dimensional rotation matrix from the rotation angles `ang`
     about the successive axes `ax`.
 
     Parameters
     ----------
     ang : float, int, list, tuple, or np.ndarray
         Angle of rotation in radians (or degrees if `degs` is True).
-    ax : {0, 1, 2}, float, int, list, tuple, or np.ndarray, default 2
-        Axis index about which to rotate. The x axis is 0, the y axis is 1,
-        and the z axis is 2.
+    ax : str, float, int, list, tuple, or np.ndarray, default None
+        Axis name(s) ('x', 'y', or 'z') or index(es) (x:0, y:1, or z:2) about
+        which to rotate.
     degs : bool, default False
         Flag to interpret angles as degrees.
 
     Returns
     -------
     C : (3, 3) np.ndarray
         Rotation matrix.
 
     See Also
     --------
     rpy_to_dcm
     """
 
-    # Control the input types.
+    # Check the angle.
     if np.ndim(ang) == 0: # scalar
         ang = np.array([float(ang)])
     elif isinstance(ang, (list, tuple)):
         ang = np.array(ang, dtype=float)
-    if np.ndim(ax) == 0: # scalar
+
+    # Check the axis.
+    if isinstance(ax, str): # string
+        ax = ax.lower()
+        ax_dict = {'x': 0, 'y': 1, 'z': 2}
+        ax = np.array([ax_dict[k] for k in ax if k in ax_dict.keys()])
+    elif np.ndim(ax) == 0: # scalar
         ax = np.array([int(ax)])
     elif isinstance(ax, (list, tuple)):
         ax = np.array(ax, dtype=int)
     elif isinstance(ax, np.ndarray) and ax.dtype is not int:
         ax = ax.astype(int)
+
+    # Check the degrees flag.
     s = np.pi/180 if degs else 1.0
 
     # Build the rotation matrix.
     N = len(ang)
+    C = np.eye(3)
     for n in range(N):
         # Skip trivial rotations.
         if ang[n] == 0:
             continue
 
         # Get the cosine and sine of ang.
         co = np.cos(s*ang[n])
@@ -1287,18 +1322,15 @@
             C_n = np.array([[1, 0, 0], [0, co, si], [0, -si, co]])
         elif ax[n] == 1:
             C_n = np.array([[co, 0, -si], [0, 1, 0], [si, 0, co]])
         elif ax[n] == 2:
             C_n = np.array([[co, si, 0], [-si, co, 0], [0, 0, 1]])
 
         # Pre-multiply the old rotation matrix by the new.
-        if n == 0:
-            C = C_n.copy()
-        else:
-            C = C_n @ C
+        C = C_n @ C
 
     return C
 
 
 def quat_to_rpy(q, degs=False):
     """
     Convert from a quaternion right-handed frame rotation to a roll, pitch, and
```

### Comparing `r3f-2.0.3/src/r3f/test_r3f.py` & `r3f-2.0.4/src/r3f/test_r3f.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,17 +357,22 @@
 
     A = np.array([
         [1, 0, 0],
         [0, irt2, irt2],
         [0, -irt2, irt2]])
     assert np.allclose(r3f.rot(45, 0, True), A)
 
+    # Multiple rotations
     R = r3f.rot([45, 45, 45], [2, 1, 0], True)
     assert np.allclose(R, A @ B @ C)
 
+    # String axes
+    R = r3f.rot([45, 45, 45], "zyx", True)
+    assert np.allclose(R, A @ B @ C)
+
     # preserve units
     ang = np.array([45, 45, 45])
     ax = np.array([2, 1, 0])
     R = r3f.rot(ang, ax, True)
     assert np.allclose(ang, np.array([45, 45, 45]))
 
 # -------------------------
```

### Comparing `r3f-2.0.3/src/r3f.egg-info/PKG-INFO` & `r3f-2.0.4/src/r3f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.3
+Version: 2.0.4
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

