# Comparing `tmp/jobqueues-0.9.6.tar.gz` & `tmp/jobqueues-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobqueues-0.9.6.tar", last modified: Mon May 20 13:55:47 2024, max compression
+gzip compressed data, was "jobqueues-0.9.7.tar", last modified: Tue May 28 11:34:19 2024, max compression
```

## Comparing `jobqueues-0.9.6.tar` & `jobqueues-0.9.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 13:54:52.000000 jobqueues-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 13:55:47.362477 jobqueues-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 13:54:52.000000 jobqueues-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/jobqueues/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 13:55:47.362477 jobqueues-0.9.6/jobqueues/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/jobqueues/celeryfiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/celeryfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/celeryfiles/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/celeryfiles/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/celeryqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/config_lsf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/config_slurm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/localqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/logging.ini
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/lsfqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/pbsqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/sgequeue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/simqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/slurmqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/jobqueues/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/templates/SGE_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/templates/SLURM_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-20 13:54:52.000000 jobqueues-0.9.6/jobqueues/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/jobqueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 13:55:47.000000 jobqueues-0.9.6/jobqueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-20 13:55:47.000000 jobqueues-0.9.6/jobqueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:55:47.000000 jobqueues-0.9.6/jobqueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:55:38.000000 jobqueues-0.9.6/jobqueues.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 13:55:47.000000 jobqueues-0.9.6/jobqueues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:55:47.000000 jobqueues-0.9.6/jobqueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 13:54:52.000000 jobqueues-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 13:55:47.362477 jobqueues-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 13:54:52.000000 jobqueues-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:55:47.362477 jobqueues-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-20 13:54:52.000000 jobqueues-0.9.6/tests/test_slurmqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.984199 jobqueues-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 11:33:20.000000 jobqueues-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 11:34:19.984199 jobqueues-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 11:33:20.000000 jobqueues-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.984199 jobqueues-0.9.7/jobqueues/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-28 11:34:19.984199 jobqueues-0.9.7/jobqueues/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.980199 jobqueues-0.9.7/jobqueues/celeryfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/celeryfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/celeryfiles/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/celeryfiles/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/celeryqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/config_lsf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/config_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/localqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/lsfqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/pbsqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/sgequeue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/simqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20995 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/slurmqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.980199 jobqueues-0.9.7/jobqueues/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/templates/SGE_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/templates/SLURM_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-28 11:33:20.000000 jobqueues-0.9.7/jobqueues/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.984199 jobqueues-0.9.7/jobqueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 11:34:19.000000 jobqueues-0.9.7/jobqueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-28 11:34:19.000000 jobqueues-0.9.7/jobqueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:34:19.000000 jobqueues-0.9.7/jobqueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:34:11.000000 jobqueues-0.9.7/jobqueues.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 11:34:19.000000 jobqueues-0.9.7/jobqueues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 11:34:19.000000 jobqueues-0.9.7/jobqueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-28 11:33:20.000000 jobqueues-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 11:34:19.984199 jobqueues-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 11:33:20.000000 jobqueues-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:34:19.980199 jobqueues-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-28 11:33:20.000000 jobqueues-0.9.7/tests/test_slurmqueue.py
```

### Comparing `jobqueues-0.9.6/PKG-INFO` & `jobqueues-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.6
+Version: 0.9.7
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.6/jobqueues/celeryfiles/tasks.py` & `jobqueues-0.9.7/jobqueues/celeryfiles/tasks.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/celeryqueue.py` & `jobqueues-0.9.7/jobqueues/celeryqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/config.py` & `jobqueues-0.9.7/jobqueues/config.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/home.py` & `jobqueues-0.9.7/jobqueues/home.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/localqueue.py` & `jobqueues-0.9.7/jobqueues/localqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/lsfqueue.py` & `jobqueues-0.9.7/jobqueues/lsfqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/pbsqueue.py` & `jobqueues-0.9.7/jobqueues/pbsqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/playqueue.py` & `jobqueues-0.9.7/jobqueues/playqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/sgequeue.py` & `jobqueues-0.9.7/jobqueues/sgequeue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/simqueue.py` & `jobqueues-0.9.7/jobqueues/simqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/slurmqueue.py` & `jobqueues-0.9.7/jobqueues/slurmqueue.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,18 +324,23 @@
                 return None
             raise FileNotFoundError(
                 "Could not find required executable [{}]".format(binary)
             )
         ret = os.path.abspath(ret)
         return ret
 
-    def _createJobScript(self, fname, workdir, runsh, nvidia_mps=False):
+    def _createJobScript(self, fname, workdir, runsh, nvidia_mps=False, commands=None):
         from jobqueues.config import template_env
 
+        # Create a list of lists with the directory of the run.sh and the run.sh itself
         runsh = ensurelist(runsh)
