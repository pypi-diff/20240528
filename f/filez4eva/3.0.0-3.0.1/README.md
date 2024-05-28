# Comparing `tmp/filez4eva-3.0.0.tar.gz` & `tmp/filez4eva-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filez4eva-3.0.0.tar", max compression
+gzip compressed data, was "filez4eva-3.0.1.tar", max compression
```

## Comparing `filez4eva-3.0.0.tar` & `filez4eva-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1616 2024-05-14 04:26:37.137152 filez4eva-3.0.0/README.md
--rw-r--r--   0        0        0      168 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/__init__.py
--rw-r--r--   0        0        0       98 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/__main__.py
--rw-r--r--   0        0        0      291 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/__init__.py
--rw-r--r--   0        0        0     2770 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/scan_command.py
--rw-r--r--   0        0        0     3866 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/stow_command.py
--rw-r--r--   0        0        0       42 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/error.py
--rw-r--r--   0        0        0      585 2024-05-14 04:26:47.818143 filez4eva-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 filez4eva-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1616 2024-05-28 02:01:52.548662 filez4eva-3.0.1/README.md
+-rw-r--r--   0        0        0      353 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/__main__.py
+-rw-r--r--   0        0        0      102 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/command/__init__.py
+-rw-r--r--   0        0        0     2790 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/command/scan_dir_command.py
+-rw-r--r--   0        0        0     3875 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/command/stow_file_command.py
+-rw-r--r--   0        0        0       42 2024-05-28 02:01:52.548662 filez4eva-3.0.1/filez4eva/error.py
+-rw-r--r--   0        0        0      585 2024-05-28 02:02:03.211699 filez4eva-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 filez4eva-3.0.1/PKG-INFO
```

### Comparing `filez4eva-3.0.0/README.md` & `filez4eva-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `filez4eva-3.0.0/filez4eva/command/scan_command.py` & `filez4eva-3.0.1/filez4eva/command/scan_dir_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from wizlib.parser import WizParser
 from wizlib.ui import Chooser
 from wizlib.ui.shell_ui import Emphasis
 from wizlib.app import AppCancellation
 
 from filez4eva.command import Filez4EvaCommand
-from filez4eva.command.stow_command import StowCommand
+from filez4eva.command.stow_file_command import StowFileCommand
 
 
-class ScanCommand(Filez4EvaCommand):
+class StowDirCommand(Filez4EvaCommand):
     """Handle files from a directory"""
 
-    name = 'scan'
+    name = 'stow-dir'
 
     @classmethod
     def add_args(cls, parser: WizParser):
         super().add_args(parser)
         parser.add_argument('dir')
 
     @Filez4EvaCommand.wrap
@@ -59,15 +59,15 @@
             elif action == 'delete':
                 confirm = self.app.ui.get_option(self.DELETE_CHOOSER)
                 if confirm != 'Yes':
                     continue
                 os.remove(file)
                 self.increment_result('Deleted')
             elif action == 'stow':
-                command = StowCommand(self.app, file=str(file))
+                command = StowFileCommand(self.app, file=str(file))
                 command.execute()
                 if command.status:
                     self.increment_result('Stowed')
                 else:
                     self.app.ui.send(file.name)
                     continue
             elif action == 'quit':
```

### Comparing `filez4eva-3.0.0/filez4eva/command/stow_command.py` & `filez4eva-3.0.1/filez4eva/command/stow_file_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from filez4eva.command import Filez4EvaCommand
 from filez4eva.error import Filez4EvaError
 
 
 FILE_PATTERN = re.compile(r'\d{8}\-([a-zA-Z0-9-]+)\.(\w+)')
 
 
-class StowCommand(Filez4EvaCommand):
+class StowFileCommand(Filez4EvaCommand):
     """Move filez to the right place with the right name"""
 
-    name = 'stow'
+    name = 'stow-file'
 
     date: str
     account: str
     part: str
 
     @classmethod
     def add_args(cls, parser: WizParser):
```

### Comparing `filez4eva-3.0.0/pyproject.toml` & `filez4eva-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "filez4eva"
 description = "Shift scans, photos, and other files into structured folders for permanent safekeeping"
 authors = ["Francis Potter <francis@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
-version = "3.0.0"
+version = "3.0.1"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 watchdog = "^3.0.0"
-wizlib = "^3.0.0"
+wizlib = "^3.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.11.0"
 coverage = "^7.3.0"
 autopep8 = "^2.0.4"
 
 [build-system]
```

### Comparing `filez4eva-3.0.0/PKG-INFO` & `filez4eva-3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: filez4eva
-Version: 3.0.0
+Version: 3.0.1
 Summary: Shift scans, photos, and other files into structured folders for permanent safekeeping
 License: MIT
 Author: Francis Potter
 Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
-Requires-Dist: wizlib (>=3.0.0,<4.0.0)
+Requires-Dist: wizlib (>=3.1.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Filez4Eva
 
 Shift scans, photos, and other files into structured folders for permanent safekeeping
 ---
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: filez4eva Version: 3.0.0 Summary: Shift scans,
+Metadata-Version: 2.1 Name: filez4eva Version: 3.0.1 Summary: Shift scans,
 photos, and other files into structured folders for permanent safekeeping
 License: MIT Author: Francis Potter Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: watchdog (>=3.0.0,<4.0.0) Requires-
-Dist: wizlib (>=3.0.0,<4.0.0) Description-Content-Type: text/markdown #
+Dist: wizlib (>=3.1.1,<4.0.0) Description-Content-Type: text/markdown #
 Filez4Eva Shift scans, photos, and other files into structured folders for
 permanent safekeeping --- _E_l_e_p_h_a_n_t_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_l_a_t_ _I_c_o_n_s_ _-_ _F_l_a_t_i_c_o_n I keep
 files named and organized in a certain way in DropBox. This tool names new
 files correctly and puts them in the right directory. ## Installation It's best
 to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if
 you need it. Then: ```bash pipx install filez4eva ``` ## Usage The directory
 pattern for account documents is: ``` ~/Dropbox/accounts///-. ``` Where: -
```

