# Comparing `tmp/camlab-0.1.1.tar.gz` & `tmp/camlab-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.1.1.tar", last modified: Mon May 27 05:58:01 2024, max compression
+gzip compressed data, was "camlab-0.1.1.1.tar", last modified: Tue May 28 15:27:06 2024, max compression
```

## Comparing `camlab-0.1.1.tar` & `camlab-0.1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:58:01.591128 camlab-0.1.1/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.1.1/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-05-27 05:58:01.590942 camlab-0.1.1/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.1.1/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      539 2024-05-27 05:57:14.000000 camlab-0.1.1/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-05-27 05:58:01.591189 camlab-0.1.1/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:58:01.588433 camlab-0.1.1/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:58:01.589835 camlab-0.1.1/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)     2294 2024-05-27 05:25:50.000000 camlab-0.1.1/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     7127 2024-05-27 05:25:50.000000 camlab-0.1.1/src/camlab/camera.py
--rw-r--r--   0 muzhan     (501) staff       (20)     3311 2024-05-27 05:56:18.000000 camlab-0.1.1/src/camlab/camera_torch.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:58:01.590746 camlab-0.1.1/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-05-27 05:58:01.000000 camlab-0.1.1/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      239 2024-05-27 05:58:01.000000 camlab-0.1.1/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-05-27 05:58:01.000000 camlab-0.1.1/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-05-27 05:58:01.000000 camlab-0.1.1/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.086759 camlab-0.1.1.1/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-05-28 15:23:20.000000 camlab-0.1.1.1/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:27:06.086579 camlab-0.1.1.1/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-05-28 15:23:20.000000 camlab-0.1.1.1/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-05-28 15:24:23.000000 camlab-0.1.1.1/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-05-28 15:27:06.086806 camlab-0.1.1.1/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.083464 camlab-0.1.1.1/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.084957 camlab-0.1.1.1/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2365 2024-05-28 15:25:05.000000 camlab-0.1.1.1/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-05-28 15:23:21.000000 camlab-0.1.1.1/src/camlab/camera.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     3435 2024-05-28 15:24:54.000000 camlab-0.1.1.1/src/camlab/camera_torch.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-28 15:27:06.086249 camlab-0.1.1.1/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      239 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-05-28 15:27:06.000000 camlab-0.1.1.1/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.1.1/LICENSE` & `camlab-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1/PKG-INFO` & `camlab-0.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.1.1/README.md` & `camlab-0.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.1.1/pyproject.toml` & `camlab-0.1.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.1.1"
+version = "0.1.1.1"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.1.1/src/camlab/__init__.py` & `camlab-0.1.1.1/src/camlab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,43 +8,44 @@
     return pixels / (2 * math.tan(fov / 2))
 
 
 def focal2fov(focal, pixels):
     return 2 * math.atan(pixels / (2 * focal))
 
 
-def load_3dgs_camera(cam_gs, tensor_style=False):
+def load_3dgs_camera(cam_gs, device="cpu"):
     """
     Support 3D Gaussian Splatting Camera-Class Object
     """
-    if not tensor_style:
+    if device.startswith("cpu"):
         cam = CameraObj(image_name=cam_gs.image_name)
         cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
                         w=cam_gs.image_width, h=cam_gs.image_height)
 
         ext = np.eye(4)
         ext[:3, :3] = np.transpose(cam_gs.R)
         ext[:3, 3] = cam_gs.T
         c2w = np.linalg.inv(ext)
         c2w[:3, 1:3] *= -1
 
         cam.R = c2w[:3, :3]
         cam.T = c2w[:3, 3]
     else:
-        cam = CameraObjTensor(image_name=cam_gs.image_name)
+        cam = CameraObjTensor(image_name=cam_gs.image_name,
+                              device=device)
         cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
                         w=cam_gs.image_width, h=cam_gs.image_height)
         ext = np.eye(4)
         ext[:3, :3] = np.transpose(cam_gs.R)
         ext[:3, 3] = cam_gs.T
         c2w = np.linalg.inv(ext)
         c2w[:3, 1:3] *= -1
 
-        cam.R = torch.FloatTensor(c2w[:3, :3])
-        cam.T = torch.FloatTensor(c2w[:3, 3])
+        cam.R = torch.FloatTensor(c2w[:3, :3]).to(device)
+        cam.Tr = torch.FloatTensor(c2w[:3, 3]).to(device)
 
     return cam
 
 
 def approximate(n, o=1e8):
     return int(n * o) / o
 
