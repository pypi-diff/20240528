# Comparing `tmp/package_auto_assembler-0.1.4.tar.gz` & `tmp/package_auto_assembler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.1.4.tar", last modified: Wed May 22 01:11:31 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.1.5.tar", last modified: Tue May 28 00:48:21 2024, max compression
```

## Comparing `package_auto_assembler-0.1.4.tar` & `package_auto_assembler-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 01:07:41.000000 package_auto_assembler-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-22 01:07:41.000000 package_auto_assembler-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.244322 package_auto_assembler-0.1.4/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:10:45.000000 package_auto_assembler-0.1.4/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64814 2024-05-22 01:10:45.000000 package_auto_assembler-0.1.4/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-22 01:11:30.000000 package_auto_assembler-0.1.4/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 00:44:05.000000 package_auto_assembler-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-28 00:44:05.000000 package_auto_assembler-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.198304 package_auto_assembler-0.1.5/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:48:07.000000 package_auto_assembler-0.1.5/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76197 2024-05-28 00:48:07.000000 package_auto_assembler-0.1.5/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 00:48:20.000000 package_auto_assembler-0.1.5/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/setup.cfg
```

### Comparing `package_auto_assembler-0.1.4/LICENSE` & `package_auto_assembler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.4/PKG-INFO` & `package_auto_assembler-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_auto_assembler
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,47 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
-Its purpose is to automate as many aspects of python package creation as possible,
-to shorten a development cycle of reusable components, maintain certain standard of quality
-for reusable code. It provides tool to simplify the process of package creatrion
-to a point that it can be triggered automatically within ci/cd pipelines,
-with minimal preparations and requirements for new modules.
-
-
-
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
-            ReleaseNotesHandler, PackageAutoAssembler)
+            ReleaseNotesHandler, MkDocsHandler, PackageAutoAssembler)
 ```
 
-## Usage examples
-
-The examples contain: 
-1. package versioning
-2. import mapping
-3. extracting and merging requirements
-4. preparing metadata
-5. merging local dependacies into single module
-6. prepare README
-7. assembling setup directory
-8. making a package
-9. creating release notes from commit messages
-
 ### 1. Package versioning
 
 #### Initialize VersionHandler
 
 
 ```python
 pv = VersionHandler(
@@ -165,27 +141,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -276,15 +252,15 @@
     custom_modules_filepath="../tests/package_auto_assembler/dependancies"
 )
 ```
 
 
 
 
-    ['example_local_dependacy_1', 'example_local_dependacy_2']
+    ['example_local_dependacy_2', 'example_local_dependacy_1']
 
 
 
 #### Check if module is a standard python library
 
 
 ```python
@@ -898,15 +874,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
@@ -917,43 +893,36 @@
     label_name = 'example_module',
     # new version to be used in release notes
     version = '0.0.2'
 )
 ```
 
     No relevant commit messages found!
-
-
     ..trying depth 2 !
-
-
     No relevant commit messages found!
-
-
     No messages to clean were provided
 
 
 ##### - overwritting commit messages from example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README',
-     'Update requirements',
-     '[package_auto_assembler] test_install_package() method for local testing',
-     'simpler test_install_package.py script',
-     'Update package version tracking files',
-     'Update README',
-     'Update requirements']
+    ['slight changes to gh-pages workflow',
+     'adding package_auto_assembler to usage examples test run exceptions',
+     'updated gh-pages workflow',
+     'testing newer MkDocsHandler',
+     'updated workflows',
+     'package name parameter for gh-pages workflow']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
@@ -1033,7 +1002,78 @@
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
      '\n',
      '    - initial version of example_module\n']
 
 
+
+### 10. Making simple MkDocs site
+
+##### - preparing inputs
+
+
+```python
+package_name = "example_module"
+
+module_content = LongDocHandler().read_module_content(filepath=f"../tests/package_auto_assembler/{package_name}.py")
+
+docstring = LongDocHandler().extract_module_docstring(module_content=module_content)
+pypi_link = LongDocHandler().get_pypi_badge(module_name=package_name)
+
+
+docs_file_paths = {
+    "../example_module.md" : "usage-examples.md",
+    '../tests/package_auto_assembler/release_notes.md' : 'release_notes.md'
+}
+```
+
+
+```python
+mdh = MkDocsHandler(
+    # required
+    ## name of the package to be displayed
+    package_name = package_name,
+    ## dictionary of markdown files, with path as keys
+    docs_file_paths = docs_file_paths,
+    # optional
+    ## module docstring to be displayed in the index
+    module_docstring = docstring,
+    ## pypi badge to be displayed in the index
+    pypi_badge = pypi_link,
+    ## license badge to be displayed in the index
+    license_badge="[![License](https://img.shields.io/github/license/Kiril-Mordan/reusables)](https://github.com/Kiril-Mordan/reusables/blob/main/LICENSE)",
+    ## name of the project directory
+    project_name = "temp_project")
+```
+
+##### - preparing site
+
+
+```python
+mdh.create_mkdocs_dir()
+mdh.move_files_to_docs()
+mdh.generate_markdown_for_images()
+mdh.create_index()
+mdh.create_mkdocs_yml()
+mdh.build_mkdocs_site()
+```
+
+    Created new MkDocs dir: temp_project
+    Copied ../example_module.md to temp_project/docs/usage-examples.md
+    Copied ../tests/package_auto_assembler/release_notes.md to temp_project/docs/release_notes.md
+    index.md has been created with site_name: example-module
+    mkdocs.yml has been created with site_name: Example module
+    Custom CSS created at temp_project/docs/css/extra.css
+
+
+    INFO    -  Cleaning site directory
+    INFO    -  Building documentation to directory: /Users/user/reusables/example_notebooks/temp_project/site
+    INFO    -  Documentation built in 0.80 seconds
+
+
+##### - test runing site
+
+
+```python
+mdh.serve_mkdocs_site()
+```
```

