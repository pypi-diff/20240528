# Comparing `tmp/jutge-joapuiib-1.0.7.tar.gz` & `tmp/jutge_joapuiib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jutge-joapuiib-1.0.7.tar", last modified: Tue Feb 13 09:43:37 2024, max compression
+gzip compressed data, was "jutge_joapuiib-1.0.9.tar", last modified: Tue May 28 14:27:16 2024, max compression
```

## Comparing `jutge-joapuiib-1.0.7.tar` & `jutge_joapuiib-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.835813 jutge-joapuiib-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-13 09:43:37.835813 jutge-joapuiib-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-13 09:43:37.835813 jutge-joapuiib-1.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.831813 jutge-joapuiib-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.831813 jutge-joapuiib-1.0.7/src/jutge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/check_repo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6022 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/grade_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.831813 jutge-joapuiib-1.0.7/src/jutge/judges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/judges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/judges/base_judge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/judges/java_judge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/judges/sql_judge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.831813 jutge-joapuiib-1.0.7/src/jutge/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/models/exercise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/models/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/src/jutge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.835813 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-13 09:43:37.000000 jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:43:37.835813 jutge-joapuiib-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-13 09:43:30.000000 jutge-joapuiib-1.0.7/tests/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 14:27:16.722653 jutge_joapuiib-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.714653 jutge_joapuiib-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/src/jutge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/check_repo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/grade_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/src/jutge/judges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/judges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/judges/base_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/judges/java_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/judges/mongodb_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/judges/sql_judge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/src/jutge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/models/exercise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/models/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/src/jutge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 14:27:16.000000 jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:27:16.718653 jutge_joapuiib-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 14:27:13.000000 jutge_joapuiib-1.0.9/tests/test_sql.py
```

### Comparing `jutge-joapuiib-1.0.7/PKG-INFO` & `jutge_joapuiib-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jutge-joapuiib
-Version: 1.0.7
+Version: 1.0.9
 Summary: CLI Judge to validate SQL and Java exercises
 Home-page: https://github.com/joapuiib/jutge
 Author: joapuiib
 Author-email: joapuiib@gmail.com
 Project-URL: Source, https://github.com/joapuiib/jutge/
 Project-URL: Issues, https://github.com/joapuiib/jutge/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jutge-joapuiib-1.0.7/README.md` & `jutge_joapuiib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/setup.cfg` & `jutge_joapuiib-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jutge-joapuiib
-version = 1.0.7
+version = 1.0.9
 author = joapuiib
 author_email = joapuiib@gmail.com
 description = CLI Judge to validate SQL and Java exercises
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joapuiib/jutge
 project_urls =
```

### Comparing `jutge-joapuiib-1.0.7/src/jutge/check_repo.py` & `jutge_joapuiib-1.0.9/src/jutge/check_repo.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge/grade_repo.py` & `jutge_joapuiib-1.0.9/src/jutge/grade_repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3.8
 import argparse
 import yaml
 import os
 from colorama import Fore
 from datetime import datetime
-import sys
+# import sys
 import git
 from jutge.judges.java_judge import JavaJudge
 from jutge.judges.sql_judge import SQLJudge
+from jutge.judges.mongodb_judge import MongoDBJudge
 from jutge.utils import run_or_exit, prettify_dict, load_file, copy_clipboard
 import jutge.utils as utils
 
 def loadYAML(filename):
     with open(filename, 'r') as stream:
         try:
             return yaml.safe_load(stream)
@@ -28,14 +29,15 @@
         self.result = {}
 
         self.tests = self.load_tests(args.test_cases)
 
         self.available_judges = {}
         self.available_judges["java"] = JavaJudge
         self.available_judges["sql"] = SQLJudge
+        self.available_judges["mongodb"] = MongoDBJudge
 
 
     def find_and_load_yaml_files(self, tests, tests_dir):
         if isinstance(tests, list):
             for i, el in enumerate(tests):
                 tests[i] = self.find_and_load_yaml_files(el, tests_dir)
         elif isinstance(tests, dict):
