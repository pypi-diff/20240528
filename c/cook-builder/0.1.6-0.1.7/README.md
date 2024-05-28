# Comparing `tmp/cook_builder-0.1.6.tar.gz` & `tmp/cook_builder-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.1.6.tar", last modified: Mon May 27 15:12:58 2024, max compression
+gzip compressed data, was "cook_builder-0.1.7.tar", last modified: Tue May 28 18:30:17 2024, max compression
```

## Comparing `cook_builder-0.1.6.tar` & `cook_builder-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:12:58.763667 cook_builder-0.1.6/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.6/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3078 2024-05-27 15:12:58.763667 cook_builder-0.1.6/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      915 2024-05-27 15:05:43.000000 cook_builder-0.1.6/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:12:58.763667 cook_builder-0.1.6/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       36 2024-04-23 18:58:25.000000 cook_builder-0.1.6/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.6/cook/build.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3881 2024-05-27 15:12:03.000000 cook_builder-0.1.6/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.6/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2915 2024-05-24 16:57:07.000000 cook_builder-0.1.6/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.6/cook/exception.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2390 2024-05-24 16:59:53.000000 cook_builder-0.1.6/cook/executors.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      981 2024-05-24 16:59:49.000000 cook_builder-0.1.6/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2455 2024-05-24 16:50:34.000000 cook_builder-0.1.6/cook/main.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1065 2024-05-24 16:30:49.000000 cook_builder-0.1.6/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.6/cook/rsync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.6/cook/sync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.6/cook/watchers.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:12:58.763667 cook_builder-0.1.6/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3078 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       46 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-05-27 15:12:58.000000 cook_builder-0.1.6/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1165 2024-05-27 15:12:25.000000 cook_builder-0.1.6/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-27 15:12:58.763667 cook_builder-0.1.6/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-28 18:30:17.225206 cook_builder-0.1.7/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.7/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2903 2024-05-28 18:30:17.225206 cook_builder-0.1.7/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      740 2024-05-28 18:29:48.000000 cook_builder-0.1.7/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-28 18:30:17.225206 cook_builder-0.1.7/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       36 2024-04-23 18:58:25.000000 cook_builder-0.1.7/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.7/cook/build.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4130 2024-05-28 17:55:21.000000 cook_builder-0.1.7/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5033 2024-05-28 18:22:57.000000 cook_builder-0.1.7/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2915 2024-05-28 18:22:19.000000 cook_builder-0.1.7/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.7/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2390 2024-05-24 16:59:53.000000 cook_builder-0.1.7/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      981 2024-05-24 16:59:49.000000 cook_builder-0.1.7/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2455 2024-05-28 18:11:00.000000 cook_builder-0.1.7/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1065 2024-05-24 16:30:49.000000 cook_builder-0.1.7/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.7/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.7/cook/sync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.7/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-28 18:30:17.225206 cook_builder-0.1.7/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2903 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       46 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-05-28 18:30:17.000000 cook_builder-0.1.7/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1165 2024-05-28 18:28:54.000000 cook_builder-0.1.7/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-28 18:30:17.225206 cook_builder-0.1.7/setup.cfg
```

### Comparing `cook_builder-0.1.6/LICENSE` & `cook_builder-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/PKG-INFO` & `cook_builder-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.6
+Version: 0.1.7
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,16 +75,8 @@
 
 ```sh
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install -e .
 ```
 
