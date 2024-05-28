# Comparing `tmp/python_project_manager-2.1.1.tar.gz` & `tmp/python_project_manager-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_manager-2.1.1.tar", last modified: Fri May 24 15:54:53 2024, max compression
+gzip compressed data, was "python_project_manager-2.1.2.tar", last modified: Tue May 28 13:28:22 2024, max compression
```

## Comparing `python_project_manager-2.1.1.tar` & `python_project_manager-2.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:54:53.204695 python_project_manager-2.1.1/
--rw-rw-rw-   0        0        0    35821 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      263 2024-05-24 15:54:53.202406 python_project_manager-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/README.md
--rw-rw-rw-   0        0        0     1061 2024-05-24 15:54:46.000000 python_project_manager-2.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-24 15:54:53.156652 python_project_manager-2.1.1/python_project_manager/
--rw-rw-rw-   0        0        0       97 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/__init__.py
--rw-rw-rw-   0        0        0    12665 2024-05-24 13:51:44.000000 python_project_manager-2.1.1/python_project_manager/app.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:54:53.182416 python_project_manager-2.1.1/python_project_manager/builtin_engines/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/__init__.py
--rw-rw-rw-   0        0        0     1829 2024-05-21 21:52:42.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/builtin_pyinstaller.py
--rw-rw-rw-   0        0        0     5196 2024-05-21 21:55:05.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/builtin_setuptools.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:54:53.197881 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/
--rw-rw-rw-   0        0        0      985 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/__init__.py
--rw-rw-rw-   0        0        0    39995 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/decoder.py
--rw-rw-rw-   0        0        0    10240 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/encoder.py
--rw-rw-rw-   0        0        0      377 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/ordered.py
--rw-rw-rw-   0        0        0      725 2024-05-21 12:45:57.000000 python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/tz.py
--rw-rw-rw-   0        0        0     3764 2024-05-24 15:53:44.000000 python_project_manager-2.1.1/python_project_manager/config.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:54:53.200402 python_project_manager-2.1.1/python_project_manager.egg-info/
--rw-rw-rw-   0        0        0      263 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      691 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-24 15:54:53.000000 python_project_manager-2.1.1/python_project_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 15:54:45.000000 python_project_manager-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:54:53.206581 python_project_manager-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 13:28:22.070597 python_project_manager-2.1.2/
+-rw-rw-rw-   0        0        0    35821 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      263 2024-05-28 13:28:22.068057 python_project_manager-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/README.md
+-rw-rw-rw-   0        0        0     1061 2024-05-28 13:28:15.000000 python_project_manager-2.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-28 13:28:22.017059 python_project_manager-2.1.2/python_project_manager/
+-rw-rw-rw-   0        0        0       97 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/__init__.py
+-rw-rw-rw-   0        0        0    13655 2024-05-28 13:27:17.000000 python_project_manager-2.1.2/python_project_manager/app.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:28:22.046874 python_project_manager-2.1.2/python_project_manager/builtin_engines/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/__init__.py
+-rw-rw-rw-   0        0        0     1829 2024-05-21 21:52:42.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/builtin_pyinstaller.py
+-rw-rw-rw-   0        0        0     5196 2024-05-21 21:55:05.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/builtin_setuptools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:28:22.063049 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/
+-rw-rw-rw-   0        0        0      985 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/__init__.py
+-rw-rw-rw-   0        0        0    39995 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/decoder.py
+-rw-rw-rw-   0        0        0    10240 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/encoder.py
+-rw-rw-rw-   0        0        0      377 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/ordered.py
+-rw-rw-rw-   0        0        0      725 2024-05-21 12:45:57.000000 python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/tz.py
+-rw-rw-rw-   0        0        0     3764 2024-05-24 15:53:44.000000 python_project_manager-2.1.2/python_project_manager/config.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:28:22.064551 python_project_manager-2.1.2/python_project_manager.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      691 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-28 13:28:21.000000 python_project_manager-2.1.2/python_project_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2024-05-28 13:12:54.000000 python_project_manager-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:28:22.071590 python_project_manager-2.1.2/setup.cfg
```

### Comparing `python_project_manager-2.1.1/LICENSE.txt` & `python_project_manager-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/pyproject.toml` & `python_project_manager-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "python-project-manager"
 description = "A Python package."
 authors = []
 readme = "README.md"
 keywords = []