@@ -73,7 +74,8 @@
     expo = pow(10, acc)
     distance = np.linalg.norm(closest_point_line1 - closest_point_line2, ord=2)
     distance = approximate(distance, o=expo)
     closest_point_line1 = [approximate(n, o=expo) for n in list(closest_point_line1)]
     closest_point_line2 = [approximate(n, o=expo) for n in list(closest_point_line2)]
 
     return closest_point_line1, closest_point_line2, distance
+
```

### Comparing `camlab-0.1.1/src/camlab/camera.py` & `camlab-0.1.1.1/src/camlab/camera.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 
-
 class CameraObj:
-    def __init__(self, intri_mat=None, image_name=None):
+    def __init__(self, intri_mat=None):
         # intrinsic
         self.focal_x = None
         self.focal_y = None
         self.o_x = None
         self.o_y = None
         self.K = None
 
@@ -14,18 +13,15 @@
         self.h = None
         self.w = None
 
         # extrinsic
         self.R = None
         self.T = None
         self.is_intri_set = False
-
-        # image
-        self.image_name = image_name
-
+        
         self.touch = 0
 
         if intri_mat:
             self.K = intri_mat
             self.focal_x = intri_mat[0][0]
             self.focal_y = intri_mat[1][1]
             self.o_x = intri_mat[0][2]
@@ -56,15 +52,14 @@
             print("please set intri parameters !")
             raise Exception
 
     def world2cam(self, p):
         if self.R is None or self.T is None:
             print("Please init the extrinsic params!")
             return -1
