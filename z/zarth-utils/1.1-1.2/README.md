# Comparing `tmp/zarth_utils-1.1.tar.gz` & `tmp/zarth_utils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarth_utils-1.1.tar", last modified: Sun May 12 15:18:13 2024, max compression
+gzip compressed data, was "zarth_utils-1.2.tar", last modified: Tue May 28 09:40:17 2024, max compression
```

## Comparing `zarth_utils-1.1.tar` & `zarth_utils-1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.871268 zarth_utils-1.1/
--rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-12 15:18:13.871041 zarth_utils-1.1/PKG-INFO
--rw-r--r--   0 ghzhang    (501) staff       (20)       57 2023-11-29 00:34:14.000000 zarth_utils-1.1/README.md
--rw-r--r--   0 ghzhang    (501) staff       (20)      614 2024-05-12 15:12:05.000000 zarth_utils-1.1/pyproject.toml
--rw-r--r--   0 ghzhang    (501) staff       (20)       90 2023-11-29 00:34:14.000000 zarth_utils-1.1/requirements.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)       38 2024-05-12 15:18:13.871322 zarth_utils-1.1/setup.cfg
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.866597 zarth_utils-1.1/tests/
--rw-r--r--   0 ghzhang    (501) staff       (20)     1227 2023-11-29 00:35:23.000000 zarth_utils-1.1/tests/test_config.py
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.869183 zarth_utils-1.1/zarth_utils/
--rw-r--r--   0 ghzhang    (501) staff       (20)       78 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/__init__.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     9939 2024-05-12 15:11:46.000000 zarth_utils-1.1/zarth_utils/config.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     7215 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/drawer.py
--rw-r--r--   0 ghzhang    (501) staff       (20)      517 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/general_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)      276 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/jupyter_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     1547 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/logger.py
--rw-r--r--   0 ghzhang    (501) staff       (20)    10011 2023-11-29 00:35:23.000000 zarth_utils-1.1/zarth_utils/nn_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)    13043 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/result_recorder.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     2255 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/text_processing.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     2583 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/timer.py
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.870072 zarth_utils-1.1/zarth_utils.egg-info/
--rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/PKG-INFO
--rw-r--r--   0 ghzhang    (501) staff       (20)      491 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)        1 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)      211 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/requires.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)       12 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-28 09:40:17.260881 zarth_utils-1.2/
+-rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-28 09:40:17.260609 zarth_utils-1.2/PKG-INFO
+-rw-r--r--   0 ghzhang    (501) staff       (20)       57 2023-11-29 00:34:14.000000 zarth_utils-1.2/README.md
+-rw-r--r--   0 ghzhang    (501) staff       (20)      614 2024-05-28 09:40:06.000000 zarth_utils-1.2/pyproject.toml
+-rw-r--r--   0 ghzhang    (501) staff       (20)       90 2023-11-29 00:34:14.000000 zarth_utils-1.2/requirements.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)       38 2024-05-28 09:40:17.260944 zarth_utils-1.2/setup.cfg
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-28 09:40:17.255879 zarth_utils-1.2/tests/
+-rw-r--r--   0 ghzhang    (501) staff       (20)     1227 2023-11-29 00:35:23.000000 zarth_utils-1.2/tests/test_config.py
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-28 09:40:17.258608 zarth_utils-1.2/zarth_utils/
+-rw-r--r--   0 ghzhang    (501) staff       (20)       78 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/__init__.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)    10018 2024-05-28 08:54:22.000000 zarth_utils-1.2/zarth_utils/config.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     7215 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/drawer.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)      517 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/general_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)      276 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/jupyter_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     1547 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/logger.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)    10011 2023-11-29 00:35:23.000000 zarth_utils-1.2/zarth_utils/nn_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)    13905 2024-05-28 09:38:02.000000 zarth_utils-1.2/zarth_utils/recorder.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     2255 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/text_processing.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     2583 2023-11-29 00:34:14.000000 zarth_utils-1.2/zarth_utils/timer.py
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-28 09:40:17.259621 zarth_utils-1.2/zarth_utils.egg-info/
+-rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-28 09:40:17.000000 zarth_utils-1.2/zarth_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ghzhang    (501) staff       (20)      484 2024-05-28 09:40:17.000000 zarth_utils-1.2/zarth_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)        1 2024-05-28 09:40:17.000000 zarth_utils-1.2/zarth_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)      211 2024-05-28 09:40:17.000000 zarth_utils-1.2/zarth_utils.egg-info/requires.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)       12 2024-05-28 09:40:17.000000 zarth_utils-1.2/zarth_utils.egg-info/top_level.txt
```

### Comparing `zarth_utils-1.1/PKG-INFO` & `zarth_utils-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarth_utils
-Version: 1.1
+Version: 1.2
 Summary: Package used for my personal development on ML projects.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: pandas
 Requires-Dist: numpy
