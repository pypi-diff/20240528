# Comparing `tmp/eyegestures-2.0.0.tar.gz` & `tmp/eyegestures-2.1.0.tar.gz`

## Comparing `eyegestures-2.0.0.tar` & `eyegestures-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/Fixation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/__init__.py
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/calibration_v1.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/calibration_v2.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/eye.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/eyegestures.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/face.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gazeContexter.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gazeEstimator.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gevent.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/processing.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/scalling_test.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker_test.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/utils.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/clusters.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/dataPoints.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/heatmap.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/screenTracker.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eyegestures-2.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-2.0.0/LICENSE
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 eyegestures-2.0.0/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    48245 2020-02-02 00:00:00.000000 eyegestures-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/Fixation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/__init__.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/calibration_v1.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/calibration_v2.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/eye.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/eyegestures.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/face.py
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/gazeContexter.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/gazeEstimator.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/gevent.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/processing.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/scalling_test.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/screenTracker_test.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/utils.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/screenTracker/clusters.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/screenTracker/dataPoints.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/screenTracker/heatmap.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 eyegestures-2.1.0/eyeGestures/screenTracker/screenTracker.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 eyegestures-2.1.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 eyegestures-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 eyegestures-2.1.0/README.md
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 eyegestures-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    48474 2020-02-02 00:00:00.000000 eyegestures-2.1.0/PKG-INFO
```

### Comparing `eyegestures-2.0.0/eyeGestures/calibration_v1.py` & `eyegestures-2.1.0/eyeGestures/calibration_v1.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import time
-
-
-class CalibrationPositions:
-    LEFT = "left"
-    RIGHT = "right"
-    TOP = "top"
-    BOTTOM = "bottom"
-
-class Calibrator:
-
-    def __init__(self, width, height, start_x, start_y):
-        self.width = width
-        self.height = height
-        self.start_x = start_x
-        self.start_y = start_y
-
-        self.prev_x = 0
-        self.prev_y = 0
-
-        self.calibration_margin = 200
-        self.calibration_steps = []
-        self.__set_order()
-
-        self.calibrate_left = False
-        self.calibrate_right = False
-        self.calibrate_top = False
-        self.calibrate_bottom = False
-
-        self.calibration = False
-        self.drawn = False
-        self.prev_point = None
-        self.last_calib = time.time()
-        pass
-
-    def __add_left(self):
-        self.calibration_steps.append(CalibrationPositions.LEFT)
-        return self
-    def __add_right(self):
-        self.calibration_steps.append(CalibrationPositions.RIGHT)
-        return self
-
-    def __add_top(self):
-        self.calibration_steps.append(CalibrationPositions.TOP)
-        return self
-
-    def __add_bottom(self):
-        self.calibration_steps.append(CalibrationPositions.BOTTOM)
-        return self
-
-    def __set_order(self):
-        if self.start_x < self.width/2 and CalibrationPositions.LEFT not in self.calibration_steps:
-            self.__add_left().__add_right()
-        elif self.start_x > self.width/2 and CalibrationPositions.RIGHT not in self.calibration_steps:
-            self.__add_right().__add_left()
-
-        if self.start_y < self.height/2 and CalibrationPositions.TOP not in self.calibration_steps:
-            self.__add_top().__add_bottom()
-        elif self.start_y > self.height/2 and CalibrationPositions.BOTTOM not in self.calibration_steps:
-            self.__add_bottom().__add_top()
-
-    def add_recalibrate(self,recalibrate_step):
-
-        if recalibrate_step not in self.calibration_steps:
-            self.calibration_steps.append(recalibrate_step)
-
-    def get_current_point(self):
-        if len(self.calibration_steps) > 0:
-            if CalibrationPositions.LEFT == self.calibration_steps[0]:
-                return (self.calibration_margin, int(self.height/2))
-            elif CalibrationPositions.RIGHT == self.calibration_steps[0]:
-                return (self.width - self.calibration_margin, int(self.height/2))
-            elif CalibrationPositions.TOP == self.calibration_steps[0]:
-                return (int(self.width/2), self.calibration_margin)
-            elif CalibrationPositions.BOTTOM == self.calibration_steps[0]:
-                return (int(self.width/2), self.height - self.calibration_margin)
-        else:
-            return (0,0)
-
-    def calibrate(self,x,y,fix):
-
-        if abs(x - self.width/2) > 150 and self.prev_point in [CalibrationPositions.TOP, CalibrationPositions.BOTTOM]:
-            if x - self.width/2 < 0:
-                self.add_recalibrate(CalibrationPositions.LEFT)
-            else:
-                self.add_recalibrate(CalibrationPositions.RIGHT)
-
-        if abs(y - self.height/2) > 150  and self.prev_point in [CalibrationPositions.LEFT, CalibrationPositions.RIGHT]:
-            if y - self.height/2 < 0:
-                self.add_recalibrate(CalibrationPositions.TOP)
-            else:
-                self.add_recalibrate(CalibrationPositions.BOTTOM)
-
-        self.prev_y = y
-        self.prev_x = x
-        if len(self.calibration_steps) <= 0:
-            self.prev_point = None
-            return False
-
-        fixation_thresh = 0.3
-        if fix > fixation_thresh and (time.time() - self.last_calib) > 5.0:
-            if CalibrationPositions.LEFT == self.calibration_steps[0] and x < self.calibration_margin:
-                if CalibrationPositions.LEFT in self.calibration_steps:
-                    self.calibration_steps.remove(CalibrationPositions.LEFT)
-                self.prev_point = CalibrationPositions.LEFT
-                self.drawn = False
-                self.last_calib = time.time()
-                return True
-            elif CalibrationPositions.RIGHT == self.calibration_steps[0] and x > self.width - self.calibration_margin:
-                if CalibrationPositions.RIGHT in self.calibration_steps:
-                    self.calibration_steps.remove(CalibrationPositions.RIGHT)
-                self.prev_point = CalibrationPositions.RIGHT
-                self.drawn = False
-                self.last_calib = time.time()
-                return True
-            elif CalibrationPositions.TOP == self.calibration_steps[0] and y < self.calibration_margin:
-                if CalibrationPositions.TOP in self.calibration_steps:
-                    self.calibration_steps.remove(CalibrationPositions.TOP)
-                self.prev_point = CalibrationPositions.TOP
-                self.drawn = False
-                self.last_calib = time.time()
-                return True
-            elif CalibrationPositions.BOTTOM == self.calibration_steps[0] and y > self.height - self.calibration_margin:
-                if CalibrationPositions.BOTTOM in self.calibration_steps:
-                    self.calibration_steps.remove(CalibrationPositions.BOTTOM)
-                self.prev_point = CalibrationPositions.BOTTOM
-                self.drawn = False
-                self.last_calib = time.time()
-                return True
-            else:
-                # TODO: somewhere here is bug breaking entire program
-                self.last_calib = time.time()
-                self.drawn = False
-                self.prev_point = None
-
-                if self.calibration_steps[0] in [CalibrationPositions.RIGHT,CalibrationPositions.LEFT]:
-                    if x < self.width/2:
-                        if CalibrationPositions.RIGHT in self.calibration_steps:
-                            self.calibration_steps.remove(CalibrationPositions.RIGHT)
-                        self.calibration_steps.insert(0,CalibrationPositions.RIGHT)
-                    else:
-                        if CalibrationPositions.LEFT in self.calibration_steps:
-                            self.calibration_steps.remove(CalibrationPositions.LEFT)
-                        self.calibration_steps.insert(0,CalibrationPositions.LEFT)
-                    return True
-
-                if self.calibration_steps[0] is CalibrationPositions.TOP:
-                    self.calibration_steps.insert(0,CalibrationPositions.BOTTOM)
-                    return True
-                else:
-                    self.calibration_steps.insert(0,CalibrationPositions.TOP)
-                    return True
-
-        self.prev_point = None
-        return False
-
-    def calibrated(self):
-        return len(self.calibration_steps) <= 0
-
-
+import time
+
+
+class CalibrationPositions:
+    LEFT = "left"
+    RIGHT = "right"
+    TOP = "top"
+    BOTTOM = "bottom"
+
+class Calibrator:
+
+    def __init__(self, width, height, start_x, start_y):
+        self.width = width
+        self.height = height
+        self.start_x = start_x
+        self.start_y = start_y
+
+        self.prev_x = 0
+        self.prev_y = 0
+
+        self.calibration_margin = 200
+        self.calibration_steps = []
+        self.__set_order()
+
+        self.calibrate_left = False
+        self.calibrate_right = False
+        self.calibrate_top = False
+        self.calibrate_bottom = False
+
+        self.calibration = False
+        self.drawn = False
+        self.prev_point = None
+        self.last_calib = time.time()
+        pass
+
+    def __add_left(self):
+        self.calibration_steps.append(CalibrationPositions.LEFT)
+        return self
+    def __add_right(self):
+        self.calibration_steps.append(CalibrationPositions.RIGHT)
+        return self
+
+    def __add_top(self):
+        self.calibration_steps.append(CalibrationPositions.TOP)
+        return self
+
+    def __add_bottom(self):
+        self.calibration_steps.append(CalibrationPositions.BOTTOM)
+        return self
+
+    def __set_order(self):
+        if self.start_x < self.width/2 and CalibrationPositions.LEFT not in self.calibration_steps:
+            self.__add_left().__add_right()
+        elif self.start_x > self.width/2 and CalibrationPositions.RIGHT not in self.calibration_steps:
+            self.__add_right().__add_left()
+
+        if self.start_y < self.height/2 and CalibrationPositions.TOP not in self.calibration_steps:
+            self.__add_top().__add_bottom()
+        elif self.start_y > self.height/2 and CalibrationPositions.BOTTOM not in self.calibration_steps:
+            self.__add_bottom().__add_top()
+
+    def add_recalibrate(self,recalibrate_step):
+
+        if recalibrate_step not in self.calibration_steps:
+            self.calibration_steps.append(recalibrate_step)
+
+    def get_current_point(self):
+        if len(self.calibration_steps) > 0:
+            if CalibrationPositions.LEFT == self.calibration_steps[0]:
+                return (self.calibration_margin, int(self.height/2))
+            elif CalibrationPositions.RIGHT == self.calibration_steps[0]:
+                return (self.width - self.calibration_margin, int(self.height/2))
+            elif CalibrationPositions.TOP == self.calibration_steps[0]:
+                return (int(self.width/2), self.calibration_margin)
+            elif CalibrationPositions.BOTTOM == self.calibration_steps[0]:
+                return (int(self.width/2), self.height - self.calibration_margin)
+        else:
+            return (0,0)
+
+    def calibrate(self,x,y,fix):
+
+        if abs(x - self.width/2) > 150 and self.prev_point in [CalibrationPositions.TOP, CalibrationPositions.BOTTOM]:
+            if x - self.width/2 < 0:
+                self.add_recalibrate(CalibrationPositions.LEFT)
+            else:
+                self.add_recalibrate(CalibrationPositions.RIGHT)
+
+        if abs(y - self.height/2) > 150  and self.prev_point in [CalibrationPositions.LEFT, CalibrationPositions.RIGHT]:
+            if y - self.height/2 < 0:
+                self.add_recalibrate(CalibrationPositions.TOP)
+            else:
+                self.add_recalibrate(CalibrationPositions.BOTTOM)
+
+        self.prev_y = y
+        self.prev_x = x
+        if len(self.calibration_steps) <= 0:
+            self.prev_point = None
+            return False
+
+        fixation_thresh = 0.3
+        if fix > fixation_thresh and (time.time() - self.last_calib) > 5.0:
+            if CalibrationPositions.LEFT == self.calibration_steps[0] and x < self.calibration_margin:
+                if CalibrationPositions.LEFT in self.calibration_steps:
+                    self.calibration_steps.remove(CalibrationPositions.LEFT)
+                self.prev_point = CalibrationPositions.LEFT
+                self.drawn = False
+                self.last_calib = time.time()
+                return True
+            elif CalibrationPositions.RIGHT == self.calibration_steps[0] and x > self.width - self.calibration_margin:
+                if CalibrationPositions.RIGHT in self.calibration_steps:
+                    self.calibration_steps.remove(CalibrationPositions.RIGHT)
+                self.prev_point = CalibrationPositions.RIGHT
+                self.drawn = False
+                self.last_calib = time.time()
+                return True
+            elif CalibrationPositions.TOP == self.calibration_steps[0] and y < self.calibration_margin:
+                if CalibrationPositions.TOP in self.calibration_steps:
+                    self.calibration_steps.remove(CalibrationPositions.TOP)
+                self.prev_point = CalibrationPositions.TOP
+                self.drawn = False
+                self.last_calib = time.time()
+                return True
+            elif CalibrationPositions.BOTTOM == self.calibration_steps[0] and y > self.height - self.calibration_margin:
+                if CalibrationPositions.BOTTOM in self.calibration_steps:
+                    self.calibration_steps.remove(CalibrationPositions.BOTTOM)
+                self.prev_point = CalibrationPositions.BOTTOM
+                self.drawn = False
+                self.last_calib = time.time()
+                return True
+            else:
+                # TODO: somewhere here is bug breaking entire program
+                self.last_calib = time.time()
+                self.drawn = False
+                self.prev_point = None
+
+                if self.calibration_steps[0] in [CalibrationPositions.RIGHT,CalibrationPositions.LEFT]:
+                    if x < self.width/2:
+                        if CalibrationPositions.RIGHT in self.calibration_steps:
+                            self.calibration_steps.remove(CalibrationPositions.RIGHT)
+                        self.calibration_steps.insert(0,CalibrationPositions.RIGHT)
+                    else:
+                        if CalibrationPositions.LEFT in self.calibration_steps:
+                            self.calibration_steps.remove(CalibrationPositions.LEFT)
+                        self.calibration_steps.insert(0,CalibrationPositions.LEFT)
+                    return True
+
+                if self.calibration_steps[0] is CalibrationPositions.TOP:
+                    self.calibration_steps.insert(0,CalibrationPositions.BOTTOM)
+                    return True
+                else:
+                    self.calibration_steps.insert(0,CalibrationPositions.TOP)
+                    return True
+
+        self.prev_point = None
+        return False
+
+    def calibrated(self):
+        return len(self.calibration_steps) <= 0
+
+
```

### Comparing `eyegestures-2.0.0/eyeGestures/eye.py` & `eyegestures-2.1.0/eyeGestures/eye.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-"""Module providing a extraction of eye from face object."""
-
-import cv2
-import numpy as np
-import mediapipe as mp
-
-
-class Eye:
-    """Class storing data related and representing a eye"""
-    LEFT_EYE_KEYPOINTS = np.array(
-        list(mp.solutions.face_mesh.FACEMESH_LEFT_EYE))[:, 0]
-    RIGHT_EYE_KEYPOINTS = np.array(
-        list(mp.solutions.face_mesh.FACEMESH_RIGHT_EYE))[:, 0]
-    LEFT_EYE_IRIS_KEYPOINT = []
-    RIGHT_EYE_IRIS_KEYPOINT = []
-    LEFT_EYE_PUPIL_KEYPOINT = [473]
-    RIGHT_EYE_PUPIL_KEYPOINT = [468]
-
-    # LEFT_EYE_KEYPOINTS = [36, 37, 38, 39, 40, 41] # keypoint indices for left eye
-    # RIGHT_EYE_KEYPOINTS = [42, 43, 44, 45, 46, 47] # keypoint indices for right eye
-
-    scale = (150, 100)
-
-    def __init__(self, side: int):
-
-        # check if eye is left or right
-        if side == 1:
-            self.side = "right"
-            self.pupil_index = self.RIGHT_EYE_PUPIL_KEYPOINT
-        elif side == 0:
-            self.side = "left"
-            self.pupil_index = self.LEFT_EYE_PUPIL_KEYPOINT
-
-        self.x = 0
-        self.y = 0
-        self.width = 0
-        self.height = 0
-        self.center_x = 0
-        self.center_y = 0
-        self.image = None
-        self.pupil = None
-        self.offset = None
-        self.region = None
-        self.cut_image = None
-        self.landmarks = None
-
-        # self._process(self.image,self.region)
-
-    def update(self, image: np.ndarray, landmarks: list, offset: np.ndarray):
-        """function updating data stored inside eye object"""
-
-        self.image = image
-        self.offset = offset
-        self.landmarks = landmarks
-
-        # check if eye is left or right
-        if self.side == "right":
-            self.region = np.array(
-                landmarks[self.RIGHT_EYE_KEYPOINTS], dtype=np.int32)
-
-        elif self.side == "left":
-            self.region = np.array(
-                landmarks[self.LEFT_EYE_KEYPOINTS], dtype=np.int32)
-
-        self.pupil = landmarks[self.pupil_index][0]
-        self._process(self.image, self.region)
-
-    def getCenter(self):
-        """function returning center of eye"""
-
-        return (self.center_x, self.center_y)
-
-    def getPos(self):
-        """function returning position of eye in the image"""
-
-        return (self.x, self.y)
-
-    def getPupil(self):
-        """function returning pupil object"""
-
-        # return self.pupil.getCoords()
-        return self.pupil
-
-    def getBlink(self):
-        """function returning blink event"""
-        # return self.pupil.getCoords()
-        return (self.height) <= 3  # 2x margin
-
-    def getImage(self):
-        """function returning image of the eye cut from the entire face image"""
-
-        # TODO: draw additional parameters
-        return self.cut_image
-
-    def getGaze(self, gaze_buffor, y_correction=0, x_correction=0):
-        """function returning gaze position"""
-
-        # pupilCoords = self.pupil.getCoords()
-        center = np.array((self.center_x, self.center_y)) - self.offset
-
-        region_corrected = self.region - self.offset
-        pupil_corrected = self.pupil - self.offset
-
-        vectors = region_corrected - center
-        pupil = pupil_corrected - center
-
-        vectors = vectors - pupil
-        gaze_vector = np.zeros((2))
-
-        gaze_vector[1] = np.sum(vectors, axis=0)[1] * 10 - y_correction
-        gaze_vector[0] = -np.sum(vectors, axis=0)[0] * 10 - x_correction
-
-        # print("gaze_vector: ",gaze_vector)
-        gaze_buffor.add(gaze_vector)
-        return gaze_buffor.getAvg()
-
-    def getOpenness(self):
-        """function returning eye openness"""
-
-        return self.height/2
-
-    def getLandmarks(self):
-        """function returning eye landmarks"""
-
-        return self.region
-    
-    def getBoundingBox(self):
-        return (self.x,self.y,self.width,self.height)
-
-    def _process(self, image, region):
-        h, w, _ = image.shape
-
-        mask = np.full((h, w), 0, dtype=np.uint8)
-        background = np.zeros((h, w), dtype=np.uint8)
-        cv2.fillPoly(mask, [region], 0)
-
-        masked_image = cv2.bitwise_not(background, cv2.cvtColor(
-            image.copy(), cv2.COLOR_BGR2GRAY), mask=mask)
-
-        margin = 2
-        min_x = np.min(region[:, 0]) - margin
-        max_x = np.max(region[:, 0]) + margin
-        min_y = np.min(region[:, 1]) - margin
-        max_y = np.max(region[:, 1]) + margin
-
-        self.x = min_x
-        self.y = min_y
-
-        self.width = np.max(region[:, 0]) - np.min(region[:, 0])
-        self.height = np.max(region[:, 1]) - np.min(region[:, 1])
-
-        self.center_x = (min_x + max_x)/2
-        self.center_y = (min_y + max_y)/2
-
-        # HACKETY_HACK:
-        self.pupil[1] = np.min(region[:, 1])
-
-        self.cut_image = masked_image[min_y:max_y, min_x:max_x]
-        # print(f"here: {self.cut_image.shape,min_y,max_y,min_x,max_x}")
-        self.cut_image = cv2.cvtColor(self.cut_image, cv2.COLOR_GRAY2BGR)
-
-        for point in self.region:
-            point = point - (min_x, min_y)
-            cv2.circle(self.cut_image, point.astype(
-                int), 1, (255, 0, 0, 150), 1)
-
-        pupil = self.pupil - (min_x, min_y)
-
-        # print(f"pupil: {pupil}")
-        cv2.circle(self.cut_image, pupil.astype(int), 1, (0, 255, 0, 150), 1)
-
-        self.cut_image = cv2.resize(self.cut_image, self.scale)
-
-        # save cut_image to buffor and get avg from previous buffors
-        # self.eyeBuffer.add(self.cut_image)
-        # self.cut_image = np.array(self.eyeBuffer.getAvg(), dtype=np.uint8)
-
-        # LEGACY
-        # org_scale = (max_x - min_x,max_y - min_y)
-        # self.pupil = pupil.Pupil(self.cut_image, min_x, min_y, self.scale, org_scale)
+"""Module providing a extraction of eye from face object."""
+
+import cv2
+import numpy as np
+import mediapipe as mp
+
+
+class Eye:
+    """Class storing data related and representing a eye"""
+    LEFT_EYE_KEYPOINTS = np.array(
+        list(mp.solutions.face_mesh.FACEMESH_LEFT_EYE))[:, 0]
+    RIGHT_EYE_KEYPOINTS = np.array(
+        list(mp.solutions.face_mesh.FACEMESH_RIGHT_EYE))[:, 0]
+    LEFT_EYE_IRIS_KEYPOINT = []
+    RIGHT_EYE_IRIS_KEYPOINT = []
+    LEFT_EYE_PUPIL_KEYPOINT = [473]
+    RIGHT_EYE_PUPIL_KEYPOINT = [468]
+
+    # LEFT_EYE_KEYPOINTS = [36, 37, 38, 39, 40, 41] # keypoint indices for left eye
+    # RIGHT_EYE_KEYPOINTS = [42, 43, 44, 45, 46, 47] # keypoint indices for right eye
+
+    scale = (150, 100)
+
+    def __init__(self, side: int):
+
+        # check if eye is left or right
+        if side == 1:
+            self.side = "right"
+            self.pupil_index = self.RIGHT_EYE_PUPIL_KEYPOINT
+        elif side == 0:
+            self.side = "left"
+            self.pupil_index = self.LEFT_EYE_PUPIL_KEYPOINT
+
+        self.x = 0
+        self.y = 0
+        self.width = 0
+        self.height = 0
+        self.center_x = 0
+        self.center_y = 0
+        self.image = None
+        self.pupil = None
+        self.offset = None
+        self.region = None
+        self.cut_image = None
+        self.landmarks = None
+
+        # self._process(self.image,self.region)
+
+    def update(self, image: np.ndarray, landmarks: list, offset: np.ndarray):
+        """function updating data stored inside eye object"""
+
+        self.image = image
+        self.offset = offset
+        self.landmarks = landmarks
+
+        # check if eye is left or right
+        if self.side == "right":
+            self.region = np.array(
+                landmarks[self.RIGHT_EYE_KEYPOINTS], dtype=np.int32)
+
+        elif self.side == "left":
+            self.region = np.array(
+                landmarks[self.LEFT_EYE_KEYPOINTS], dtype=np.int32)
+
+        self.pupil = landmarks[self.pupil_index][0]
+        self._process(self.image, self.region)
+
+    def getCenter(self):
+        """function returning center of eye"""
+
+        return (self.center_x, self.center_y)
+
+    def getPos(self):
+        """function returning position of eye in the image"""
+
+        return (self.x, self.y)
+
+    def getPupil(self):
+        """function returning pupil object"""
+
+        # return self.pupil.getCoords()
+        return self.pupil
+
+    def getBlink(self):
+        """function returning blink event"""
+        # return self.pupil.getCoords()
+        return (self.height) <= 3  # 2x margin
+
+    def getImage(self):
+        """function returning image of the eye cut from the entire face image"""
+
+        # TODO: draw additional parameters
+        return self.cut_image
+
+    def getGaze(self, gaze_buffor, y_correction=0, x_correction=0):
+        """function returning gaze position"""
+
+        # pupilCoords = self.pupil.getCoords()
+        center = np.array((self.center_x, self.center_y)) - self.offset
+
+        region_corrected = self.region - self.offset
+        pupil_corrected = self.pupil - self.offset
+
+        vectors = region_corrected - center
+        pupil = pupil_corrected - center
+
+        vectors = vectors - pupil
+        gaze_vector = np.zeros((2))
+
+        gaze_vector[1] = np.sum(vectors, axis=0)[1] * 10 - y_correction
+        gaze_vector[0] = -np.sum(vectors, axis=0)[0] * 10 - x_correction
+
+        # print("gaze_vector: ",gaze_vector)
+        gaze_buffor.add(gaze_vector)
+        return gaze_buffor.getAvg()
+
+    def getOpenness(self):
+        """function returning eye openness"""
+
+        return self.height/2
+
+    def getLandmarks(self):
+        """function returning eye landmarks"""
+
+        return self.region
+    
+    def getBoundingBox(self):
+        return (self.x,self.y,self.width,self.height)
+
+    def _process(self, image, region):
+        h, w, _ = image.shape
+
+        mask = np.full((h, w), 0, dtype=np.uint8)
+        background = np.zeros((h, w), dtype=np.uint8)
+        cv2.fillPoly(mask, [region], 0)
+
+        masked_image = cv2.bitwise_not(background, cv2.cvtColor(
+            image.copy(), cv2.COLOR_BGR2GRAY), mask=mask)
+
+        margin = 2
+        min_x = np.min(region[:, 0]) - margin
+        max_x = np.max(region[:, 0]) + margin
+        min_y = np.min(region[:, 1]) - margin
+        max_y = np.max(region[:, 1]) + margin
+
+        self.x = min_x
+        self.y = min_y
+
+        self.width = np.max(region[:, 0]) - np.min(region[:, 0])
+        self.height = np.max(region[:, 1]) - np.min(region[:, 1])
+
+        self.center_x = (min_x + max_x)/2
+        self.center_y = (min_y + max_y)/2
+
+        # HACKETY_HACK:
+        self.pupil[1] = np.min(region[:, 1])
+
+        self.cut_image = masked_image[min_y:max_y, min_x:max_x]
+        # print(f"here: {self.cut_image.shape,min_y,max_y,min_x,max_x}")
+        self.cut_image = cv2.cvtColor(self.cut_image, cv2.COLOR_GRAY2BGR)
+
+        for point in self.region:
+            point = point - (min_x, min_y)
+            cv2.circle(self.cut_image, point.astype(
+                int), 1, (255, 0, 0, 150), 1)
+
+        pupil = self.pupil - (min_x, min_y)
+
+        # print(f"pupil: {pupil}")
+        cv2.circle(self.cut_image, pupil.astype(int), 1, (0, 255, 0, 150), 1)
+
+        self.cut_image = cv2.resize(self.cut_image, self.scale)
+
+        # save cut_image to buffor and get avg from previous buffors
+        # self.eyeBuffer.add(self.cut_image)
+        # self.cut_image = np.array(self.eyeBuffer.getAvg(), dtype=np.uint8)
+
+        # LEGACY
+        # org_scale = (max_x - min_x,max_y - min_y)
+        # self.pupil = pupil.Pupil(self.cut_image, min_x, min_y, self.scale, org_scale)
```

### Comparing `eyegestures-2.0.0/eyeGestures/eyegestures.py` & `eyegestures-2.1.0/eyeGestures/eyegestures.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,523 +1,531 @@
-00000000: 0a66 726f 6d20 6579 6547 6573 7475 7265  .from eyeGesture
-00000010: 732e 6761 7a65 4573 7469 6d61 746f 7220  s.gazeEstimator 
-00000020: 696d 706f 7274 2047 617a 6554 7261 636b  import GazeTrack
-00000030: 6572 0a69 6d70 6f72 7420 6579 6547 6573  er.import eyeGes
-00000040: 7475 7265 732e 7363 7265 656e 5472 6163  tures.screenTrac
-00000050: 6b65 722e 6461 7461 506f 696e 7473 2061  ker.dataPoints a
-00000060: 7320 6470 0a66 726f 6d20 6579 6547 6573  s dp.from eyeGes
-00000070: 7475 7265 732e 6361 6c69 6272 6174 696f  tures.calibratio
-00000080: 6e5f 7631 2069 6d70 6f72 7420 4361 6c69  n_v1 import Cali
-00000090: 6272 6174 6f72 2061 7320 4361 6c69 6272  brator as Calibr
-000000a0: 6174 6f72 5f76 310a 6672 6f6d 2065 7965  ator_v1.from eye
-000000b0: 4765 7374 7572 6573 2e63 616c 6962 7261  Gestures.calibra
-000000c0: 7469 6f6e 5f76 3220 696d 706f 7274 2043  tion_v2 import C
-000000d0: 616c 6962 7261 746f 7220 6173 2043 616c  alibrator as Cal
-000000e0: 6962 7261 746f 725f 7632 2c20 6575 636c  ibrator_v2, eucl
-000000f0: 6964 6561 6e5f 6469 7374 616e 6365 0a66  idean_distance.f
-00000100: 726f 6d20 6579 6547 6573 7475 7265 732e  rom eyeGestures.
-00000110: 6765 7665 6e74 2069 6d70 6f72 7420 4765  gevent import Ge
-00000120: 7665 6e74 2c20 4365 7665 6e74 0a66 726f  vent, Cevent.fro
-00000130: 6d20 6579 6547 6573 7475 7265 732e 7574  m eyeGestures.ut
-00000140: 696c 7320 696d 706f 7274 2074 696d 6569  ils import timei
-00000150: 740a 696d 706f 7274 206e 756d 7079 2061  t.import numpy a
-00000160: 7320 6e70 0a69 6d70 6f72 7420 6376 320a  s np.import cv2.
-00000170: 0a69 6d70 6f72 7420 7261 6e64 6f6d 0a0a  .import random..
-00000180: 5645 5253 494f 4e20 3d20 2232 2e30 2e30  VERSION = "2.0.0
-00000190: 220a 0a63 6c61 7373 2045 7965 4765 7374  "..class EyeGest
-000001a0: 7572 6573 5f76 323a 0a20 2020 2022 2222  ures_v2:.    """
-000001b0: 4d61 696e 2063 6c61 7373 2066 6f72 2045  Main class for E
-000001c0: 7965 4765 7374 7572 6520 7472 6163 6b65  yeGesture tracke
-000001d0: 722e 2049 7420 636f 6e66 6967 7572 6573  r. It configures
-000001e0: 2061 6e64 206d 616e 6167 6573 2065 6e74   and manages ent
-000001f0: 6965 7220 616c 676f 7269 7468 6d22 2222  ier algorithm"""
-00000200: 0a0a 0a20 2020 2050 5245 4349 5349 4f4e  ...    PRECISION
-00000210: 5f4c 494d 4954 203d 2035 300a 2020 2020  _LIMIT = 50.    
-00000220: 5052 4543 4953 494f 4e5f 5354 4550 203d  PRECISION_STEP =
-00000230: 2031 300a 2020 2020 4143 4345 5054 414e   10.    ACCEPTAN
-00000240: 4345 5f52 4144 4955 5320 3d20 3530 300a  CE_RADIUS = 500.
-00000250: 2020 2020 4341 4c49 4252 4154 494f 4e5f      CALIBRATION_
-00000260: 5241 4449 5553 203d 2031 3030 300a 2020  RADIUS = 1000.  
-00000270: 2020 4559 4547 4553 5455 5245 535f 4341    EYEGESTURES_CA
-00000280: 4c49 4252 4154 494f 4e5f 5448 5245 5348  LIBRATION_THRESH
-00000290: 203d 2038 3530 0a0a 2020 2020 6465 6620   = 850..    def 
-000002a0: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0a  __init__(self):.
-000002b0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-000002c0: 6e69 746f 725f 7769 6474 6820 203d 2031  nitor_width  = 1
-000002d0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-000002e0: 6e69 746f 725f 6865 6967 6874 203d 2031  nitor_height = 1
-000002f0: 0a0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00000300: 6c62 203d 2043 616c 6962 7261 746f 725f  lb = Calibrator_
-00000310: 7632 2829 0a20 2020 2020 2020 2073 656c  v2().        sel
-00000320: 662e 6361 7020 3d20 4e6f 6e65 0a20 2020  f.cap = None.   
-00000330: 2020 2020 2073 656c 662e 6765 7374 7572       self.gestur
-00000340: 6573 203d 2045 7965 4765 7374 7572 6573  es = EyeGestures
-00000350: 5f76 3128 3238 352c 3131 352c 3430 2c31  _v1(285,115,40,1
-00000360: 3529 0a0a 2020 2020 2020 2020 7365 6c66  5)..        self
-00000370: 2e63 616c 6962 7261 7469 6f6e 203d 2046  .calibration = F
-00000380: 616c 7365 0a0a 2020 2020 2020 2020 7365  alse..        se
-00000390: 6c66 2e43 4e20 3d20 350a 0a20 2020 2020  lf.CN = 5..     
-000003a0: 2020 2073 656c 662e 7472 6163 6b65 7253     self.trackerS
-000003b0: 6967 6e61 6c20 3d20 4e6f 6e65 0a20 2020  ignal = None.   
-000003c0: 2020 2020 2073 656c 662e 6669 7453 6967       self.fitSig
-000003d0: 6e61 6c20 3d20 4e6f 6e65 0a0a 2020 2020  nal = None..    
-000003e0: 2020 2020 7365 6c66 2e61 7665 7261 6765      self.average
-000003f0: 5f70 6f69 6e74 7320 3d20 6e70 2e7a 6572  _points = np.zer
-00000400: 6f73 2828 3230 2c32 2929 0a20 2020 2020  os((20,2)).     
-00000410: 2020 2073 656c 662e 6669 6c6c 6564 5f70     self.filled_p
-00000420: 6f69 6e74 7320 3d20 300a 2020 2020 2020  oints = 0.      
-00000430: 2020 7365 6c66 2e63 616c 6962 7261 7465    self.calibrate
-00000440: 5f67 6573 7475 7265 7320 3d20 5472 7565  _gestures = True
-00000450: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-00000460: 745f 706f 696e 7420 3d20 7365 6c66 2e67  t_point = self.g
-00000470: 6574 4e65 7752 616e 646f 6d50 6f69 6e74  etNewRandomPoint
-00000480: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00000490: 2e6f 7574 7075 745f 706f 696e 7473 203d  .output_points =
-000004a0: 206e 702e 7a65 726f 7328 2835 2c32 2929   np.zeros((5,2))
-000004b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-000004c0: 7465 7261 746f 7220 3d20 300a 2020 2020  terator = 0.    
-000004d0: 2020 2020 7365 6c66 2e66 6978 203d 2030      self.fix = 0
-000004e0: 2e38 0a0a 2020 2020 2020 2020 7365 6c66  .8..        self
-000004f0: 2e70 7265 6369 7369 6f6e 5f6c 696d 6974  .precision_limit
-00000500: 203d 2073 656c 662e 5052 4543 4953 494f   = self.PRECISIO
-00000510: 4e5f 4c49 4d49 540a 2020 2020 2020 2020  N_LIMIT.        
-00000520: 7365 6c66 2e70 7265 6369 7369 6f6e 5f73  self.precision_s
-00000530: 7465 7020 3d20 7365 6c66 2e50 5245 4349  tep = self.PRECI
-00000540: 5349 4f4e 5f53 5445 500a 2020 2020 2020  SION_STEP.      
-00000550: 2020 7365 6c66 2e61 6363 6570 7461 6e63    self.acceptanc
-00000560: 655f 7261 6469 7573 203d 2073 656c 662e  e_radius = self.
-00000570: 4143 4345 5054 414e 4345 5f52 4144 4955  ACCEPTANCE_RADIU
-00000580: 530a 2020 2020 2020 2020 7365 6c66 2e63  S.        self.c
-00000590: 616c 6962 7261 7469 6f6e 5f72 6164 6975  alibration_radiu
-000005a0: 7320 3d20 7365 6c66 2e43 414c 4942 5241  s = self.CALIBRA
-000005b0: 5449 4f4e 5f52 4144 4955 530a 2020 2020  TION_RADIUS.    
-000005c0: 2020 2020 2320 6166 7465 7220 636f 7273      # after cors
-000005d0: 7369 6e67 2074 6869 7320 7468 7265 7368  sing this thresh
-000005e0: 2077 6520 6172 6520 6469 7361 626c 696e   we are disablin
-000005f0: 6720 636c 6173 7369 6361 6c20 6361 6c69  g classical cali
-00000600: 620a 2020 2020 2020 2020 7365 6c66 2e65  b.        self.e
-00000610: 7965 6765 7374 7572 6573 5f63 616c 6962  yegestures_calib
-00000620: 7261 7469 6f6e 5f74 6872 6573 686f 6c64  ration_threshold
-00000630: 203d 2073 656c 662e 4559 4547 4553 5455   = self.EYEGESTU
-00000640: 5245 535f 4341 4c49 4252 4154 494f 4e5f  RES_CALIBRATION_
-00000650: 5448 5245 5348 0a0a 2020 2020 6465 6620  THRESH..    def 
-00000660: 6765 744c 616e 646d 6172 6b73 2873 656c  getLandmarks(sel
-00000670: 662c 2066 7261 6d65 2c20 6361 6c69 6272  f, frame, calibr
-00000680: 6174 6520 3d20 4661 6c73 6529 3a0a 0a20  ate = False):.. 
-00000690: 2020 2020 2020 2066 7261 6d65 203d 2063         frame = c
-000006a0: 7632 2e63 7674 436f 6c6f 7228 6672 616d  v2.cvtColor(fram
-000006b0: 652c 2063 7632 2e43 4f4c 4f52 5f42 4752  e, cv2.COLOR_BGR
-000006c0: 3252 4742 290a 2020 2020 2020 2020 6672  2RGB).        fr
-000006d0: 616d 6520 3d20 6376 322e 666c 6970 2866  ame = cv2.flip(f
-000006e0: 7261 6d65 2c31 290a 2020 2020 2020 2020  rame,1).        
-000006f0: 2320 6672 616d 6520 3d20 6376 322e 7265  # frame = cv2.re
-00000700: 7369 7a65 2866 7261 6d65 2c20 2833 3630  size(frame, (360
-00000710: 2c20 3634 3029 290a 0a20 2020 2020 2020  , 640))..       
-00000720: 2065 7665 6e74 2c20 5f20 3d20 7365 6c66   event, _ = self
-00000730: 2e67 6573 7475 7265 732e 7374 6570 280a  .gestures.step(.
-00000740: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00000750: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
-00000760: 6d61 696e 222c 0a20 2020 2020 2020 2020  main",.         
-00000770: 2020 2063 616c 6962 7261 7465 2c20 2320     calibrate, # 
-00000780: 7365 7420 6361 6c69 6272 6174 696f 6e20  set calibration 
-00000790: 2d20 7377 6974 6368 2074 6f20 4661 6c73  - switch to Fals
-000007a0: 6520 746f 2073 746f 7020 6361 6c69 6272  e to stop calibr
-000007b0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-000007c0: 2020 7365 6c66 2e6d 6f6e 6974 6f72 5f77    self.monitor_w
-000007d0: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
-000007e0: 2020 7365 6c66 2e6d 6f6e 6974 6f72 5f68    self.monitor_h
-000007f0: 6569 6768 742c 0a20 2020 2020 2020 2020  eight,.         
-00000800: 2020 2030 2c20 302c 2073 656c 662e 6669     0, 0, self.fi
-00000810: 782c 2031 3030 290a 0a20 2020 2020 2020  x, 100)..       
-00000820: 2063 7572 736f 725f 782c 2063 7572 736f   cursor_x, curso
-00000830: 725f 7920 3d20 6576 656e 742e 706f 696e  r_y = event.poin
-00000840: 745b 305d 2c65 7665 6e74 2e70 6f69 6e74  t[0],event.point
-00000850: 5b31 5d0a 2020 2020 2020 2020 6c5f 6579  [1].        l_ey
-00000860: 655f 6c61 6e64 6d61 726b 7320 3d20 6576  e_landmarks = ev
-00000870: 656e 742e 6c5f 6579 652e 6765 744c 616e  ent.l_eye.getLan
-00000880: 646d 6172 6b73 2829 0a20 2020 2020 2020  dmarks().       
-00000890: 2072 5f65 7965 5f6c 616e 646d 6172 6b73   r_eye_landmarks
-000008a0: 203d 2065 7665 6e74 2e72 5f65 7965 2e67   = event.r_eye.g
-000008b0: 6574 4c61 6e64 6d61 726b 7328 290a 0a20  etLandmarks().. 
-000008c0: 2020 2020 2020 2063 7572 736f 7273 203d         cursors =
-000008d0: 206e 702e 6172 7261 7928 5b63 7572 736f   np.array([curso
-000008e0: 725f 782c 6375 7273 6f72 5f79 5d29 2e72  r_x,cursor_y]).r
-000008f0: 6573 6861 7065 2831 2c20 3229 0a20 2020  eshape(1, 2).   
-00000900: 2020 2020 2065 7965 5f65 7665 6e74 7320       eye_events 
-00000910: 3d20 6e70 2e61 7272 6179 285b 6576 656e  = np.array([even
-00000920: 742e 626c 696e 6b2c 6576 656e 742e 6669  t.blink,event.fi
-00000930: 7861 7469 6f6e 5d29 2e72 6573 6861 7065  xation]).reshape
-00000940: 2831 2c20 3229 0a20 2020 2020 2020 206b  (1, 2).        k
-00000950: 6579 5f70 6f69 6e74 7320 3d20 6e70 2e63  ey_points = np.c
-00000960: 6f6e 6361 7465 6e61 7465 2828 6375 7273  oncatenate((curs
-00000970: 6f72 732c 6c5f 6579 655f 6c61 6e64 6d61  ors,l_eye_landma
-00000980: 726b 732c 725f 6579 655f 6c61 6e64 6d61  rks,r_eye_landma
-00000990: 726b 732c 6579 655f 6576 656e 7473 2929  rks,eye_events))
-000009a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000009b0: 206e 702e 6172 7261 7928 2863 7572 736f   np.array((curso
-000009c0: 725f 782c 2063 7572 736f 725f 7929 292c  r_x, cursor_y)),
-000009d0: 206b 6579 5f70 6f69 6e74 732c 2065 7665   key_points, eve
-000009e0: 6e74 2e62 6c69 6e6b 2c20 6576 656e 742e  nt.blink, event.
-000009f0: 6669 7861 7469 6f6e 0a0a 2020 2020 6465  fixation..    de
-00000a00: 6620 696e 6372 6561 7365 5f70 7265 6369  f increase_preci
-00000a10: 7369 6f6e 2873 656c 6629 3a0a 2020 2020  sion(self):.    
-00000a20: 2020 2020 6966 2073 656c 662e 6163 6365      if self.acce
-00000a30: 7074 616e 6365 5f72 6164 6975 7320 3e20  ptance_radius > 
-00000a40: 7365 6c66 2e70 7265 6369 7369 6f6e 5f6c  self.precision_l
-00000a50: 696d 6974 3a0a 2020 2020 2020 2020 2020  imit:.          
-00000a60: 2020 7365 6c66 2e61 6363 6570 7461 6e63    self.acceptanc
-00000a70: 655f 7261 6469 7573 202d 3d20 7365 6c66  e_radius -= self
-00000a80: 2e70 7265 6369 7369 6f6e 5f73 7465 700a  .precision_step.
-00000a90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000aa0: 6361 6c69 6272 6174 696f 6e5f 7261 6469  calibration_radi
-00000ab0: 7573 203e 2073 656c 662e 7072 6563 6973  us > self.precis
-00000ac0: 696f 6e5f 6c69 6d69 7420 616e 6420 7365  ion_limit and se
-00000ad0: 6c66 2e61 6363 6570 7461 6e63 655f 7261  lf.acceptance_ra
-00000ae0: 6469 7573 203c 2073 656c 662e 6361 6c69  dius < self.cali
-00000af0: 6272 6174 696f 6e5f 7261 6469 7573 3a0a  bration_radius:.
-00000b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000b10: 2e63 616c 6962 7261 7469 6f6e 5f72 6164  .calibration_rad
-00000b20: 6975 7320 2d3d 2073 656c 662e 7072 6563  ius -= self.prec
-00000b30: 6973 696f 6e5f 7374 6570 0a0a 2020 2020  ision_step..    
-00000b40: 6465 6620 7365 7443 6c61 7373 6963 496d  def setClassicIm
-00000b50: 7061 6374 2873 656c 662c 696d 7061 6374  pact(self,impact
-00000b60: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000b70: 434e 203d 2069 6d70 6163 740a 0a20 2020  CN = impact..   
-00000b80: 2064 6566 2067 6574 4e65 7752 616e 646f   def getNewRando
-00000b90: 6d50 6f69 6e74 2873 656c 6629 3a0a 2020  mPoint(self):.  
-00000ba0: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
-00000bb0: 6172 7261 7928 5b72 616e 646f 6d2e 7261  array([random.ra
-00000bc0: 6e64 6f6d 2829 202a 2073 656c 662e 6d6f  ndom() * self.mo
-00000bd0: 6e69 746f 725f 7769 6474 682c 7261 6e64  nitor_width,rand
-00000be0: 6f6d 2e72 616e 646f 6d28 2920 2a20 7365  om.random() * se
-00000bf0: 6c66 2e6d 6f6e 6974 6f72 5f68 6569 6768  lf.monitor_heigh
-00000c00: 745d 290a 0a20 2020 2064 6566 2072 6573  t])..    def res
-00000c10: 6574 2873 656c 6629 3a0a 2020 2020 2020  et(self):.      
-00000c20: 2020 7365 6c66 2e61 6363 6570 7461 6e63    self.acceptanc
-00000c30: 655f 7261 6469 7573 203d 2073 656c 662e  e_radius = self.
-00000c40: 4143 4345 5054 414e 4345 5f52 4144 4955  ACCEPTANCE_RADIU
-00000c50: 530a 2020 2020 2020 2020 7365 6c66 2e63  S.        self.c
-00000c60: 616c 6962 7261 7469 6f6e 5f72 6164 6975  alibration_radiu
-00000c70: 7320 3d20 7365 6c66 2e43 414c 4942 5241  s = self.CALIBRA
-00000c80: 5449 4f4e 5f52 4144 4955 530a 2020 2020  TION_RADIUS.    
-00000c90: 2020 2020 7365 6c66 2e61 7665 7261 6765      self.average
-00000ca0: 5f70 6f69 6e74 7320 3d20 6e70 2e7a 6572  _points = np.zer
-00000cb0: 6f73 2828 3230 2c32 2929 0a20 2020 2020  os((20,2)).     
-00000cc0: 2020 2073 656c 662e 6669 6c6c 6564 5f70     self.filled_p
-00000cd0: 6f69 6e74 7320 3d20 300a 2020 2020 2020  oints = 0.      
-00000ce0: 2020 7365 6c66 2e63 6c62 2e75 6e66 6974    self.clb.unfit
-00000cf0: 2829 0a0a 2020 2020 6465 6620 7365 7446  ()..    def setF
-00000d00: 6978 6174 696f 6e28 7365 6c66 2c66 6978  ixation(self,fix
-00000d10: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000d20: 6669 7820 3d20 6669 780a 0a20 2020 2064  fix = fix..    d
-00000d30: 6566 2073 6574 436c 6173 7369 6361 6c49  ef setClassicalI
-00000d40: 6d70 6163 7428 7365 6c66 2c43 4e29 3a0a  mpact(self,CN):.
-00000d50: 2020 2020 2020 2020 7365 6c66 2e43 4e20          self.CN 
-00000d60: 3d20 434e 0a0a 2020 2020 6465 6620 7374  = CN..    def st
-00000d70: 6570 2873 656c 662c 2066 7261 6d65 2c20  ep(self, frame, 
-00000d80: 6361 6c69 6272 6174 696f 6e2c 2077 6964  calibration, wid
-00000d90: 7468 2c20 6865 6967 6874 293a 0a20 2020  th, height):.   
-00000da0: 2020 2020 2073 656c 662e 6361 6c69 6272       self.calibr
-00000db0: 6174 696f 6e20 3d20 6361 6c69 6272 6174  ation = calibrat
-00000dc0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+00000000: 0d0a 6672 6f6d 2065 7965 4765 7374 7572  ..from eyeGestur
+00000010: 6573 2e67 617a 6545 7374 696d 6174 6f72  es.gazeEstimator
+00000020: 2069 6d70 6f72 7420 4761 7a65 5472 6163   import GazeTrac
+00000030: 6b65 720d 0a69 6d70 6f72 7420 6579 6547  ker..import eyeG
+00000040: 6573 7475 7265 732e 7363 7265 656e 5472  estures.screenTr
+00000050: 6163 6b65 722e 6461 7461 506f 696e 7473  acker.dataPoints
+00000060: 2061 7320 6470 0d0a 6672 6f6d 2065 7965   as dp..from eye
+00000070: 4765 7374 7572 6573 2e63 616c 6962 7261  Gestures.calibra
+00000080: 7469 6f6e 5f76 3120 696d 706f 7274 2043  tion_v1 import C
+00000090: 616c 6962 7261 746f 7220 6173 2043 616c  alibrator as Cal
+000000a0: 6962 7261 746f 725f 7631 0d0a 6672 6f6d  ibrator_v1..from
+000000b0: 2065 7965 4765 7374 7572 6573 2e63 616c   eyeGestures.cal
+000000c0: 6962 7261 7469 6f6e 5f76 3220 696d 706f  ibration_v2 impo
+000000d0: 7274 2043 616c 6962 7261 746f 7220 6173  rt Calibrator as
+000000e0: 2043 616c 6962 7261 746f 725f 7632 2c20   Calibrator_v2, 
+000000f0: 4361 6c69 6272 6174 696f 6e4d 6174 7269  CalibrationMatri
+00000100: 782c 2065 7563 6c69 6465 616e 5f64 6973  x, euclidean_dis
+00000110: 7461 6e63 650d 0a66 726f 6d20 6579 6547  tance..from eyeG
+00000120: 6573 7475 7265 732e 6765 7665 6e74 2069  estures.gevent i
+00000130: 6d70 6f72 7420 4765 7665 6e74 2c20 4365  mport Gevent, Ce
+00000140: 7665 6e74 0d0a 6672 6f6d 2065 7965 4765  vent..from eyeGe
+00000150: 7374 7572 6573 2e75 7469 6c73 2069 6d70  stures.utils imp
+00000160: 6f72 7420 7469 6d65 6974 0d0a 696d 706f  ort timeit..impo
+00000170: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
+00000180: 696d 706f 7274 2063 7632 0d0a 0d0a 696d  import cv2....im
+00000190: 706f 7274 2072 616e 646f 6d0d 0a0d 0a56  port random....V
+000001a0: 4552 5349 4f4e 203d 2022 322e 302e 3022  ERSION = "2.0.0"
+000001b0: 0d0a 0d0a 636c 6173 7320 4579 6547 6573  ....class EyeGes
+000001c0: 7475 7265 735f 7632 3a0d 0a20 2020 2022  tures_v2:..    "
+000001d0: 2222 4d61 696e 2063 6c61 7373 2066 6f72  ""Main class for
+000001e0: 2045 7965 4765 7374 7572 6520 7472 6163   EyeGesture trac
+000001f0: 6b65 722e 2049 7420 636f 6e66 6967 7572  ker. It configur
+00000200: 6573 2061 6e64 206d 616e 6167 6573 2065  es and manages e
+00000210: 6e74 6972 6520 616c 676f 7269 7468 6d22  ntire algorithm"
+00000220: 2222 0d0a 0d0a 0d0a 2020 2020 5052 4543  ""......    PREC
+00000230: 4953 494f 4e5f 4c49 4d49 5420 3d20 3530  ISION_LIMIT = 50
+00000240: 0d0a 2020 2020 5052 4543 4953 494f 4e5f  ..    PRECISION_
+00000250: 5354 4550 203d 2031 300d 0a20 2020 2041  STEP = 10..    A
+00000260: 4343 4550 5441 4e43 455f 5241 4449 5553  CCEPTANCE_RADIUS
+00000270: 203d 2035 3030 0d0a 2020 2020 4341 4c49   = 500..    CALI
+00000280: 4252 4154 494f 4e5f 5241 4449 5553 203d  BRATION_RADIUS =
+00000290: 2031 3030 300d 0a20 2020 2045 5945 4745   1000..    EYEGE
+000002a0: 5354 5552 4553 5f43 414c 4942 5241 5449  STURES_CALIBRATI
+000002b0: 4f4e 5f54 4852 4553 4820 3d20 3835 300d  ON_THRESH = 850.
+000002c0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+000002d0: 745f 5f28 7365 6c66 293a 0d0a 0d0a 2020  t__(self):....  
+000002e0: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
+000002f0: 6f72 5f77 6964 7468 2020 3d20 310d 0a20  or_width  = 1.. 
+00000300: 2020 2020 2020 2073 656c 662e 6d6f 6e69         self.moni
+00000310: 746f 725f 6865 6967 6874 203d 2031 0d0a  tor_height = 1..
+00000320: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000330: 6c62 203d 2043 616c 6962 7261 746f 725f  lb = Calibrator_
+00000340: 7632 2829 0d0a 2020 2020 2020 2020 7365  v2()..        se
+00000350: 6c66 2e63 6170 203d 204e 6f6e 650d 0a20  lf.cap = None.. 
+00000360: 2020 2020 2020 2073 656c 662e 6765 7374         self.gest
+00000370: 7572 6573 203d 2045 7965 4765 7374 7572  ures = EyeGestur
+00000380: 6573 5f76 3128 3238 352c 3131 352c 3430  es_v1(285,115,40
+00000390: 2c31 3529 0d0a 0d0a 2020 2020 2020 2020  ,15)....        
+000003a0: 7365 6c66 2e63 616c 6962 7261 7469 6f6e  self.calibration
+000003b0: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
+000003c0: 2020 2020 7365 6c66 2e43 4e20 3d20 350d      self.CN = 5.
+000003d0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+000003e0: 7472 6163 6b65 7253 6967 6e61 6c20 3d20  trackerSignal = 
+000003f0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+00000400: 6c66 2e66 6974 5369 676e 616c 203d 204e  lf.fitSignal = N
+00000410: 6f6e 650d 0a0d 0a20 2020 2020 2020 2073  one....        s
+00000420: 656c 662e 6176 6572 6167 655f 706f 696e  elf.average_poin
+00000430: 7473 203d 206e 702e 7a65 726f 7328 2832  ts = np.zeros((2
+00000440: 302c 3229 290d 0a20 2020 2020 2020 2073  0,2))..        s
+00000450: 656c 662e 6669 6c6c 6564 5f70 6f69 6e74  elf.filled_point
+00000460: 7320 3d20 300d 0a20 2020 2020 2020 2073  s = 0..        s
+00000470: 656c 662e 6361 6c69 6272 6174 655f 6765  elf.calibrate_ge
+00000480: 7374 7572 6573 203d 2054 7275 650d 0a20  stures = True.. 
+00000490: 2020 2020 2020 2073 656c 662e 6361 6c69         self.cali
+000004a0: 6272 6174 696f 6e4d 6174 203d 2043 616c  brationMat = Cal
+000004b0: 6962 7261 7469 6f6e 4d61 7472 6978 2829  ibrationMatrix()
+000004c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
+000004d0: 6974 5f70 6f69 6e74 203d 2073 656c 662e  it_point = self.
+000004e0: 6361 6c69 6272 6174 696f 6e4d 6174 2e67  calibrationMat.g
+000004f0: 6574 4e65 7874 506f 696e 7428 290d 0a0d  etNextPoint()...
+00000500: 0a20 2020 2020 2020 2073 656c 662e 6974  .        self.it
+00000510: 6572 6174 6f72 203d 2030 0d0a 2020 2020  erator = 0..    
+00000520: 2020 2020 7365 6c66 2e66 6978 203d 2030      self.fix = 0
+00000530: 2e38 0d0a 0d0a 2020 2020 2020 2020 7365  .8....        se
+00000540: 6c66 2e70 7265 6369 7369 6f6e 5f6c 696d  lf.precision_lim
+00000550: 6974 203d 2073 656c 662e 5052 4543 4953  it = self.PRECIS
+00000560: 494f 4e5f 4c49 4d49 540d 0a20 2020 2020  ION_LIMIT..     
+00000570: 2020 2073 656c 662e 7072 6563 6973 696f     self.precisio
+00000580: 6e5f 7374 6570 203d 2073 656c 662e 5052  n_step = self.PR
+00000590: 4543 4953 494f 4e5f 5354 4550 0d0a 2020  ECISION_STEP..  
+000005a0: 2020 2020 2020 7365 6c66 2e61 6363 6570        self.accep
+000005b0: 7461 6e63 655f 7261 6469 7573 203d 2073  tance_radius = s
+000005c0: 656c 662e 4143 4345 5054 414e 4345 5f52  elf.ACCEPTANCE_R
+000005d0: 4144 4955 530d 0a20 2020 2020 2020 2073  ADIUS..        s
+000005e0: 656c 662e 6361 6c69 6272 6174 696f 6e5f  elf.calibration_
+000005f0: 7261 6469 7573 203d 2073 656c 662e 4341  radius = self.CA
+00000600: 4c49 4252 4154 494f 4e5f 5241 4449 5553  LIBRATION_RADIUS
+00000610: 0d0a 2020 2020 2020 2020 2320 6166 7465  ..        # afte
+00000620: 7220 636f 7273 7369 6e67 2074 6869 7320  r corssing this 
+00000630: 7468 7265 7368 2077 6520 6172 6520 6469  thresh we are di
+00000640: 7361 626c 696e 6720 636c 6173 7369 6361  sabling classica
+00000650: 6c20 6361 6c69 620d 0a20 2020 2020 2020  l calib..       
+00000660: 2073 656c 662e 6579 6567 6573 7475 7265   self.eyegesture
+00000670: 735f 6361 6c69 6272 6174 696f 6e5f 7468  s_calibration_th
+00000680: 7265 7368 6f6c 6420 3d20 7365 6c66 2e45  reshold = self.E
+00000690: 5945 4745 5354 5552 4553 5f43 414c 4942  YEGESTURES_CALIB
+000006a0: 5241 5449 4f4e 5f54 4852 4553 480d 0a0d  RATION_THRESH...
+000006b0: 0a20 2020 2064 6566 2067 6574 4c61 6e64  .    def getLand
+000006c0: 6d61 726b 7328 7365 6c66 2c20 6672 616d  marks(self, fram
+000006d0: 652c 2063 616c 6962 7261 7465 203d 2046  e, calibrate = F
+000006e0: 616c 7365 293a 0d0a 0d0a 2020 2020 2020  alse):....      
+000006f0: 2020 6672 616d 6520 3d20 6376 322e 6376    frame = cv2.cv
+00000700: 7443 6f6c 6f72 2866 7261 6d65 2c20 6376  tColor(frame, cv
+00000710: 322e 434f 4c4f 525f 4247 5232 5247 4229  2.COLOR_BGR2RGB)
+00000720: 0d0a 2020 2020 2020 2020 6672 616d 6520  ..        frame 
+00000730: 3d20 6376 322e 666c 6970 2866 7261 6d65  = cv2.flip(frame
+00000740: 2c31 290d 0a20 2020 2020 2020 2023 2066  ,1)..        # f
+00000750: 7261 6d65 203d 2063 7632 2e72 6573 697a  rame = cv2.resiz
+00000760: 6528 6672 616d 652c 2028 3336 302c 2036  e(frame, (360, 6
+00000770: 3430 2929 0d0a 0d0a 2020 2020 2020 2020  40))....        
+00000780: 6576 656e 742c 205f 203d 2073 656c 662e  event, _ = self.
+00000790: 6765 7374 7572 6573 2e73 7465 7028 0d0a  gestures.step(..
+000007a0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000007b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000007c0: 226d 6169 6e22 2c0d 0a20 2020 2020 2020  "main",..       
+000007d0: 2020 2020 2063 616c 6962 7261 7465 2c20       calibrate, 
+000007e0: 2320 7365 7420 6361 6c69 6272 6174 696f  # set calibratio
+000007f0: 6e20 2d20 7377 6974 6368 2074 6f20 4661  n - switch to Fa
+00000800: 6c73 6520 746f 2073 746f 7020 6361 6c69  lse to stop cali
+00000810: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00000820: 2020 2020 2073 656c 662e 6d6f 6e69 746f       self.monito
+00000830: 725f 7769 6474 682c 0d0a 2020 2020 2020  r_width,..      
+00000840: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
+00000850: 6f72 5f68 6569 6768 742c 0d0a 2020 2020  or_height,..    
+00000860: 2020 2020 2020 2020 302c 2030 2c20 7365          0, 0, se
+00000870: 6c66 2e66 6978 2c20 3130 3029 0d0a 0d0a  lf.fix, 100)....
+00000880: 2020 2020 2020 2020 6375 7273 6f72 5f78          cursor_x
+00000890: 2c20 6375 7273 6f72 5f79 203d 2065 7665  , cursor_y = eve
+000008a0: 6e74 2e70 6f69 6e74 5b30 5d2c 6576 656e  nt.point[0],even
+000008b0: 742e 706f 696e 745b 315d 0d0a 2020 2020  t.point[1]..    
+000008c0: 2020 2020 6c5f 6579 655f 6c61 6e64 6d61      l_eye_landma
+000008d0: 726b 7320 3d20 6576 656e 742e 6c5f 6579  rks = event.l_ey
+000008e0: 652e 6765 744c 616e 646d 6172 6b73 2829  e.getLandmarks()
+000008f0: 0d0a 2020 2020 2020 2020 725f 6579 655f  ..        r_eye_
+00000900: 6c61 6e64 6d61 726b 7320 3d20 6576 656e  landmarks = even
+00000910: 742e 725f 6579 652e 6765 744c 616e 646d  t.r_eye.getLandm
+00000920: 6172 6b73 2829 0d0a 0d0a 2020 2020 2020  arks()....      
+00000930: 2020 6375 7273 6f72 7320 3d20 6e70 2e61    cursors = np.a
+00000940: 7272 6179 285b 6375 7273 6f72 5f78 2c63  rray([cursor_x,c
+00000950: 7572 736f 725f 795d 292e 7265 7368 6170  ursor_y]).reshap
+00000960: 6528 312c 2032 290d 0a20 2020 2020 2020  e(1, 2)..       
+00000970: 2065 7965 5f65 7665 6e74 7320 3d20 6e70   eye_events = np
+00000980: 2e61 7272 6179 285b 6576 656e 742e 626c  .array([event.bl
+00000990: 696e 6b2c 6576 656e 742e 6669 7861 7469  ink,event.fixati
+000009a0: 6f6e 5d29 2e72 6573 6861 7065 2831 2c20  on]).reshape(1, 
+000009b0: 3229 0d0a 2020 2020 2020 2020 6b65 795f  2)..        key_
+000009c0: 706f 696e 7473 203d 206e 702e 636f 6e63  points = np.conc
+000009d0: 6174 656e 6174 6528 2863 7572 736f 7273  atenate((cursors
+000009e0: 2c6c 5f65 7965 5f6c 616e 646d 6172 6b73  ,l_eye_landmarks
+000009f0: 2c72 5f65 7965 5f6c 616e 646d 6172 6b73  ,r_eye_landmarks
+00000a00: 2c65 7965 5f65 7665 6e74 7329 290d 0a20  ,eye_events)).. 
+00000a10: 2020 2020 2020 2072 6574 7572 6e20 206e         return  n
+00000a20: 702e 6172 7261 7928 2863 7572 736f 725f  p.array((cursor_
+00000a30: 782c 2063 7572 736f 725f 7929 292c 206b  x, cursor_y)), k
+00000a40: 6579 5f70 6f69 6e74 732c 2065 7665 6e74  ey_points, event
+00000a50: 2e62 6c69 6e6b 2c20 6576 656e 742e 6669  .blink, event.fi
+00000a60: 7861 7469 6f6e 0d0a 0d0a 2020 2020 6465  xation....    de
+00000a70: 6620 696e 6372 6561 7365 5f70 7265 6369  f increase_preci
+00000a80: 7369 6f6e 2873 656c 6629 3a0d 0a20 2020  sion(self):..   
+00000a90: 2020 2020 2069 6620 7365 6c66 2e61 6363       if self.acc
+00000aa0: 6570 7461 6e63 655f 7261 6469 7573 203e  eptance_radius >
+00000ab0: 2073 656c 662e 7072 6563 6973 696f 6e5f   self.precision_
+00000ac0: 6c69 6d69 743a 0d0a 2020 2020 2020 2020  limit:..        
+00000ad0: 2020 2020 7365 6c66 2e61 6363 6570 7461      self.accepta
+00000ae0: 6e63 655f 7261 6469 7573 202d 3d20 7365  nce_radius -= se
+00000af0: 6c66 2e70 7265 6369 7369 6f6e 5f73 7465  lf.precision_ste
+00000b00: 700d 0a20 2020 2020 2020 2069 6620 7365  p..        if se
+00000b10: 6c66 2e63 616c 6962 7261 7469 6f6e 5f72  lf.calibration_r
+00000b20: 6164 6975 7320 3e20 7365 6c66 2e70 7265  adius > self.pre
+00000b30: 6369 7369 6f6e 5f6c 696d 6974 2061 6e64  cision_limit and
+00000b40: 2073 656c 662e 6163 6365 7074 616e 6365   self.acceptance
+00000b50: 5f72 6164 6975 7320 3c20 7365 6c66 2e63  _radius < self.c
+00000b60: 616c 6962 7261 7469 6f6e 5f72 6164 6975  alibration_radiu
+00000b70: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000b80: 7365 6c66 2e63 616c 6962 7261 7469 6f6e  self.calibration
+00000b90: 5f72 6164 6975 7320 2d3d 2073 656c 662e  _radius -= self.
+00000ba0: 7072 6563 6973 696f 6e5f 7374 6570 0d0a  precision_step..
+00000bb0: 0d0a 2020 2020 6465 6620 7365 7443 6c61  ..    def setCla
+00000bc0: 7373 6963 496d 7061 6374 2873 656c 662c  ssicImpact(self,
+00000bd0: 696d 7061 6374 293a 0d0a 2020 2020 2020  impact):..      
+00000be0: 2020 7365 6c66 2e43 4e20 3d20 696d 7061    self.CN = impa
+00000bf0: 6374 0d0a 0d0a 2020 2020 6465 6620 7265  ct....    def re
+00000c00: 7365 7428 7365 6c66 293a 0d0a 2020 2020  set(self):..    
+00000c10: 2020 2020 7365 6c66 2e61 6363 6570 7461      self.accepta
+00000c20: 6e63 655f 7261 6469 7573 203d 2073 656c  nce_radius = sel
+00000c30: 662e 4143 4345 5054 414e 4345 5f52 4144  f.ACCEPTANCE_RAD
+00000c40: 4955 530d 0a20 2020 2020 2020 2073 656c  IUS..        sel
+00000c50: 662e 6361 6c69 6272 6174 696f 6e5f 7261  f.calibration_ra
+00000c60: 6469 7573 203d 2073 656c 662e 4341 4c49  dius = self.CALI
+00000c70: 4252 4154 494f 4e5f 5241 4449 5553 0d0a  BRATION_RADIUS..
+00000c80: 2020 2020 2020 2020 7365 6c66 2e61 7665          self.ave
+00000c90: 7261 6765 5f70 6f69 6e74 7320 3d20 6e70  rage_points = np
+00000ca0: 2e7a 6572 6f73 2828 3230 2c32 2929 0d0a  .zeros((20,2))..
+00000cb0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00000cc0: 6c65 645f 706f 696e 7473 203d 2030 0d0a  led_points = 0..
+00000cd0: 2020 2020 2020 2020 7365 6c66 2e63 6c62          self.clb
+00000ce0: 2e75 6e66 6974 2829 0d0a 0d0a 2020 2020  .unfit()....    
+00000cf0: 6465 6620 7365 7446 6978 6174 696f 6e28  def setFixation(
+00000d00: 7365 6c66 2c66 6978 293a 0d0a 2020 2020  self,fix):..    
+00000d10: 2020 2020 7365 6c66 2e66 6978 203d 2066      self.fix = f
+00000d20: 6978 0d0a 0d0a 2020 2020 6465 6620 7365  ix....    def se
+00000d30: 7443 6c61 7373 6963 616c 496d 7061 6374  tClassicalImpact
+00000d40: 2873 656c 662c 434e 293a 0d0a 2020 2020  (self,CN):..    
+00000d50: 2020 2020 7365 6c66 2e43 4e20 3d20 434e      self.CN = CN
+00000d60: 0d0a 0d0a 2020 2020 6465 6620 7374 6570  ....    def step
+00000d70: 2873 656c 662c 2066 7261 6d65 2c20 6361  (self, frame, ca
+00000d80: 6c69 6272 6174 696f 6e2c 2077 6964 7468  libration, width
+00000d90: 2c20 6865 6967 6874 293a 0d0a 2020 2020  , height):..    
+00000da0: 2020 2020 7365 6c66 2e63 616c 6962 7261      self.calibra
+00000db0: 7469 6f6e 203d 2063 616c 6962 7261 7469  tion = calibrati
+00000dc0: 6f6e 0d0a 2020 2020 2020 2020 7365 6c66  on..        self
 00000dd0: 2e6d 6f6e 6974 6f72 5f77 6964 7468 203d  .monitor_width =
-00000de0: 2077 6964 7468 0a20 2020 2020 2020 2073   width.        s
-00000df0: 656c 662e 6d6f 6e69 746f 725f 6865 6967  elf.monitor_heig
-00000e00: 6874 203d 2068 6569 6768 740a 0a20 2020  ht = height..   
-00000e10: 2020 2020 2063 6c61 7373 6963 5f70 6f69       classic_poi
-00000e20: 6e74 2c20 6b65 795f 706f 696e 7473 2c20  nt, key_points, 
-00000e30: 626c 696e 6b2c 2066 6978 6174 696f 6e20  blink, fixation 
-00000e40: 3d20 7365 6c66 2e67 6574 4c61 6e64 6d61  = self.getLandma
-00000e50: 726b 7328 6672 616d 652c 7365 6c66 2e63  rks(frame,self.c
-00000e60: 616c 6962 7261 7465 5f67 6573 7475 7265  alibrate_gesture
-00000e70: 7329 0a0a 2020 2020 2020 2020 6d61 7267  s)..        marg
-00000e80: 696e 203d 2031 300a 2020 2020 2020 2020  in = 10.        
-00000e90: 6966 2063 6c61 7373 6963 5f70 6f69 6e74  if classic_point
-00000ea0: 5b30 5d20 3c3d 206d 6172 6769 6e20 616e  [0] <= margin an
-00000eb0: 6420 7365 6c66 2e63 616c 6962 7261 7469  d self.calibrati
-00000ec0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00000ed0: 7365 6c66 2e63 616c 6962 7261 7465 5f67  self.calibrate_g
-00000ee0: 6573 7475 7265 7320 3d20 5472 7565 0a20  estures = True. 
-00000ef0: 2020 2020 2020 2065 6c69 6620 636c 6173         elif clas
-00000f00: 7369 635f 706f 696e 745b 305d 203e 3d20  sic_point[0] >= 
-00000f10: 7769 6474 6820 2d20 6d61 7267 696e 2061  width - margin a
-00000f20: 6e64 2073 656c 662e 6361 6c69 6272 6174  nd self.calibrat
-00000f30: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00000f40: 2073 656c 662e 6361 6c69 6272 6174 655f   self.calibrate_
-00000f50: 6765 7374 7572 6573 203d 2054 7275 650a  gestures = True.
-00000f60: 2020 2020 2020 2020 656c 6966 2063 6c61          elif cla
-00000f70: 7373 6963 5f70 6f69 6e74 5b31 5d20 3c3d  ssic_point[1] <=
-00000f80: 206d 6172 6769 6e20 616e 6420 7365 6c66   margin and self
-00000f90: 2e63 616c 6962 7261 7469 6f6e 3a0a 2020  .calibration:.  
-00000fa0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00000fb0: 616c 6962 7261 7465 5f67 6573 7475 7265  alibrate_gesture
-00000fc0: 7320 3d20 5472 7565 0a20 2020 2020 2020  s = True.       
-00000fd0: 2065 6c69 6620 636c 6173 7369 635f 706f   elif classic_po
-00000fe0: 696e 745b 315d 203e 3d20 6865 6967 6874  int[1] >= height
-00000ff0: 202d 206d 6172 6769 6e20 616e 6420 7365   - margin and se
-00001000: 6c66 2e63 616c 6962 7261 7469 6f6e 3a0a  lf.calibration:.
-00001010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001020: 2e63 616c 6962 7261 7465 5f67 6573 7475  .calibrate_gestu
-00001030: 7265 7320 3d20 5472 7565 0a20 2020 2020  res = True.     
-00001040: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00001050: 2020 2020 2073 656c 662e 6361 6c69 6272       self.calibr
-00001060: 6174 655f 6765 7374 7572 6573 203d 2046  ate_gestures = F
-00001070: 616c 7365 0a0a 2020 2020 2020 2020 795f  alse..        y_
-00001080: 706f 696e 7420 3d20 7365 6c66 2e63 6c62  point = self.clb
-00001090: 2e70 7265 6469 6374 286b 6579 5f70 6f69  .predict(key_poi
-000010a0: 6e74 7329 0a20 2020 2020 2020 2073 656c  nts).        sel
-000010b0: 662e 6176 6572 6167 655f 706f 696e 7473  f.average_points
-000010c0: 5b31 3a2c 3a5d 203d 2073 656c 662e 6176  [1:,:] = self.av
-000010d0: 6572 6167 655f 706f 696e 7473 5b3a 2873  erage_points[:(s
-000010e0: 656c 662e 6176 6572 6167 655f 706f 696e  elf.average_poin
-000010f0: 7473 2e73 6861 7065 5b30 5d20 2d20 3129  ts.shape[0] - 1)
-00001100: 2c3a 5d0a 2020 2020 2020 2020 6966 2066  ,:].        if f
-00001110: 6978 6174 696f 6e20 3c3d 2073 656c 662e  ixation <= self.
-00001120: 6669 783a 0a20 2020 2020 2020 2020 2020  fix:.           
-00001130: 2073 656c 662e 6176 6572 6167 655f 706f   self.average_po
-00001140: 696e 7473 5b30 2c3a 5d20 3d20 795f 706f  ints[0,:] = y_po
-00001150: 696e 740a 0a20 2020 2020 2020 2069 6620  int..        if 
-00001160: 7365 6c66 2e66 696c 6c65 645f 706f 696e  self.filled_poin
-00001170: 7473 203c 2073 656c 662e 6176 6572 6167  ts < self.averag
-00001180: 655f 706f 696e 7473 2e73 6861 7065 5b30  e_points.shape[0
-00001190: 5d20 616e 6420 2879 5f70 6f69 6e74 2021  ] and (y_point !
-000011a0: 3d20 6e70 2e61 7272 6179 285b 302e 302c  = np.array([0.0,
-000011b0: 302e 305d 2929 2e61 6e79 2829 3a0a 2020  0.0])).any():.  
-000011c0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-000011d0: 696c 6c65 645f 706f 696e 7473 202b 3d20  illed_points += 
-000011e0: 310a 0a20 2020 2020 2020 2061 7665 7261  1..        avera
-000011f0: 6765 645f 706f 696e 7420 3d20 286e 702e  ged_point = (np.
-00001200: 7375 6d28 7365 6c66 2e61 7665 7261 6765  sum(self.average
-00001210: 5f70 6f69 6e74 735b 3a2c 3a5d 2c61 7869  _points[:,:],axi
-00001220: 733d 3029 202b 2028 636c 6173 7369 635f  s=0) + (classic_
-00001230: 706f 696e 7420 2a20 7365 6c66 2e43 4e29  point * self.CN)
-00001240: 292f 2873 656c 662e 6669 6c6c 6564 5f70  )/(self.filled_p
-00001250: 6f69 6e74 7320 2b20 7365 6c66 2e43 4e29  oints + self.CN)
-00001260: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001270: 662e 6361 6c69 6272 6174 696f 6e20 616e  f.calibration an
-00001280: 6420 2865 7563 6c69 6465 616e 5f64 6973  d (euclidean_dis
-00001290: 7461 6e63 6528 6176 6572 6167 6564 5f70  tance(averaged_p
-000012a0: 6f69 6e74 2c73 656c 662e 6669 745f 706f  oint,self.fit_po
-000012b0: 696e 7429 203c 2073 656c 662e 6361 6c69  int) < self.cali
-000012c0: 6272 6174 696f 6e5f 7261 6469 7573 206f  bration_radius o
-000012d0: 7220 7365 6c66 2e66 696c 6c65 645f 706f  r self.filled_po
-000012e0: 696e 7473 203c 2073 656c 662e 6176 6572  ints < self.aver
-000012f0: 6167 655f 706f 696e 7473 2e73 6861 7065  age_points.shape
-00001300: 5b30 5d20 2a20 3130 293a 0a20 2020 2020  [0] * 10):.     
-00001310: 2020 2020 2020 2073 656c 662e 636c 622e         self.clb.
-00001320: 6164 6428 6b65 795f 706f 696e 7473 2c73  add(key_points,s
-00001330: 656c 662e 6669 745f 706f 696e 742c 636c  elf.fit_point,cl
-00001340: 6173 7369 635f 706f 696e 742c 795f 706f  assic_point,y_po
-00001350: 696e 7429 0a0a 2020 2020 2020 2020 6966  int)..        if
-00001360: 2065 7563 6c69 6465 616e 5f64 6973 7461   euclidean_dista
-00001370: 6e63 6528 6176 6572 6167 6564 5f70 6f69  nce(averaged_poi
-00001380: 6e74 2c73 656c 662e 6669 745f 706f 696e  nt,self.fit_poin
-00001390: 7429 203c 2073 656c 662e 6163 6365 7074  t) < self.accept
-000013a0: 616e 6365 5f72 6164 6975 733a 0a20 2020  ance_radius:.   
-000013b0: 2020 2020 2020 2020 2073 656c 662e 6974           self.it
-000013c0: 6572 6174 6f72 202b 3d20 310a 2020 2020  erator += 1.    
-000013d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000013e0: 6974 6572 6174 6f72 203e 2031 303a 0a20  iterator > 10:. 
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001400: 656c 662e 6974 6572 6174 6f72 203d 2030  elf.iterator = 0
-00001410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001420: 2073 656c 662e 6669 745f 706f 696e 7420   self.fit_point 
-00001430: 3d20 7365 6c66 2e67 6574 4e65 7752 616e  = self.getNewRan
-00001440: 646f 6d50 6f69 6e74 2829 0a20 2020 2020  domPoint().     
-00001450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001460: 696e 6372 6561 7365 5f70 7265 6369 7369  increase_precisi
-00001470: 6f6e 2829 0a0a 2020 2020 2020 2020 6765  on()..        ge
-00001480: 7665 6e74 203d 2047 6576 656e 7428 6176  vent = Gevent(av
-00001490: 6572 6167 6564 5f70 6f69 6e74 2c62 6c69  eraged_point,bli
-000014a0: 6e6b 2c66 6978 6174 696f 6e20 3e3d 2073  nk,fixation >= s
-000014b0: 656c 662e 6669 7829 0a20 2020 2020 2020  elf.fix).       
-000014c0: 2063 6576 656e 7420 3d20 4365 7665 6e74   cevent = Cevent
-000014d0: 2873 656c 662e 6669 745f 706f 696e 742c  (self.fit_point,
-000014e0: 7365 6c66 2e61 6363 6570 7461 6e63 655f  self.acceptance_
-000014f0: 7261 6469 7573 2c20 7365 6c66 2e63 616c  radius, self.cal
-00001500: 6962 7261 7469 6f6e 5f72 6164 6975 7329  ibration_radius)
-00001510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001520: 2867 6576 656e 742c 2063 6576 656e 7429  (gevent, cevent)
-00001530: 0a0a 636c 6173 7320 4579 6547 6573 7475  ..class EyeGestu
-00001540: 7265 735f 7631 3a0a 2020 2020 2222 224d  res_v1:.    """M
-00001550: 6169 6e20 636c 6173 7320 666f 7220 4579  ain class for Ey
-00001560: 6547 6573 7475 7265 2074 7261 636b 6572  eGesture tracker
-00001570: 2e20 4974 2063 6f6e 6669 6775 7265 7320  . It configures 
-00001580: 616e 6420 6d61 6e61 6765 7320 656e 7469  and manages enti
-00001590: 6572 2061 6c67 6f72 6974 686d 2222 220a  er algorithm""".
-000015a0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000015b0: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
-000015c0: 2020 2020 2020 2020 2072 6f69 5f78 3d32           roi_x=2
-000015d0: 3235 2c0a 2020 2020 2020 2020 2020 2020  25,.            
-000015e0: 2020 2020 2072 6f69 5f79 3d31 3035 2c0a       roi_y=105,.
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2072 6f69 5f77 6964 7468 3d38 302c 0a20   roi_width=80,. 
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 726f 695f 6865 6967 6874 3d31 3529 3a0a  roi_height=15):.
-00001630: 0a20 2020 2020 2020 2073 6372 6565 6e5f  .        screen_
-00001640: 7769 6474 6820 3d20 3530 300a 2020 2020  width = 500.    
-00001650: 2020 2020 7363 7265 656e 5f68 6569 6768      screen_heigh
-00001660: 7420 3d20 3530 300a 2020 2020 2020 2020  t = 500.        
-00001670: 6865 6967 6874 203d 2032 3530 0a20 2020  height = 250.   
-00001680: 2020 2020 2077 6964 7468 203d 2032 3530       width = 250
-00001690: 0a0a 2020 2020 2020 2020 726f 695f 7820  ..        roi_x 
-000016a0: 3d20 726f 695f 7820 2520 7363 7265 656e  = roi_x % screen
-000016b0: 5f77 6964 7468 0a20 2020 2020 2020 2072  _width.        r
-000016c0: 6f69 5f79 203d 2072 6f69 5f79 2025 2073  oi_y = roi_y % s
-000016d0: 6372 6565 6e5f 6865 6967 6874 0a20 2020  creen_height.   
-000016e0: 2020 2020 2072 6f69 5f77 6964 7468 203d       roi_width =
-000016f0: 2072 6f69 5f77 6964 7468 2025 2073 6372   roi_width % scr
-00001700: 6565 6e5f 7769 6474 680a 2020 2020 2020  een_width.      
-00001710: 2020 726f 695f 6865 6967 6874 203d 2072    roi_height = r
-00001720: 6f69 5f68 6569 6768 7420 2520 7363 7265  oi_height % scre
-00001730: 656e 5f68 6569 6768 740a 0a20 2020 2020  en_height..     
-00001740: 2020 2073 656c 662e 7363 7265 656e 5f77     self.screen_w
-00001750: 6964 7468 203d 2073 6372 6565 6e5f 7769  idth = screen_wi
-00001760: 6474 680a 2020 2020 2020 2020 7365 6c66  dth.        self
-00001770: 2e73 6372 6565 6e5f 6865 6967 6874 203d  .screen_height =
-00001780: 2073 6372 6565 6e5f 6865 6967 6874 0a0a   screen_height..
-00001790: 2020 2020 2020 2020 7365 6c66 2e73 6372          self.scr
-000017a0: 6565 6e20 3d20 6470 2e53 6372 6565 6e28  een = dp.Screen(
-000017b0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-000017c0: 6565 6e5f 7769 6474 682c 0a20 2020 2020  een_width,.     
-000017d0: 2020 2020 2020 2073 6372 6565 6e5f 6865         screen_he
-000017e0: 6967 6874 290a 0a20 2020 2020 2020 2073  ight)..        s
-000017f0: 656c 662e 6761 7a65 203d 2047 617a 6554  elf.gaze = GazeT
-00001800: 7261 636b 6572 2873 6372 6565 6e5f 7769  racker(screen_wi
-00001810: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 2020 2073 6372 6565 6e5f 6865 6967       screen_heig
-00001840: 6874 2c0a 2020 2020 2020 2020 2020 2020  ht,.            
-00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001860: 2020 2020 7769 6474 682c 0a20 2020 2020      width,.     
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-00001890: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018b0: 2020 2072 6f69 5f78 2c0a 2020 2020 2020     roi_x,.      
+00000de0: 2077 6964 7468 0d0a 2020 2020 2020 2020   width..        
+00000df0: 7365 6c66 2e6d 6f6e 6974 6f72 5f68 6569  self.monitor_hei
+00000e00: 6768 7420 3d20 6865 6967 6874 0d0a 0d0a  ght = height....
+00000e10: 2020 2020 2020 2020 636c 6173 7369 635f          classic_
+00000e20: 706f 696e 742c 206b 6579 5f70 6f69 6e74  point, key_point
+00000e30: 732c 2062 6c69 6e6b 2c20 6669 7861 7469  s, blink, fixati
+00000e40: 6f6e 203d 2073 656c 662e 6765 744c 616e  on = self.getLan
+00000e50: 646d 6172 6b73 2866 7261 6d65 2c73 656c  dmarks(frame,sel
+00000e60: 662e 6361 6c69 6272 6174 655f 6765 7374  f.calibrate_gest
+00000e70: 7572 6573 290d 0a0d 0a20 2020 2020 2020  ures)....       
+00000e80: 206d 6172 6769 6e20 3d20 3130 0d0a 2020   margin = 10..  
+00000e90: 2020 2020 2020 6966 2063 6c61 7373 6963        if classic
+00000ea0: 5f70 6f69 6e74 5b30 5d20 3c3d 206d 6172  _point[0] <= mar
+00000eb0: 6769 6e20 616e 6420 7365 6c66 2e63 616c  gin and self.cal
+00000ec0: 6962 7261 7469 6f6e 3a0d 0a20 2020 2020  ibration:..     
+00000ed0: 2020 2020 2020 2073 656c 662e 6361 6c69         self.cali
+00000ee0: 6272 6174 655f 6765 7374 7572 6573 203d  brate_gestures =
+00000ef0: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
+00000f00: 6c69 6620 636c 6173 7369 635f 706f 696e  lif classic_poin
+00000f10: 745b 305d 203e 3d20 7769 6474 6820 2d20  t[0] >= width - 
+00000f20: 6d61 7267 696e 2061 6e64 2073 656c 662e  margin and self.
+00000f30: 6361 6c69 6272 6174 696f 6e3a 0d0a 2020  calibration:..  
+00000f40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00000f50: 616c 6962 7261 7465 5f67 6573 7475 7265  alibrate_gesture
+00000f60: 7320 3d20 5472 7565 0d0a 2020 2020 2020  s = True..      
+00000f70: 2020 656c 6966 2063 6c61 7373 6963 5f70    elif classic_p
+00000f80: 6f69 6e74 5b31 5d20 3c3d 206d 6172 6769  oint[1] <= margi
+00000f90: 6e20 616e 6420 7365 6c66 2e63 616c 6962  n and self.calib
+00000fa0: 7261 7469 6f6e 3a0d 0a20 2020 2020 2020  ration:..       
+00000fb0: 2020 2020 2073 656c 662e 6361 6c69 6272       self.calibr
+00000fc0: 6174 655f 6765 7374 7572 6573 203d 2054  ate_gestures = T
+00000fd0: 7275 650d 0a20 2020 2020 2020 2065 6c69  rue..        eli
+00000fe0: 6620 636c 6173 7369 635f 706f 696e 745b  f classic_point[
+00000ff0: 315d 203e 3d20 6865 6967 6874 202d 206d  1] >= height - m
+00001000: 6172 6769 6e20 616e 6420 7365 6c66 2e63  argin and self.c
+00001010: 616c 6962 7261 7469 6f6e 3a0d 0a20 2020  alibration:..   
+00001020: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+00001030: 6c69 6272 6174 655f 6765 7374 7572 6573  librate_gestures
+00001040: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00001050: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001060: 2020 2020 7365 6c66 2e63 616c 6962 7261      self.calibra
+00001070: 7465 5f67 6573 7475 7265 7320 3d20 4661  te_gestures = Fa
+00001080: 6c73 650d 0a0d 0a20 2020 2020 2020 2079  lse....        y
+00001090: 5f70 6f69 6e74 203d 2073 656c 662e 636c  _point = self.cl
+000010a0: 622e 7072 6564 6963 7428 6b65 795f 706f  b.predict(key_po
+000010b0: 696e 7473 290d 0a20 2020 2020 2020 2073  ints)..        s
+000010c0: 656c 662e 6176 6572 6167 655f 706f 696e  elf.average_poin
+000010d0: 7473 5b31 3a2c 3a5d 203d 2073 656c 662e  ts[1:,:] = self.
+000010e0: 6176 6572 6167 655f 706f 696e 7473 5b3a  average_points[:
+000010f0: 2873 656c 662e 6176 6572 6167 655f 706f  (self.average_po
+00001100: 696e 7473 2e73 6861 7065 5b30 5d20 2d20  ints.shape[0] - 
+00001110: 3129 2c3a 5d0d 0a20 2020 2020 2020 2069  1),:]..        i
+00001120: 6620 6669 7861 7469 6f6e 203c 3d20 7365  f fixation <= se
+00001130: 6c66 2e66 6978 3a0d 0a20 2020 2020 2020  lf.fix:..       
+00001140: 2020 2020 2073 656c 662e 6176 6572 6167       self.averag
+00001150: 655f 706f 696e 7473 5b30 2c3a 5d20 3d20  e_points[0,:] = 
+00001160: 795f 706f 696e 740d 0a0d 0a20 2020 2020  y_point....     
+00001170: 2020 2069 6620 7365 6c66 2e66 696c 6c65     if self.fille
+00001180: 645f 706f 696e 7473 203c 2073 656c 662e  d_points < self.
+00001190: 6176 6572 6167 655f 706f 696e 7473 2e73  average_points.s
+000011a0: 6861 7065 5b30 5d20 616e 6420 2879 5f70  hape[0] and (y_p
+000011b0: 6f69 6e74 2021 3d20 6e70 2e61 7272 6179  oint != np.array
+000011c0: 285b 302e 302c 302e 305d 2929 2e61 6e79  ([0.0,0.0])).any
+000011d0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000011e0: 2073 656c 662e 6669 6c6c 6564 5f70 6f69   self.filled_poi
+000011f0: 6e74 7320 2b3d 2031 0d0a 0d0a 2020 2020  nts += 1....    
+00001200: 2020 2020 6176 6572 6167 6564 5f70 6f69      averaged_poi
+00001210: 6e74 203d 2028 6e70 2e73 756d 2873 656c  nt = (np.sum(sel
+00001220: 662e 6176 6572 6167 655f 706f 696e 7473  f.average_points
+00001230: 5b3a 2c3a 5d2c 6178 6973 3d30 2920 2b20  [:,:],axis=0) + 
+00001240: 2863 6c61 7373 6963 5f70 6f69 6e74 202a  (classic_point *
+00001250: 2073 656c 662e 434e 2929 2f28 7365 6c66   self.CN))/(self
+00001260: 2e66 696c 6c65 645f 706f 696e 7473 202b  .filled_points +
+00001270: 2073 656c 662e 434e 290d 0a0d 0a20 2020   self.CN)....   
+00001280: 2020 2020 2069 6620 7365 6c66 2e63 616c       if self.cal
+00001290: 6962 7261 7469 6f6e 2061 6e64 2028 6575  ibration and (eu
+000012a0: 636c 6964 6561 6e5f 6469 7374 616e 6365  clidean_distance
+000012b0: 2861 7665 7261 6765 645f 706f 696e 742c  (averaged_point,
+000012c0: 7365 6c66 2e66 6974 5f70 6f69 6e74 2920  self.fit_point) 
+000012d0: 3c20 7365 6c66 2e63 616c 6962 7261 7469  < self.calibrati
+000012e0: 6f6e 5f72 6164 6975 7320 6f72 2073 656c  on_radius or sel
+000012f0: 662e 6669 6c6c 6564 5f70 6f69 6e74 7320  f.filled_points 
+00001300: 3c20 7365 6c66 2e61 7665 7261 6765 5f70  < self.average_p
+00001310: 6f69 6e74 732e 7368 6170 655b 305d 202a  oints.shape[0] *
+00001320: 2031 3029 3a0d 0a20 2020 2020 2020 2020   10):..         
+00001330: 2020 2073 656c 662e 636c 622e 6164 6428     self.clb.add(
+00001340: 6b65 795f 706f 696e 7473 2c73 656c 662e  key_points,self.
+00001350: 6669 745f 706f 696e 7429 0d0a 0d0a 2020  fit_point)....  
+00001360: 2020 2020 2020 6966 2065 7563 6c69 6465        if euclide
+00001370: 616e 5f64 6973 7461 6e63 6528 6176 6572  an_distance(aver
+00001380: 6167 6564 5f70 6f69 6e74 2c73 656c 662e  aged_point,self.
+00001390: 6669 745f 706f 696e 7429 203c 2073 656c  fit_point) < sel
+000013a0: 662e 6163 6365 7074 616e 6365 5f72 6164  f.acceptance_rad
+000013b0: 6975 733a 0d0a 2020 2020 2020 2020 2020  ius:..          
+000013c0: 2020 7365 6c66 2e69 7465 7261 746f 7220    self.iterator 
+000013d0: 2b3d 2031 0d0a 2020 2020 2020 2020 2020  += 1..          
+000013e0: 2020 6966 2073 656c 662e 6974 6572 6174    if self.iterat
+000013f0: 6f72 203e 2031 303a 0d0a 2020 2020 2020  or > 10:..      
+00001400: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00001410: 7465 7261 746f 7220 3d20 300d 0a20 2020  terator = 0..   
+00001420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001430: 662e 6669 745f 706f 696e 7420 3d20 7365  f.fit_point = se
+00001440: 6c66 2e63 616c 6962 7261 7469 6f6e 4d61  lf.calibrationMa
+00001450: 742e 6765 744e 6578 7450 6f69 6e74 2877  t.getNextPoint(w
+00001460: 6964 7468 2c68 6569 6768 7429 0d0a 2020  idth,height)..  
+00001470: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001480: 6c66 2e69 6e63 7265 6173 655f 7072 6563  lf.increase_prec
+00001490: 6973 696f 6e28 290d 0a0d 0a20 2020 2020  ision()....     
+000014a0: 2020 2067 6576 656e 7420 3d20 4765 7665     gevent = Geve
+000014b0: 6e74 2861 7665 7261 6765 645f 706f 696e  nt(averaged_poin
+000014c0: 742c 626c 696e 6b2c 6669 7861 7469 6f6e  t,blink,fixation
+000014d0: 203e 3d20 7365 6c66 2e66 6978 290d 0a20   >= self.fix).. 
+000014e0: 2020 2020 2020 2063 6576 656e 7420 3d20         cevent = 
+000014f0: 4365 7665 6e74 2873 656c 662e 6669 745f  Cevent(self.fit_
+00001500: 706f 696e 742c 7365 6c66 2e61 6363 6570  point,self.accep
+00001510: 7461 6e63 655f 7261 6469 7573 2c20 7365  tance_radius, se
+00001520: 6c66 2e63 616c 6962 7261 7469 6f6e 5f72  lf.calibration_r
+00001530: 6164 6975 7329 0d0a 2020 2020 2020 2020  adius)..        
+00001540: 7265 7475 726e 2028 6765 7665 6e74 2c20  return (gevent, 
+00001550: 6365 7665 6e74 290d 0a0d 0a63 6c61 7373  cevent)....class
+00001560: 2045 7965 4765 7374 7572 6573 5f76 313a   EyeGestures_v1:
+00001570: 0d0a 2020 2020 2222 224d 6169 6e20 636c  ..    """Main cl
+00001580: 6173 7320 666f 7220 4579 6547 6573 7475  ass for EyeGestu
+00001590: 7265 2074 7261 636b 6572 2e20 4974 2063  re tracker. It c
+000015a0: 6f6e 6669 6775 7265 7320 616e 6420 6d61  onfigures and ma
+000015b0: 6e61 6765 7320 656e 7469 6572 2061 6c67  nages entier alg
+000015c0: 6f72 6974 686d 2222 220d 0a0d 0a20 2020  orithm"""....   
+000015d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000015e0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+000015f0: 2020 2020 2020 726f 695f 783d 3232 352c        roi_x=225,
+00001600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001610: 2020 2072 6f69 5f79 3d31 3035 2c0d 0a20     roi_y=105,.. 
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 726f 695f 7769 6474 683d 3830 2c0d 0a20  roi_width=80,.. 
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 726f 695f 6865 6967 6874 3d31 3529 3a0d  roi_height=15):.
+00001660: 0a0d 0a20 2020 2020 2020 2073 6372 6565  ...        scree
+00001670: 6e5f 7769 6474 6820 3d20 3530 300d 0a20  n_width = 500.. 
+00001680: 2020 2020 2020 2073 6372 6565 6e5f 6865         screen_he
+00001690: 6967 6874 203d 2035 3030 0d0a 2020 2020  ight = 500..    
+000016a0: 2020 2020 6865 6967 6874 203d 2032 3530      height = 250
+000016b0: 0d0a 2020 2020 2020 2020 7769 6474 6820  ..        width 
+000016c0: 3d20 3235 300d 0a0d 0a20 2020 2020 2020  = 250....       
+000016d0: 2072 6f69 5f78 203d 2072 6f69 5f78 2025   roi_x = roi_x %
+000016e0: 2073 6372 6565 6e5f 7769 6474 680d 0a20   screen_width.. 
+000016f0: 2020 2020 2020 2072 6f69 5f79 203d 2072         roi_y = r
+00001700: 6f69 5f79 2025 2073 6372 6565 6e5f 6865  oi_y % screen_he
+00001710: 6967 6874 0d0a 2020 2020 2020 2020 726f  ight..        ro
+00001720: 695f 7769 6474 6820 3d20 726f 695f 7769  i_width = roi_wi
+00001730: 6474 6820 2520 7363 7265 656e 5f77 6964  dth % screen_wid
+00001740: 7468 0d0a 2020 2020 2020 2020 726f 695f  th..        roi_
+00001750: 6865 6967 6874 203d 2072 6f69 5f68 6569  height = roi_hei
+00001760: 6768 7420 2520 7363 7265 656e 5f68 6569  ght % screen_hei
+00001770: 6768 740d 0a0d 0a20 2020 2020 2020 2073  ght....        s
+00001780: 656c 662e 7363 7265 656e 5f77 6964 7468  elf.screen_width
+00001790: 203d 2073 6372 6565 6e5f 7769 6474 680d   = screen_width.
+000017a0: 0a20 2020 2020 2020 2073 656c 662e 7363  .        self.sc
+000017b0: 7265 656e 5f68 6569 6768 7420 3d20 7363  reen_height = sc
+000017c0: 7265 656e 5f68 6569 6768 740d 0a0d 0a20  reen_height.... 
+000017d0: 2020 2020 2020 2073 656c 662e 7363 7265         self.scre
+000017e0: 656e 203d 2064 702e 5363 7265 656e 280d  en = dp.Screen(.
+000017f0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00001800: 6565 6e5f 7769 6474 682c 0d0a 2020 2020  een_width,..    
+00001810: 2020 2020 2020 2020 7363 7265 656e 5f68          screen_h
+00001820: 6569 6768 7429 0d0a 0d0a 2020 2020 2020  eight)....      
+00001830: 2020 7365 6c66 2e67 617a 6520 3d20 4761    self.gaze = Ga
+00001840: 7a65 5472 6163 6b65 7228 7363 7265 656e  zeTracker(screen
+00001850: 5f77 6964 7468 2c0d 0a20 2020 2020 2020  _width,..       
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 2020 2073 6372 6565 6e5f           screen_
+00001880: 6865 6967 6874 2c0d 0a20 2020 2020 2020  height,..       
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 2020 2020 2020 2020 2077 6964 7468 2c0d           width,.
+000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 2020 2020 2020 2020 726f 695f 792c            roi_y,
-000018e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001900: 2072 6f69 5f77 6964 7468 2c0a 2020 2020   roi_width,.    
+000018d0: 2068 6569 6768 742c 0d0a 2020 2020 2020   height,..      
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2020 2020 2020 2020 726f 695f 782c            roi_x,
+00001900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 2020 2020 2020 2020 2020 726f 695f              roi_
-00001930: 6865 6967 6874 290a 2020 2020 2020 2020  height).        
-00001940: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-00001950: 6c69 6272 6174 6f72 7320 3d20 6469 6374  librators = dict
-00001960: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00001970: 6361 6c69 6272 6174 6520 3d20 4661 6c73  calibrate = Fals
-00001980: 650a 0a20 2020 2064 6566 2067 6574 4665  e..    def getFe
-00001990: 6174 7572 6573 2873 656c 662c 2069 6d61  atures(self, ima
-000019a0: 6765 293a 0a20 2020 2020 2020 2022 2222  ge):.        """
-000019b0: 5b4e 4f54 2052 4543 4f4d 4d45 4e44 4544  [NOT RECOMMENDED
-000019c0: 5d20 4675 6e63 7469 6f6e 2061 6c6c 6f77  ] Function allow
-000019d0: 696e 6720 666f 7220 6578 7472 6163 7469  ing for extracti
-000019e0: 6f6e 206f 6620 6761 7a65 2066 6561 7475  on of gaze featu
-000019f0: 7265 7320 6672 6f6d 2069 6d61 6765 2222  res from image""
-00001a00: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00001a10: 6e20 7365 6c66 2e67 617a 652e 6765 7446  n self.gaze.getF
-00001a20: 6561 7475 7265 7328 696d 6167 6529 0a0a  eatures(image)..
-00001a30: 2020 2020 2320 4074 696d 6569 740a 2020      # @timeit.  
-00001a40: 2020 2320 302e 3031 3120 2d20 302e 3031    # 0.011 - 0.01
-00001a50: 3520 7320 666f 7220 6578 6563 7574 696f  5 s for executio
-00001a60: 6e0a 2020 2020 6465 6620 7374 6570 2873  n.    def step(s
-00001a70: 656c 662c 2069 6d61 6765 2c0a 2020 2020  elf, image,.    
-00001a80: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001a90: 7465 7874 2c0a 2020 2020 2020 2020 2020  text,.          
-00001aa0: 2020 2020 2020 2063 616c 6962 7261 7469         calibrati
-00001ab0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00001ac0: 2020 2020 2064 6973 706c 6179 5f77 6964       display_wid
-00001ad0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00001ae0: 2020 2020 2064 6973 706c 6179 5f68 6569       display_hei
-00001af0: 6768 742c 0a20 2020 2020 2020 2020 2020  ght,.           
-00001b00: 2020 2020 2020 6469 7370 6c61 795f 6f66        display_of
-00001b10: 6673 6574 5f78 3d30 2c0a 2020 2020 2020  fset_x=0,.      
-00001b20: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00001b30: 6179 5f6f 6666 7365 745f 793d 302c 0a20  ay_offset_y=0,. 
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 6669 7861 7469 6f6e 5f66 7265 657a 653d  fixation_freeze=
-00001b60: 302e 372c 0a20 2020 2020 2020 2020 2020  0.7,.           
-00001b70: 2020 2020 2020 6672 6565 7a65 5f72 6164        freeze_rad
-00001b80: 6975 733d 3230 2c0a 2020 2020 2020 2020  ius=20,.        
-00001b90: 2020 2020 2020 2020 206f 6666 7365 745f           offset_
-00001ba0: 783d 302c 0a20 2020 2020 2020 2020 2020  x=0,.           
-00001bb0: 2020 2020 2020 6f66 6673 6574 5f79 3d30        offset_y=0
-00001bc0: 293a 0a20 2020 2020 2020 2022 2222 4675  ):.        """Fu
-00001bd0: 6e63 7469 6f6e 2070 6572 666f 726d 696e  nction performin
-00001be0: 6720 6573 7469 6d61 7469 6f6e 2061 6e64  g estimation and
-00001bf0: 2072 6574 7572 6e69 6e67 2065 7665 6e74   returning event
-00001c00: 206f 626a 6563 7422 2222 0a0a 2020 2020   object"""..    
-00001c10: 2020 2020 6469 7370 6c61 7920 3d20 6470      display = dp
-00001c20: 2e44 6973 706c 6179 280a 2020 2020 2020  .Display(.      
-00001c30: 2020 2020 2020 6469 7370 6c61 795f 7769        display_wi
-00001c40: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
-00001c50: 2064 6973 706c 6179 5f68 6569 6768 742c   display_height,
-00001c60: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00001c70: 706c 6179 5f6f 6666 7365 745f 782c 0a20  play_offset_x,. 
-00001c80: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00001c90: 6179 5f6f 6666 7365 745f 790a 2020 2020  ay_offset_y.    
-00001ca0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00001cb0: 2061 6c6c 6f77 2066 6f72 2072 616e 646f   allow for rando
-00001cc0: 6d20 7265 6361 6c69 6272 6174 696f 6e20  m recalibration 
-00001cd0: 7368 6f74 0a20 2020 2020 2020 2065 7665  shot.        eve
-00001ce0: 6e74 203d 2073 656c 662e 6761 7a65 2e65  nt = self.gaze.e
-00001cf0: 7374 696d 6174 6528 696d 6167 652c 0a20  stimate(image,. 
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2064 6973 706c 6179 2c0a 2020 2020 2020   display,.      
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00001d50: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2020 2020 2020 2063 616c 6962 7261 7469         calibrati
-00001d80: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 6669 7861 7469 6f6e 5f66        fixation_f
-00001db0: 7265 657a 652c 0a20 2020 2020 2020 2020  reeze,.         
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 2020 2020 2066 7265 657a 655f           freeze_
-00001de0: 7261 6469 7573 2c0a 2020 2020 2020 2020  radius,.        
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 2020 2020 2020 6f66 6673 6574            offset
-00001e10: 5f78 2c0a 2020 2020 2020 2020 2020 2020  _x,.            
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2020 2020 6f66 6673 6574 5f79 290a        offset_y).
-00001e40: 0a20 2020 2020 2020 2063 7572 736f 725f  .        cursor_
-00001e50: 782c 6375 7273 6f72 5f79 203d 2065 7665  x,cursor_y = eve
-00001e60: 6e74 2e70 6f69 6e74 5b30 5d2c 6576 656e  nt.point[0],even
-00001e70: 742e 706f 696e 745b 315d 0a20 2020 2020  t.point[1].     
-00001e80: 2020 2069 6620 636f 6e74 6578 7420 696e     if context in
-00001e90: 2073 656c 662e 6361 6c69 6272 6174 6f72   self.calibrator
-00001ea0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00001eb0: 656c 662e 6361 6c69 6272 6174 6520 3d20  elf.calibrate = 
-00001ec0: 7365 6c66 2e63 616c 6962 7261 746f 7273  self.calibrators
-00001ed0: 5b63 6f6e 7465 7874 5d2e 6361 6c69 6272  [context].calibr
-00001ee0: 6174 6528 6375 7273 6f72 5f78 2c63 7572  ate(cursor_x,cur
-00001ef0: 736f 725f 792c 6576 656e 742e 6669 7861  sor_y,event.fixa
-00001f00: 7469 6f6e 290a 2020 2020 2020 2020 656c  tion).        el
-00001f10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00001f20: 7365 6c66 2e63 616c 6962 7261 746f 7273  self.calibrators
-00001f30: 5b63 6f6e 7465 7874 5d20 3d20 4361 6c69  [context] = Cali
-00001f40: 6272 6174 6f72 5f76 3128 6469 7370 6c61  brator_v1(displa
-00001f50: 795f 7769 6474 682c 6469 7370 6c61 795f  y_width,display_
-00001f60: 6865 6967 6874 2c63 7572 736f 725f 782c  height,cursor_x,
-00001f70: 6375 7273 6f72 5f79 290a 2020 2020 2020  cursor_y).      
-00001f80: 2020 2020 2020 7365 6c66 2e63 616c 6962        self.calib
-00001f90: 7261 7465 203d 2073 656c 662e 6361 6c69  rate = self.cali
-00001fa0: 6272 6174 6f72 735b 636f 6e74 6578 745d  brators[context]
-00001fb0: 2e63 616c 6962 7261 7465 2863 7572 736f  .calibrate(curso
-00001fc0: 725f 782c 6375 7273 6f72 5f79 2c65 7665  r_x,cursor_y,eve
-00001fd0: 6e74 2e66 6978 6174 696f 6e29 0a0a 2020  nt.fixation)..  
-00001fe0: 2020 2020 2020 6370 6f69 6e74 203d 2073        cpoint = s
-00001ff0: 656c 662e 6361 6c69 6272 6174 6f72 735b  elf.calibrators[
-00002000: 636f 6e74 6578 745d 2e67 6574 5f63 7572  context].get_cur
-00002010: 7265 6e74 5f70 6f69 6e74 2829 0a20 2020  rent_point().   
-00002020: 2020 2020 2063 616c 6962 7261 7469 6f6e       calibration
-00002030: 203d 2073 656c 662e 6361 6c69 6272 6174   = self.calibrat
-00002040: 6520 616e 6420 6370 6f69 6e74 2021 3d20  e and cpoint != 
-00002050: 2830 2c30 290a 2020 2020 2020 2020 6365  (0,0).        ce
-00002060: 7665 6e74 203d 2043 6576 656e 7428 6370  vent = Cevent(cp
-00002070: 6f69 6e74 2c31 3030 2c20 3130 302c 2063  oint,100, 100, c
-00002080: 616c 6962 7261 7469 6f6e 290a 0a20 2020  alibration)..   
-00002090: 2020 2020 2072 6574 7572 6e20 2865 7665       return (eve
-000020a0: 6e74 2c20 6365 7665 6e74 29              nt, cevent)
+00001920: 2020 726f 695f 792c 0d0a 2020 2020 2020    roi_y,..      
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 2020 2020 2020 2020 2020 726f 695f 7769            roi_wi
+00001950: 6474 682c 0d0a 2020 2020 2020 2020 2020  dth,..          
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 726f 695f 6865 6967 6874        roi_height
+00001980: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00001990: 2020 2020 2073 656c 662e 6361 6c69 6272       self.calibr
+000019a0: 6174 6f72 7320 3d20 6469 6374 2829 0d0a  ators = dict()..
+000019b0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+000019c0: 6962 7261 7465 203d 2046 616c 7365 0d0a  ibrate = False..
+000019d0: 0d0a 2020 2020 6465 6620 6765 7446 6561  ..    def getFea
+000019e0: 7475 7265 7328 7365 6c66 2c20 696d 6167  tures(self, imag
+000019f0: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00001a00: 5b4e 4f54 2052 4543 4f4d 4d45 4e44 4544  [NOT RECOMMENDED
+00001a10: 5d20 4675 6e63 7469 6f6e 2061 6c6c 6f77  ] Function allow
+00001a20: 696e 6720 666f 7220 6578 7472 6163 7469  ing for extracti
+00001a30: 6f6e 206f 6620 6761 7a65 2066 6561 7475  on of gaze featu
+00001a40: 7265 7320 6672 6f6d 2069 6d61 6765 2222  res from image""
+00001a50: 220d 0a0d 0a20 2020 2020 2020 2072 6574  "....        ret
+00001a60: 7572 6e20 7365 6c66 2e67 617a 652e 6765  urn self.gaze.ge
+00001a70: 7446 6561 7475 7265 7328 696d 6167 6529  tFeatures(image)
+00001a80: 0d0a 0d0a 2020 2020 2320 4074 696d 6569  ....    # @timei
+00001a90: 740d 0a20 2020 2023 2030 2e30 3131 202d  t..    # 0.011 -
+00001aa0: 2030 2e30 3135 2073 2066 6f72 2065 7865   0.015 s for exe
+00001ab0: 6375 7469 6f6e 0d0a 2020 2020 6465 6620  cution..    def 
+00001ac0: 7374 6570 2873 656c 662c 2069 6d61 6765  step(self, image
+00001ad0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001ae0: 2020 2020 636f 6e74 6578 742c 0d0a 2020      context,..  
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001b00: 616c 6962 7261 7469 6f6e 2c0d 0a20 2020  alibration,..   
+00001b10: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001b20: 7370 6c61 795f 7769 6474 682c 0d0a 2020  splay_width,..  
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00001b40: 6973 706c 6179 5f68 6569 6768 742c 0d0a  isplay_height,..
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2064 6973 706c 6179 5f6f 6666 7365 745f   display_offset_
+00001b70: 783d 302c 0d0a 2020 2020 2020 2020 2020  x=0,..          
+00001b80: 2020 2020 2020 2064 6973 706c 6179 5f6f         display_o
+00001b90: 6666 7365 745f 793d 302c 0d0a 2020 2020  ffset_y=0,..    
+00001ba0: 2020 2020 2020 2020 2020 2020 2066 6978               fix
+00001bb0: 6174 696f 6e5f 6672 6565 7a65 3d30 2e37  ation_freeze=0.7
+00001bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001bd0: 2020 2020 6672 6565 7a65 5f72 6164 6975      freeze_radiu
+00001be0: 733d 3230 2c0d 0a20 2020 2020 2020 2020  s=20,..         
+00001bf0: 2020 2020 2020 2020 6f66 6673 6574 5f78          offset_x
+00001c00: 3d30 2c0d 0a20 2020 2020 2020 2020 2020  =0,..           
+00001c10: 2020 2020 2020 6f66 6673 6574 5f79 3d30        offset_y=0
+00001c20: 293a 0d0a 2020 2020 2020 2020 2222 2246  ):..        """F
+00001c30: 756e 6374 696f 6e20 7065 7266 6f72 6d69  unction performi
+00001c40: 6e67 2065 7374 696d 6174 696f 6e20 616e  ng estimation an
+00001c50: 6420 7265 7475 726e 696e 6720 6576 656e  d returning even
+00001c60: 7420 6f62 6a65 6374 2222 220d 0a0d 0a20  t object""".... 
+00001c70: 2020 2020 2020 2064 6973 706c 6179 203d         display =
+00001c80: 2064 702e 4469 7370 6c61 7928 0d0a 2020   dp.Display(..  
+00001c90: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00001ca0: 795f 7769 6474 682c 0d0a 2020 2020 2020  y_width,..      
+00001cb0: 2020 2020 2020 6469 7370 6c61 795f 6865        display_he
+00001cc0: 6967 6874 2c0d 0a20 2020 2020 2020 2020  ight,..         
+00001cd0: 2020 2064 6973 706c 6179 5f6f 6666 7365     display_offse
+00001ce0: 745f 782c 0d0a 2020 2020 2020 2020 2020  t_x,..          
+00001cf0: 2020 6469 7370 6c61 795f 6f66 6673 6574    display_offset
+00001d00: 5f79 0d0a 2020 2020 2020 2020 290d 0a0d  _y..        )...
+00001d10: 0a20 2020 2020 2020 2023 2061 6c6c 6f77  .        # allow
+00001d20: 2066 6f72 2072 616e 646f 6d20 7265 6361   for random reca
+00001d30: 6c69 6272 6174 696f 6e20 7368 6f74 0d0a  libration shot..
+00001d40: 2020 2020 2020 2020 6576 656e 7420 3d20          event = 
+00001d50: 7365 6c66 2e67 617a 652e 6573 7469 6d61  self.gaze.estima
+00001d60: 7465 2869 6d61 6765 2c0d 0a20 2020 2020  te(image,..     
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00001d90: 706c 6179 2c0d 0a20 2020 2020 2020 2020  play,..         
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001db0: 2020 2020 2020 2020 2063 6f6e 7465 7874           context
+00001dc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2063 616c 6962 7261 7469 6f6e       calibration
+00001df0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e10: 2020 2020 2066 6978 6174 696f 6e5f 6672       fixation_fr
+00001e20: 6565 7a65 2c0d 0a20 2020 2020 2020 2020  eeze,..         
+00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e40: 2020 2020 2020 2020 2066 7265 657a 655f           freeze_
+00001e50: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2020 2020 2020 2020 2020 206f 6666 7365             offse
+00001e80: 745f 782c 0d0a 2020 2020 2020 2020 2020  t_x,..          
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 2020 2020 2020 2020 6f66 6673 6574 5f79          offset_y
+00001eb0: 290d 0a0d 0a20 2020 2020 2020 2063 7572  )....        cur
+00001ec0: 736f 725f 782c 6375 7273 6f72 5f79 203d  sor_x,cursor_y =
+00001ed0: 2065 7665 6e74 2e70 6f69 6e74 5b30 5d2c   event.point[0],
+00001ee0: 6576 656e 742e 706f 696e 745b 315d 0d0a  event.point[1]..
+00001ef0: 2020 2020 2020 2020 6966 2063 6f6e 7465          if conte
+00001f00: 7874 2069 6e20 7365 6c66 2e63 616c 6962  xt in self.calib
+00001f10: 7261 746f 7273 3a0d 0a20 2020 2020 2020  rators:..       
+00001f20: 2020 2020 2073 656c 662e 6361 6c69 6272       self.calibr
+00001f30: 6174 6520 3d20 7365 6c66 2e63 616c 6962  ate = self.calib
+00001f40: 7261 746f 7273 5b63 6f6e 7465 7874 5d2e  rators[context].
+00001f50: 6361 6c69 6272 6174 6528 6375 7273 6f72  calibrate(cursor
+00001f60: 5f78 2c63 7572 736f 725f 792c 6576 656e  _x,cursor_y,even
+00001f70: 742e 6669 7861 7469 6f6e 290d 0a20 2020  t.fixation)..   
+00001f80: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001f90: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+00001fa0: 6962 7261 746f 7273 5b63 6f6e 7465 7874  ibrators[context
+00001fb0: 5d20 3d20 4361 6c69 6272 6174 6f72 5f76  ] = Calibrator_v
+00001fc0: 3128 6469 7370 6c61 795f 7769 6474 682c  1(display_width,
+00001fd0: 6469 7370 6c61 795f 6865 6967 6874 2c63  display_height,c
+00001fe0: 7572 736f 725f 782c 6375 7273 6f72 5f79  ursor_x,cursor_y
+00001ff0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00002000: 656c 662e 6361 6c69 6272 6174 6520 3d20  elf.calibrate = 
+00002010: 7365 6c66 2e63 616c 6962 7261 746f 7273  self.calibrators
+00002020: 5b63 6f6e 7465 7874 5d2e 6361 6c69 6272  [context].calibr
+00002030: 6174 6528 6375 7273 6f72 5f78 2c63 7572  ate(cursor_x,cur
+00002040: 736f 725f 792c 6576 656e 742e 6669 7861  sor_y,event.fixa
+00002050: 7469 6f6e 290d 0a0d 0a20 2020 2020 2020  tion)....       
+00002060: 2063 706f 696e 7420 3d20 7365 6c66 2e63   cpoint = self.c
+00002070: 616c 6962 7261 746f 7273 5b63 6f6e 7465  alibrators[conte
+00002080: 7874 5d2e 6765 745f 6375 7272 656e 745f  xt].get_current_
+00002090: 706f 696e 7428 290d 0a20 2020 2020 2020  point()..       
+000020a0: 2063 616c 6962 7261 7469 6f6e 203d 2073   calibration = s
+000020b0: 656c 662e 6361 6c69 6272 6174 6520 616e  elf.calibrate an
+000020c0: 6420 6370 6f69 6e74 2021 3d20 2830 2c30  d cpoint != (0,0
+000020d0: 290d 0a20 2020 2020 2020 2063 6576 656e  )..        ceven
+000020e0: 7420 3d20 4365 7665 6e74 2863 706f 696e  t = Cevent(cpoin
+000020f0: 742c 3130 302c 2031 3030 2c20 6361 6c69  t,100, 100, cali
+00002100: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+00002110: 2020 2020 7265 7475 726e 2028 6576 656e      return (even
+00002120: 742c 2063 6576 656e 7429                 t, cevent)
```

### Comparing `eyegestures-2.0.0/eyeGestures/gazeEstimator.py` & `eyegestures-2.1.0/eyeGestures/gazeEstimator.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-
-import numpy as np
-from eyeGestures.gevent import Gevent
-from eyeGestures.face import FaceFinder, Face
-from eyeGestures.Fixation import Fixation
-from eyeGestures.processing import EyeProcessor
-from eyeGestures.gazeContexter import GazeContext
-from eyeGestures.screenTracker.screenTracker import ScreenManager
-import eyeGestures.screenTracker.dataPoints as dp
-from eyeGestures.utils import Buffor
-
-
-def isInside(circle_x, circle_y, r, x, y):
-    """Function checking if points are inside the circle"""
-
-    # Compare radius of circle
-    # with distance of its center
-    # from given point
-    if ((x - circle_x) * (x - circle_x) +
-            (y - circle_y) * (y - circle_y) <= r * r):
-        return True
-    else:
-        return False
-
-
-class GazeTracker:
-    """Class processing images and returning gaze tracker"""
-
-    N_FEATURES = 16
-
-    def __init__(self, screen_width, screen_heigth,
-                 eye_screen_w, eye_screen_h,
-                 roi_x, roi_y,
-                 roi_width, roi_height,
-                 monitor_offset_x=0,
-                 monitor_offset_y=0):
-
-        self.screen = dp.Screen(screen_width, screen_heigth)
-
-        self.offset_x = 0
-        self.offset_y = 0
-
-        self.roi_x = roi_x
-        self.roi_y = roi_y
-        self.roi_width = roi_width
-        self.roi_height = roi_height
-
-        self.eye_screen_w = eye_screen_w
-        self.eye_screen_h = eye_screen_h
-
-        self.eyeProcessorLeft = EyeProcessor(eye_screen_w, eye_screen_h)
-        self.eyeProcessorRight = EyeProcessor(eye_screen_w, eye_screen_h)
-
-        self.screen_man = ScreenManager()
-
-        self.finder = FaceFinder()
-
-        # those are used for analysis
-        self.__headDir = [0.5, 0.5]
-
-        self.point_screen = [0.0, 0.0]
-        self.freezed_point = [0.0, 0.0]
-
-        self.face = Face()
-        self.GContext = GazeContext()
-    #     self.calibration = False
-
-    def __gaze_intersection(self, l_eye, r_eye, l_buff, r_buff):
-        l_pupil = l_eye.getPupil()
-        l_gaze = l_eye.getGaze(l_buff)
-
-        r_pupil = r_eye.getPupil()
-        r_gaze = r_eye.getGaze(r_buff)
-
-        l_end = l_gaze + l_pupil
-        r_end = r_gaze + r_pupil
-
-        l_m = (l_end[1] - l_pupil[1])/(l_end[0] - l_pupil[0])
-        r_m = (r_end[1] - r_pupil[1])/(r_end[0] - r_pupil[0])
-
-        l_b = l_end[1] - l_m * l_end[0]
-        r_b = r_end[1] - r_m * r_end[0]
-
-        i_x = (r_b - l_b)/(l_m - r_m)
-        i_y = r_m * i_x + r_b
-        return (i_x, i_y)
-
-    def __pupil(self, eye, eyeProcessor, intersection_x, buffor):
-
-        eyeProcessor.append(eye.getPupil(), eye.getLandmarks(), buffor)
-        point = eyeProcessor.getAvgPupil(
-            self.eye_screen_w, self.eye_screen_h, buffor)
-        point = np.array((int(intersection_x), point[1]))
-
-        return point, buffor
-
-    def estimate(self,
-                 image,
-                 display,
-                 context_id,
-                 calibration,
-                 fixation_freeze=0.7,
-                 freeze_radius=20,
-                 offset_x=0,
-                 offset_y=0):
-        """Function estimating gaze and returning gaze event based on image"""
-
-        event = None
-        face_mesh = self.getFeatures(image)
-        if not face_mesh:
-            return None
-
-        self.face.process(image, face_mesh)
-
-        context = self.GContext.get(context_id, display,
-            face = None,
-            roi =dp.ScreenROI(
-                self.roi_x,
-                self.roi_y,
-                self.roi_width,
-                self.roi_height),
-            edges=dp.ScreenROI(285, 105, 80, 15),
-            cluster_boundaries=dp.ScreenROI(225, 125, 20, 20),
-            buffor=Buffor(200),
-            l_pupil=Buffor(20),
-            r_pupil=Buffor(20),
-            l_eye_buff=Buffor(20),
-            r_eye_buff=Buffor(20),
-            fixation=Fixation(0, 0, 100))
-        context.calibration = calibration
-
-        if not self.face is None:
-
-            if context.face == None:
-                x,y,w,h=self.face.getBoundingBox()
-                i_w = self.face.image_w
-                i_h = self.face.image_h
-                context.face = (x,y,w,h,i_w,i_h)
-
-
-            l_eye = self.face.getLeftEye()
-            r_eye = self.face.getRightEye()
-
-            # TODO: check what happens here before with l_pupil
-            intersection_x, _ = self.__gaze_intersection(
-                l_eye, r_eye, context.l_eye_buff, context.r_eye_buff)
-            l_point, l_buffor = self.__pupil(
-                l_eye, self.eyeProcessorLeft,  intersection_x, context.l_pupil)
-            r_point, r_buffor = self.__pupil(
-                r_eye, self.eyeProcessorRight, intersection_x, context.r_pupil)
-
-            context.l_pupil = l_buffor
-            context.r_pupil = r_buffor
-
-            compound_point = np.array(((l_point + r_point)/2), dtype=np.uint32)
-
-            blink = l_eye.getBlink() or r_eye.getBlink()
-            if blink != True:
-                context.gazeBuffor.add(compound_point)
-
-            if blink != True:
-                # current face radius
-                face_x,face_y,face_w,face_h = self.face.getBoundingBox()
-                image_w = self.face.image_w
-                image_h = self.face.image_h
-
-                face_w_perc = face_w/image_w
-                face_h_perc = face_h/image_h
-
-                # # prev current face radius
-                c_face_x,c_face_y,c_face_w,c_face_h,c_image_w,c_image_h = context.face
-
-                c_face_w_perc = c_face_w/c_image_w
-                c_face_h_perc = c_face_h/c_image_h
-
-                x,y,w,h=self.face.getBoundingBox()
-                i_w = self.face.image_w
-                i_h = self.face.image_h
-                context.face = (x,y,w,h,i_w,i_h)
-
-                # roi update
-
-                # context.roi.x -= diff_face_x * 500 # current size of virtual display
-                # context.roi.y -= diff_face_y * 500 # current size of virtual display
-                if abs(face_w_perc/c_face_w_perc - 1.0) > 0.02:
-                    context.roi.width  = context.roi.width * abs(face_w_perc/c_face_w_perc)
-                    # context.edges.width= context.edges.width * abs(face_w_perc/c_face_w_perc)
-                    context.gazeBuffor.flush()
-                    # context.calibration = True
-                if abs(face_h_perc/c_face_h_perc - 1.0) > 0.02:
-                    context.roi.height = context.roi.height* abs(face_h_perc/c_face_h_perc)
-                    # context.edges.height= context.edges.height * abs(face_w_perc/c_face_w_perc)
-                    context.gazeBuffor.flush()
-                    # context.calibration = True
-
-            self.point_screen, roi, cluster = self.screen_man.process(context.gazeBuffor,
-                                                                      context.roi,
-                                                                      context.edges,
-                                                                      self.screen,
-                                                                      context.display,
-                                                                      context.calibration,
-                                                                      (offset_x,
-                                                                       offset_y)
-                                                                      )
-
-            context.roi = roi
-            if cluster:
-                x, y, width, height = cluster.getBoundaries()
-                context.cluster_boundaries.x = x
-                context.cluster_boundaries.y = y
-                context.cluster_boundaries.width = width
-                context.cluster_boundaries.height = height
-
-            self.GContext.update(context_id, context)
-
-            ###########################################################
-
-            fix = context.fixation.process(
-                self.point_screen[0], self.point_screen[1])
-            # this should prevent of sudden movement down when blinking - not perfect yet
-
-            if fix > fixation_freeze:
-                r = freeze_radius
-                if not isInside(self.freezed_point[0], self.freezed_point[1], r, self.point_screen[0], self.point_screen[1]):
-                    self.freezed_point = self.point_screen
-
-                event = Gevent(self.freezed_point,
-                               blink,
-                               fix,
-                               l_eye,
-                               r_eye,
-                               display,
-                               context.roi,
-                               context.edges,
-                               context.cluster_boundaries,
-                               context_id)
-            else:
-                self.freezed_point = self.point_screen
-                event = Gevent(self.point_screen,
-                               blink,
-                               fix,
-                               l_eye,
-                               r_eye,
-                               display,
-                               context.roi,
-                               context.edges,
-                               context.cluster_boundaries,
-                               context_id)
-
-        return event
-
-    # def get_contextes(self):
-    #     """Function returning contextes"""
-
-    #     return self.GContext.get_contextes()
-
-    # def add_offset(self,x,y):
-    #     """Function adding offsets to tracker"""
-
-    #     self.screen_man.push_window(x,y)
-
-    def getFeatures(self, image):
-        """Function returning face landmarks"""
-
-        face_mesh = self.finder.find(image)
-        return face_mesh
+
+import numpy as np
+from eyeGestures.gevent import Gevent
+from eyeGestures.face import FaceFinder, Face
+from eyeGestures.Fixation import Fixation
+from eyeGestures.processing import EyeProcessor
+from eyeGestures.gazeContexter import GazeContext
+from eyeGestures.screenTracker.screenTracker import ScreenManager
+import eyeGestures.screenTracker.dataPoints as dp
+from eyeGestures.utils import Buffor
+
+
+def isInside(circle_x, circle_y, r, x, y):
+    """Function checking if points are inside the circle"""
+
+    # Compare radius of circle
+    # with distance of its center
+    # from given point
+    if ((x - circle_x) * (x - circle_x) +
+            (y - circle_y) * (y - circle_y) <= r * r):
+        return True
+    else:
+        return False
+
+
+class GazeTracker:
+    """Class processing images and returning gaze tracker"""
+
+    N_FEATURES = 16
+
+    def __init__(self, screen_width, screen_heigth,
+                 eye_screen_w, eye_screen_h,
+                 roi_x, roi_y,
+                 roi_width, roi_height,
+                 monitor_offset_x=0,
+                 monitor_offset_y=0):
+
+        self.screen = dp.Screen(screen_width, screen_heigth)
+
+        self.offset_x = 0
+        self.offset_y = 0
+
+        self.roi_x = roi_x
+        self.roi_y = roi_y
+        self.roi_width = roi_width
+        self.roi_height = roi_height
+
+        self.eye_screen_w = eye_screen_w
+        self.eye_screen_h = eye_screen_h
+
+        self.eyeProcessorLeft = EyeProcessor(eye_screen_w, eye_screen_h)
+        self.eyeProcessorRight = EyeProcessor(eye_screen_w, eye_screen_h)
+
+        self.screen_man = ScreenManager()
+
+        self.finder = FaceFinder()
+
+        # those are used for analysis
+        self.__headDir = [0.5, 0.5]
+
+        self.point_screen = [0.0, 0.0]
+        self.freezed_point = [0.0, 0.0]
+
+        self.face = Face()
+        self.GContext = GazeContext()
+    #     self.calibration = False
+
+    def __gaze_intersection(self, l_eye, r_eye, l_buff, r_buff):
+        l_pupil = l_eye.getPupil()
+        l_gaze = l_eye.getGaze(l_buff)
+
+        r_pupil = r_eye.getPupil()
+        r_gaze = r_eye.getGaze(r_buff)
+
+        l_end = l_gaze + l_pupil
+        r_end = r_gaze + r_pupil
+
+        l_m = (l_end[1] - l_pupil[1])/(l_end[0] - l_pupil[0])
+        r_m = (r_end[1] - r_pupil[1])/(r_end[0] - r_pupil[0])
+
+        l_b = l_end[1] - l_m * l_end[0]
+        r_b = r_end[1] - r_m * r_end[0]
+
+        i_x = (r_b - l_b)/(l_m - r_m)
+        i_y = r_m * i_x + r_b
+        return (i_x, i_y)
+
+    def __pupil(self, eye, eyeProcessor, intersection_x, buffor):
+
+        eyeProcessor.append(eye.getPupil(), eye.getLandmarks(), buffor)
+        point = eyeProcessor.getAvgPupil(
+            self.eye_screen_w, self.eye_screen_h, buffor)
+        point = np.array((int(intersection_x), point[1]))
+
+        return point, buffor
+
+    def estimate(self,
+                 image,
+                 display,
+                 context_id,
+                 calibration,
+                 fixation_freeze=0.7,
+                 freeze_radius=20,
+                 offset_x=0,
+                 offset_y=0):
+        """Function estimating gaze and returning gaze event based on image"""
+
+        event = None
+        face_mesh = self.getFeatures(image)
+        if not face_mesh:
+            return None
+
+        self.face.process(image, face_mesh)
+
+        context = self.GContext.get(context_id, display,
+            face = None,
+            roi =dp.ScreenROI(
+                self.roi_x,
+                self.roi_y,
+                self.roi_width,
+                self.roi_height),
+            edges=dp.ScreenROI(285, 105, 80, 15),
+            cluster_boundaries=dp.ScreenROI(225, 125, 20, 20),
+            buffor=Buffor(200),
+            l_pupil=Buffor(20),
+            r_pupil=Buffor(20),
+            l_eye_buff=Buffor(20),
+            r_eye_buff=Buffor(20),
+            fixation=Fixation(0, 0, 100))
+        context.calibration = calibration
+
+        if not self.face is None:
+
+            if context.face == None:
+                x,y,w,h=self.face.getBoundingBox()
+                i_w = self.face.image_w
+                i_h = self.face.image_h
+                context.face = (x,y,w,h,i_w,i_h)
+
+
+            l_eye = self.face.getLeftEye()
+            r_eye = self.face.getRightEye()
+
+            # TODO: check what happens here before with l_pupil
+            intersection_x, _ = self.__gaze_intersection(
+                l_eye, r_eye, context.l_eye_buff, context.r_eye_buff)
+            l_point, l_buffor = self.__pupil(
+                l_eye, self.eyeProcessorLeft,  intersection_x, context.l_pupil)
+            r_point, r_buffor = self.__pupil(
+                r_eye, self.eyeProcessorRight, intersection_x, context.r_pupil)
+
+            context.l_pupil = l_buffor
+            context.r_pupil = r_buffor
+
+            compound_point = np.array(((l_point + r_point)/2), dtype=np.uint32)
+
+            blink = l_eye.getBlink() or r_eye.getBlink()
+            if blink != True:
+                context.gazeBuffor.add(compound_point)
+
+            if blink != True:
+                # current face radius
+                face_x,face_y,face_w,face_h = self.face.getBoundingBox()
+                image_w = self.face.image_w
+                image_h = self.face.image_h
+
+                face_w_perc = face_w/image_w
+                face_h_perc = face_h/image_h
+
+                # # prev current face radius
+                c_face_x,c_face_y,c_face_w,c_face_h,c_image_w,c_image_h = context.face
+
+                c_face_w_perc = c_face_w/c_image_w
+                c_face_h_perc = c_face_h/c_image_h
+
+                x,y,w,h=self.face.getBoundingBox()
+                i_w = self.face.image_w
+                i_h = self.face.image_h
+                context.face = (x,y,w,h,i_w,i_h)
+
+                # roi update
+
+                # context.roi.x -= diff_face_x * 500 # current size of virtual display
+                # context.roi.y -= diff_face_y * 500 # current size of virtual display
+                if abs(face_w_perc/c_face_w_perc - 1.0) > 0.02:
+                    context.roi.width  = context.roi.width * abs(face_w_perc/c_face_w_perc)
+                    # context.edges.width= context.edges.width * abs(face_w_perc/c_face_w_perc)
+                    context.gazeBuffor.flush()
+                    # context.calibration = True
+                if abs(face_h_perc/c_face_h_perc - 1.0) > 0.02:
+                    context.roi.height = context.roi.height* abs(face_h_perc/c_face_h_perc)
+                    # context.edges.height= context.edges.height * abs(face_w_perc/c_face_w_perc)
+                    context.gazeBuffor.flush()
+                    # context.calibration = True
+
+            self.point_screen, roi, cluster = self.screen_man.process(context.gazeBuffor,
+                                                                      context.roi,
+                                                                      context.edges,
+                                                                      self.screen,
+                                                                      context.display,
+                                                                      context.calibration,
+                                                                      (offset_x,
+                                                                       offset_y)
+                                                                      )
+
+            context.roi = roi
+            if cluster:
+                x, y, width, height = cluster.getBoundaries()
+                context.cluster_boundaries.x = x
+                context.cluster_boundaries.y = y
+                context.cluster_boundaries.width = width
+                context.cluster_boundaries.height = height
+
+            self.GContext.update(context_id, context)
+
+            ###########################################################
+
+            fix = context.fixation.process(
+                self.point_screen[0], self.point_screen[1])
+            # this should prevent of sudden movement down when blinking - not perfect yet
+
+            if fix > fixation_freeze:
+                r = freeze_radius
+                if not isInside(self.freezed_point[0], self.freezed_point[1], r, self.point_screen[0], self.point_screen[1]):
+                    self.freezed_point = self.point_screen
+
+                event = Gevent(self.freezed_point,
+                               blink,
+                               fix,
+                               l_eye,
+                               r_eye,
+                               display,
+                               context.roi,
+                               context.edges,
+                               context.cluster_boundaries,
+                               context_id)
+            else:
+                self.freezed_point = self.point_screen
+                event = Gevent(self.point_screen,
+                               blink,
+                               fix,
+                               l_eye,
+                               r_eye,
+                               display,
+                               context.roi,
+                               context.edges,
+                               context.cluster_boundaries,
+                               context_id)
+
+        return event
+
+    # def get_contextes(self):
+    #     """Function returning contextes"""
+
+    #     return self.GContext.get_contextes()
+
+    # def add_offset(self,x,y):
+    #     """Function adding offsets to tracker"""
+
+    #     self.screen_man.push_window(x,y)
+
+    def getFeatures(self, image):
+        """Function returning face landmarks"""
+
+        face_mesh = self.finder.find(image)
+        return face_mesh
```

### Comparing `eyegestures-2.0.0/eyeGestures/gevent.py` & `eyegestures-2.1.0/eyeGestures/gevent.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""Module providing a Gaze Events."""
-
-
-class Gevent:
-    """Class representing gaze event, with tracked points scaled to screen, blink and fixation."""
-
-    def __init__(self,
-                 point,
-                 blink,
-                 fixation,
-                 l_eye = None,
-                 r_eye = None,
-                 screen_man = None,
-                 roi = None,
-                 edges = None,
-                 cluster = None,
-                 context = None):
-
-        self.point = point
-        self.blink = blink
-        self.fixation = fixation
-
-        # ALL DEBUG DATA
-        self.roi = roi
-        self.edges = edges
-        self.l_eye = l_eye
-        self.r_eye = r_eye
-        self.cluster = cluster
-        self.context = context
-        self.screen_man = screen_man
-
-
-class Cevent:
-    """Class representing gaze event, with tracked points scaled to screen, blink and fixation."""
-
-    def __init__(self,
-                 point,
-                 acceptance_radius,
-                 calibration_radius,
-                 calibration = False):
-
-        self.point = point
-        self.acceptance_radius = acceptance_radius
-        self.calibration_radius = calibration_radius
-        self.calibration = calibration
+"""Module providing a Gaze Events."""
+
+
+class Gevent:
+    """Class representing gaze event, with tracked points scaled to screen, blink and fixation."""
+
+    def __init__(self,
+                 point,
+                 blink,
+                 fixation,
+                 l_eye = None,
+                 r_eye = None,
+                 screen_man = None,
+                 roi = None,
+                 edges = None,
+                 cluster = None,
+                 context = None):
+
+        self.point = point
+        self.blink = blink
+        self.fixation = fixation
+
+        # ALL DEBUG DATA
+        self.roi = roi
+        self.edges = edges
+        self.l_eye = l_eye
+        self.r_eye = r_eye
+        self.cluster = cluster
+        self.context = context
+        self.screen_man = screen_man
+
+
+class Cevent:
+    """Class representing gaze event, with tracked points scaled to screen, blink and fixation."""
+
+    def __init__(self,
+                 point,
+                 acceptance_radius,
+                 calibration_radius,
+                 calibration = False):
+
+        self.point = point
+        self.acceptance_radius = acceptance_radius
+        self.calibration_radius = calibration_radius
+        self.calibration = calibration
```

### Comparing `eyegestures-2.0.0/eyeGestures/screenTracker_test.py` & `eyegestures-2.1.0/eyeGestures/screenTracker_test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import eyeGestures.screenTracker.dataPoints as dp
-import eyeGestures.screenTracker.screenTracker as scrtr
-
-# virtual tracking ScreenProcessor
-SCREEN_WIDTH = 500
-SCREEN_HEIGHT = 500
-
-# region of interest inside the virtual ScreenProcessor
-ROI_WIDTH = 50
-ROI_HEIGHT = 50
-
-# size of real display
-DISPLAY_WIDTH = 1200
-DISPLAY_HEIGHT = 1800
-
-####################### ScreenProcessor 2 display Tests #################################
-
-
-def test_screen2display_1_1():
-    """[TEST]"""
-    point = (1, 1)
-
-    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (point[0]/ROI_WIDTH * DISPLAY_WIDTH,
-                 point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
-
-
-def test_screen2display_55_1():
-    """[TEST]"""
-    point = (55, 1)
-
-    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (DISPLAY_WIDTH,
-                 point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
-
-
-def test_screen2display_55_55():
-    """[TEST]"""
-    point = (55, 55)
-
-    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (DISPLAY_WIDTH,
-                 DISPLAY_HEIGHT)
-
-
-def test_screen2display_0_0():
-    """[TEST]"""
-    point = (0, 0)
-
-    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (0, 0)
-
-
-def test_screen2display_1_1_pos_50_50():
-    """[TEST]"""
-    point = (51, 51)
-    pos = (50, 50)
-
-    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == ((point[0] - pos[0])/ROI_WIDTH * DISPLAY_WIDTH,
-                 (point[1] - pos[1])/ROI_HEIGHT * DISPLAY_HEIGHT)
-
-
-def test_screen2display_55_55_pos_50_50():
-    """[TEST]"""
-    point = (105, 105)
-    pos = (50, 50)
-
-    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (DISPLAY_WIDTH,
-                 DISPLAY_HEIGHT)
-
-
-def test_screen2display_0_0_pos_50_50():
-    """[TEST]"""
-    point = (0, 0)
-    pos = (50, 50)
-
-    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
-
-    tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point, roi, display)
-
-    assert p == (0, 0)
+import eyeGestures.screenTracker.dataPoints as dp
+import eyeGestures.screenTracker.screenTracker as scrtr
+
+# virtual tracking ScreenProcessor
+SCREEN_WIDTH = 500
+SCREEN_HEIGHT = 500
+
+# region of interest inside the virtual ScreenProcessor
+ROI_WIDTH = 50
+ROI_HEIGHT = 50
+
+# size of real display
+DISPLAY_WIDTH = 1200
+DISPLAY_HEIGHT = 1800
+
+####################### ScreenProcessor 2 display Tests #################################
+
+
+def test_screen2display_1_1():
+    """[TEST]"""
+    point = (1, 1)
+
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (point[0]/ROI_WIDTH * DISPLAY_WIDTH,
+                 point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
+
+
+def test_screen2display_55_1():
+    """[TEST]"""
+    point = (55, 1)
+
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (DISPLAY_WIDTH,
+                 point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
+
+
+def test_screen2display_55_55():
+    """[TEST]"""
+    point = (55, 55)
+
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (DISPLAY_WIDTH,
+                 DISPLAY_HEIGHT)
+
+
+def test_screen2display_0_0():
+    """[TEST]"""
+    point = (0, 0)
+
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (0, 0)
+
+
+def test_screen2display_1_1_pos_50_50():
+    """[TEST]"""
+    point = (51, 51)
+    pos = (50, 50)
+
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == ((point[0] - pos[0])/ROI_WIDTH * DISPLAY_WIDTH,
+                 (point[1] - pos[1])/ROI_HEIGHT * DISPLAY_HEIGHT)
+
+
+def test_screen2display_55_55_pos_50_50():
+    """[TEST]"""
+    point = (105, 105)
+    pos = (50, 50)
+
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (DISPLAY_WIDTH,
+                 DISPLAY_HEIGHT)
+
+
+def test_screen2display_0_0_pos_50_50():
+    """[TEST]"""
+    point = (0, 0)
+    pos = (50, 50)
+
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
+
+    tracker = scrtr.ScreenProcessor()
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (0, 0)
```

### Comparing `eyegestures-2.0.0/eyeGestures/utils.py` & `eyegestures-2.1.0/eyeGestures/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,198 +1,202 @@
-import time
-import queue
-import pickle
-import platform
-import threading
-
-import cv2
-import numpy as np
-
-# Make predictions for new data points
-
-
-def timeit(func):
-    """
-    timeit
-    """
-    def inner(*args, **kwargs):
-        """
-        inner
-        """
-        start = time.time()
-        ret = func(*args, **kwargs)
-        print(f"Elapsed time: {time.time() - start}")
-        return ret
-    return inner
-
-
-def shape_to_np(shape, dtype="int"):
-    """
-    shape_to_np
-    """
-    coords = np.zeros((68, 2), dtype=dtype)
-    for i in range(0, 68):
-        coords[i] = (shape.part(i).x, shape.part(i).y)
-    return coords
-
-
-def make_image_grid(images, rows, cols):
-    """
-    Make a grid of images.
-
-    Parameters:
-    - images: list of images to form the grid (all images must be of the same size and type)
-    - rows, cols: number of rows and columns in the grid
-
-    Returns:
-    - grid_image: image grid as a single image
-    """
-    # Check if the list of images is not empty and that we have enough to fill the grid
-    assert images, "List of images is empty"
-    # assert len(images) >= rows * cols, "Not enough images to fill the grid"
-
-    # Get image dimensions
-    img_h, img_w = images[0].shape[:2]
-
-    if len(images[0].shape) > 2:
-        # Create a black canvas to draw the grid on
-        grid_image = np.zeros(
-            (img_h * rows, img_w * cols, images[0].shape[2]), dtype=np.uint8)
-    else:
-        grid_image = np.zeros((img_h * rows, img_w * cols), dtype=np.uint8)
-
-    # Copy images to the grid
-    for i, img in enumerate(images):
-        if i >= rows * cols:
-            break  # Stop if we have filled the grid
-        row = i // cols
-        col = i % cols
-        grid_image[row * img_h:(row + 1) * img_h, col *
-                   img_w:(col + 1) * img_w] = img
-
-    return grid_image
-
-
-class var:
-
-    def __init__(self, var):
-        self.__var = var
-
-    def set(self, var):
-        self.__var = var
-
-    def get(self):
-        return self.__var
-
-
-class Buffor:
-
-    def __init__(self, length):
-        self.length = length
-        self.__buffor = []
-
-    def add(self, var):
-        if len(self.__buffor) >= self.length:
-            self.__buffor.pop(0)
-
-        self.__buffor.append(var)
-
-    def getAvg(self, lenght=0):
-        return np.sum(self.__buffor[-lenght:], axis=0) / len(self.__buffor[-lenght:])
-
-    def getBuffor(self):
-        return self.__buffor
-
-    def loadBuffor(self, buffor):
-        self.__buffor = buffor
-
-    def getLast(self):
-        return self.__buffor[0]
-
-    def getFirst(self):
-        return self.__buffor[len(self.__buffor) - 1]
-
-    def getLen(self):
-        return len(self.__buffor)
-    
-    def flush(self):
-        tmp = self.__buffor[-1]
-        self.__buffor = []
-        self.__buffor.append(tmp)
-
-    def clear(self):
-        self.__buffor = []
-
-# Bufforless
-
-
-class VideoCapture:
-    """Wrapper on openCV2 stream making it bufforless and adding camera search"""
-
-    def __init__(self, name, bufforless=True):
-        self.bufforless = bufforless
-        self.run = True
-
-        if isinstance(name, str):
-            if ".pkl" in name:
-                self.stream = False
-            else:
-                self.stream = True
-        else:
-            self.stream = True
-
-        if self.stream:
-            self.prev_frame = None
-
-            self.__openCam(name)
-
-            self.q = queue.Queue()
-            self.t = threading.Thread(target=self.__reader)
-            self.t.start()
-        else:
-            self.frames = []
-            with open(name, 'rb') as file:
-                self.frames = pickle.load(file)
-
-    def __openCam(self, name):
-        if isinstance(name, int):
-            if "Windows" in platform.system():
-                self.cap = cv2.VideoCapture(name, cv2.CAP_DSHOW)
-            else:
-                self.cap = cv2.VideoCapture(name)
-
-            if self.cap is None or not self.cap.isOpened():
-                print(f"Was unable to open camera: {name}.")
-                print(f"Trying to open camera: {name}.")
-                if name + 1 < 10:
-                    self.__openCam(name + 1)
-        else:
-            self.cap = cv2.VideoCapture(name)
-
-    def __reader(self):
-        while self.run:
-            ret, frame = self.cap.read()
-            if not ret:
-                break
-            if not self.q.empty() and self.bufforless:
-                try:
-                    self.q.get_nowait()
-                except queue.Empty:
-                    pass
-            self.q.put((ret, frame))
-
-        self.run = False
-
-    def read(self):
-        """Function returning latest frame"""
-        if self.stream:
-            return self.q.get()
-        else:
-            frame = self.frames.pop(0)
-            self.frames.pop(0)
-            return ((len(self.frames) >= 1), frame)
-
-    def close(self):
-        """Function closing stream"""
-        self.run = False
-        self.t.join()
-        self.cap.release()
+import time
+import queue
+import pickle
+import platform
+import threading
+
+import cv2
+import numpy as np
+
+# Make predictions for new data points
+
+
+def timeit(func):
+    """
+    timeit
+    """
+    def inner(*args, **kwargs):
+        """
+        inner
+        """
+        start = time.time()
+        ret = func(*args, **kwargs)
+        print(f"Elapsed time: {time.time() - start}")
+        return ret
+    return inner
+
+
+def shape_to_np(shape, dtype="int"):
+    """
+    shape_to_np
+    """
+    coords = np.zeros((68, 2), dtype=dtype)
+    for i in range(0, 68):
+        coords[i] = (shape.part(i).x, shape.part(i).y)
+    return coords
+
+
+def make_image_grid(images, rows, cols):
+    """
+    Make a grid of images.
+
+    Parameters:
+    - images: list of images to form the grid (all images must be of the same size and type)
+    - rows, cols: number of rows and columns in the grid
+
+    Returns:
+    - grid_image: image grid as a single image
+    """
+    # Check if the list of images is not empty and that we have enough to fill the grid
+    assert images, "List of images is empty"
+    # assert len(images) >= rows * cols, "Not enough images to fill the grid"
+
+    # Get image dimensions
+    img_h, img_w = images[0].shape[:2]
+
+    if len(images[0].shape) > 2:
+        # Create a black canvas to draw the grid on
+        grid_image = np.zeros(
+            (img_h * rows, img_w * cols, images[0].shape[2]), dtype=np.uint8)
+    else:
+        grid_image = np.zeros((img_h * rows, img_w * cols), dtype=np.uint8)
+
+    # Copy images to the grid
+    for i, img in enumerate(images):
+        if i >= rows * cols:
+            break  # Stop if we have filled the grid
+        row = i // cols
+        col = i % cols
+        grid_image[row * img_h:(row + 1) * img_h, col *
+                   img_w:(col + 1) * img_w] = img
+
+    return grid_image
+
+
+class var:
+
+    def __init__(self, var):
+        self.__var = var
+
+    def set(self, var):
+        self.__var = var
+
+    def get(self):
+        return self.__var
+
+
+class Buffor:
+
+    def __init__(self, length):
+        self.length = length
+        self.__buffor = []
+
+    def add(self, var):
+        if len(self.__buffor) >= self.length:
+            self.__buffor.pop(0)
+
+        self.__buffor.append(var)
+
+    def getAvg(self, lenght=0):
+        return np.sum(self.__buffor[-lenght:], axis=0) / len(self.__buffor[-lenght:])
+
+    def getBuffor(self):
+        return self.__buffor
+
+    def loadBuffor(self, buffor):
+        self.__buffor = buffor
+
+    def getLast(self):
+        return self.__buffor[0]
+
+    def getFirst(self):
+        return self.__buffor[len(self.__buffor) - 1]
+
+    def getLen(self):
+        return len(self.__buffor)
+    
+    def flush(self):
+        tmp = self.__buffor[-1]
+        self.__buffor = []
+        self.__buffor.append(tmp)
+
+    def clear(self):
+        self.__buffor = []
+
+# Bufforless
+
+
+class VideoCapture:
+    """Wrapper on openCV2 stream making it bufforless and adding camera search"""
+
+    def __init__(self, name, bufforless=True):
+        self.bufforless = bufforless
+        self.run = True
+
+        if isinstance(name, str):
+            if ".pkl" in name:
+                self.stream = False
+            else:
+                self.stream = True
+        else:
+            self.stream = True
+
+        if self.stream:
+            self.prev_frame = None
+
+            self.__openCam(name)
+
+            self.q = queue.Queue()
+            self.t = threading.Thread(target=self.__reader)
+            self.t.start()
+        else:
+            self.frames = []
+            with open(name, 'rb') as file:
+                self.frames = pickle.load(file)
+
+    def __openCam(self, name):
+        if isinstance(name, int):
+            if "Windows" in platform.system():
+                self.cap = cv2.VideoCapture(name, cv2.CAP_DSHOW)
+            else:
+                self.cap = cv2.VideoCapture(name)
+
+            if self.cap is None or not self.cap.isOpened():
+                print(f"Was unable to open camera: {name}.")
+                print(f"Trying to open camera: {name}.")
+                if name + 1 < 10:
+                    self.__openCam(name + 1)
+        else:
+            self.cap = cv2.VideoCapture(name)
+
+    def __reader(self):
+        while self.run:
+            ret, frame = self.cap.read()
+            if not ret:
+                break
+            if not self.q.empty() and self.bufforless:
+                try:
+                    self.q.get_nowait()
+                except queue.Empty:
+                    pass
+            self.q.put((ret, frame))
+
+        self.flush()
+
+    def flush(self):
+        while not self.q.empty():
+            self.q.get()
+
+    def read(self):
+        """Function returning latest frame"""
+        if self.stream:
+            return self.q.get()
+        else:
+            frame = self.frames.pop(0)
+            self.frames.pop(0)
+            return ((len(self.frames) >= 1), frame)
+
+    def close(self):
+        """Function closing stream"""
+        self.run = False
+        self.t.join()
+        self.cap.release()
```

### Comparing `eyegestures-2.0.0/eyeGestures/screenTracker/clusters.py` & `eyegestures-2.1.0/eyeGestures/screenTracker/clusters.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from sklearn.cluster import DBSCAN
-import numpy as np
-
-class Cluster:
-    """Class representing one ROI cluster"""
-
-    def __init__(self, label, points):
-        
-        self.label    = label
-        self.points   = np.array(points)
-        self.weight   = len(self.points)
-        self.__centroid = self.centroid(points)
-
-        x,y,w,h = self.boundaries(points)
-
-        self.x =  x
-        self.y =  y
-        self.w =  w
-        self.h =  h
-
-    def centroid(self,points):
-        """Function calculating and returning center of ROI"""
-        
-        x,y,w,h = self.boundaries(points)
-
-        c_x, c_y = (x+w/2,y+h/2)
-
-        x,y = sum(points)/len(points)
-
-        c_x, c_y = (c_x + x)/2, (c_y + y)/2
-        return (c_x, c_y)
-
-    def boundaries(self,points):
-        """Function calculating and returning boundaries of cluster"""
-
-        x = np.min(points[:,0]) 
-        width = abs(np.max(points[:,0]) - x) 
-
-        y = np.min(points[:,1]) 
-        height = abs(np.max(points[:,1]) - y) 
-
-        return (x,y,width,height)
-    
-    def getBoundaries(self):
-        """Function returning boundaries of cluster"""
-        return (self.x,self.y,self.w,self.h)
-    
-    def getCenter(self):
-        """Function returning center of ROI"""
-        return (self.__centroid)
-    
-class Clusters:
-    """Algorithm dividing tracked points into clusters so it can be estimated were is center of ROI"""
-
-    def __init__(self,buffer):
-        buffer = np.array(buffer)
-        
-        self.head = len(buffer) - 1
-        self.main_cluster = None
-        self.clusters = []
-
-        dbScan     = DBSCAN(eps=12, min_samples=3)
-        clustering = dbScan.fit(buffer)
-
-        labels = clustering.labels_
-        unique_labels = set(labels) - {-1}
-
-        for u_label in unique_labels:
-            core_sample_indices = clustering.core_sample_indices_
-            cluster_points = buffer[core_sample_indices][labels[clustering.core_sample_indices_] == u_label]
-            self.clusters.append(Cluster(u_label,cluster_points))
-
-        # return sorted(self.clusters, key=lambda cluster: cluster.weight)[-1]
-        if len(self.clusters) > 0:
-            self.main_cluster = self.clusters[
-                    labels[self.head]
-                ]
-        else:
-            self.main_cluster = None
-
-    def clearPoints(self):
-        """[Possibly dead code] Function reseting cluster"""
-        self.head = 0
-
-    def getClusters(self):
-        """Function returning all clusters"""
-        return self.clusters
-    
-    def getMainCluster(self):
-        """Function returning main clusters"""
-        return self.main_cluster
+from sklearn.cluster import DBSCAN
+import numpy as np
+
+class Cluster:
+    """Class representing one ROI cluster"""
+
+    def __init__(self, label, points):
+        
+        self.label    = label
+        self.points   = np.array(points)
+        self.weight   = len(self.points)
+        self.__centroid = self.centroid(points)
+
+        x,y,w,h = self.boundaries(points)
+
+        self.x =  x
+        self.y =  y
+        self.w =  w
+        self.h =  h
+
+    def centroid(self,points):
+        """Function calculating and returning center of ROI"""
+        
+        x,y,w,h = self.boundaries(points)
+
+        c_x, c_y = (x+w/2,y+h/2)
+
+        x,y = sum(points)/len(points)
+
+        c_x, c_y = (c_x + x)/2, (c_y + y)/2
+        return (c_x, c_y)
+
+    def boundaries(self,points):
+        """Function calculating and returning boundaries of cluster"""
+
+        x = np.min(points[:,0]) 
+        width = abs(np.max(points[:,0]) - x) 
+
+        y = np.min(points[:,1]) 
+        height = abs(np.max(points[:,1]) - y) 
+
+        return (x,y,width,height)
+    
+    def getBoundaries(self):
+        """Function returning boundaries of cluster"""
+        return (self.x,self.y,self.w,self.h)
+    
+    def getCenter(self):
+        """Function returning center of ROI"""
+        return (self.__centroid)
+    
+class Clusters:
+    """Algorithm dividing tracked points into clusters so it can be estimated were is center of ROI"""
+
+    def __init__(self,buffer):
+        buffer = np.array(buffer)
+        
+        self.head = len(buffer) - 1
+        self.main_cluster = None
+        self.clusters = []
+
+        dbScan     = DBSCAN(eps=12, min_samples=3)
+        clustering = dbScan.fit(buffer)
+
+        labels = clustering.labels_
+        unique_labels = set(labels) - {-1}
+
+        for u_label in unique_labels:
+            core_sample_indices = clustering.core_sample_indices_
+            cluster_points = buffer[core_sample_indices][labels[clustering.core_sample_indices_] == u_label]
+            self.clusters.append(Cluster(u_label,cluster_points))
+
+        # return sorted(self.clusters, key=lambda cluster: cluster.weight)[-1]
+        if len(self.clusters) > 0:
+            self.main_cluster = self.clusters[
+                    labels[self.head]
+                ]
+        else:
+            self.main_cluster = None
+
+    def clearPoints(self):
+        """[Possibly dead code] Function reseting cluster"""
+        self.head = 0
+
+    def getClusters(self):
+        """Function returning all clusters"""
+        return self.clusters
+    
+    def getMainCluster(self):
+        """Function returning main clusters"""
+        return self.main_cluster
```

### Comparing `eyegestures-2.0.0/eyeGestures/screenTracker/dataPoints.py` & `eyegestures-2.1.0/eyeGestures/screenTracker/dataPoints.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import math
-import numpy as np
-
-from scipy import signal
-
-class Center():
-    """Helper representing Center of object with x,y,width,height"""
-
-    def __init__(self,x,y,width,height):
-        self.x = (x + width)/2
-        self.y = (y + height)/2
-
-class Screen():
-    """Helper representing screen by making box of width,height"""
-
-    def __init__(self,width,height):
-        self.x = 0
-        self.y = 0
-        self.width = width
-        self.height= height
-
-    def getCenter(self):
-        """Function returnig center of the screen"""
-        return Center(self.x,self.y,self.width, self.height)
-
-class ScreenROI():
-    """Helper representing ROI by making box of width,height with x and y offset"""
-
-    def __init__(self,x,y,width,height):
-        self.x = x 
-        self.y = y
-        self.width = width
-        self.height= height
-
-    def setCenter(self,x, y):
-        """Function allowing to move ROI by changing its center"""
-        self.x = x - self.width/2
-        self.y = y - self.height/2
-
-    def getCenter(self):
-        """Function returnig center of the ROI"""
-        return Center(self.x, self.y, self.width, self.height)
-
-    def getBoundaries(self):
-        """Function returnig boundaries of the ROI"""
-        return (self.x,self.y,self.width, self.height)
-
-
-class Display():
-    """Helper representing Display by making box of width,height with x and y offset"""
-
-    def __init__(self,width,height,offset_x,offset_y):
-        self.width = width
-        self.height = height
-        self.offset_x = offset_x
-        self.offset_y = offset_y
-
-        # self.buffor = Buffor(20)
-
-    def getCenter(self):
-        """Function returnig center of the Display"""
-        return self.__center
+import math
+import numpy as np
+
+from scipy import signal
+
+class Center():
+    """Helper representing Center of object with x,y,width,height"""
+
+    def __init__(self,x,y,width,height):
+        self.x = (x + width)/2
+        self.y = (y + height)/2
+
+class Screen():
+    """Helper representing screen by making box of width,height"""
+
+    def __init__(self,width,height):
+        self.x = 0
+        self.y = 0
+        self.width = width
+        self.height= height
+
+    def getCenter(self):
+        """Function returnig center of the screen"""
+        return Center(self.x,self.y,self.width, self.height)
+
+class ScreenROI():
+    """Helper representing ROI by making box of width,height with x and y offset"""
+
+    def __init__(self,x,y,width,height):
+        self.x = x 
+        self.y = y
+        self.width = width
+        self.height= height
+
+    def setCenter(self,x, y):
+        """Function allowing to move ROI by changing its center"""
+        self.x = x - self.width/2
+        self.y = y - self.height/2
+
+    def getCenter(self):
+        """Function returnig center of the ROI"""
+        return Center(self.x, self.y, self.width, self.height)
+
+    def getBoundaries(self):
+        """Function returnig boundaries of the ROI"""
+        return (self.x,self.y,self.width, self.height)
+
+
+class Display():
+    """Helper representing Display by making box of width,height with x and y offset"""
+
+    def __init__(self,width,height,offset_x,offset_y):
+        self.width = width
+        self.height = height
+        self.offset_x = offset_x
+        self.offset_y = offset_y
+
+        # self.buffor = Buffor(20)
+
+    def getCenter(self):
+        """Function returnig center of the Display"""
+        return self.__center
```

### Comparing `eyegestures-2.0.0/eyeGestures/screenTracker/heatmap.py` & `eyegestures-2.1.0/eyeGestures/screenTracker/heatmap.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import numpy as np
-
-class Heatmap():
-    """Helper representing Heatmap of tracked points"""
-
-    def __init__(self,width,height,buffor):
-        self.inc_step = 10
-        self.step = 10
-        bars = self.step
-
-        self.width = width
-        self.height = height
-
-        bars_x = int(width/self.step)
-        bars_y = int(height/self.step)
-
-        self.axis_x = np.zeros((bars_x))
-        self.axis_y = np.zeros((bars_y))
-
-        for point in buffor:
-            x = point[0]
-            y = point[1]
-
-            self.axis_x[min(abs(int(x/bars)),bars_x - 1)] += self.inc_step
-            self.axis_y[min(abs(int(y/bars)),bars_x - 1)] += self.inc_step
-
-        self.min_x = self.__getParam((self.axis_x > self.inc_step*4),last=False)
-        self.max_x = self.__getParam((self.axis_x > self.inc_step*4),last=True)
-        self.min_y = self.__getParam((self.axis_y > self.inc_step*4),last=False)
-        self.max_y = self.__getParam((self.axis_y > self.inc_step*4),last=True)
-
-    def __getParam(self,param,last : bool = False):
-        ret = 0
-        retArray = np.where(param)
-
-        if len(retArray[0]) > 0:
-            ret = retArray[0][- int(last)] * self.step
-
-            if not ret == np.NAN:
-                ret = int(ret)
-
-        return ret
-
-    def getBoundaries(self):
-        """Function returning boundaries of heatmap"""
-        x = self.min_x
-        y = self.min_y
-        w = self.max_x - self.min_x
-        h = self.max_y - self.min_y
-        return (x,y,w,h)
-
-    def getCenter(self):
-        """Function returning center of heatmap"""
-        center_x = int((self.max_x - self.min_x)/2 + self.min_x)
-        center_y = int((self.max_y - self.min_y)/2 + self.min_y)
-        return (center_x,center_y)
-
-    def getPeak(self):
-        """Function returning peak of heatmap"""
-        x = int(np.argmax(self.axis_x)*self.inc_step)
-        y = int(np.argmax(self.axis_y)*self.inc_step)
-        return (x,y)
-
-    def getHist(self):
-        """Function returning histogram of the heatmap. This heatmap is simply 2d histogram, so this function returns values for each axis."""
-        return (self.axis_x/self.inc_step,self.axis_y/self.inc_step)
+import numpy as np
+
+class Heatmap():
+    """Helper representing Heatmap of tracked points"""
+
+    def __init__(self,width,height,buffor):
+        self.inc_step = 10
+        self.step = 10
+        bars = self.step
+
+        self.width = width
+        self.height = height
+
+        bars_x = int(width/self.step)
+        bars_y = int(height/self.step)
+
+        self.axis_x = np.zeros((bars_x))
+        self.axis_y = np.zeros((bars_y))
+
+        for point in buffor:
+            x = point[0]
+            y = point[1]
+
+            self.axis_x[min(abs(int(x/bars)),bars_x - 1)] += self.inc_step
+            self.axis_y[min(abs(int(y/bars)),bars_x - 1)] += self.inc_step
+
+        self.min_x = self.__getParam((self.axis_x > self.inc_step*4),last=False)
+        self.max_x = self.__getParam((self.axis_x > self.inc_step*4),last=True)
+        self.min_y = self.__getParam((self.axis_y > self.inc_step*4),last=False)
+        self.max_y = self.__getParam((self.axis_y > self.inc_step*4),last=True)
+
+    def __getParam(self,param,last : bool = False):
+        ret = 0
+        retArray = np.where(param)
+
+        if len(retArray[0]) > 0:
+            ret = retArray[0][- int(last)] * self.step
+
+            if not ret == np.NAN:
+                ret = int(ret)
+
+        return ret
+
+    def getBoundaries(self):
+        """Function returning boundaries of heatmap"""
+        x = self.min_x
+        y = self.min_y
+        w = self.max_x - self.min_x
+        h = self.max_y - self.min_y
+        return (x,y,w,h)
+
+    def getCenter(self):
+        """Function returning center of heatmap"""
+        center_x = int((self.max_x - self.min_x)/2 + self.min_x)
+        center_y = int((self.max_y - self.min_y)/2 + self.min_y)
+        return (center_x,center_y)
+
+    def getPeak(self):
+        """Function returning peak of heatmap"""
+        x = int(np.argmax(self.axis_x)*self.inc_step)
+        y = int(np.argmax(self.axis_y)*self.inc_step)
+        return (x,y)
+
+    def getHist(self):
+        """Function returning histogram of the heatmap. This heatmap is simply 2d histogram, so this function returns values for each axis."""
+        return (self.axis_x/self.inc_step,self.axis_y/self.inc_step)
```

### Comparing `eyegestures-2.0.0/LICENSE` & `eyegestures-2.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `eyegestures-2.0.0/README.md` & `eyegestures-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,182 +1,197 @@
-<p align="center">
-  <picture>
-    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/ddfc8b96-5a7e-4487-9307-6fbd62e8915e" media="(prefers-color-scheme: light)"/>   
-    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/6d42b8a2-24ea-4cbc-bdb0-ad688ee26c36" media="(prefers-color-scheme: dark)"/>    
-   <img width="300px" height="300px"/>
-  </picture>
-</p>
-
-## EYEGESTURES
-
-
-EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
-
-Our [Mission](https://github.com/NativeSensors/EyeGestures/blob/Engine_v2/MISSION.md)! 
-
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
-<a href="https://polar.sh/NativeSensors"><img src="https://polar.sh/embed/seeks-funding-shield.svg?org=NativeSensors" /></a>
-### 💜 Sponsors: 
-
-```
-For enterprise avoiding GPL3 licensing there is commercial license!
-```
-We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
-
-```
-Sponsor us and we can add your link, banner or other promo materials!
-```
-<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
-
-
-
-<!-- POLAR-END id=eizdelwu -->
-
-<p align="center">
-  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
-<img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
-" height="150">
-</p>
-<p align="center">
-  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/3b38d73d-bb6f-4f31-b67d-231ac4cd04cb" width="300" height="150">
-  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/1715b4df-7ac3-479e-b51a-f6d800ea8ea5" width="300" height="150">
-</p>
-
-<p align="center">
-  <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
-</p>
-
-### 💻 Install
-```
-python3 -m pip install eyeGestures
-```
-
-### ⚙️ Run 
-```
-python3 examples/simple_example.py
-```
-
-### 🪟 Run Windows App 
-```
-python3 apps/win_app.py
-```
-
-Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
-
-### 🔧 How to use [WiP - adding Enginge V2]:
-
-#### Using EyeGesture Engine V2 - Machine Learning Approach:
-
-```python
-from eyeGestures.utils import VideoCapture
-from eyeGestures.eyegestures import EyeGestures_v2
-
-# Initialize gesture engine and video capture
-gestures = EyeGestures_v2()
-cap = VideoCapture(0)  
-
-# Process each frame
-point, calibration_point, blink, fixation, acceptance_radius, calibration_radius = gestures.step(frame, calibrate, screen_width, screen_height)
-# point: x, y positions of cursor
-# calibration_point: x, y position of current calibration point
-# acceptance_radius: precision required for calibration
-# calibration_radius: radius for data collection during calibration
-```
-
-<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
-
-
-
-<!-- POLAR-END id=eizdelwu -->
-
-#### Using EyeGesture Engine V1 - Model-Based Approach:
-
-```python
-from eyeGestures.utils import VideoCapture
-from eyeGestures.eyegestures import EyeGestures_v1
-
-# Initialize gesture engine with RoI parameters
-gestures = EyeGestures_v1()
-
-cap = VideoCapture(0)  
-ret, frame = cap.read()
-
-# Obtain estimations from camera frames
-event = gestures.estimate(
-    frame,
-    "main",
-    True,  # set calibration - switch to False to stop calibration
-    screen_width,
-    screen_height,
-    0, 0, 0.8, 10
-)
-cursor_x, cursor_y = event.point[0], event.point[1]
-```
-
-Feel free to copy and paste the relevant code snippets for your project.
-
-### 🔥 Web Demos:
-
-- [Main page](https://eyegestures.com/)
-- [Game demo](https://eyegestures.com/game)
-- [Cinema demo](https://eyegestures.com/cinema)
-- [Restaurant](https://eyegestures.com/restaurant)
-
-### rules of using
-
-If you are building publicly available product, and have no commercial license, please mention us somewhere in your interface. 
-
-**Promo Materials:**
-
-https://github.com/NativeSensors/EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f
-
-<img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f" width="300
-">
-
-https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37
-
-<img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37" width="200
-">
-
-### 📇 Find us:
-- [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
-- [discord](https://discord.gg/FV3RYTuV)
-- [twitter](https://twitter.com/PW4ltz)
-- email: contact@eyegestures.com
-
-Follow us on polar (it costs nothing but you help project!):
-
-<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
-
-### 📢 Announcements:
-
-<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
-
-### 💻 Contributors
-
-<a href="https://github.com/OWNER/REPO/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=NativeSensors/EyeGestures" />
-</a>
-
-### 💵 Support the project 
-
-<a href="https://polar.sh/NativeSensors/subscriptions"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/tiers.svg?org=NativeSensors&darkmode"><img alt="Subscription Tiers on Polar" src="https://polar.sh/embed/tiers.svg?org=NativeSensors"></picture></a>
-
-<picture>
-  <source
-    media="(prefers-color-scheme: dark)"
-    srcset="
-      https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date&theme=dark
-    "
-  />
-  <source
-    media="(prefers-color-scheme: light)"
-    srcset="
-      https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date
-    "
-  />
-  <img
-    alt="Star History Chart"
-    src="https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date"
-  />
-</picture>
-
+<p align="center">
+  <picture>
+    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/ddfc8b96-5a7e-4487-9307-6fbd62e8915e" media="(prefers-color-scheme: light)"/>   
+    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/6d42b8a2-24ea-4cbc-bdb0-ad688ee26c36" media="(prefers-color-scheme: dark)"/>    
+   <img width="300px" height="300px"/>
+  </picture>
+</p>
+
+## EYEGESTURES
+
+
+EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eye-tracking and eye-driven interfaces without requirement of obtaining expensive hardware.
+
+Our [Mission](https://github.com/NativeSensors/EyeGestures/blob/Engine_v2/MISSION.md)! 
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
+<a href="https://polar.sh/NativeSensors"><img src="https://polar.sh/embed/seeks-funding-shield.svg?org=NativeSensors" /></a>
+### 💜 Sponsors: 
+
+```
+For enterprise avoiding GPL3 licensing there is commercial license!
+```
+We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
+
+```
+Sponsor us and we can add your link, banner or other promo materials!
+```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+
+<!-- POLAR-END id=eizdelwu -->
+
+<p align="center">
+  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
+<img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
+" height="150">
+</p>
+<p align="center">
+  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/3b38d73d-bb6f-4f31-b67d-231ac4cd04cb" width="300" height="150">
+  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/1715b4df-7ac3-479e-b51a-f6d800ea8ea5" width="300" height="150">
+</p>
+
+<p align="center">
+  <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+</p>
+<p align="center">
+  <a href="https://ko-fi.com/Y8Y1SGTBV"><picture><img src="https://ko-fi.com/img/githubbutton_sm.svg"/></a>
+</p>
+
+
+### 💻 Install
+```
+python3 -m pip install eyeGestures
+```
+
+### ⚙️ Run 
+```
+python3 examples/simple_example.py
+```
+
+```
+python3 examples/simple_example_v2.py
+```
+
+### 🪟 Run Windows App [Not updated to latest engine, may crash]
+```
+python3 apps/win_app.py
+```
+
+Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
+
+### 🔧 How to use [WiP - adding Enginge V2]:
+
+#### Using EyeGesture Engine V2 - Machine Learning Approach:
+
+```python
+from eyeGestures.utils import VideoCapture
+from eyeGestures.eyegestures import EyeGestures_v2
+
+# Initialize gesture engine and video capture
+gestures = EyeGestures_v2()
+cap = VideoCapture(0)  
+ret, frame = cap.read()
+calibrate = True
+screen_width = 500
+screen_height= 500
+
+# Process each frame
+event, cevent = gestures.step(frame, True, screen_width, screen_height)
+
+cursor_x, cursor_y = event.point[0], event.point[1]
+# calibration_radius: radius for data collection during calibration
+```
+
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+
+<!-- POLAR-END id=eizdelwu -->
+
+#### Using EyeGesture Engine V1 - Model-Based Approach:
+
+```python
+from eyeGestures.utils import VideoCapture
+from eyeGestures.eyegestures import EyeGestures_v1
+
+# Initialize gesture engine with RoI parameters
+gestures = EyeGestures_v1()
+
+cap = VideoCapture(0)  
+ret, frame = cap.read()
+calibrate = True
+screen_width = 500
+screen_height= 500
+
+# Obtain estimations from camera frames
+event, cevent = gestures.estimate(
+    frame,
+    "main",
+    calibrate,  # set calibration - switch to False to stop calibration
+    screen_width,
+    screen_height,
+    0, 0, 0.8, 10
+)
+cursor_x, cursor_y = event.point[0], event.point[1]
+# cevent - is calibration event
+```
+
+Feel free to copy and paste the relevant code snippets for your project.
+
+### 🔥 Web Demos:
+
+- [Main page](https://eyegestures.com/)
+- [Game demo](https://eyegestures.com/game)
+- [Cinema demo](https://eyegestures.com/cinema)
+- [Restaurant](https://eyegestures.com/restaurant)
+
+### rules of using
+
+If you are building publicly available product, and have no commercial license, please mention us somewhere in your interface. 
+
+**Promo Materials:**
+
+https://github.com/NativeSensors/EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f
+
+<img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f" width="300
+">
+
+https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37
+
+<img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37" width="200
+">
+
+### 📇 Find us:
+- [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
+- [discord](https://discord.gg/EnFu7hYy)
+- [twitter](https://twitter.com/PW4ltz)
+- email: contact@eyegestures.com
+
+Follow us on polar (it costs nothing but you help project!):
+
+<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+
+### 📢 Announcements:
+
+<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
+
+### 💻 Contributors
+
+<a href="https://github.com/OWNER/REPO/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=NativeSensors/EyeGestures" />
+</a>
+
+### 💵 Support the project 
+
+<a href="https://polar.sh/NativeSensors/subscriptions"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/tiers.svg?org=NativeSensors&darkmode"><img alt="Subscription Tiers on Polar" src="https://polar.sh/embed/tiers.svg?org=NativeSensors"></picture></a>
+
+<picture>
+  <source
+    media="(prefers-color-scheme: dark)"
+    srcset="
+      https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date&theme=dark
+    "
+  />
+  <source
+    media="(prefers-color-scheme: light)"
+    srcset="
+      https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date
+    "
+  />
+  <img
+    alt="Star History Chart"
+    src="https://api.star-history.com/svg?repos=NativeSensors/EyeGestures&type=Date"
+  />
+</picture>
+
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                     [Image]
 ## EYEGESTURES EyeGestures is open source eyetracking software/library using
 native webcams and phone camers for achieving its goal. The aim of library is
-to bring accessibility of eyetracking and eyedriven interfaces without
+to bring accessibility of eye-tracking and eye-driven interfaces without
 requirement of obtaining expensive hardware. Our [Mission](https://github.com/
 NativeSensors/EyeGestures/blob/Engine_v2/MISSION.md)! ![PyPI - Downloads]
 (https://img.shields.io/pypi/dm/eyeGestures) _[_h_t_t_p_s_:_/_/_p_o_l_a_r_._s_h_/_e_m_b_e_d_/_s_e_e_k_s_-
 _f_u_n_d_i_n_g_-_s_h_i_e_l_d_._s_v_g_?_o_r_g_=_N_a_t_i_v_e_S_e_n_s_o_r_s_]### ð Sponsors: ``` For enterprise
 avoiding GPL3 licensing there is commercial license! ``` We offer custom
 integration and managed services. For businesses requiring invoices message us
 `contact@eyegestures.com`. ``` Sponsor us and we can add your link, banner or
@@ -13,47 +13,49 @@
  [https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-
  47d4-b25f-c47ba7f0f4f3][https://github.com/PeterWaIIace/PeterWaIIace/assets/
                 40773550/f3132843-063a-439a-8e1c-2385ddfdccda]
  [https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/3b38d73d-bb6f-
  4f31-b67d-231ac4cd04cb][https://github.com/PeterWaIIace/PeterWaIIace/assets/
                 40773550/1715b4df-7ac3-479e-b51a-f6d800ea8ea5]
                              _[_S_u_b_s_c_r_i_b_e_ _o_n_ _P_o_l_a_r_]
+                  _[_h_t_t_p_s_:_/_/_k_o_-_f_i_._c_o_m_/_i_m_g_/_g_i_t_h_u_b_b_u_t_t_o_n___s_m_._s_v_g_]
 ### ð» Install ``` python3 -m pip install eyeGestures ``` ### âï¸ Run ```
-python3 examples/simple_example.py ``` ### ðª Run Windows App ``` python3
-apps/win_app.py ``` Or download it from [`releases`](https://github.com/
-NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3) ### ð§ How to use
-[WiP - adding Enginge V2]: #### Using EyeGesture Engine V2 - Machine Learning
-Approach: ```python from eyeGestures.utils import VideoCapture from
-eyeGestures.eyegestures import EyeGestures_v2 # Initialize gesture engine and
-video capture gestures = EyeGestures_v2() cap = VideoCapture(0) # Process each
-frame point, calibration_point, blink, fixation, acceptance_radius,
-calibration_radius = gestures.step(frame, calibrate, screen_width,
-screen_height) # point: x, y positions of cursor # calibration_point: x, y
-position of current calibration point # acceptance_radius: precision required
-for calibration # calibration_radius: radius for data collection during
-calibration ``` #### Using EyeGesture Engine V1 - Model-Based Approach:
+python3 examples/simple_example.py ``` ``` python3 examples/
+simple_example_v2.py ``` ### ðª Run Windows App [Not updated to latest
+engine, may crash] ``` python3 apps/win_app.py ``` Or download it from
+[`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/
+1.3.4_App_0.0.3) ### ð§ How to use [WiP - adding Enginge V2]: #### Using
+EyeGesture Engine V2 - Machine Learning Approach: ```python from
+eyeGestures.utils import VideoCapture from eyeGestures.eyegestures import
+EyeGestures_v2 # Initialize gesture engine and video capture gestures =
+EyeGestures_v2() cap = VideoCapture(0) ret, frame = cap.read() calibrate = True
+screen_width = 500 screen_height= 500 # Process each frame event, cevent =
+gestures.step(frame, True, screen_width, screen_height) cursor_x, cursor_y =
+event.point[0], event.point[1] # calibration_radius: radius for data collection
+during calibration ``` #### Using EyeGesture Engine V1 - Model-Based Approach:
 ```python from eyeGestures.utils import VideoCapture from
 eyeGestures.eyegestures import EyeGestures_v1 # Initialize gesture engine with
 RoI parameters gestures = EyeGestures_v1() cap = VideoCapture(0) ret, frame =
-cap.read() # Obtain estimations from camera frames event = gestures.estimate
-( frame, "main", True, # set calibration - switch to False to stop calibration
+cap.read() calibrate = True screen_width = 500 screen_height= 500 # Obtain
+estimations from camera frames event, cevent = gestures.estimate( frame,
+"main", calibrate, # set calibration - switch to False to stop calibration
 screen_width, screen_height, 0, 0, 0.8, 10 ) cursor_x, cursor_y = event.point
-[0], event.point[1] ``` Feel free to copy and paste the relevant code snippets
-for your project. ### ð¥ Web Demos: - [Main page](https://eyegestures.com/) -
-[Game demo](https://eyegestures.com/game) - [Cinema demo](https://
-eyegestures.com/cinema) - [Restaurant](https://eyegestures.com/restaurant) ###
-rules of using If you are building publicly available product, and have no
-commercial license, please mention us somewhere in your interface. **Promo
-Materials:** https://github.com/NativeSensors/EyeGestures/assets/40773550/
-4ca842b9-ba32-4ffd-b2e4-179ff67ee47f [https://github.com/NativeSensors/
-EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f]https://
-github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-
-3a6bb4159b37 [https://github.com/NativeSensors/EyeGestures/assets/40773550/
-6a7c74b5-b069-4eec-bc96-3a6bb4159b37]### ð Find us: - [RSS](https://
-polar.sh/NativeSensors/
+[0], event.point[1] # cevent - is calibration event ``` Feel free to copy and
+paste the relevant code snippets for your project. ### ð¥ Web Demos: - [Main
+page](https://eyegestures.com/) - [Game demo](https://eyegestures.com/game) -
+[Cinema demo](https://eyegestures.com/cinema) - [Restaurant](https://
+eyegestures.com/restaurant) ### rules of using If you are building publicly
+available product, and have no commercial license, please mention us somewhere
+in your interface. **Promo Materials:** https://github.com/NativeSensors/
+EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-179ff67ee47f [https://
+github.com/NativeSensors/EyeGestures/assets/40773550/4ca842b9-ba32-4ffd-b2e4-
+179ff67ee47f]https://github.com/NativeSensors/EyeGestures/assets/40773550/
+6a7c74b5-b069-4eec-bc96-3a6bb4159b37 [https://github.com/NativeSensors/
+EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37]### ð Find
+us: - [RSS](https://polar.sh/NativeSensors/
 rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-
-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U) - [discord](https://discord.gg/FV3RYTuV) -
+xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U) - [discord](https://discord.gg/EnFu7hYy) -
 [twitter](https://twitter.com/PW4ltz) - email: contact@eyegestures.com Follow
 us on polar (it costs nothing but you help project!): _[_S_u_b_s_c_r_i_b_e_ _o_n_ _P_o_l_a_r_]###
 ð¢ Announcements: _[_P_o_s_t_s_ _o_n_ _P_o_l_a_r_]### ð» Contributors _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_N_a_t_i_v_e_S_e_n_s_o_r_s_/_E_y_e_G_e_s_t_u_r_e_s_]### ðµ Support the project
 _[_S_u_b_s_c_r_i_p_t_i_o_n_ _T_i_e_r_s_ _o_n_ _P_o_l_a_r_][Star History Chart]
```

### Comparing `eyegestures-2.0.0/PKG-INFO` & `eyegestures-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eyeGestures
-Version: 2.0.0
+Version: 2.1.0
 Summary: Package for eye tracking algorithm allowing for development of gaze controlled computer interface
 Project-URL: Homepage, https://github.com/NativeSensors/EyeGestures
 Project-URL: Issues, https://github.com/NativeSensors/EyeGestures/Issues
 Author-email: Piotr Walas <piotr.walas@eyegestures.com>
 Maintainer-email: Piotr Walas <piotr.walas@eyegestures.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -695,15 +695,15 @@
    <img width="300px" height="300px"/>
   </picture>
 </p>
 
 ## EYEGESTURES
 
 
-EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
+EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eye-tracking and eye-driven interfaces without requirement of obtaining expensive hardware.
 
 Our [Mission](https://github.com/NativeSensors/EyeGestures/blob/Engine_v2/MISSION.md)! 
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
 <a href="https://polar.sh/NativeSensors"><img src="https://polar.sh/embed/seeks-funding-shield.svg?org=NativeSensors" /></a>
 ### 💜 Sponsors: 
 
@@ -730,26 +730,34 @@
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/3b38d73d-bb6f-4f31-b67d-231ac4cd04cb" width="300" height="150">
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/1715b4df-7ac3-479e-b51a-f6d800ea8ea5" width="300" height="150">
 </p>
 
 <p align="center">
   <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
 </p>
+<p align="center">
+  <a href="https://ko-fi.com/Y8Y1SGTBV"><picture><img src="https://ko-fi.com/img/githubbutton_sm.svg"/></a>
+</p>
+
 
 ### 💻 Install
 ```
 python3 -m pip install eyeGestures
 ```
 
 ### ⚙️ Run 
 ```
 python3 examples/simple_example.py
 ```
 
-### 🪟 Run Windows App 
+```
+python3 examples/simple_example_v2.py
+```
+
+### 🪟 Run Windows App [Not updated to latest engine, may crash]
 ```
 python3 apps/win_app.py
 ```
 
 Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
 
 ### 🔧 How to use [WiP - adding Enginge V2]:
@@ -759,20 +767,23 @@
 ```python
 from eyeGestures.utils import VideoCapture
 from eyeGestures.eyegestures import EyeGestures_v2
 
 # Initialize gesture engine and video capture
 gestures = EyeGestures_v2()
 cap = VideoCapture(0)  
+ret, frame = cap.read()
+calibrate = True
+screen_width = 500
+screen_height= 500
 
 # Process each frame
-point, calibration_point, blink, fixation, acceptance_radius, calibration_radius = gestures.step(frame, calibrate, screen_width, screen_height)
-# point: x, y positions of cursor
-# calibration_point: x, y position of current calibration point
-# acceptance_radius: precision required for calibration
+event, cevent = gestures.step(frame, True, screen_width, screen_height)
+
+cursor_x, cursor_y = event.point[0], event.point[1]
 # calibration_radius: radius for data collection during calibration
 ```
 
 <!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
 
 
 
@@ -785,25 +796,29 @@
 from eyeGestures.eyegestures import EyeGestures_v1
 
 # Initialize gesture engine with RoI parameters
 gestures = EyeGestures_v1()
 
 cap = VideoCapture(0)  
 ret, frame = cap.read()
+calibrate = True
+screen_width = 500
+screen_height= 500
 
 # Obtain estimations from camera frames
-event = gestures.estimate(
+event, cevent = gestures.estimate(
     frame,
     "main",
-    True,  # set calibration - switch to False to stop calibration
+    calibrate,  # set calibration - switch to False to stop calibration
     screen_width,
     screen_height,
     0, 0, 0.8, 10
 )
 cursor_x, cursor_y = event.point[0], event.point[1]
+# cevent - is calibration event
 ```
 
 Feel free to copy and paste the relevant code snippets for your project.
 
 ### 🔥 Web Demos:
 
 - [Main page](https://eyegestures.com/)
@@ -825,15 +840,15 @@
 https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37
 
 <img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37" width="200
 ">
 
 ### 📇 Find us:
 - [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
-- [discord](https://discord.gg/FV3RYTuV)
+- [discord](https://discord.gg/EnFu7hYy)
 - [twitter](https://twitter.com/PW4ltz)
 - email: contact@eyegestures.com
 
 Follow us on polar (it costs nothing but you help project!):
 
 <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
```