-        print(np.dot(p - self.T, self.R))
         return np.dot(p - self.T, self.R)
 
     def cam2screen(self, p, to_int=False):
         """
                           x                                y
             x_im = f_x * --- + offset_x      y_im = f_y * --- + offset_y
                           z                                z
@@ -94,15 +89,15 @@
 
         x, y = screen_p
         direction = np.array([(x - self.o_x) / self.focal_x, - (y - self.o_y) / self.focal_y, -1])
         ray_d = np.sum(direction[None] * R, -1)
         ray_o = T
 
         return ray_o, ray_d
-
+     
     def quaternion2rotation(self, quater):
         self.touch += 1
         w, x, y, z = quater
         r11 = 1 - 2 * y * y - 2 * x * x
         r12 = 2 * x * y - 2 * z * w
         r13 = 2 * x * z + 2 * y * w
         r21 = 2 * x * y + 2 * z * w
@@ -125,92 +120,91 @@
         extri = np.eye(4)
         extri[:3, :3] = rot
         extri[0][-1] = trans[0]
         extri[1][-1] = trans[1]
         extri[2][-1] = trans[2]
         return extri
 
+       
 
 def _test1():
     import cv2
     intri = [[1111.0, 0.0, 400.0],
-             [0.0, 1111.0, 400.0],
-             [0.0, 0.0, 1.0]]
+         [0.0, 1111.0, 400.0],
+         [0.0, 0.0, 1.0]]
     extri = np.array(
-        [[-9.9990e-01, 4.1922e-03, -1.3346e-02, -5.3798e-02],
-         [-1.3989e-02, -2.9966e-01, 9.5394e-01, 3.8455e+00],
-         [-4.6566e-10, 9.5404e-01, 2.9969e-01, 1.2081e+00],
-         [0.0, 0.0, 0.0, 1.0]])
-    extri1 = np.array([[-3.0373e-01, -8.6047e-01, 4.0907e-01, 1.6490e+00],
-                       [9.5276e-01, -2.7431e-01, 1.3041e-01, 5.2569e-01],
-                       [-7.4506e-09, 4.2936e-01, 9.0313e-01, 3.6407e+00],
-                       [0.0, 0.0, 0.0, 1.0]])
+        [[-9.9990e-01,  4.1922e-03, -1.3346e-02, -5.3798e-02],
+        [-1.3989e-02, -2.9966e-01,  9.5394e-01,  3.8455e+00],
+        [-4.6566e-10,  9.5404e-01,  2.9969e-01,  1.2081e+00],
+        [0.0, 0.0, 0.0, 1.0]])
+    extri1 = np.array([[-3.0373e-01, -8.6047e-01,  4.0907e-01,  1.6490e+00],
+        [ 9.5276e-01, -2.7431e-01,  1.3041e-01,  5.2569e-01],
+        [-7.4506e-09,  4.2936e-01,  9.0313e-01,  3.6407e+00],
+        [0.0, 0.0, 0.0, 1.0]])
     extri2 = np.array(
         [[0.4429636299610138, 0.31377720832824707, -0.8398374915122986, -3.385493516921997],
          [-0.8965396881103516, 0.1550314873456955, -0.41494810581207275, -1.6727094650268555],
          [0.0, 0.936754584312439, 0.3499869406223297, 1.4108426570892334],
          [0.0, 0.0, 0.0, 1.0]])
 
     cam_obj = CameraObj(intri)
     cam_obj.load_extrinsic(extri)
-    print(cam_obj.world2screen([-1, -1, -1]))
-    return
 
     vertex = [[-1, -1, -1], [1, -1, -1], [1, 1, -1], [-1, 1, -1], [-1, 1, 1], [1, 1, 1], [1, -1, 1], [-1, -1, 1]]
     # vertex = [[-.5, -.5, -.5], [.5, -.5, -.5], [.5, .5, -.5], [-.5, .5, -.5], [-.5, .5, .5], [.5, .5, .5], [.5, -.5, .5], [-.5, -.5, .5]]
 
     # blank = np.zeros((800, 800, 3), np.uint8)
     blank = cv2.imread("r_0.png")
-    # print(blank.shape)
+    print(blank.shape)
 
     p_s = [cam_obj.world2screen(p_, to_int=True) for p_ in vertex]
     print(p_s)
 
     for i in range(len(p_s)):
         p1 = p_s[i]
         p2 = p_s[i + 1] if i < len(p_s) - 1 else p_s[0]
         cv2.line(blank, p1, p2, (255, 255, 0), 1)
     cv2.line(blank, p_s[3], p_s[0], (255, 255, 0), 1)
     cv2.line(blank, p_s[4], p_s[7], (255, 255, 0), 1)
     cv2.line(blank, p_s[1], p_s[6], (255, 255, 0), 1)
     cv2.line(blank, p_s[2], p_s[5], (255, 255, 0), 1)
     cv2.imwrite("demo.png", blank)
 
-
 def _test2():
     intri = [[1111.0, 0.0, 400.0],
-             [0.0, 1111.0, 400.0],
-             [0.0, 0.0, 1.0]]
+         [0.0, 1111.0, 400.0],
+         [0.0, 0.0, 1.0]]
     extri = np.array(
-        [[-9.9990e-01, 4.1922e-03, -1.3346e-02, -5.3798e-02],
-         [-1.3989e-02, -2.9966e-01, 9.5394e-01, 3.8455e+00],
-         [-4.6566e-10, 9.5404e-01, 2.9969e-01, 1.2081e+00],
-         [0.0, 0.0, 0.0, 1.0]])
-    extri1 = np.array([[-3.0373e-01, -8.6047e-01, 4.0907e-01, 1.6490e+00],
-                       [9.5276e-01, -2.7431e-01, 1.3041e-01, 5.2569e-01],
-                       [-7.4506e-09, 4.2936e-01, 9.0313e-01, 3.6407e+00],
-                       [0.0, 0.0, 0.0, 1.0]])
+        [[-9.9990e-01,  4.1922e-03, -1.3346e-02, -5.3798e-02],
+        [-1.3989e-02, -2.9966e-01,  9.5394e-01,  3.8455e+00],
+        [-4.6566e-10,  9.5404e-01,  2.9969e-01,  1.2081e+00],
+        [0.0, 0.0, 0.0, 1.0]])
+    extri1 = np.array([[-3.0373e-01, -8.6047e-01,  4.0907e-01,  1.6490e+00],
+        [ 9.5276e-01, -2.7431e-01,  1.3041e-01,  5.2569e-01],
+        [-7.4506e-09,  4.2936e-01,  9.0313e-01,  3.6407e+00],
+        [0.0, 0.0, 0.0, 1.0]])
     extri2 = np.array(
         [[0.4429636299610138, 0.31377720832824707, -0.8398374915122986, -3.385493516921997],
          [-0.8965396881103516, 0.1550314873456955, -0.41494810581207275, -1.6727094650268555],
          [0.0, 0.936754584312439, 0.3499869406223297, 1.4108426570892334],
          [0.0, 0.0, 0.0, 1.0]])
 
     cam_obj = CameraObj(intri)
     cam_obj.load_extrinsic(extri2)
 
     p = (400, 400)
     rayo, rayd = cam_obj.make_ray(p)
     ps = cam_obj.world2screen(rayd - rayo, to_int=True)
     print(rayo, rayd)
     print(ps)
-
+    
     quater = [0.980317, 0.002613, -0.19732, 0.005964]
     print(cam_obj.quaternion2rotation(quater))
 
     colmap_params = [0.980317, 0.002613, -0.19732, 0.005964, 5.91824, 0.099605, 0.691238]
     print(cam_obj.colmap2extri(colmap_params))
 
 
+
 if __name__ == "__main__":
-    _test1()
-    # _test2()
+    # _test1()
+    _test2()
```

### Comparing `camlab-0.1.1/src/camlab/camera_torch.py` & `camlab-0.1.1.1/src/camlab/camera_torch.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         # screen
         self.h = None
         self.w = None
 
         # extrinsic
         self.R = None
-        self.T = None
+        self.Tr = None
         self.is_intri_set = False
 
         # image
         self.image_name = image_name
 
         self.touch = 0
 
@@ -53,48 +53,52 @@
         self.w = w
         self.h = h
         self.o_x = w / 2
         self.o_y = h / 2
         self.is_intri_set = True
 
         intrinsic = np.eye(3)
-        intrinsic[0][0] = self.focal_x
+        intrinsic[0][0] = self.focal_x * -1
         intrinsic[1][1] = self.focal_y
         intrinsic[0][2] = self.o_x
         intrinsic[1][2] = self.o_y
 
         self.intrinsic = torch.FloatTensor(intrinsic)
         self.intrinsic = self.intrinsic.to(self.device)
 
     def load_extrinsic(self, extrinsic):
         self.R = torch.FloatTensor(extrinsic[:3, :3]).to(self.device)
-        self.T = torch.FloatTensor(extrinsic[:3, -1]).to(self.device)
+        self.Tr = torch.FloatTensor(extrinsic[:3, -1]).to(self.device)
 
     def intri_check(self):
         if not self.is_intri_set:
             print("please set intri parameters !")
             raise Exception
 
     def world2cam(self, p):
-        if self.R is None or self.T is None:
+        if self.R is None or self.Tr is None:
             print("Please init the extrinsic params!")
             return -1
-        return torch.mm(p - self.T, self.R).T
+        return torch.matmul(p - self.Tr, self.R).T
 
     def cam2screen(self, p):
         """
                           x                                y
             x_im = f_x * --- + offset_x      y_im = f_y * --- + offset_y
                           z                                z
         """
-        return torch.mm(self.intrinsic, p) / p[2]
+        res = torch.matmul(self.intrinsic, p) / p[2]
+        return res.T[:, :2]
 
-    def world2screen(self, p):
+    def world2screen(self, p, to_int=False):
         self.intri_check()
-        return self.cam2screen(self.world2cam(p))
+        res = self.cam2screen(self.world2cam(p))
+        if to_int:
+            res = res.long()
+        return res
 
 
 def _test():
     intri = [[1111.0, 0.0, 400.0],
              [0.0, 1111.0, 400.0],
              [0.0, 0.0, 1.0]]
     extri = np.array(
@@ -102,17 +106,18 @@
          [-1.3989e-02, -2.9966e-01, 9.5394e-01, 3.8455e+00],
          [-4.6566e-10, 9.5404e-01, 2.9969e-01, 1.2081e+00],
          [0.0, 0.0, 0.0, 1.0]])
 
     cam_obj = CameraObjTensor(intri)
     cam_obj.load_extrinsic(extri)
 
-    a = [[-1, -1, -1] for _ in range(1000000)]
+    a = [[-1, 1, -1] for _ in range(1000000)]
     p = torch.FloatTensor(a)
     p = p.to("cuda:0")
     p1 = cam_obj.world2screen(p)
     print(p1[0])
     print(p1.shape)
 
 
 if __name__ == "__main__":
     _test()
+
```

### Comparing `camlab-0.1.1/src/camlab.egg-info/PKG-INFO` & `camlab-0.1.1.1/src/camlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