### Comparing `package_auto_assembler-0.1.4/README.md` & `package_auto_assembler-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 ## Content:
  
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package auto assembler is a tool that meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
 [module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
```

### Comparing `package_auto_assembler-0.1.4/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.1.5/package_auto_assembler/package_auto_assembler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
-Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
+Package auto assembler is a tool that meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 """
 
@@ -25,14 +23,15 @@
 import yaml
 import nbformat
 from nbconvert import MarkdownExporter
 from nbconvert.preprocessors import ExecutePreprocessor
 import attr #>=22.2.0
 from stdlib_list import stdlib_list
 import tempfile
+import requests
 import pip_audit #==2.7.3
 
 
 # Metadata for package creation
 __package_metadata__ = {
     "author": "Kyrylo Mordan",
     "author_email": "parachute.repo@gmail.com",
@@ -963,24 +962,67 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
+    def read_module_content(self,
+                     filepath : str) -> str:
+
+        """
+        Method for reading in module.
+        """
+
+        with open(filepath, 'r') as file:
+            return file.read()
+
+    def extract_module_docstring(self,
+                                 module_content : str) -> str:
+
+        """
+        Method for extracting title, module level docstring.
+        """
+
+        match = re.search(r'^("""(.*?)"""|\'\'\'(.*?)\'\'\')', module_content, flags=re.DOTALL)
+        if match:
+            docstring_content = match.group(2) if match.group(2) is not None else match.group(3)
+            return docstring_content.strip()
+        return None
+
     def _format_title(self, filename : str) -> str:
         """
         Formats the filename into a more readable title by removing the '.md' extension,
         replacing underscores with spaces, and capitalizing each word.
         """
         title_without_extension = os.path.splitext(filename)[0]  # Remove the .md extension
         title_with_spaces = title_without_extension.replace('_', ' ')  # Replace underscores with spaces
         # Capitalize the first letter of each word
         return ' '.join(word.capitalize() for word in title_with_spaces.split())
 
+    def get_pypi_badge(self, module_name : str):
+
+        """
+        Get badge for module that was pushed to pypi.
+        """
+
+        # Convert underscores to hyphens
+        module_name_hyphenated = module_name.replace('_', '-')
+        pypi_module_link = f"https://pypi.org/project/{module_name_hyphenated}/"
+        pypi_link = ""
+
+        # Send a HEAD request to the PyPI module link
+        response = requests.head(pypi_module_link)
+
+        # Check if the response status code is 200 (OK)
+        if response.status_code == 200:
+            pypi_link = f"[![PyPiVersion](https://img.shields.io/pypi/v/{module_name_hyphenated})]({pypi_module_link})"
+
+        return pypi_link
+
 
     def convert_notebook_to_md(self,
                                notebook_path : str = None,
                                output_path : str = None):
 
         """
         Convert example notebook to md without executing.
@@ -1208,14 +1250,15 @@
         # Creating temporary __init__.py file
         init_file_path = os.path.join(setup_directory, '__init__.py')
         with open(init_file_path, 'w') as init_file:
             init_file.write(f"from .{module_name} import *\n")
 
     def write_setup_file(self,
                          module_name : str = None,
+                         module_docstring : str = None,
                          metadata : dict = None,
                          requirements : str = None,
                          classifiers : list = None,
                          setup_directory : str = None):
 
         """
         Create setup.py for the package.
@@ -1236,37 +1279,50 @@
         if classifiers is None:
             classifiers = self.classifiers
 
         if setup_directory is None:
             setup_directory = self.setup_directory
 
         metadata_str = ', '.join([f'{key}="{value}"' for key, value in metadata.items()])
+
+        title = module_name.capitalize()
+        title = title.replace("_"," ")
+
+        long_description_intro = f"""# {title}\n\n"""
+
+        if module_docstring:
+            long_description_intro += f"""{module_docstring}\n\n"""
+
         setup_content = f"""from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 path_to_readme = os.path.join(here, "README.md")
 
+"""
+
+        setup_content += f'long_description = """{long_description_intro}"""'
+
+        setup_content += f"""
+
 if os.path.exists(path_to_readme):
   with codecs.open(path_to_readme, encoding="utf-8") as fh:
-      long_description = fh.read()
-else:
-  long_description = ''
+      long_description += fh.read()
 
 setup(
     name="{module_name}",
     packages=["{module_name}"],
     install_requires={requirements},
     classifiers={classifiers},
     long_description=long_description,
     long_description_content_type='text/markdown',
     {metadata_str}
 )
-        """
+"""
         with open(os.path.join(setup_directory, 'setup.py'), 'w') as file:
             file.write(setup_content)
 
 @attr.s
 class ReleaseNotesHandler:
 
     # inputs
@@ -1524,14 +1580,324 @@
 
         if self.processed_messages != []:
             # Write the updated or new contents back to the file
             with open(filepath, 'w') as file:
                 file.writelines(note_entries)
 
 
+@attr.s
+class MkDocsHandler:
+
+    # inputs
+    package_name = attr.ib(type=str)
+    docs_file_paths = attr.ib(type=list)
+
+    module_docstring = attr.ib(default=None, type=str)
+    pypi_badge = attr.ib(default='', type=str)
+    license_badge = attr.ib(default='', type=str)
+
+    project_name = attr.ib(default="temp_project", type=str)
+
+    # processed
+    logger = attr.ib(default=None)
+    logger_name = attr.ib(default='MkDocs Handler')
+    loggerLvl = attr.ib(default=logging.INFO)
+    logger_format = attr.ib(default=None)
+
+    def __attrs_post_init__(self):
+        self._initialize_logger()
+
+    def _initialize_logger(self):
+        """
+        Initialize a logger for the class instance based on the specified logging level and logger name.
+        """
+
+        if self.logger is None:
+            logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
+            logger = logging.getLogger(self.logger_name)
+            logger.setLevel(self.loggerLvl)
+
+            self.logger = logger
+
+    def create_mkdocs_project(self, project_name: str = None):
+        """
+        Create a new MkDocs project.
+        """
+
+        if project_name is None:
+            project_name = self.project_name
+
+        subprocess.run(["mkdocs", "new", project_name])
+        print(f"Created new MkDocs project: {project_name}")
+
+    def create_mkdocs_dir(self, project_name: str = None):
+        """
+        Create a new dir for MkDocs project.
+        """
+
+        if project_name is None:
+            project_name = self.project_name
+
+        if os.path.exists(project_name):
+            shutil.rmtree(project_name)
+        os.makedirs(project_name)
+
+        print(f"Created new MkDocs dir: {project_name}")
+
+    def move_files_to_docs(self, file_paths: dict = None, project_name: str = None):
+        """
+        Move files from given list of paths to the docs directory.
+        """
+
+        if file_paths is None:
+            file_paths = self.docs_file_paths
+
+        if project_name is None:
+            project_name = self.project_name
+
+        docs_dir = os.path.join(project_name, "docs")
+        if not os.path.exists(docs_dir):
+            os.makedirs(docs_dir)
+
+        for file_path in file_paths:
+            if os.path.exists(file_path):
+                filename = file_paths[file_path]
+                destination = os.path.join(docs_dir, filename)
+
+                # Ensure unique filenames
+                if os.path.exists(destination):
+                    base, extension = os.path.splitext(filename)
+                    counter = 1
+                    while os.path.exists(destination):
+                        new_filename = f"{base}_{counter}{extension}"
+                        destination = os.path.join(docs_dir, new_filename)
+                        counter += 1
+
+                shutil.copy(file_path, destination)
+                print(f"Copied {file_path} to {destination}")
+            else:
+                print(f"File not found: {file_path}")
+
+    def _clean_filename(self, filename: str, package_name: str) -> str:
+        """
+        Remove the package name prefix from the filename.
+
+        Args:
+            filename (str): The original filename.
+            package_name (str): The package name to remove.
+
+        Returns:
+            str: The cleaned filename without the package name prefix.
+        """
+        if filename.startswith(f"{package_name}-"):
+          return filename[len(package_name)+1:]
+        # if filename == f"{package_name}.md":
+        #   return "usage-examples.md"
+
+        return filename
+
+    def create_index(self,
+                     project_name: str = None,
+                     module_docstring : str = None,
+                     pypi_badge : str = None,
+                     license_badge : str = None):
+
+        """
+        Create index page with small intro.
+        """
+
+        if project_name is None:
+            project_name = self.package_name
+
+        if module_docstring is None:
+            module_docstring = self.module_docstring
+
+        if pypi_badge is None:
+            pypi_badge = self.pypi_badge
+
+        if license_badge is None:
+            license_badge = self.license_badge
+
+        package_name = project_name.replace("_","-")
+
+        content = f"""# Intro
+
+{pypi_badge} {license_badge}
+
+{module_docstring}
+
+## Installation
+
+```bash
+pip install {package_name}
+```
+        """
+
+        mkdocs_index_path = os.path.join("temp_project","docs", "index.md")
+        with open(mkdocs_index_path, 'w', encoding='utf-8') as file:
+            file.write(content)
+        print(f"index.md has been created with site_name: {package_name}")
+
+
+
+    def generate_markdown_for_images(self, package_name: str = None, project_name: str = None):
+        """
+        Generate .md files for each .png file in the specified directory based on naming rules.
+
+        Args:
+            directory (str): Path to the directory containing .png files.
+            package_name (str): The package name to use for naming conventions.
+        """
+
+        if package_name is None:
+            package_name = self.package_name
+
+        if project_name is None:
+            project_name = self.project_name
+
+        directory = os.path.join(project_name, "docs")
+
+        if not os.path.exists(directory):
+            print(f"The directory {directory} does not exist.")
+            return
+
+        for filename in os.listdir(directory):
+            if filename.endswith('.png'):
+                cleaned_name = self._clean_filename(filename, package_name)
+                md_filename = f"{os.path.splitext(cleaned_name)[0]}.md"
+
+                md_filepath = os.path.join(directory, md_filename)
+
+                # Write Markdown content
+                with open(md_filepath, 'w') as md_file:
+                    md_content = f"![{filename}](./{filename})"
+                    md_file.write(md_content)
+                print(f"Created {md_filepath}")
+
+    def create_mkdocs_yml(self, package_name: str = None, project_name: str = None):
+        """
+        Create mkdocs.yml with a given site_name.
+        """
+
+        if project_name is None:
+            project_name = self.project_name
+
+        if package_name is None:
+            package_name = self.package_name
+
+        package_name = package_name.capitalize()
+        package_name = package_name.replace("_"," ")
+
+        content = f"""site_name: {package_name}
+
+theme:
+  name: material
+  palette:
+    # Palette toggle for light mode
+    - scheme: default
+      primary: green
+      accent: green
+      toggle:
+        icon: material/lightbulb
+        name: Switch to dark mode
+
+    # Palette toggle for dark mode
+    - scheme: slate
+      primary: green
+      accent: green
+      toggle:
+        icon: material/lightbulb-outline
+        name: Switch to light mode
+
+extra_css:
+  - css/extra.css
+        """
+
+        mkdocs_yml_path = os.path.join(project_name, "mkdocs.yml")
+        with open(mkdocs_yml_path, "w") as file:
+            file.write(content.strip())
+        print(f"mkdocs.yml has been created with site_name: {package_name}")
+
+        css_dir = os.path.join(project_name, "docs", "css")
+        if not os.path.exists(css_dir):
+            os.makedirs(css_dir)
+
+        css_content = """
+/* Ensure tables are scrollable horizontally */
+table {
+  display: block;
+  width: 100%;
+  overflow-x: auto;
+  white-space: nowrap;
+}
+
+/* Ensure tables and their parent divs don't overflow the content area */
+.dataframe {
+  display: block;
+  width: 100%;
+  overflow-x: auto;
+  white-space: nowrap;
+}
+
+.dataframe thead th {
+  text-align: right;
+}
+
+.dataframe tbody tr th {
+  vertical-align: top;
+}
+
+.dataframe tbody tr th:only-of-type {
+  vertical-align: middle;
+}
+
+/* Ensure the whole content area is scrollable */
+.md-content__inner {
+  overflow-x: auto;
+  padding: 20px; /* Add some padding for better readability */
+}
+
+/* Fix layout issues caused by the theme */
+.md-main__inner {
+  max-width: none;
+}
+        """
+
+        css_path = os.path.join(css_dir, "extra.css")
+        with open(css_path, "w") as file:
+            file.write(css_content.strip())
+        print(f"Custom CSS created at {css_path}")
+
+    def build_mkdocs_site(self, project_name: str = None):
+        """
+        Serve the MkDocs site.
+        """
+
+        if project_name is None:
+            project_name = self.project_name
+
+        os.chdir(project_name)
+        subprocess.run(["mkdocs", "build"])
+        os.chdir("..")
+
+    def serve_mkdocs_site(self, project_name: str = None):
+        """
+        Serve the MkDocs site.
+        """
+
+        if project_name is None:
+            project_name = self.project_name
+
+        try:
+            os.chdir(project_name)
+            subprocess.run(["mkdocs", "serve"])
+        except Exception as e:
+            print(e)
+        finally:
+            os.chdir("..")
 
 
 @attr.s
 class PackageAutoAssembler:
     # pylint: disable=too-many-instance-attributes
 
     ## inputs
@@ -1847,18 +2213,22 @@
             )
         else:
             self.long_doc_h.convert_notebook_to_md(
                 notebook_path = example_notebook_path,
                 output_path = output_path
             )
 
+
     def prep_setup_file(self,
+                       module_name : str = None,
                        metadata : dict = None,
                        requirements : str = None,
-                       classifiers : list = None):
+                       classifiers : list = None,
+                       module_filepath : str = None,
+                       module_docstring : str = None):
 
         """
         Assemble setup.py file.
         """
 
         if self.setup_dir_h is None:
             self._initialize_setup_dir_handler()
@@ -1868,16 +2238,33 @@
 
         if requirements is None:
             requirements = self.requirements_list
 
         if classifiers is None:
             classifiers = self.classifiers
 
+        if module_filepath is None:
+            module_filepath = self.module_filepath
+
+        if module_name is None:
+            module_name = self.module_name
+
+        if module_docstring is None:
+
+            if self.long_doc_h is None:
+                self._initialize_long_doc_handler()
+
+            module_content = self.long_doc_h.read_module_content(filepath = module_filepath)
+
+            module_docstring = self.long_doc_h.extract_module_docstring(module_content = module_content)
+
         # create setup.py
-        self.setup_dir_h.write_setup_file(metadata = metadata,
+        self.setup_dir_h.write_setup_file(module_name = module_name,
+                                          module_docstring = module_docstring,
+                                          metadata = metadata,
                                           requirements = requirements,
                                           classifiers = classifiers)
 
     def make_package(self,
                      setup_directory : str = None):
 
         """
```

### Comparing `package_auto_assembler-0.1.4/package_auto_assembler/setup.py` & `package_auto_assembler-0.1.5/package_auto_assembler/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'pandas', 'pip_audit==2.7.3', 'nbformat', 'pyyaml', 'attrs>=22.2.0', 'stdlib-list', 'nbconvert'],
+    install_requires=['### package_auto_assembler.py', 'pip_audit==2.7.3', 'pyyaml', 'nbconvert', 'pandas', 'requests', 'attrs>=22.2.0', 'nbformat', 'stdlib-list'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.4"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.5"
 )