-version = "2.1.1"
+version = "2.1.2"
 dynamic = [ "dependencies",]
 
 [project.scripts]
 ppm = "python_project_manager.app:cli"
 ppm-builtin-setuptools-build = "python_project_manager.builtin_engines.builtin_setuptools:_build"
 ppm-builtin-setuptools-install = "python_project_manager.builtin_engines.builtin_setuptools:_install"
 ppm-builtin-setuptools-uninstall = "python_project_manager.builtin_engines.builtin_setuptools:_uninstall"
```

### Comparing `python_project_manager-2.1.1/python_project_manager/app.py` & `python_project_manager-2.1.2/python_project_manager/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 import re
 from types import ModuleType
 from typing import Any, Callable
 import click
 from python_project_manager import Config
 
-VENV = f'venv\\Scripts\\activate'
+ACTIVATE_VENV = f'venv\\Scripts\\activate'
+DEACTIVATE_VENV = f'venv\\Scripts\\deactivate'
 
 InitRunner = {
     'ConfigValues': {},
         'scripts.start': 'py -m %src_dir%.app',
         'src_dir': 'src',
         'version': '0.0.0',
     'Dependencies': [],
@@ -151,34 +152,39 @@
         with open(os.path.join(os.getcwd(), file['Target']), 'w') as f:
             f.write(file['Content'])
 
     return True
 
 @cli.command()
 @click.argument('script_name', type=str, required=True)
-def run(script_name) -> None:
+@click.option('--non_venv', '-n', is_flag=True, help='Run the script without the virtual environment')
+def run(script_name, non_venv) -> None:
     '''
     <script_name> - Name of the script to be run
     '''
     
     cli_command: str = Config.get(f'scripts.{script_name}')
     
     pass_command_to_engine('run', _run,
-        script_name=script_name, cli_command=cli_command)
+        script_name=script_name, cli_command=cli_command, non_venv=non_venv)
 
 def _run(**kwargs) -> bool:
     cli_command: str = kwargs.get('cli_command', None)
     script_name: str = kwargs.get('script_name', None)
+    non_venv: bool = kwargs.get('non_venv', False)
+
+    cli_command = re.sub(r'ppm\s.*?(?=\s&&|$)', lambda x: f'{DEACTIVATE_VENV} && {x.group(0)} && {ACTIVATE_VENV}', cli_command)
 
     if not cli_command:
         print(f"Script '{script_name}' not found")
         return
 
     ## Smart change directory
-    cwd = os.getcwd() # Get the current working directory
+    old_cwd = os.getcwd() # Get the current working directory
+    new_cwd = old_cwd
 
     # Checks if 'cwd' is in the 'src' directory
     skip_chdir = re.search(r'(^|\s)cd\s\w*', cli_command) # Check for 'cd' command
     skip_chdir = skip_chdir and re.search(r'(^|\s)unittest\s\w', cli_command) # Check for 'unittest' command
     if not skip_chdir:
         # Searches for the 'python' command along with the script path
         python_command = re.search(r'python.*\.py', cli_command)
@@ -186,22 +192,35 @@
             # Get the python path
             python_path = re.search(r'\S*\.py', python_command[0])
             if python_path:
                 # Get the first dir in python path
                 targ_dir = re.search(r'^\w*(.|\|/)(?!py)', python_path[0])
                 if targ_dir:
                     # Join the target dir with the current working directory
-                    cwd = os.path.join(cwd, targ_dir[0][:-1])
+                    new_cwd = os.path.join(old_cwd, targ_dir[0][:-1])
                     # Remove targ_dir from python_path
                     cli_command = cli_command.replace(python_path[0],python_path[0].replace(targ_dir[0], ""))
                     if targ_dir[0][:-1] == Config.get('test_dir'):
                         cli_command = f'set PYTHONPATH=C:\\{Config.get('src_dir')};%PYTHONPATH% && {cli_command}'
                         
