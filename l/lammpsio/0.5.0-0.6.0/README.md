# Comparing `tmp/lammpsio-0.5.0.tar.gz` & `tmp/lammpsio-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammpsio-0.5.0.tar", last modified: Mon Apr 29 17:46:29 2024, max compression
+gzip compressed data, was "lammpsio-0.6.0.tar", last modified: Tue May 28 17:54:46 2024, max compression
```

## Comparing `lammpsio-0.5.0.tar` & `lammpsio-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 17:46:23.000000 lammpsio-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 17:46:29.794054 lammpsio-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-29 17:46:23.000000 lammpsio-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 17:46:23.000000 lammpsio-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 17:46:29.794054 lammpsio-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:46:23.000000 lammpsio-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.790054 lammpsio-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/src/lammpsio/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/box.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/src/lammpsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_dump_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:54:46.373794 lammpsio-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-28 17:54:36.000000 lammpsio-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-28 17:54:46.373794 lammpsio-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-28 17:54:36.000000 lammpsio-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 17:54:36.000000 lammpsio-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-28 17:54:46.373794 lammpsio-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:54:36.000000 lammpsio-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:54:46.369794 lammpsio-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:54:46.373794 lammpsio-0.6.0/src/lammpsio/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-28 17:54:36.000000 lammpsio-0.6.0/src/lammpsio/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:54:46.373794 lammpsio-0.6.0/src/lammpsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-28 17:54:46.000000 lammpsio-0.6.0/src/lammpsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 17:54:46.000000 lammpsio-0.6.0/src/lammpsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:54:46.000000 lammpsio-0.6.0/src/lammpsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 17:54:46.000000 lammpsio-0.6.0/src/lammpsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 17:54:46.000000 lammpsio-0.6.0/src/lammpsio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:54:46.373794 lammpsio-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-28 17:54:36.000000 lammpsio-0.6.0/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-05-28 17:54:36.000000 lammpsio-0.6.0/tests/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-28 17:54:36.000000 lammpsio-0.6.0/tests/test_dump_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-28 17:54:36.000000 lammpsio-0.6.0/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-28 17:54:36.000000 lammpsio-0.6.0/tests/test_topology.py
```

### Comparing `lammpsio-0.5.0/LICENSE` & `lammpsio-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/PKG-INFO` & `lammpsio-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lammpsio-0.5.0/README.md` & `lammpsio-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/setup.cfg` & `lammpsio-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/src/lammpsio/box.py` & `lammpsio-0.6.0/src/lammpsio/box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/src/lammpsio/data.py` & `lammpsio-0.6.0/src/lammpsio/data.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/src/lammpsio/dump.py` & `lammpsio-0.6.0/src/lammpsio/dump.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 import numpy
 
 from .box import Box
 from .data import _readline
 from .snapshot import Snapshot
 