+        if commands is None:
+            runsh = [[os.path.dirname(os.path.abspath(x)), x] for x in runsh]
+        else:
+            runsh = [[workdir, runsh[0]]]
 
         workdir = os.path.abspath(workdir)
         sentinel = os.path.normpath(os.path.join(workdir, self._sentinel))
 
         # Move completed trajectories
         odir = None
         if self.datadir is not None:
@@ -352,16 +357,14 @@
         errorstream = self.errorstream
         outputstream = self.outputstream
         if not self.useworkdir:
             workdir = "/tmp/"
             errorstream = None
             outputstream = None
             sentinel = None
-        else:
-            prerun += [f"cd {workdir}"]
 
         template = template_env.get_template("SLURM_job.sh.j2")
         job_str = template.render(
             jobname=self.jobname,
             partition=",".join(ensurelist(self.partition)),
             ncpu=self.ncpu,
             memory=self.memory,
@@ -460,15 +463,15 @@
             if self.jobname is None:
                 self.jobname = self._autoJobName(d)
 
             runscript = commands[i] if commands is not None else self._getRunScript(d)
             self._cleanSentinel(d)
 
             jobscript = os.path.abspath(os.path.join(d, self.jobscript))
-            self._createJobScript(jobscript, d, runscript)
+            self._createJobScript(jobscript, d, runscript, commands=commands)
             try:
                 if _dryrun:
                     logger.info(f"Dry run. Here it would call submit on {jobscript}")
                 else:
                     ret = check_output([self._qsubmit, jobscript])
                     logger.debug(ret.decode("ascii"))
             except CalledProcessError as e:
```

### Comparing `jobqueues-0.9.6/jobqueues/templates/SGE_job.sh.j2` & `jobqueues-0.9.7/jobqueues/templates/SGE_job.sh.j2`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues/templates/SLURM_job.sh.j2` & `jobqueues-0.9.7/jobqueues/templates/SLURM_job.sh.j2`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,21 @@
 # mps-control remaps the index of the device it is running on to 0 so we 
 # need to unset it to avoid "cuda_error_no_device"
 
 unset CUDA_VISIBLE_DEVICES
 {% endif %}
 
 {% for rsh in runsh %}
-{{ rsh }} {% if run_as_daemon %} | tee log_{{loop.index}}.txt &{% endif %}
+cd {{ rsh[0] }}
+{{ rsh[1] }} {% if run_as_daemon %} | tee log_{{loop.index}}.txt &{% endif %}
 
 {% endfor %}
+{% if runsh|length > 1 %}
+cd {{ workdir }}
+{% endif %}
 
 {% if nvidia_mps %}
 wait
 # quit the server and the control. It will only quit the one corresponding to the CUDA_MPS_PIPE_DIRECTORY env variable
 echo quit | nvidia-cuda-mps-control
 {% endif %}
```

### Comparing `jobqueues-0.9.6/jobqueues/util.py` & `jobqueues-0.9.7/jobqueues/util.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/jobqueues.egg-info/PKG-INFO` & `jobqueues-0.9.7/jobqueues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.6
+Version: 0.9.7
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.6/jobqueues.egg-info/SOURCES.txt` & `jobqueues-0.9.7/jobqueues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/pyproject.toml` & `jobqueues-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.6/tests/test_slurmqueue.py` & `jobqueues-0.9.7/tests/test_slurmqueue.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,35 +61,31 @@
         for key in reference[appkey]:
             assert (
                 sq.__getattribute__(key) == reference[appkey][key]
             ), f'Config setup of SlurmQueue failed on app "{appkey}" and key "{key}""'
 
 
 def _test_submit_command(datadir):
-    import tempfile
+    execdir = str(datadir.join("0"))
+    os.makedirs(execdir, exist_ok=True)
 
     sl = SlurmQueue(_findExecutables=False)
     sl.partition = "jobqueues_test"
     sl.ngpu = 2
     sl.gpumemory = 2000
     sl.exclude = ["node1", "node4"]
     sl.nodelist = ["node2"]
     sl.envvars = "TEST=3"
     sl.useworkdir = False
 
-    with tempfile.TemporaryDirectory() as tmpdir:
-        try:
-            sl.submit([tmpdir], commands=["sleep 5"])
-        except Exception as e:
-            print(e)
-            pass
-
-        _compare_jobsh(
-            os.path.join(tmpdir, "job.sh"), datadir.join("_submit_command.sh"), tmpdir
-        )
+    sl.submit([execdir], commands=["sleep 5"], _dryrun=True)
+
+    _compare_jobsh(
+        os.path.join(execdir, "job.sh"), datadir.join("_submit_command.sh"), datadir
+    )
 
 
 def _test_submit_folder(datadir):
     execdir = _create_execdir(str(datadir.join("0")))
 
     sl = SlurmQueue(_findExecutables=False)
     sl.partition = "jobqueues_test"
```

