# Comparing `tmp/pwdata-0.2.12.tar.gz` & `tmp/pwdata-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdata-0.2.12.tar", last modified: Mon Apr  8 07:25:17 2024, max compression
+gzip compressed data, was "pwdata-0.2.13.tar", last modified: Tue May 28 02:07:45 2024, max compression
```

## Comparing `pwdata-0.2.12.tar` & `pwdata-0.2.13.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.098070 pwdata-0.2.12/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.12/LICENSE
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-04-08 07:25:17.097621 pwdata-0.2.12/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.12/README.md
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.056021 pwdata-0.2.12/pwdata/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.12/pwdata/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.12/pwdata/atomconfig.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.079212 pwdata-0.2.12/pwdata/build/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.12/pwdata/build/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.12/pwdata/build/cell.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.12/pwdata/build/geometry.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.12/pwdata/build/supercells.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    15467 2024-03-29 08:35:53.000000 pwdata-0.2.12/pwdata/build/write_struc.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.094991 pwdata-0.2.12/pwdata/calculators/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.12/pwdata/calculators/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.12/pwdata/calculators/const.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.12/pwdata/calculators/unitconvert_lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.12/pwdata/calculators/units.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.12/pwdata/cp2kdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.12/pwdata/datasets_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5975 2024-03-25 05:49:22.000000 pwdata-0.2.12/pwdata/deepmd.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.12/pwdata/dump.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1648 2024-03-05 02:49:25.000000 pwdata-0.2.12/pwdata/extendedxyz.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11432 2024-03-29 08:35:05.000000 pwdata-0.2.12/pwdata/image.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.12/pwdata/lammpsdata.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.12/pwdata/lmps.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16592 2024-03-27 09:50:17.000000 pwdata-0.2.12/pwdata/main.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.12/pwdata/movement.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.12/pwdata/movement_saver.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6768 2024-04-08 07:19:40.000000 pwdata-0.2.12/pwdata/outcar.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.096517 pwdata-0.2.12/pwdata/pertub/
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.12/pwdata/pertub/__init__.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.12/pwdata/pertub/perturbation.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.12/pwdata/pertub/scale.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.12/pwdata/poscar.py
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2877 2024-04-08 07:24:28.000000 pwdata-0.2.12/pwdata/pwmlff.py
-drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-04-08 07:25:17.097089 pwdata-0.2.12/pwdata.egg-info/
--rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-04-08 07:25:16.000000 pwdata-0.2.12/pwdata.egg-info/PKG-INFO
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      777 2024-04-08 07:25:16.000000 pwdata-0.2.12/pwdata.egg-info/SOURCES.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-04-08 07:25:16.000000 pwdata-0.2.12/pwdata.egg-info/dependency_links.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-04-08 07:25:16.000000 pwdata-0.2.12/pwdata.egg-info/top_level.txt
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-04-08 07:25:17.098174 pwdata-0.2.12/setup.cfg
--rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      825 2024-04-08 07:25:11.000000 pwdata-0.2.12/setup.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.129897 pwdata-0.2.13/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    35148 2024-02-27 08:01:20.000000 pwdata-0.2.13/LICENSE
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-28 02:07:45.129295 pwdata-0.2.13/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       51 2024-03-08 09:41:47.000000 pwdata-0.2.13/README.md
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.011114 pwdata-0.2.13/pwdata/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      283 2024-03-05 03:01:36.000000 pwdata-0.2.13/pwdata/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2657 2024-02-28 03:42:10.000000 pwdata-0.2.13/pwdata/atomconfig.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.029347 pwdata-0.2.13/pwdata/build/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:13.000000 pwdata-0.2.13/pwdata/build/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5902 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/build/cell.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2815 2024-02-28 03:47:20.000000 pwdata-0.2.13/pwdata/build/geometry.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3886 2024-03-05 02:57:00.000000 pwdata-0.2.13/pwdata/build/supercells.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    15467 2024-03-29 08:35:53.000000 pwdata-0.2.13/pwdata/build/write_struc.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.082070 pwdata-0.2.13/pwdata/calculators/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:16.000000 pwdata-0.2.13/pwdata/calculators/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14172 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/calculators/const.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     4873 2024-02-27 07:50:22.000000 pwdata-0.2.13/pwdata/calculators/unitconvert_lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     7964 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/calculators/units.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    14250 2024-02-28 03:43:29.000000 pwdata-0.2.13/pwdata/cp2kdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5439 2024-03-01 02:53:29.000000 pwdata-0.2.13/pwdata/datasets_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6069 2024-05-27 01:29:52.000000 pwdata-0.2.13/pwdata/deepmd.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     8826 2024-02-28 03:44:14.000000 pwdata-0.2.13/pwdata/dump.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1649 2024-05-16 06:19:11.000000 pwdata-0.2.13/pwdata/extendedxyz.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    11611 2024-04-08 08:59:39.000000 pwdata-0.2.13/pwdata/image.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    13928 2024-02-28 03:45:13.000000 pwdata-0.2.13/pwdata/lammpsdata.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     1661 2024-02-27 07:43:28.000000 pwdata-0.2.13/pwdata/lmps.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)    16592 2024-03-27 09:50:17.000000 pwdata-0.2.13/pwdata/main.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     5350 2024-03-18 07:39:03.000000 pwdata-0.2.13/pwdata/movement.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2587 2024-03-05 02:49:08.000000 pwdata-0.2.13/pwdata/movement_saver.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     6925 2024-04-08 09:00:41.000000 pwdata-0.2.13/pwdata/outcar.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.128104 pwdata-0.2.13/pwdata/pertub/
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        0 2024-02-28 01:41:19.000000 pwdata-0.2.13/pwdata/pertub/__init__.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     9133 2024-03-05 02:56:31.000000 pwdata-0.2.13/pwdata/pertub/perturbation.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2446 2024-03-05 02:56:46.000000 pwdata-0.2.13/pwdata/pertub/scale.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     3066 2024-02-28 03:46:19.000000 pwdata-0.2.13/pwdata/poscar.py
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)     2837 2024-04-08 07:46:55.000000 pwdata-0.2.13/pwdata/pwmlff.py
+drwxrwxr-x   0 hfhuang  (10186) hfhuang  (10186)        0 2024-05-28 02:07:45.128637 pwdata-0.2.13/pwdata.egg-info/
+-rw-r--r--   0 hfhuang  (10186) hfhuang  (10186)      660 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/PKG-INFO
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      777 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        1 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)        7 2024-05-28 02:07:44.000000 pwdata-0.2.13/pwdata.egg-info/top_level.txt
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)       38 2024-05-28 02:07:45.130009 pwdata-0.2.13/setup.cfg
+-rw-rw-r--   0 hfhuang  (10186) hfhuang  (10186)      825 2024-05-28 02:07:26.000000 pwdata-0.2.13/setup.py
```

### Comparing `pwdata-0.2.12/LICENSE` & `pwdata-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/PKG-INFO` & `pwdata-0.2.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.12
+Version: 0.2.13
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.12/pwdata/atomconfig.py` & `pwdata-0.2.13/pwdata/atomconfig.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/build/cell.py` & `pwdata-0.2.13/pwdata/build/cell.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/build/geometry.py` & `pwdata-0.2.13/pwdata/build/geometry.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/build/supercells.py` & `pwdata-0.2.13/pwdata/build/supercells.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/build/write_struc.py` & `pwdata-0.2.13/pwdata/build/write_struc.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/calculators/const.py` & `pwdata-0.2.13/pwdata/calculators/const.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/calculators/unitconvert_lmps.py` & `pwdata-0.2.13/pwdata/calculators/unitconvert_lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/calculators/units.py` & `pwdata-0.2.13/pwdata/calculators/units.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/cp2kdata.py` & `pwdata-0.2.13/pwdata/cp2kdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/datasets_saver.py` & `pwdata-0.2.13/pwdata/datasets_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/deepmd.py` & `pwdata-0.2.13/pwdata/deepmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,25 @@
         atom_type = list(sc.keys())
         atom_type_num = list(sc.values())
         # atom_type_num = [atom_types_image.count(atom) for atom in set(atom_types_image)]
 
         box, coord, energy, force, virial, image_nums = self.load_npy(npy_files, atom_nums)
 
         for i in range(image_nums):
