# Comparing `tmp/pymodins-2.0.2.tar.gz` & `tmp/pymodins-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-x1jnk81n\pymodins-2.0.2.tar", last modified: Sun May 26 08:02:31 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-2ozr1yeo\pymodins-2.0.3.tar", last modified: Tue May 28 09:17:16 2024, max compression
```

## Comparing `pymodins-2.0.2.tar` & `pymodins-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.223269 pymodins-2.0.2/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-05-26 08:02:31.220091 pymodins-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3232 2024-05-20 10:01:59.000000 pymodins-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.193446 pymodins-2.0.2/pymodins/
--rw-rw-rw-   0        0        0      335 2024-05-26 08:02:18.000000 pymodins-2.0.2/pymodins/__init__.py
--rw-rw-rw-   0        0        0    55881 2024-05-26 08:01:52.000000 pymodins-2.0.2/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.219091 pymodins-2.0.2/pymodins.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 08:02:31.223269 pymodins-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-05-26 08:02:23.000000 pymodins-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.838189 pymodins-2.0.3/
+-rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4355 2024-05-28 09:17:16.833621 pymodins-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3733 2024-05-27 12:55:01.000000 pymodins-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.808206 pymodins-2.0.3/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-05-26 16:45:06.000000 pymodins-2.0.3/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    56322 2024-05-28 09:16:36.000000 pymodins-2.0.3/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.829781 pymodins-2.0.3/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     4355 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:17:16.838189 pymodins-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-26 09:49:24.000000 pymodins-2.0.3/setup.py
```

### Comparing `pymodins-2.0.2/LICENSE` & `pymodins-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.2/PKG-INFO` & `pymodins-2.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pymodins
-Version: 2.0.2
-Summary: A module to install various Python packages.
-Home-page: https://github.com/Nandhan-KA/pymodins
-Author: Nandhan K
-Author-email: nandhan2003alamelu@gmail.com 
-Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rich
-Requires-Dist: pymsgbox
-
 # PYMODINS
 
 [pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
@@ -101,30 +84,39 @@
 SOFTWARE.
 ```
 
 ## Expected Output
 
 ```
 
-              \ |   \    \ | _ \ |  |   \    \ |    |  / 
-             .  |  _ \  .  | |  |__ |  _ \  .  |    . <  
-            _|\_|_/  _\_|\_|___/_| _|_/  _\_|\_|   _|\_\ 
+ _______  ____  ____  ____    ____   ___   ______   _____  ____  _____   ______   
+|_   __ \|_  _||_  _||_   \  /   _|.'   `.|_   _ `.|_   _||_   \|_   _|.' ____ \  
+  | |__) | \ \  / /    |   \/   | /  .-.  \ | | `. \ | |    |   \ | |  | (___ \_| 
+  |  ___/   \ \/ /     | |\  /| | | |   | | | |  | | | |    | |\ \| |   _.____`.  
+ _| |_      _|  |_    _| |_\/_| |_\  `-'  /_| |_.' /_| |_  _| |_\   |_ | \____) | 
+|_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
 
+    
 Creator: Nandhan K
 Github: @github.com/Nandhan-KA
+System Platform: win32
+Python verion: 3.8.0 (tags/v3.8.0:fa919fd, Oct 14 2019, 19:37:50) [MSC v.1916 64 bit (AMD64)]
+pip version: pip 24.0 from c:\users\{username}\appdata\local\programs\python\python38\lib\site-packages\pip (python 3.8)
+
+Please select the type of modules you want to install:
+
+1. Basic Modules
+2. Advanced Modules
+3. Science Modules
+4. Computer Vision Modules
+5. Machine Learning Modules
+6. Deep Learning Modules
+7. Full Stack Development Modules
+8. Network Modules
+9. Build Modules
+10. Jupyter Modules
 
-            1. Basic Modules
-            2. Advanced Modules
-            3. Science Modules
-            4. Computer Vision Modules
-            5. Machine Learning Modules
-            6. Deep Learning Modules
-            7. Full Stack Development Modules
-            8. Network Modules
-            9. Build Modules
-            10.Jupyter Modules
-
-Enter the number corresponding to the module type:
+Enter the number corresponding to your choice: 
 ```
 
-# ðŸŽ‰ Thank you for using this project!
-# Feel free to ask your queries ðŸ˜Š
+# Thank you for using this project!
+# Feel free to ask your queries
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymodins-2.0.2/pymodins/installer.py` & `pymodins-2.0.3/pymodins/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import getpass
 import sys
-import re
+import pip
 import urllib.request
 from datetime import datetime
 import subprocess
 import ctypes
 import webbrowser
 import pymsgbox
 from rich.console import Console
