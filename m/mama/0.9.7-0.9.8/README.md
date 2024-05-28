# Comparing `tmp/mama-0.9.7.tar.gz` & `tmp/mama-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.7.tar", last modified: Thu May  2 08:35:12 2024, max compression
+gzip compressed data, was "mama-0.9.8.tar", last modified: Tue May 28 15:29:38 2024, max compression
```

## Comparing `mama-0.9.7.tar` & `mama-0.9.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.509394 mama-0.9.7/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.7/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-02 08:35:12.509394 mama-0.9.7/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.7/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.499394 mama-0.9.7/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.7/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-25 09:35:15.000000 mama-0.9.7/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    40004 2024-05-02 07:54:51.000000 mama-0.9.7/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-25 09:35:15.000000 mama-0.9.7/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-02 07:54:51.000000 mama-0.9.7/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-04-07 19:34:43.000000 mama-0.9.7/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-04-30 10:10:25.000000 mama-0.9.7/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.7/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-03-25 09:35:15.000000 mama-0.9.7/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.7/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 10:23:16.000000 mama-0.9.7/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.7/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.7/mama/papa_upload.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.7/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.509394 mama-0.9.7/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.7/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.7/mama/platforms/android.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.7/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.7/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.509394 mama-0.9.7/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.7/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.7/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.7/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.7/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.7/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.7/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.7/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.509394 mama-0.9.7/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.7/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2024-01-20 16:30:57.000000 mama-0.9.7/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.7/mama/utils/gnu_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2024-01-20 16:30:57.000000 mama-0.9.7/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.7/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.7/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.7/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1310 2024-05-02 08:29:37.000000 mama-0.9.7/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-02 08:35:12.509394 mama-0.9.7/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-02 08:35:12.000000 mama-0.9.7/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-02 08:29:44.000000 mama-0.9.7/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-02 08:35:12.509394 mama-0.9.7/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.8/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-28 15:29:38.805647 mama-0.9.8/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.8/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.795647 mama-0.9.8/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.8/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-25 09:35:15.000000 mama-0.9.8/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    40004 2024-05-02 07:54:51.000000 mama-0.9.8/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-25 09:35:15.000000 mama-0.9.8/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-02 07:54:51.000000 mama-0.9.8/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-04-07 19:34:43.000000 mama-0.9.8/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-04-30 10:10:25.000000 mama-0.9.8/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.8/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-03-25 09:35:15.000000 mama-0.9.8/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.8/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 10:23:16.000000 mama-0.9.8/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.8/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.8/mama/papa_upload.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.8/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/android.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.8/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.8/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.8/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.8/mama/utils/gnu_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1063 2024-05-28 15:28:16.000000 mama-0.9.8/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.8/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.8/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1310 2024-05-02 08:29:37.000000 mama-0.9.8/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-28 15:26:08.000000 mama-0.9.8/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-28 15:29:38.805647 mama-0.9.8/setup.cfg
```

### Comparing `mama-0.9.7/LICENSE` & `mama-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/PKG-INFO` & `mama-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.7
+Version: 0.9.8
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.7/README.md` & `mama-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/artifactory.py` & `mama-0.9.8/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/build_config.py` & `mama-0.9.8/mama/build_config.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/build_dependency.py` & `mama-0.9.8/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/build_target.py` & `mama-0.9.8/mama/build_target.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/cmake_configure.py` & `mama-0.9.8/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/dependency_chain.py` & `mama-0.9.8/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/init_project.py` & `mama-0.9.8/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/main.py` & `mama-0.9.8/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/msbuild.py` & `mama-0.9.8/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/package.py` & `mama-0.9.8/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/papa_deploy.py` & `mama-0.9.8/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/papa_upload.py` & `mama-0.9.8/mama/papa_upload.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/parse_mamafile.py` & `mama-0.9.8/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/platforms/android.py` & `mama-0.9.8/mama/platforms/android.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/platforms/mips.py` & `mama-0.9.8/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/platforms/oclea.py` & `mama-0.9.8/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/types/artifactory_pkg.py` & `mama-0.9.8/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/types/asset.py` & `mama-0.9.8/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/types/dep_source.py` & `mama-0.9.8/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/types/git.py` & `mama-0.9.8/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/types/local_source.py` & `mama-0.9.8/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/util.py` & `mama-0.9.8/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/gdb.py` & `mama-0.9.8/mama/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/gnu_project.py` & `mama-0.9.8/mama/utils/gnu_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/gtest.py` & `mama-0.9.8/mama/utils/gtest.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 def run_gtest(target: BuildTarget, executable: str, args='', src_dir=False, gdb=False):
     args, gdb = filter_gdb_arg(args, gdb)
     ## gtest flags:
     # https://github.com/google/googletest/blob/main/googletest/src/gtest.cc#L238
     params = f' --gtest_output="xml:{target.source_dir("test/report.xml")}"'
     if args:
-        params += f' --gtest_filter="*{args}*"'
+        for arg in args.split(' '):
+            if arg.startswith('--gtest_'):
+                params += f' {arg}'
+            else:
+                params += f' --gtest_filter="*{arg}*"'
 
     if gdb:
         run_gdb(target, f'{executable} {params}', src_dir=src_dir)
     else:
         dirname = os.path.dirname(executable)
         exename = os.path.basename(executable)
         dir = target.source_dir(dirname) if src_dir else target.build_dir(dirname)
```

### Comparing `mama-0.9.7/mama/utils/nonblocking_io.py` & `mama-0.9.8/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/run.py` & `mama-0.9.8/mama/utils/run.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/sub_process.py` & `mama-0.9.8/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama/utils/system.py` & `mama-0.9.8/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/mama.egg-info/PKG-INFO` & `mama-0.9.8/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.7
+Version: 0.9.8
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.7/mama.egg-info/SOURCES.txt` & `mama-0.9.8/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.9.7/pyproject.toml` & `mama-0.9.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.9.7"
+version = "0.9.8"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

