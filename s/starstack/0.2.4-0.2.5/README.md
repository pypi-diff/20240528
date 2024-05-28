# Comparing `tmp/starstack-0.2.4.tar.gz` & `tmp/starstack-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starstack-0.2.4.tar", last modified: Tue Feb 27 18:19:02 2024, max compression
+gzip compressed data, was "starstack-0.2.5.tar", last modified: Tue May 28 17:03:11 2024, max compression
```

## Comparing `starstack-0.2.4.tar` & `starstack-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:19:02.525974 starstack-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-27 18:18:17.000000 starstack-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-27 18:18:17.000000 starstack-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-27 18:19:02.525974 starstack-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-27 18:18:17.000000 starstack-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 18:18:17.000000 starstack-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 18:19:02.525974 starstack-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-27 18:18:17.000000 starstack-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:19:02.525974 starstack-0.2.4/starstack/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 18:18:17.000000 starstack-0.2.4/starstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-27 18:18:17.000000 starstack-0.2.4/starstack/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-02-27 18:18:17.000000 starstack-0.2.4/starstack/mrcFileStack.py
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-02-27 18:18:17.000000 starstack-0.2.4/starstack/particlesStar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:19:02.525974 starstack-0.2.4/starstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-27 18:19:02.000000 starstack-0.2.4/starstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-27 18:19:02.000000 starstack-0.2.4/starstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 18:19:02.000000 starstack-0.2.4/starstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-27 18:19:02.000000 starstack-0.2.4/starstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 18:19:02.000000 starstack-0.2.4/starstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:19:02.525974 starstack-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 18:18:17.000000 starstack-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-02-27 18:18:17.000000 starstack-0.2.4/tests/test_particlesStar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:03:11.672057 starstack-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-28 17:02:44.000000 starstack-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 17:02:44.000000 starstack-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-28 17:03:11.672057 starstack-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-28 17:02:44.000000 starstack-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:02:44.000000 starstack-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:03:11.672057 starstack-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 17:02:44.000000 starstack-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:03:11.672057 starstack-0.2.5/starstack/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 17:02:44.000000 starstack-0.2.5/starstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 17:02:44.000000 starstack-0.2.5/starstack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-28 17:02:44.000000 starstack-0.2.5/starstack/mrcFileStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-05-28 17:02:44.000000 starstack-0.2.5/starstack/particlesStar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:03:11.672057 starstack-0.2.5/starstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-28 17:03:11.000000 starstack-0.2.5/starstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 17:03:11.000000 starstack-0.2.5/starstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:03:11.000000 starstack-0.2.5/starstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 17:03:11.000000 starstack-0.2.5/starstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 17:03:11.000000 starstack-0.2.5/starstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:03:11.672057 starstack-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:02:44.000000 starstack-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-28 17:02:44.000000 starstack-0.2.5/tests/test_particlesStar.py
```

### Comparing `starstack-0.2.4/LICENSE` & `starstack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starstack-0.2.4/PKG-INFO` & `starstack-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starstack
-Version: 0.2.4
+Version: 0.2.5
 Summary: A relion star mrcs stack class
 Home-page: https://github.com/rsanchezgarc/starstack
 Author: Ruben Sanchez Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: relion cryoem star stack mrcs
 License-File: LICENSE
 Requires-Dist: mrcfile