```

### Comparing `package_auto_assembler-0.1.4/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.1.5/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package-auto-assembler
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,47 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Package Auto Assembler
-
-This tool is meant to streamline creation of single module packages.
-Its purpose is to automate as many aspects of python package creation as possible,
-to shorten a development cycle of reusable components, maintain certain standard of quality
-for reusable code. It provides tool to simplify the process of package creatrion
-to a point that it can be triggered automatically within ci/cd pipelines,
-with minimal preparations and requirements for new modules.
-
-
-
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
-            ReleaseNotesHandler, PackageAutoAssembler)
+            ReleaseNotesHandler, MkDocsHandler, PackageAutoAssembler)
 ```
 
-## Usage examples
-
-The examples contain: 
-1. package versioning
-2. import mapping
-3. extracting and merging requirements
-4. preparing metadata
-5. merging local dependacies into single module
-6. prepare README
-7. assembling setup directory
-8. making a package
-9. creating release notes from commit messages
-
 ### 1. Package versioning
 
 #### Initialize VersionHandler
 
 
 ```python
 pv = VersionHandler(
@@ -165,27 +141,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-22 01:10:59</td>
+      <td>2024-05-28 01:28:20</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -276,15 +252,15 @@
     custom_modules_filepath="../tests/package_auto_assembler/dependancies"
 )
 ```
 
 
 
 
-    ['example_local_dependacy_1', 'example_local_dependacy_2']
+    ['example_local_dependacy_2', 'example_local_dependacy_1']
 
 
 
 #### Check if module is a standard python library
 
 
 ```python
