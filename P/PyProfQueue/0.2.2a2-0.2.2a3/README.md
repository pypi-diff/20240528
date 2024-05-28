# Comparing `tmp/PyProfQueue-0.2.2a2.tar.gz` & `tmp/PyProfQueue-0.2.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.2.2a2.tar", last modified: Tue May 28 14:55:47 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.2a3.tar", last modified: Tue May 28 15:01:12 2024, max compression
```

## Comparing `PyProfQueue-0.2.2a2.tar` & `PyProfQueue-0.2.2a3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1569 2024-05-28 12:53:45.000000 PyProfQueue-0.2.2a2/PyProfQueue/Test_PyProfQueue.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      405 2024-05-28 14:52:21.000000 PyProfQueue-0.2.2a2/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/profilers/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       46 2024-05-28 14:52:35.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/_template_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1688 2024-05-28 11:24:21.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/linaro_forge_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     7854 2024-05-28 14:48:01.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/likwid.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4308 2024-05-28 11:55:18.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/linaro_forge.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a2/PyProfQueue/profilers/prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a2/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a2/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      698 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-28 14:55:47.000000 PyProfQueue-0.2.2a2/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a2/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-28 14:55:47.487489 PyProfQueue-0.2.2a2/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-28 14:49:01.000000 PyProfQueue-0.2.2a2/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1570 2024-05-28 14:57:47.000000 PyProfQueue-0.2.2a3/PyProfQueue/Test_PyProfQueue.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      405 2024-05-28 15:00:59.000000 PyProfQueue-0.2.2a3/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       46 2024-05-28 14:52:35.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1695 2024-05-28 15:00:59.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       64 2024-05-22 13:33:14.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/linaro_forge_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     7854 2024-05-28 14:48:01.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4308 2024-05-28 11:55:18.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/linaro_forge.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2a3/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2a3/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2a3/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23308 2024-05-28 15:01:12.000000 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      698 2024-05-28 15:01:12.000000 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-28 15:01:12.000000 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-28 15:01:12.000000 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-28 15:01:12.000000 PyProfQueue-0.2.2a3/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2a3/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-28 15:01:12.761370 PyProfQueue-0.2.2a3/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1508 2024-05-28 15:00:59.000000 PyProfQueue-0.2.2a3/setup.py
```

### Comparing `PyProfQueue-0.2.2a2/PKG-INFO` & `PyProfQueue-0.2.2a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/Test_PyProfQueue.py` & `PyProfQueue-0.2.2a3/PyProfQueue/Test_PyProfQueue.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 
 ppq.submit(ProfileScript,
            tmp_work_script='/home/marcuskeil/Projects/RSE/Package_Development/Test/tmp_work.sh',
            tmp_profile_script='/home/marcuskeil/Projects/RSE/Package_Development/Test/tmp_profile.sh',
            bash_options=['/cosma5/data/do011/dc-keil1/TestFiles/Codes/export_variables.source', '${WORKING_DIR}'],
            leave_scripts=True,
            test=True)
+
```

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/likwid_commands.txt` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/likwid_commands.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 sleep 1
 echo 'Program Performance' >> ${LIK_OUTPUT}
 grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' ${WORKING_DIR}/job_output_setup.txt >> ${LIK_OUTPUT}
 
 echo 'Plotting Likwid output as series'
 ${PYTHON_INSTANCE} -c "import PyProfQueue.profilers.likwid as lik;"\
 "lik.plot_roof_timeseries(likwid_file='${LIKWID_RUNNING_DIR}/likwid_output.txt', "\
-"name_prefix='${WORKING_DIR}/Likwid', maxperf=${BEST_PERF}, maxband=${BEST_BAND})"
+"name_prefix='${LIKWID_RUNNING_DIR}/Likwid', maxperf=${BEST_PERF}, maxband=${BEST_BAND})"
```

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/prometheus_commands.txt` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/data/read_prometheus.py` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/likwid.py` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/likwid.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/linaro_forge.py` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/linaro_forge.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/profilers/prometheus.py` & `PyProfQueue-0.2.2a3/PyProfQueue/profilers/prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/script.py` & `PyProfQueue-0.2.2a3/PyProfQueue/script.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue/submission.py` & `PyProfQueue-0.2.2a3/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.2.2a3/PyProfQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.2a2/PyProfQueue.egg-info/SOURCES.txt` & `PyProfQueue-0.2.2a3/PyProfQueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/ReadMe.md` & `PyProfQueue-0.2.2a3/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.2a2/setup.py` & `PyProfQueue-0.2.2a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.2.2a2',
+    version='0.2.2a3',
     url='https://github.com/uksrc-developers/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md',
```