```

### Comparing `zarth_utils-1.1/pyproject.toml` & `zarth_utils-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zarth_utils"
 description = "Package used for my personal development on ML projects."
-version = "1.1"
+version = "1.2"
 dynamic = ["readme", "dependencies"]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 all = ["nltk", "torch", "tensorflow", "jupyterlab"]
 hf = ["transformers", "accelerate", "trl", "datasets", "diffusers", "tokenizers", "huggingface_hub"]
```

### Comparing `zarth_utils-1.1/tests/test_config.py` & `zarth_utils-1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/config.py` & `zarth_utils-1.2/zarth_utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .general_utils import get_random_time_stamp, makedir_if_not_exist
 from .logger import logging_info
 
 try:
     import wandb
 except ModuleNotFoundError as err:
     logging.warning("WandB not installed!")
+except TypeError as err:
+    logging.warning("WandB not properly installed!")
 
 dir_configs = os.path.join(os.getcwd(), "configs")
 
 
 def smart_load(path_file):
     if path_file.endswith("json"):
         return json.load(open(path_file, "r", encoding="utf-8"))
@@ -226,15 +228,15 @@
     """
     Parse the arguments from args into a config.
     """
     args_dict = vars(args)
     return Config(default_config_dict=args_dict, use_argparse=False)
 
 
-def is_configs_same(config_a, config_b, ignored_keys=("load_epoch",)):
+def are_configs_same(config_a, config_b, ignored_keys=("load_epoch",)):
     """
     Judge whether two configs are the same.
     Args:
         config_a: the first config
         config_b: the second config
         ignored_keys: thes keys that will be ignored when comparing
```

### Comparing `zarth_utils-1.1/zarth_utils/drawer.py` & `zarth_utils-1.2/zarth_utils/drawer.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/general_utils.py` & `zarth_utils-1.2/zarth_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/logger.py` & `zarth_utils-1.2/zarth_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/nn_utils.py` & `zarth_utils-1.2/zarth_utils/nn_utils.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/result_recorder.py` & `zarth_utils-1.2/zarth_utils/recorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,84 @@
-import json
 import os
+import sys
+import json
+import logging
+import platform
 import shutil
 import stat
 from json import JSONDecodeError
 
 import git
 import joblib
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from .config import Config
-from .general_utils import get_random_time_stamp
+from .general_utils import get_random_time_stamp, get_datetime
 from .logger import logging_info
-import logging
 
 try:
     import wandb
 except ModuleNotFoundError as err:
     logging.warning("WandB not installed!")
+except TypeError as err:
+    logging.warning("WandB not properly installed!")
 
 
-class ResultRecorder:
-    def __init__(self, path_record, initial_record=None, use_git=True, use_wandb=False):
+class Recorder:
+    def __init__(self, path_record, config=None, use_git=True, use_wandb=False):
         """
         Initialize the result recorder. The results will be saved in a temporary file defined by path_record.temp.
         To end recording and transfer the temporary files, self.end_recording() must be called.
         :param path_record: the saving path of the recorded results.
         :type path_record: str