@@ -898,15 +874,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
@@ -917,43 +893,36 @@
     label_name = 'example_module',
     # new version to be used in release notes
     version = '0.0.2'
 )
 ```
 
     No relevant commit messages found!
-
-
     ..trying depth 2 !
-
-
     No relevant commit messages found!
-
-
     No messages to clean were provided
 
 
 ##### - overwritting commit messages from example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README',
-     'Update requirements',
-     '[package_auto_assembler] test_install_package() method for local testing',
-     'simpler test_install_package.py script',
-     'Update package version tracking files',
-     'Update README',
-     'Update requirements']
+    ['slight changes to gh-pages workflow',
+     'adding package_auto_assembler to usage examples test run exceptions',
+     'updated gh-pages workflow',
+     'testing newer MkDocsHandler',
+     'updated workflows',
+     'package name parameter for gh-pages workflow']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
@@ -1033,7 +1002,78 @@
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
      '\n',
      '    - initial version of example_module\n']
 
 
+
+### 10. Making simple MkDocs site
+
+##### - preparing inputs
+
+
+```python
+package_name = "example_module"
+
+module_content = LongDocHandler().read_module_content(filepath=f"../tests/package_auto_assembler/{package_name}.py")
+
+docstring = LongDocHandler().extract_module_docstring(module_content=module_content)
+pypi_link = LongDocHandler().get_pypi_badge(module_name=package_name)
+
+
+docs_file_paths = {
+    "../example_module.md" : "usage-examples.md",
+    '../tests/package_auto_assembler/release_notes.md' : 'release_notes.md'
+}
+```
+
+
+```python
+mdh = MkDocsHandler(
+    # required
+    ## name of the package to be displayed
+    package_name = package_name,
+    ## dictionary of markdown files, with path as keys
+    docs_file_paths = docs_file_paths,
+    # optional
+    ## module docstring to be displayed in the index
+    module_docstring = docstring,
+    ## pypi badge to be displayed in the index
+    pypi_badge = pypi_link,
+    ## license badge to be displayed in the index
+    license_badge="[![License](https://img.shields.io/github/license/Kiril-Mordan/reusables)](https://github.com/Kiril-Mordan/reusables/blob/main/LICENSE)",
+    ## name of the project directory
+    project_name = "temp_project")
+```
+
+##### - preparing site
+
+
+```python
+mdh.create_mkdocs_dir()
+mdh.move_files_to_docs()
+mdh.generate_markdown_for_images()
+mdh.create_index()
+mdh.create_mkdocs_yml()
+mdh.build_mkdocs_site()
+```
+
+    Created new MkDocs dir: temp_project
+    Copied ../example_module.md to temp_project/docs/usage-examples.md
+    Copied ../tests/package_auto_assembler/release_notes.md to temp_project/docs/release_notes.md
+    index.md has been created with site_name: example-module
+    mkdocs.yml has been created with site_name: Example module
+    Custom CSS created at temp_project/docs/css/extra.css
+
+
+    INFO    -  Cleaning site directory
+    INFO    -  Building documentation to directory: /Users/user/reusables/example_notebooks/temp_project/site
+    INFO    -  Documentation built in 0.80 seconds
+
+
+##### - test runing site
+
+
+```python
+mdh.serve_mkdocs_site()
+```
```