@@ -46,16 +46,14 @@
     print("System Platform:", sys.platform)
     print("Python verion:", sys.version)
     try:
         pip_version = subprocess.check_output(['pip', '--version']).decode().strip()
         print("pip version:", pip_version)
     except Exception as e:
         print("Error:", e,"Reinstall Python with PIP and add PIP to the System PATH")
-import subprocess
-import pip
 
 def upgrade_pip():
     try:
         installed_version = pip.__version__
 
         latest_pip_version_output = subprocess.check_output(['pip', 'install', '--upgrade', 'pip']).decode().strip()
         print("Latest pip version output:", latest_pip_version_output)
@@ -76,18 +74,18 @@
 def install_vscode_build_tools():
     def run_command(command):
         result = subprocess.run(command, shell=True)
         return result.returncode
 
     def install_chocolatey():
         choco_install_cmd = (
-            '@"%"SystemRoot%"\\System32\\WindowsPowerShell\\v1.0\\powershell.exe" '
-            '-NoProfile -InputFormat None -ExecutionPolicy Bypass -Command '
-            '"iex ((New-Object System.Net.WebClient).DownloadString(\'https://chocolatey.org/install.ps1\'))" '
-            '&& SET "PATH=%PATH%;%ALLUSERSPROFILE%\\chocolatey\\bin"'
+            'runas /user:Administrator @"%"SystemRoot%"\\System32\\WindowsPowerShell\\v1.0\\powershell.exe" '
+        '-NoProfile -InputFormat None -ExecutionPolicy Bypass -Command '
+        '"iex ((New-Object System.Net.WebClient).DownloadString(\'https://chocolatey.org/install.ps1\'))" '
+        '&& SET "PATH=%PATH%;%ALLUSERSPROFILE%\\chocolatey\\bin"'
         )
         return run_command(choco_install_cmd)
 
     def install_vs_build_tools():
         vs_build_tools_cmd = 'choco install -y visualstudio2019buildtools'
         return run_command(vs_build_tools_cmd)
 
@@ -360,14 +358,15 @@
         print("No Internet Connection")
 
 
 def run():
     installer()
 
 def install_basic_modules():
+    banner()
     selected_option = 1
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -456,14 +455,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_advanced_modules():
+    banner()
     selected_option = 2
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -552,14 +552,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_machinelearning_modules():
+    banner()
     selected_option = 5
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -647,14 +648,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_deeplearning_modules():
+    banner()
     selected_option = 6
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -742,14 +744,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_fullstack_modules():
+    banner()
     selected_option = 7
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -837,14 +840,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_science_modules():
+    banner()
     selected_option = 3
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -931,14 +935,15 @@
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 def install_computervision_modules():
+    banner()
     selected_option = 4
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -1048,14 +1053,15 @@
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 def install_network_modules():
+    banner()
     selected_option = 8
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -1143,14 +1149,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_build_modules():
+    banner()
     selected_option = 9
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -1189,14 +1196,17 @@
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
                 python_folder = str(*versions)
 
             for module in modules:
                 if module == 'rust':
                     pymsgbox.alert("This Modules Required VSBuild Tools")
+                    print("Installing VSBuild Tools")
+                    install_vscode_build_tools()
+                    clear
                     print("Module rust needs to be installed separately.")
                     x = input("Do you want to install Rust? (y/n): ").lower()
                     if x == "y":
                         if install_rust():
                             print("Rust installed successfully.")
                         else:
                             print("Failed to install Rust. Opening the Rust installation webpage.")
@@ -1238,18 +1248,22 @@
             if len(versions) == 2:
                 print(f"\nYou have two folders in your Python installation:")
                 print("(1)", versions[0])
                 print("(2)", versions[1])
                 python_folder = versions[int(
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
-                python_folder = str(*versions)
+                python_folder = str(*versions) 
                 
             if selected_module == 'rust':
                 pymsgbox.alert("This Modules Required VSBuild Tools")
+                print("Installing VSBuild Tools")
+                install_vscode_build_tools()
+                clear
+                pymsgbox.alert("This Modules Required VSBuild Tools")
                 print("Module rust needs to be installed separately.")
                 x = input("Do you want to install Rust? (y/n): ").lower()
                 if x == "y":
                     if install_rust():
                         print("Rust installed successfully.")
                     else:
                         print("Failed to install Rust. Opening the Rust installation webpage.")
@@ -1263,14 +1277,15 @@
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
 
 
 def install_jupyter_modules():
+    banner()
     selected_option = 10
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
         'Science Modules',
@@ -1354,9 +1369,8 @@
             os.system(command)
 
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
-                installer()
-run()
+                installer()
```

### Comparing `pymodins-2.0.2/setup.py` & `pymodins-2.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="2.0.2",
+    version="2.0.3",
     packages=find_packages(),
     install_requires=[
         "rich",
         "pymsgbox"
     ],
     entry_points={
         "console_scripts": [
```

