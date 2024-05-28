# Comparing `tmp/PyProfQueue-0.2.2a1.tar.gz` & `tmp/PyProfQueue-0.2.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.2.2a1.tar", last modified: Tue May 28 11:25:19 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.2a2.tar", last modified: Tue May 28 14:55:47 2024, max compression
```

## Comparing `PyProfQueue-0.2.2a1.tar` & `PyProfQueue-0.2.2a2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      407 2024-05-28 11:25:07.000000 PyProfQueue-0.2.2a1/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue/profilers/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/_template_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1688 2024-05-28 11:24:21.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/linaro_forge_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8049 2024-05-28 08:56:46.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/likwid.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4305 2024-05-22 14:18:57.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/linaro_forge.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a1/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a1/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      666 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a1/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-28 11:25:07.000000 PyProfQueue-0.2.2a1/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1569 2024-05-28 12:53:45.000000 PyProfQueue-0.2.2a2/PyProfQueue/Test_PyProfQueue.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      405 2024-05-28 14:52:21.000000 PyProfQueue-0.2.2a2/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       46 2024-05-28 14:52:35.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1688 2024-05-28 11:24:21.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/linaro_forge_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     7854 2024-05-28 14:48:01.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4308 2024-05-28 11:55:18.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/linaro_forge.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a2/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a2/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      698 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a2/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-28 14:49:01.000000 PyProfQueue-0.2.2a2/setup.py
```

### Comparing `PyProfQueue-0.2.2a1/PKG-INFO` & `PyProfQueue-0.2.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/likwid_commands.txt` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/prometheus_commands.txt` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/read_prometheus.py` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/likwid.py` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/likwid.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     tmp_work_script: str = Path and name of the temporary work script that contains all the users code minus
         queue options.
 
     Returns
     -------
     None
     """
-    profilefile.write('likwid-perfctr -g MEM_DP -t 10s -o ${LIKWID_RUNNING_DIR}/likwid_output.txt -O -f bash ' +
+    profilefile.write('likwid-perfctr -g MEM_DP -t 5m -o ${LIKWID_RUNNING_DIR}/likwid_output.txt -O -f bash ' +
                       '{} {}\n'.format(tmp_work_script, ' '.join(str(x) for x in bash_options)))
     profilefile.write('\n')
     return
 
 
 def define_end(profilefile: io.TextIOWrapper):
     """
@@ -159,38 +159,34 @@
     return time, op_int, flop_s
 
 
 def plot_roof_timeseries(likwid_file: str, name_prefix: str, maxperf: float, maxband: float, code_name: str = 'code'):
     time_series, code_opint, code_mflop = read_timeseries(likwid_file)
     points = np.array([code_opint, code_mflop]).T.reshape(-1, 1, 2)
     segments = np.concatenate([points[:-1], points[1:]], axis=1)
-    if code_opint.mean() * maxband < maxperf:
-        percentage = int((code_mflop.mean() / (code_opint.mean() * maxband)) * 100)
-    else:
-        percentage = int((code_mflop.mean() / maxperf) * 100)
 
     if maxperf / maxband > 1:
         max_x = (maxperf / maxband) * 2
     else:
         max_x = 1
 
-    if max_x < code_opint.max():
-        max_x = code_opint
+    if max_x < code_opint.mean():
+        max_x = code_opint.mean()
 
     x_axis = np.append(np.linspace(0, maxperf / maxband, 10), max_x)
     y = np.array([x * maxband if ((x * maxband) < maxperf) else maxperf for x in x_axis])
 
     fig, axs = plt.subplots(1, 1, sharex=True, sharey=True)
     norm = plt.Normalize(time_series.min(), time_series.max())
 
     lc = collection.LineCollection(segments, cmap='viridis', norm=norm)
     lc.set_array(time_series)
     lc.set_linewidth(2)
 
-    pc = collection.RegularPolyCollection(numsides=4, offsets=points.reshape(12, 2), offset_transform=axs.transData,
+    pc = collection.RegularPolyCollection(numsides=4, offsets=points.reshape(-1, 2), offset_transform=axs.transData,
                                           cmap='viridis', norm=norm, sizes=[100] * len(time_series))
     pc.set_array(time_series)
     pc.set_label(code_name)
 
     axs.plot(x_axis, y, label="Hardware Roofline")
     axs.vlines(maxperf / maxband, 0, maxperf, linestyle='--', color='gray', alpha=0.5,
                label='Mem BandWidth to CPU limit boarder')
```

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/linaro_forge.py` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/linaro_forge.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,23 +26,22 @@
     global linaro_forge_initEndSplit
     if 'code_line' not in profilerdict.keys():
         exit("Linaro Forge requires the 'code_line' entry containing the string of the line where Linaro Forge "
              "should be used for profiling.")
     if 'work_script' not in profilerdict.keys():
         exit("Linaro Forge requires the 'work_script' entry listing the path of the file that should have profiling "
              "injected into it.")
-
+    
     with open(profilerdict['work_script'], 'r') as work_script:
         work = work_script.readlines()
         for line in work:
             for code_line in profilerdict['code_line']:
                 if code_line == line:
                     line = "map --profile --no-queue " + line
 
-
     profilefile.write('# linaro_forge initialisation declarations\n')
     if 'requirements' in profilerdict.keys():
         for i in profilerdict['requirements']:
             profilefile.write(i)
             profilefile.write('\n')
     profilefile.write('\n')
     profilefile.write('export LINARO_FORGE_RUNNING_DIR=${WORKING_DIR}/<Template_Profiler>\n')
```

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/profilers/prometheus.py` & `PyProfQueue-0.2.2a2/PyProfQueue/profilers/prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/script.py` & `PyProfQueue-0.2.2a2/PyProfQueue/script.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue/submission.py` & `PyProfQueue-0.2.2a2/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.2.2a2/PyProfQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a1/PyProfQueue.egg-info/SOURCES.txt` & `PyProfQueue-0.2.2a2/PyProfQueue.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 setup.py
+PyProfQueue/Test_PyProfQueue.py
 PyProfQueue/__init__.py
 PyProfQueue/script.py
 PyProfQueue/submission.py
 PyProfQueue.egg-info/PKG-INFO
 PyProfQueue.egg-info/SOURCES.txt
 PyProfQueue.egg-info/dependency_links.txt
 PyProfQueue.egg-info/requires.txt
```

### Comparing `PyProfQueue-0.2.2a1/ReadMe.md` & `PyProfQueue-0.2.2a2/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a1/setup.py` & `PyProfQueue-0.2.2a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.2.2a1',
+    version='0.2.2a2',
     url='https://github.com/uksrc-developers/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md',
```