-<!-- RELEASING
-1. Update version in pyproject.toml
-2. Build and upload wheels to PyPI:
-    pip install --upgrade build twine
-    python3 -m build
-    twine upload dist/*
--->
-
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.6/README.md` & `cook_builder-0.1.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -29,16 +29,8 @@
 
 ```sh
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install -e .
 ```
 
-<!-- RELEASING
-1. Update version in pyproject.toml
-2. Build and upload wheels to PyPI:
-    pip install --upgrade build twine
-    python3 -m build
-    twine upload dist/*
--->
-
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.6/cook/build.py` & `cook_builder-0.1.7/cook/build.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/cli.py` & `cook_builder-0.1.7/cook/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,42 @@
         self.args = {}
         self.flags = []
 
 
 settings = Settings()
 
 
+def list_items(recipe_path, build_servers, default_build_server, projects, default_project):
+    rprint(f'[bold]Items defined in {recipe_path}')
+
+    list_item('Build Servers', build_servers, default_build_server)
+    list_item('Projects', projects, default_project)
+
+
+def list_item(message, iterable, default):
+    if not iterable:
+        rprint(f'[bold][#fcac00]{message}[/] not defined.')
+        return
+
+    rprint(f'[bold #fcac00]{message}[/]:')
+    for item in iterable:
+        if item == default:
+            msg = f'  [#555555 on #cccccc]{item}[/]'
+        else:
+            msg = f'  {item}'
+        rprint(msg)
+
+
+def select_interactively(message, choices, default):
+    if choices is None:
+        return
+
+    return questionary.select(message, choices=choices, default=default).unsafe_ask()
+
+
 def parse_user_args(user_args):
     args = {}
     flags = []
 
     for user_arg in user_args:
         if '=' in user_arg:
             key, value = user_arg.split('=')
@@ -46,15 +74,15 @@
     parser.add_argument('-f', '--format', action='store_true', help='Format output using Rich.')
     parser.add_argument('-l', '--list', action='store_true', help='List available projects and build servers.')
     parser.add_argument('-d', '--dry', action='store_true', help='Dry run.')
     parser.add_argument('-q', '--quiet', action='store_true', help='Suppress stdout.')
     parser.add_argument(
         '-u', '--user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format either `key=value` or `flag`.'
     )
-    parser.add_argument('-p', '--project', default=None, help='Project to build. Uses value of `default_project` if left unspecified.')
+    parser.add_argument('-p', '--project', help='Project to build. Uses value of `default_project` if left unspecified.')
     parser.add_argument('-i', '--interactive', action='store_true', help='Force interactive selection.')
 
     args = parser.parse_args()
 
     user_args, user_flags = parse_user_args(args.user_args)
     settings.args.update(user_args)
     settings.flags.extend(user_flags)
@@ -73,41 +101,27 @@
     build_servers, default_build_server = main_program.get_build_servers()
 
     project = args.project or default_project
     build_server = args.build_server or default_build_server
 
     if to_list:
         recipe_path = main_program.get_recipe_path()
-        rprint(f'[bold]Items defined in {recipe_path}')
-
-        rprint('[bold #fcac00]Build Servers[/]:')
-        for build_server in build_servers:
-            if build_server == default_build_server:
-                msg = f'  [#555555 on #cccccc]{build_server}[/]'
-            else:
-                msg = f'  {build_server}'
-            rprint(msg)
-
-        rprint('[bold #fcac00]Projects[/]:')
-        for project in projects:
-            if project == default_project:
-                msg = f'  [#555555 on #cccccc]{project}[/]'
-            else:
-                msg = f'  {project}'
-            rprint(msg)
-        return
+        list_items(recipe_path, build_servers, default_build_server, projects, default_project)
+        return 0
 
     # TODO: parse user args interactively before loading the recipe
-    if args.interactive or project is None:
-        project = questionary.select('Project', choices=projects, default=default_project).ask()
-        if project is None:
-            exit(1)
-
-    if args.interactive or build_server is None:
-        build_server = questionary.select('Build Server', choices=build_servers, default=default_build_server).ask()
-        if build_server is None:
-            exit(1)
+
+    try:
+        if args.interactive or project is None:
+            project = select_interactively('Project', projects, default_project)
+
+        if args.interactive or build_server is None:
+            build_server = select_interactively('Build Server', build_servers, default_build_server)
+
+    except KeyboardInterrupt:
+        print("\nCancelled by user\n")
+        return 1
 
     main_program.configure(project, build_server)
     main_program.set_output(rich_output, quiet)
 
     main_program.run(dry_run=dry_run)
```

### Comparing `cook_builder-0.1.6/cook/configuration.py` & `cook_builder-0.1.7/cook/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,21 @@
 
         self.base_path = recipe.base_path
         self.skip = False
 
     def setup(self, project=None, server=None):
         if project is None:
             project = self.default_project
+        if project is None:
+            raise ConfigurationError('No project selected!')
 
         if server is None:
             server = self.default_build_server
+        if server is None:
+            raise ConfigurationError('No build server selected!')
 
         self._set_project(project)
         self._set_build_server(server)
 
         if not self._is_composite():
             self._update_paths()
```

### Comparing `cook_builder-0.1.6/cook/cook.py` & `cook_builder-0.1.7/cook/cook.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/executors.py` & `cook_builder-0.1.7/cook/executors.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/logger.py` & `cook_builder-0.1.7/cook/logger.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/main.py` & `cook_builder-0.1.7/cook/main.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/recipe.py` & `cook_builder-0.1.7/cook/recipe.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/rsync.py` & `cook_builder-0.1.7/cook/rsync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook/sync.py` & `cook_builder-0.1.7/cook/sync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.6/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.7/cook_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.6
+Version: 0.1.7
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,16 +75,8 @@
 
 ```sh
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install -e .
 ```
 
-<!-- RELEASING
-1. Update version in pyproject.toml
-2. Build and upload wheels to PyPI:
-    pip install --upgrade build twine
-    python3 -m build
-    twine upload dist/*
--->
-
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.6/pyproject.toml` & `cook_builder-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
   "questionary==2.0.1",
 ]
 requires-python = ">=3.10"
 authors = [
```