```

### Comparing `starstack-0.2.4/README.md` & `starstack-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `starstack-0.2.4/setup.py` & `starstack-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `starstack-0.2.4/starstack/constants.py` & `starstack-0.2.5/starstack/constants.py`

 * *Files identical despite different names*

### Comparing `starstack-0.2.4/starstack/mrcFileStack.py` & `starstack-0.2.5/starstack/mrcFileStack.py`

 * *Files identical despite different names*

### Comparing `starstack-0.2.4/starstack/particlesStar.py` & `starstack-0.2.5/starstack/particlesStar.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         :param particlesDf: The particles metadata as a pandas dataframe
         :param npImages: The images, as a numpy array of shape (Nx3) to store or as an iterator of np images.
         :param overwrite: True if the files are to be overwritten.
         :param basenameInStarImageName: True if the mrcs filenames are going to be stored as basenames
         :return:
         """
 
-        assert "rlnImageName" in particlesDf, ("rlnImageName will be automatically assigned when the stack is created, "
-                                               "it need to be removed from starDf")
+        # assert "rlnImageName" in particlesDf, ("rlnImageName will be automatically assigned when the stack is created, "
+        #                                        "it needs to be removed from particlesDf")
 
         newStackName = osp.splitext(newStarFname)[0] + ".mrcs"
         _newStackName = newStackName if not basenameInStarImageName else osp.basename(newStackName)
         particlesDf["rlnImageName"] = ["%06d@%s" % (i, _newStackName) for i in range(1, 1 + len(particlesDf))]
 
         if isinstance(npImages, np.ndarray):
             assert npImages.shape[-1] == opticsDf["rlnImageSize"].unique().item(), \
@@ -179,18 +179,21 @@
         star_data = {}
         if self.optics_md is not None:
             star_data["optics"] = self.optics_md
         star_data["particles"] = new_particles_md
 
         starfile.write(star_data, starFname, overwrite=True)
 
-    def updateMd(self, ids: List[str], colname2change: Dict[str, Any]):
+    def updateMd(self, ids: Optional[List[str]], colname2change: Dict[str, Any]):
 
         for col, vals in colname2change.items():
-            self.particles_md.loc[ids, col] = vals
+            if ids is not None:
+                self.particles_md.loc[ids, col] = vals
+            else:
+                self.particles_md[col] = vals
 
     def __getitem__(self, idx):
         if isinstance(idx, slice):
             imgs, mds = zip(*[self.__getitem(ii) for ii in range(*idx.indices(len(self)))])
             return np.stack(imgs, 0), pd.DataFrame(mds)
         elif isinstance(idx, (list, tuple)):
             imgs, mds = zip(*[self.__getitem(ii) for ii in idx])
@@ -205,25 +208,31 @@
     def __len__(self):
         return len(self.particles_md)
 
     def getPose(self, idx: Union[int,List[int]]) -> Tuple[np.ndarray, np.ndarray]:
         md = self.particles_md.iloc[idx, :]
         return self.getPoseFromMd(md)
 
-    def setPose(self, idx: Union[int,List[int]], eulerDegs: np.ndarray | None = None, shiftsAngst: np.ndarray | None = None,
-                confidence: np.ndarray | None = None):
+    def setPose(self, idx: Union[int,List[int]], eulerDegs: Optional[np.ndarray] = None, shiftsAngst: Optional[np.ndarray] = None,
+                confidence: Optional[np.ndarray] = None):
 
         if eulerDegs is not None:
-            self.particles_md.iloc[idx, [self.particles_md.columns.get_loc(col) for col in RELION_ANGLES_NAMES]] = eulerDegs
+            self.particles_md.iloc[idx,
+                                [self.particles_md.columns.get_loc(col) for col in RELION_ANGLES_NAMES]] = eulerDegs
 
         if shiftsAngst is not None:
-            self.particles_md.iloc[idx, [self.particles_md.columns.get_loc(col) for col in RELION_SHIFTS_NAMES]] = shiftsAngst
+            self.particles_md.iloc[idx,
+                                [self.particles_md.columns.get_loc(col) for col in RELION_SHIFTS_NAMES]] = shiftsAngst
 
         if confidence is not None:
-            self.particles_md.iloc[idx, self.particles_md.columns.get_loc(RELION_PRED_POSE_CONFIDENCE_NAME)] = confidence
+            if RELION_PRED_POSE_CONFIDENCE_NAME not in self.particles_md.columns:
+                self.particles_md[RELION_PRED_POSE_CONFIDENCE_NAME] = confidence
+            else:
+                self.particles_md.iloc[idx,
+                                    self.particles_md.columns.get_loc(RELION_PRED_POSE_CONFIDENCE_NAME)] = confidence
 
 
     @classmethod
     def getPoseFromMd(cls, md):
         anglesDegs = [md[name] for name in RELION_ANGLES_NAMES]
         xyShiftAngs = [md[name] for name in RELION_SHIFTS_NAMES]
         anglesDegs = np.array(anglesDegs).T
@@ -256,15 +265,15 @@
         # Combine optics metadata if available
         if self.optics_md is not None and other.optics_md is not None:
             # Determine the next available optics group ID
             next_optics_group_id = self.optics_md['rlnOpticsGroup'].max() + 1
 
             # Update the optics group IDs in the other optics DataFrame
             other_optics_md = other.optics_md.copy()
-            other_optics_md['rlnOpticsGroup'] += next_optics_group_id
+            other_optics_md['rlnOpticsGroup'] = next_optics_group_id
 
             suffix = f"_{next_optics_group_id}"
             other_optics_md['rlnOpticsGroupName'] = other_optics_md['rlnOpticsGroupName'].apply(lambda x: x + suffix)
             # Combine the optics DataFrames
             combined_optics = pd.concat([self.optics_md, other_optics_md])
             combined_optics.drop_duplicates(ignore_index=True, inplace=True)
             ps.optics_md = combined_optics
```

### Comparing `starstack-0.2.4/starstack.egg-info/PKG-INFO` & `starstack-0.2.5/starstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starstack
-Version: 0.2.4
+Version: 0.2.5
 Summary: A relion star mrcs stack class
 Home-page: https://github.com/rsanchezgarc/starstack
 Author: Ruben Sanchez Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: relion cryoem star stack mrcs
 License-File: LICENSE
 Requires-Dist: mrcfile
```

### Comparing `starstack-0.2.4/tests/test_particlesStar.py` & `starstack-0.2.5/tests/test_particlesStar.py`

 * *Files identical despite different names*