-        :param initial_record: a record to be initialize with, usually the config in practice
+        :param config: a record to be initialize with, usually the config in practice
         """
         self.__ending = False
         self.__record = dict()
         self.use_wandb = use_wandb
 
-        self.__path_temp_record = "%s.result.temp" % path_record if not path_record.endswith(".result") \
-            else path_record + ".temp"
-        self.__path_record = "%s.result" % path_record if not path_record.endswith(".result") \
-            else path_record
-
-        if os.path.exists(self.__path_temp_record):
-            shutil.move(self.__path_temp_record, self.__path_temp_record + ".%s" % get_random_time_stamp())
-        if os.path.exists(self.__path_record):
-            shutil.move(self.__path_record, self.__path_record + ".%s" % get_random_time_stamp())
+        self.path_temp_record = "%s.result.temp" % path_record
+        self.path_record = "%s.result" % path_record
 
-        if initial_record is not None:
-            self.update(initial_record)
+        if os.path.exists(self.path_temp_record):
+            shutil.move(self.path_temp_record, self.path_temp_record + ".mv.%s" % get_random_time_stamp())
+        if os.path.exists(self.path_record):
+            shutil.move(self.path_record, self.path_record + ".mv.%s" % get_random_time_stamp())
+
+        if config is not None:
+            for k in config.keys():
+                self.__setitem__("config." + k, config[k])
+
+        self.__setitem__("meta_data.operating_system", platform.system())
+        self.__setitem__("meta_data.os_release", platform.release())
+        self.__setitem__("meta_data.platform", platform.platform())
+        self.__setitem__("meta_data.processor", platform.processor())
+        self.__setitem__("meta_data.args", " ".join(sys.argv))
+        self.__setitem__("meta_data.run_dir", os.getcwd())
+        self.__setitem__("meta_data.start_time", get_datetime())
 
         if use_git:
             repo = git.Repo(path=os.getcwd())
             assert not repo.is_dirty()
-            self.__setitem__("git_commit", repo.head.object.hexsha)
+            self.__setitem__("meta_data." + "git_commit", repo.head.object.hexsha)
+
+        self.path_requirement = "%s.env" % path_record
+        if os.path.exists(self.path_requirement):
+            shutil.move(self.path_requirement, self.path_requirement + ".mv.%s" % get_random_time_stamp())
+        os.system("conda env export --file %s" % self.path_requirement)
 
     def write_record(self, line):
         """
         Add a line to the recorded result file.
         :param line: the content to be write
         :type line: str
         """
-        with open(self.__path_temp_record, "a", encoding="utf-8") as fin:
+        with open(self.path_temp_record, "a", encoding="utf-8") as fin:
             fin.write(line + "\n")
 
     def keys(self):
         return self.__record.keys()
 
     def __getitem__(self, key):
         """
@@ -114,29 +130,32 @@
 
     def end_recording(self):
         """
         End the recording. This function will remove the .temp suffix of the recording file and add an END signal.
         :return:
         :rtype:
         """
+        assert "meta_data.end_time" not in self.keys()
+        self.__setitem__("meta_data.end_time", get_datetime())
         self.__ending = True
         self.write_record("\n$END$\n")
-        shutil.move(self.__path_temp_record, self.__path_record)
-        os.chmod(self.__path_record, stat.S_IREAD)
+
+        shutil.move(self.path_temp_record, self.path_record)
+        os.chmod(self.path_record, stat.S_IREAD)
 
     def dump(self, path_dump):
         """
         Dump the result record in the path_dump.
         :param path_dump: the path to dump the result record
         :type path_dump: str
         """
         assert self.__ending
         path_dump = "%s.result" % path_dump if not path_dump.endswith(".result") else path_dump
         assert not os.path.exists(path_dump)
-        shutil.copy(self.__path_record, path_dump)
+        shutil.copy(self.path_record, path_dump)
 
     def to_dict(self):
         """
         Return the results as a dict.
         :return: the results
         :rtype: dict
         """
```

### Comparing `zarth_utils-1.1/zarth_utils/text_processing.py` & `zarth_utils-1.2/zarth_utils/text_processing.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils/timer.py` & `zarth_utils-1.2/zarth_utils/timer.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.1/zarth_utils.egg-info/PKG-INFO` & `zarth_utils-1.2/zarth_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarth_utils
-Version: 1.1
+Version: 1.2
 Summary: Package used for my personal development on ML projects.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: pandas
 Requires-Dist: numpy
```