-            image = Image(lattice=box[i], position=coord[i], force=force[i], Ep=energy[i], stress=virial[i],
+            virial_image = virial[i] if virial is not None else None
+            image = Image(lattice=box[i], position=coord[i], force=force[i], Ep=energy[i], stress=virial_image,
                           atom_type=atom_type, atom_nums=atom_nums, atom_types_image=atom_types_image, atom_type_num=atom_type_num,
                           cartesian=True, image_nums=i)
             atomic_energy, _, _, _ = np.linalg.lstsq([atom_type_num], np.array([image.Ep]), rcond=1e-3)
             atomic_energy = np.repeat(atomic_energy, atom_type_num)
             image.atomic_energy = atomic_energy.tolist()
             self.image_list.append(image)
         
     def load_npy(self, npy_files, atom_nums):
+        virial = None
         for npy_file in tqdm(npy_files, desc="Loading data"):
             if "box" in npy_file:
                 box = np.load(npy_file).reshape(-1, 3, 3).astype(np.float64)
             elif "coord" in npy_file:
                 coord = np.load(npy_file).reshape(-1, atom_nums, 3)
             elif "energy" in npy_file:
                 energy = np.load(npy_file)
```

### Comparing `pwdata-0.2.12/pwdata/dump.py` & `pwdata-0.2.13/pwdata/dump.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/extendedxyz.py` & `pwdata-0.2.13/pwdata/extendedxyz.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     data_name = open(os.path.join(output_path, data_name), write_patthen)
     for i in range(len(image_data_all)):
         image_data = image_data_all[i]
         if not image_data.cartesian:
             image_data._set_cartesian()
         data_name.write("%d\n" % image_data.atom_nums)
         # data_name.write("Iteration: %s\n" % image_data.iteration)
-        output_head = 'Lattice="%.2f %.2f %.2f %.2f %.2f %.2f %.2f %.2f %.2f" Properties=species:S:1:pos:R:3:force:R:3:local_energy:R:1 pbc="T T T" energy={}\n'.format(image_data.Ep)
+        output_head = 'Lattice="%.2f %.2f %.2f %.2f %.2f %.2f %.2f %.2f %.2f" Properties=species:S:1:pos:R:3:forces:R:3:local_energy:R:1 pbc="T T T" energy={}\n'.format(image_data.Ep)
         output_extended = (image_data.lattice[0][0], image_data.lattice[0][1], image_data.lattice[0][2], 
                                 image_data.lattice[1][0], image_data.lattice[1][1], image_data.lattice[1][2], 
                                 image_data.lattice[2][0], image_data.lattice[2][1], image_data.lattice[2][2])
         data_name.write(output_head % output_extended)
         for j in range(image_data.atom_nums):
             properties_format = "%s %14.8f %14.8f %14.8f %14.8f %14.8f %14.8f %14.8f\n"
             properties = (elements[image_data.atom_types_image[j]], image_data.position[j][0], image_data.position[j][1], image_data.position[j][2],
```

### Comparing `pwdata-0.2.12/pwdata/image.py` & `pwdata-0.2.13/pwdata/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,18 +235,20 @@
         >>> atom_nums = 56
         >>> elements_to_order(atom_names, atom_types_image, atom_nums)
         [6, 6, 6, 6, 6, ... , 7, 7, 7, 7, 7, ... , 7]
         
     Returns:
         list: Updated list of atom types per atom.
     """
-    for idx, name in enumerate(atom_names):
-        for ii in range(atom_nums):
-            if name in elements and atom_types_image[ii] == idx+1:
-                atom_types_image[ii] = elements.index(name)
+    # for idx, name in enumerate(atom_names):
+    #     for ii in range(atom_nums):
+    #         if name in elements and atom_types_image[ii] == idx+1:
+    #             atom_types_image[ii] = elements.index(name)
+    type_mapping = {idx+1: elements.index(name) for idx, name in enumerate(atom_names)}
+    atom_types_image = [type_mapping[atom_type] for atom_type in atom_types_image]
     return atom_types_image
 
 def frac2cart(position, lattice):
     """
     Convert fractional coordinates to Cartesian coordinates.
 
     Args:
```

### Comparing `pwdata-0.2.12/pwdata/lammpsdata.py` & `pwdata-0.2.13/pwdata/lammpsdata.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/lmps.py` & `pwdata-0.2.13/pwdata/lmps.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/main.py` & `pwdata-0.2.13/pwdata/main.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/movement.py` & `pwdata-0.2.13/pwdata/movement.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/movement_saver.py` & `pwdata-0.2.13/pwdata/movement_saver.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/outcar.py` & `pwdata-0.2.13/pwdata/outcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,18 @@
         atom_type_num = None
         nelm = None
         for idx, ii in enumerate(outcar_contents):
             if "POTCAR" in ii:
                 # get atom names from POTCAR info, tested only for PAW_PBE ...
                 _ii = ii.split()[2]
                 if '_' in _ii:
-                    atom_names.append(_ii.split('_')[0])
+                    # atom_names.append(_ii.split('_')[0])
+                    atom_name = _ii.split('_')[0]
+                    if atom_name not in atom_names:
+                        atom_names.append(atom_name)
                 else:
                     atom_name = _ii
                     if atom_name not in atom_names:
                         atom_names.append(atom_name)
             elif 'ions per type' in ii:
                 atom_type_num_ = [int(s) for s in ii.split()[4:]]
                 if atom_type_num is None:
```

### Comparing `pwdata-0.2.12/pwdata/pertub/perturbation.py` & `pwdata-0.2.13/pwdata/pertub/perturbation.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/pertub/scale.py` & `pwdata-0.2.13/pwdata/pertub/scale.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/poscar.py` & `pwdata-0.2.13/pwdata/poscar.py`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/pwdata/pwmlff.py` & `pwdata-0.2.13/pwdata/pwmlff.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,8 +54,8 @@
             elif "position" in npy_file:
                 coord = np.load(npy_file) if coord is None else np.concatenate((coord, np.load(npy_file)))
 
         image_nums = len(Ep)
         atom_nums = len(atom_types_image)
         stress = stress.reshape(-1, 3, 3) if stress is not None else None
 
-        return atom_type, atomic_energy.squeeze(), Ep.squeeze(), force.squeeze(), atom_types_image, lattice.squeeze(), coord.squeeze(), stress, image_nums, atom_nums
+        return atom_type, atomic_energy, Ep.squeeze(), force, atom_types_image, lattice, coord, stress, image_nums, atom_nums
```

### Comparing `pwdata-0.2.12/pwdata.egg-info/PKG-INFO` & `pwdata-0.2.13/pwdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdata
-Version: 0.2.12
+Version: 0.2.13
 Summary: pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.
 Home-page: https://github.com/LonxunQuantum/pwdata
 Author: LonxunQuantum
 Author-email: lonxun@pwmat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pwdata-0.2.12/pwdata.egg-info/SOURCES.txt` & `pwdata-0.2.13/pwdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwdata-0.2.12/setup.py` & `pwdata-0.2.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pwdata", 
-    version="0.2.12",
+    version="0.2.13",
     author="LonxunQuantum",
     author_email="lonxun@pwmat.com",
     description="pwdata is a data pre-processing tool for PWMLFF, which can be used to extract features and labels. It also provides convenient interfaces for data conversion between different software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LonxunQuantum/pwdata",
     packages=setuptools.find_packages(),
```