+try:
+    import pyzstd
+
+    _has_pyzstd = True
+except ModuleNotFoundError:
+    _has_pyzstd = False
+
 
 class DumpFile:
     """LAMMPS dump file.
 
     The dump file is a flexible file format, so a ``schema`` can be given
     to parse the atom data. The ``schema`` is given as a dictionary of column
     indexes. Valid keys for the schema match the names and shapes in the `Snapshot`.
@@ -88,34 +95,35 @@
             for snap in snapshots:
                 f.write("ITEM: TIMESTEP\n" f"{snap.step}\n")
 
                 f.write("ITEM: NUMBER OF ATOMS\n")
                 f.write(f"{snap.N}\n")
 
                 # always assume periodic in all directions
-                box_header = "ITEM: BOX BOUNDS pp pp pp"
                 if snap.box.tilt is not None:
+                    f.write("ITEM: BOX BOUNDS xy xz yz pp pp pp\n")
                     xy, xz, yz = snap.box.tilt
-                    box_header += f" {xy:f} {xz:f} {yz:f}"
                     lo = [
                         snap.box.low[0] + min([0.0, xy, xz, xy + xz]),
                         snap.box.low[1] + min([0.0, yz]),
                         snap.box.low[2],
                     ]
                     hi = [
                         snap.box.high[0] + max([0.0, xy, xz, xy + xz]),
                         snap.box.high[1] + max([0.0, yz]),
                         snap.box.high[2],
                     ]
+                    for i in range(3):
+                        f.write(f"{lo[i]:f} {hi[i]:f} {snap.box.tilt[i]:f}\n")
                 else:
+                    f.write("ITEM: BOX BOUNDS pp pp pp\n")
                     lo = snap.box.low
                     hi = snap.box.high
-                f.write(box_header + "\n")
-                for i in range(3):
-                    f.write(f"{lo[i]:f} {hi[i]:f}\n")
+                    for i in range(3):
+                        f.write(f"{lo[i]:f} {hi[i]:f}\n")
 
                 # mapping from lammpsio to LAMMPS dump keys
                 lammps_fields = {
                     "id": "id",
                     "molecule": "mol",
                     "typeid": "type",
                     "mass": "mass",
@@ -153,22 +161,34 @@
                         if col > 0:
                             fmt = " " + fmt
                         line += fmt.format(val)
                     line = line.strip()
                     f.write(line + "\n")
 
         filename_path = pathlib.Path(filename)
-        if filename_path.suffix == ".gz":
+        compression = cls._compression_from_suffix(filename_path.suffix)
+        if compression:
             tmp = pathlib.Path(filename).with_suffix(filename_path.suffix + ".tmp")
-            with open(filename, "rb") as src, gzip.open(tmp, "wb") as dest:
+            with open(filename, "rb") as src, compression.open(tmp, "wb") as dest:
                 dest.writelines(src)
             os.replace(tmp, filename)
 
         return DumpFile(filename, schema)
 
+    @staticmethod
+    def _compression_from_suffix(suffix):
+        if suffix == ".gz":
+            return gzip
+        elif suffix == ".zst":
+            if not _has_pyzstd:
+                raise ModuleNotFoundError("pyzstd needed for zstd compression")
+            return pyzstd
+        else:
+            return None
+
     @property
     def copy_from(self):
         return self._copy_from
 
     @copy_from.setter
     def copy_from(self, value):
         if value is not None and not isinstance(value, Snapshot):
@@ -179,24 +199,24 @@
     def filename(self):
         """str: Path to the file."""
         return self._filename
 
     @filename.setter
     def filename(self, value):
         self._filename = value
-        self._gzip = pathlib.Path(value).suffix == ".gz"
+        self._compression = self._compression_from_suffix(pathlib.Path(value).suffix)
 
         # configure section labels of dump file
         self._section = {
             "step": "ITEM: TIMESTEP",
             "natoms": "ITEM: NUMBER OF ATOMS",
             "box": "ITEM: BOX BOUNDS",
             "atoms": "ITEM: ATOMS",
         }
-        if self._gzip:
+        if self._compression:
             for key, val in self._section.items():
                 self._section[key] = val.encode()
 
     @property
     def schema(self):
         """dict: Data schema."""
         return self._schema
@@ -211,16 +231,16 @@
                 raise ValueError("Velocity must be a 3-tuple")
             if "image" in value and len(value["image"]) != 3:
                 raise ValueError("Image must be a 3-tuple")
         self._schema = value
 
     def _open(self):
         """Open the file handle for reading."""
-        if self._gzip:
-            f = gzip.open(self.filename, "rb")
+        if self._compression:
+            f = self._compression.open(self.filename, "rb")
         else:
             f = open(self.filename, "r")
         return f
 
     def _find_frames(self):
         """Seek line numbers for each frame."""
         self._frames = []
@@ -255,38 +275,39 @@
 
                 # box size third
                 if state == 2 and self._section["box"] in line:
                     state += 1
                     box_header = line.split()
                     # check for triclinic
                     if len(box_header) == 9:
-                        box_tilt = [float(x) for x in box_header[6:9]]
+                        is_triclinic = True
                     elif len(box_header) == 6:
-                        box_tilt = None
+                        is_triclinic = False
                     else:
                         raise IOError("Incorrectly formed box bound header")
-                    box_x = _readline(f, True)
-                    box_y = _readline(f, True)
-                    box_z = _readline(f, True)
-                    x_lo, x_hi = [float(x) for x in box_x.split()]
-                    y_lo, y_hi = [float(y) for y in box_y.split()]
-                    z_lo, z_hi = [float(z) for z in box_z.split()]
-                    if box_tilt is not None:
-                        xy, xz, yz = box_tilt
+                    box_ = [
+                        [float(v) for v in _readline(f, True).split()]
+                        for line_ in range(3)
+                    ]
+                    x_lo, x_hi = box_[0][:2]
+                    y_lo, y_hi = box_[1][:2]
+                    z_lo, z_hi = box_[2][:2]
+                    if is_triclinic:
+                        xy, xz, yz = [row[2] for row in box_]
                         lo = [
                             x_lo - min([0.0, xy, xz, xy + xz]),
                             y_lo - min([0.0, yz]),
                             z_lo,
                         ]
                         hi = [
                             x_hi - max([0.0, xy, xz, xy + xz]),
                             y_hi - max([0.0, yz]),
                             z_hi,
                         ]
-                        box = Box(lo, hi, box_tilt)
+                        box = Box(lo, hi, [xy, xz, yz])
                     else:
                         box = Box([x_lo, y_lo, z_lo], [x_hi, y_hi, z_hi])
 
                 # atoms come fourth
                 if state == 3 and self._section["atoms"] in line:
                     state += 1
 
@@ -308,26 +329,26 @@
                             "vy": ("velocity", 1),
                             "vz": ("velocity", 2),
                             "q": ("charge", None),
                         }
                         schema = {}
                         schema_header = line.split()[2:]
                         for i, field in enumerate(schema_header):
-                            if self._gzip:
+                            if self._compression:
                                 field = field.decode()
                             if field in lammps_fields:
                                 key, key_idx = lammps_fields[field]
                                 if key_idx is not None:
                                     if key not in schema:
                                         schema[key] = [None, None, None]
                                     schema[key][key_idx] = i
                                 else:
                                     schema[key] = i
                         # validate tuple
-                        for key in ("position", "velocity", " image"):
+                        for key in ("position", "velocity", "image"):
                             if key in schema and any(x is None for x in schema[key]):
                                 raise IOError("lammpsio requires 3-element vectors")
                         self.schema = schema
 
                     snap = Snapshot(N, box, step)
                     for i in range(snap.N):
                         atom = _readline(f, True)
```

### Comparing `lammpsio-0.5.0/src/lammpsio/snapshot.py` & `lammpsio-0.6.0/src/lammpsio/snapshot.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/src/lammpsio/topology.py` & `lammpsio-0.6.0/src/lammpsio/topology.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/src/lammpsio.egg-info/PKG-INFO` & `lammpsio-0.6.0/src/lammpsio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lammpsio-0.5.0/tests/test_box.py` & `lammpsio-0.6.0/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/tests/test_data_file.py` & `lammpsio-0.6.0/tests/test_data_file.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/tests/test_dump_file.py` & `lammpsio-0.6.0/tests/test_dump_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import copy
 
 import numpy
 import pytest
 
 import lammpsio
 
+try:
+    import pyzstd  # noqa: F401
+
+    has_pyzstd = True
+except ModuleNotFoundError:
+    has_pyzstd = False
+
 
 @pytest.mark.parametrize("sort_ids", [False, True])
 @pytest.mark.parametrize("shuffle_ids", [False, True])
-@pytest.mark.parametrize("use_gzip", [False, True])
-def test_dump_file_min(snap, use_gzip, shuffle_ids, sort_ids, tmp_path):
+@pytest.mark.parametrize("compression_extension", ["", ".gz", ".zst"])
+def test_dump_file_min(snap, compression_extension, shuffle_ids, sort_ids, tmp_path):
+    if not has_pyzstd and compression_extension == ".zst":
+        pytest.skip("pyzstd not installed")
+
     # create file with 2 snapshots with defaults, changing N & step
     snap_2 = lammpsio.Snapshot(snap.N + 2, snap.box, snap.step + 1)
     snaps = [snap, snap_2]
     if shuffle_ids:
         for s in snaps:
             s.id = s.id[::-1]
-    if use_gzip:
-        filename = tmp_path / "atoms.lammpstrj.gz"
-    else:
-        filename = tmp_path / "atoms.lammpstrj"
+
+    filename = tmp_path / f"atoms.lammpstrj{compression_extension}"
     schema = {"id": 0, "position": (1, 2, 3)}
     f = lammpsio.DumpFile.create(filename, schema, snaps)
     assert filename.exists
     assert len(f) == 2
 
     # read it back in and check snapshots
     f2 = lammpsio.DumpFile(filename, sort_ids=sort_ids)
@@ -55,16 +63,19 @@
         assert not read_snaps[i].has_mass()
         assert not read_snaps[i].has_molecule()
         assert not read_snaps[i].has_charge()
 
 
 @pytest.mark.parametrize("sort_ids", [False, True])
 @pytest.mark.parametrize("shuffle_ids", [False, True])
-@pytest.mark.parametrize("use_gzip", [False, True])
-def test_dump_file_all(snap, use_gzip, shuffle_ids, sort_ids, tmp_path):
+@pytest.mark.parametrize("compression_extension", ["", ".gz", ".zst"])
+def test_dump_file_all(snap, compression_extension, shuffle_ids, sort_ids, tmp_path):
+    if not has_pyzstd and compression_extension == ".zst":
+        pytest.skip("pyzstd not installed")
+
     snap.position = [[0.1, 0.2, 0.3], [-0.4, -0.5, -0.6], [0.7, 0.8, 0.9]]
     snap.image = [[1, 2, 3], [-4, -5, -6], [7, 8, 9]]
     snap.velocity = [[-3, -2, -1], [6, 5, 4], [9, 8, 7]]
     snap.typeid = [2, 1, 2]
     snap.mass = [3, 2, 3]
     snap.molecule = [2, 0, 1]
     snap.charge = [-1, 0, 1]
@@ -96,18 +107,16 @@
         "image": (9, 8, 7),
         "velocity": (4, 5, 6),
         "typeid": 3,
         "mass": 2,
         "molecule": 1,
         "charge": 0,
     }
-    if use_gzip:
-        filename = tmp_path / "atoms.lammpstrj.gz"
-    else:
-        filename = tmp_path / "atoms.lammpstrj"
+
+    filename = tmp_path / f"atoms.lammpstrj{compression_extension}"
     f = lammpsio.DumpFile.create(filename, schema, snaps)
     assert filename.exists
     assert len(f) == 2
 
     # read it back in and check snapshots
     f2 = lammpsio.DumpFile(filename, sort_ids=sort_ids)
     read_snaps = [s for s in f2]
@@ -183,7 +192,44 @@
     assert numpy.all(read_snap.typeid == [1, 2, 2])
     assert read_snap.has_mass()
     assert numpy.allclose(read_snap.mass, [2, 3, 3])
     assert read_snap.has_molecule()
     assert numpy.all(read_snap.molecule == [0, 1, 2])
     assert read_snap.has_charge()
     assert numpy.allclose(read_snap.charge, [0, 1, -1])
+
+
+@pytest.mark.parametrize(
+    "schema",
+    ["x", "x y", "vx", "vx vy", "ix", "ix iy"],
+    ids=[
+        "position-1d",
+        "position-2d",
+        "velocity-1d",
+        "velocity-2d",
+        "image-1d",
+        "image-2d",
+    ],
+)
+def test_faulty_dump_schema(tmp_path, schema):
+    # test schema
+    schema_zeros = " ".join(["0"] * len(schema.split()))
+    filename = tmp_path / "atoms.lammpstrj"
+    f = open(filename, "w")
+    f.write(
+        "ITEM: TIMESTEP\n"
+        "0\n"
+        "ITEM: NUMBER OF ATOMS\n"
+        "1\n"
+        "ITEM: BOX BOUNDS pp pp pp\n"
+        "-7.0 7.0\n"
+        "-7.0 7.0\n"
+        "-7.0 7.0\n"
+        f"ITEM: ATOMS id type {schema}\n"
+        f"1 1 {schema_zeros}\n"
+    )
+    f.close()
+
+    traj = lammpsio.DumpFile(filename)
+    with pytest.raises(IOError):
+        for snap in traj:
+            pass
```

### Comparing `lammpsio-0.5.0/tests/test_snapshot.py` & `lammpsio-0.6.0/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.5.0/tests/test_topology.py` & `lammpsio-0.6.0/tests/test_topology.py`

 * *Files identical despite different names*