-    os.chdir(cwd) # Change the current working directory
-    os.system(f'{VENV} && {cli_command}') # Run the command
+    os.chdir(new_cwd) # Change the current working directory
+
+    if "VIRTUAL_ENV" in os.environ and non_venv:
+        print('Deactivating virtual environment')
+        os.system(f'venv\Scripts\deactivate.bat && {cli_command}')
+    elif non_venv:
+        print('Running without virtual environment')
+        os.system(cli_command)
+    else:
+        print('Running with virtual environment')
+        os.system(f'{ACTIVATE_VENV} && {cli_command}')
+
+    os.chdir(old_cwd) # Change the current working directory back to the original
+    if "VIRTUAL_ENV" in os.environ:
+        os.system('venv\Scripts\deactivate.bat')
 
 @cli.command()
 @click.argument('action', type=click.Choice(['inc', 'dec', 'show', 'set', 'sync']), required=True, default='show')
 @click.option('--major', '-M', type=int, default=0, help='Change the major version')
 @click.option('--minor', '-m', type=int, default=0, help='Change the minor version')
 @click.option('--patch', '-p', type=int, default=0, help='Change the patch version')
 @click.option('--timestamp', '-t', is_flag=True, help='Include timestamp in the version')
@@ -278,42 +297,42 @@
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.option('--help', '-h', is_flag=True) # Allows '--help' to be passed as an argument
 def list(args, help) -> None:
     '''
     Uses pip's 'list' command
     '''
     if help:
-        os.system(f'{VENV} && pip list --help')
+        os.system(f'{ACTIVATE_VENV} && pip list --help')
     else:
-        os.system(f'{VENV} && pip list {' '.join(args)}')
+        os.system(f'{ACTIVATE_VENV} && pip list {' '.join(args)}')
 
 @cli.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.option('--dev', '-d', is_flag=True) # Add the package to the dev requirements
 @click.option('--help', '-h', is_flag=True) # Allows '--help' to be passed as an argument
 def install(args, help, dev) -> None:
     '''
     Uses pip's 'install' command
     '''
     # Create the command
-    cmd = f'{VENV} && pip install {" ".join(args)}'.strip()
+    cmd = f'{ACTIVATE_VENV} && pip install {" ".join(args)}'.strip()
 
     # If 'pip install pip' is passed, install pip
-    if cmd == f'{VENV} && pip install pip':
-        os.system(f'{VENV} && python -m ensurepip')
+    if cmd == f'{ACTIVATE_VENV} && pip install pip':
+        os.system(f'{ACTIVATE_VENV} && python -m ensurepip')
         return
 
     # Use the help command if the '--help' flag is passed
     if help:
-        os.system(f'{VENV} && pip install --help')
+        os.system(f'{ACTIVATE_VENV} && pip install --help')
         return
 
     # If no arguments are passed, install the requirements
-    if cmd == f'{VENV} && pip install':
-        os.system(f'{VENV} && pip install -r requirements.txt -r requirements-dev.txt')
+    if cmd == f'{ACTIVATE_VENV} && pip install':
+        os.system(f'{ACTIVATE_VENV} && pip install -r requirements.txt -r requirements-dev.txt')
 
     # Otherwise, install the packages
     output = os.popen(cmd)
 
     # Read and print each line of the output
     for line in output:
         print(line.strip())
```

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/builtin_pyinstaller.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/builtin_pyinstaller.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/builtin_setuptools.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/builtin_setuptools.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/__init__.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/decoder.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/encoder.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/builtin_engines/toml/tz.py` & `python_project_manager-2.1.2/python_project_manager/builtin_engines/toml/tz.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager/config.py` & `python_project_manager-2.1.2/python_project_manager/config.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager.egg-info/SOURCES.txt` & `python_project_manager-2.1.2/python_project_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.1.1/python_project_manager.egg-info/entry_points.txt` & `python_project_manager-2.1.2/python_project_manager.egg-info/entry_points.txt`

 * *Files identical despite different names*

