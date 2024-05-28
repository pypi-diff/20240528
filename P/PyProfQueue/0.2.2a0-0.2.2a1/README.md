# Comparing `tmp/PyProfQueue-0.2.2a0.tar.gz` & `tmp/PyProfQueue-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.2.2a0.tar", last modified: Wed May 22 15:10:28 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.2a1.tar", last modified: Tue May 28 11:25:19 2024, max compression
```

## Comparing `PyProfQueue-0.2.2a0.tar` & `PyProfQueue-0.2.2a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      406 2024-05-22 15:10:24.000000 PyProfQueue-0.2.2a0/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/PyProfQueue/profilers/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/_template_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1709 2024-05-22 12:36:52.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/linaro_forge_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8049 2024-05-22 15:09:21.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/likwid.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4305 2024-05-22 14:18:57.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/linaro_forge.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a0/PyProfQueue/profilers/prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a0/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a0/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-22 15:10:28.000000 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      666 2024-05-22 15:10:28.000000 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-22 15:10:28.000000 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-22 15:10:28.000000 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-22 15:10:28.000000 PyProfQueue-0.2.2a0/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a0/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-22 15:10:28.401368 PyProfQueue-0.2.2a0/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-22 15:10:24.000000 PyProfQueue-0.2.2a0/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      407 2024-05-28 11:25:07.000000 PyProfQueue-0.2.2a1/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1688 2024-05-28 11:24:21.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/linaro_forge_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8049 2024-05-28 08:56:46.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4305 2024-05-22 14:18:57.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/linaro_forge.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a1/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a1/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a1/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 11:25:19.799447 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      666 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-28 11:25:19.000000 PyProfQueue-0.2.2a1/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a1/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-28 11:25:19.803447 PyProfQueue-0.2.2a1/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-28 11:25:07.000000 PyProfQueue-0.2.2a1/setup.py
```

### Comparing `PyProfQueue-0.2.2a0/PKG-INFO` & `PyProfQueue-0.2.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a0
+Version: 0.2.2a1
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/likwid_commands.txt` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/likwid_commands.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 likwid-bench -t load_avx -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 export BEST_BAND=$(grep -oP 'MByte/s:\s*\K\d+' ${LIK_OUTPUT} | sort -n | tail -n 1)
 # *=*
 sleep 1
 echo 'Program Performance' >> ${LIK_OUTPUT}
 grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' ${WORKING_DIR}/job_output_setup.txt >> ${LIK_OUTPUT}
 
-# Check if cwl file exists to call the script with that file
+echo 'Plotting Likwid output as series'
 ${PYTHON_INSTANCE} -c "import PyProfQueue.profilers.likwid as lik;"\
 "lik.plot_roof_timeseries(likwid_file='${LIKWID_RUNNING_DIR}/likwid_output.txt', "\
 "name_prefix='${WORKING_DIR}/Likwid', maxperf=${BEST_PERF}, maxband=${BEST_BAND})"
```

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/prometheus_commands.txt` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/data/read_prometheus.py` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/likwid.py` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/likwid.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/linaro_forge.py` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/linaro_forge.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/profilers/prometheus.py` & `PyProfQueue-0.2.2a1/PyProfQueue/profilers/prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/script.py` & `PyProfQueue-0.2.2a1/PyProfQueue/script.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue/submission.py` & `PyProfQueue-0.2.2a1/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.2.2a1/PyProfQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a0
+Version: 0.2.2a1
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a0/PyProfQueue.egg-info/SOURCES.txt` & `PyProfQueue-0.2.2a1/PyProfQueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/ReadMe.md` & `PyProfQueue-0.2.2a1/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a0/setup.py` & `PyProfQueue-0.2.2a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.2.2a0',
+    version='0.2.2a1',
     url='https://github.com/uksrc-developers/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md',
```