```

### Comparing `jutge-joapuiib-1.0.7/src/jutge/judges/java_judge.py` & `jutge_joapuiib-1.0.9/src/jutge/judges/java_judge.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge/judges/sql_judge.py` & `jutge_joapuiib-1.0.9/src/jutge/judges/sql_judge.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
     def start_container(self):
         command = (f"docker run -d --name {self.container}"
                    # f" -e LANG=en_US.utf8"
                    f" -e MYSQL_ROOT_PASSWORD={self.password}"
                    f" --health-cmd=\'mysql -u{self.user} -p{self.password}\' --health-interval=2s"
                    f" {self.image}"
+                   " mysqld --lower_case_table_names=1"
         )
         out = utils.run_or_exit(run_process, command,
                 out=f"Init {self.image} {self.container} container...",
                 err=f"Error initializing {self.image} container").stdout
 
     def get_cointainer_id(self):
         command = f"docker ps -q -f name={self.container}"
@@ -180,34 +181,39 @@
     def judge_exercise(self, exercise, interactive):
         name = exercise.name
 
         if not name:
             print(f"{Fore.RED}Error! No s'ha especificat la clau \"name\" en algun exercici.{Fore.RESET}")
             raise Exception("No class name specified")
 
-        source_path = re.sub(r"/+", "/", f"{self.base_dir}/{self.package}/{exercise.subpackage}/{name}.sql")
+        dir_path = f"{self.base_dir}/{self.package}/{exercise.subpackage}"
+        dir_path = re.sub(r"[/]+", "/", dir_path)
+        dir_path = re.sub(r"[/]+$", "", dir_path)
 
         print("=" * 20)
         print(name)
-        print(source_path)
 
-        source_file = next(iter(glob(source_path, recursive=True)), None)
+        source_file = next((os.path.join(root, file)
+                            for root, _, files in os.walk(dir_path)
+                            for file in files if re.match(r"[_]?" + name + r".sql", file)
+                            ) , None)
         if not source_file:
             print(f"{Fore.RED}{name}: Not found{Fore.RESET}")
             exercise.result["found"] = False
-            exercise.result["source_file"] = source_path
+            exercise.result["source_file"] = source_file
             print(f"{Fore.RED}Error! No script found{Fore.RESET}")
             return exercise.result
 
+        print(source_file)
         exercise.result["found"] = True
         exercise.result["source_file"] = source_file
 
         # Print sources
         with open(source_file) as f:
-            exercise.source = f.read().strip()
+            exercise.source = f.read().strip().replace("\t", "    ")
             self.print_source(exercise.source)
             print()
             # result = self.run_exercise(name, exercise, source, interactive)
             self.run_object(exercise, interactive=interactive, indent=1)
             utils.print_lines(f"- STATUS {exercise.name}: {exercise.status}", indent=1)
         print()
         return exercise.result
```

### Comparing `jutge-joapuiib-1.0.7/src/jutge/models/unit_test.py` & `jutge_joapuiib-1.0.9/src/jutge/models/unit_test.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge/process.py` & `jutge_joapuiib-1.0.9/src/jutge/process.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge/status.py` & `jutge_joapuiib-1.0.9/src/jutge/status.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge/utils.py` & `jutge_joapuiib-1.0.9/src/jutge/utils.py`

 * *Files identical despite different names*

### Comparing `jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/PKG-INFO` & `jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jutge-joapuiib
-Version: 1.0.7
+Version: 1.0.9
 Summary: CLI Judge to validate SQL and Java exercises
 Home-page: https://github.com/joapuiib/jutge
 Author: joapuiib
 Author-email: joapuiib@gmail.com
 Project-URL: Source, https://github.com/joapuiib/jutge/
 Project-URL: Issues, https://github.com/joapuiib/jutge/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jutge-joapuiib-1.0.7/src/jutge_joapuiib.egg-info/SOURCES.txt` & `jutge_joapuiib-1.0.9/src/jutge_joapuiib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/jutge/grade_repo.py
 src/jutge/process.py
 src/jutge/status.py
 src/jutge/utils.py
 src/jutge/judges/__init__.py
 src/jutge/judges/base_judge.py
 src/jutge/judges/java_judge.py
+src/jutge/judges/mongodb_judge.py
 src/jutge/judges/sql_judge.py
 src/jutge/models/__init__.py
 src/jutge/models/exercise.py
 src/jutge/models/unit_test.py
 src/jutge_joapuiib.egg-info/PKG-INFO
 src/jutge_joapuiib.egg-info/SOURCES.txt
 src/jutge_joapuiib.egg-info/dependency_links.txt
```

