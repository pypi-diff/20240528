# Comparing `tmp/tabswitcher-0.1.0.tar.gz` & `tmp/tabswitcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.0.tar", last modified: Mon May 27 00:42:31 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.1.tar", last modified: Mon May 27 22:16:58 2024, max compression
```

## Comparing `tabswitcher-0.1.0.tar` & `tabswitcher-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.544689 tabswitcher-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.544689 tabswitcher-0.1.0/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:16:58.068445 tabswitcher-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 22:16:58.068445 tabswitcher-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:16:58.068445 tabswitcher-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:16:58.064445 tabswitcher-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:16:58.064445 tabswitcher-0.1.1/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:16:58.068445 tabswitcher-0.1.1/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 22:16:53.000000 tabswitcher-0.1.1/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:16:58.068445 tabswitcher-0.1.1/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:16:58.000000 tabswitcher-0.1.1/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.0/LICENCE` & `tabswitcher-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/PKG-INFO` & `tabswitcher-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -51,14 +51,20 @@
 
 ```bash
 tabswitcher --install
 ```
 
 3. Restart the browser
 
+When using Ubuntu some extra setup is required.
+
+```bash
+sudo apt-get install qtbase5-dev libxcb-xinerama0
+```
+
 ## Usage
 
 Upon opening TabSwitcher, your most recently active tabs will be displayed in the list.
 Typing in the input field will initiate a fuzzy search of all your open tabs by title.
 
 You can focus a tab by clicking an item in the list.
 Holding Shift while clicking will also bring the browser window into focus.
@@ -77,8 +83,8 @@
 Starting a input with `!` will attempt to open a new tab with the website page (requires a [Redirect Extension](https://addons.mozilla.org/de/firefox/addon/skip-redirect/)).
 
 `Ctrl + ,` will open the settings file.
 `Ctrl + q` or `Escape` will close the window.
 
 ## Known Issues
 
-- Currently, TabSwitcher only supports Windows.
+- Currently, TabSwitcher only supports Windows and limited on Ubuntu.
```

### Comparing `tabswitcher-0.1.0/README.md` & `tabswitcher-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
 ```bash
 tabswitcher --install
 ```
 
 3. Restart the browser
 
+When using Ubuntu some extra setup is required.
+
+```bash
+sudo apt-get install qtbase5-dev libxcb-xinerama0
+```
+
 ## Usage
 
 Upon opening TabSwitcher, your most recently active tabs will be displayed in the list.
 Typing in the input field will initiate a fuzzy search of all your open tabs by title.
 
 You can focus a tab by clicking an item in the list.
 Holding Shift while clicking will also bring the browser window into focus.
@@ -48,8 +54,8 @@
 Starting a input with `!` will attempt to open a new tab with the website page (requires a [Redirect Extension](https://addons.mozilla.org/de/firefox/addon/skip-redirect/)).
 
 `Ctrl + ,` will open the settings file.
 `Ctrl + q` or `Escape` will close the window.
 
 ## Known Issues
 
-- Currently, TabSwitcher only supports Windows.
+- Currently, TabSwitcher only supports Windows and limited on Ubuntu.
```

### Comparing `tabswitcher-0.1.0/setup.py` & `tabswitcher-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.0',
+    version='0.1.1',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.1.0/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.1/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.1/src/tabswitcher/SearchInput.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 import os
 from PyQt5.QtGui import QIcon, QFont, QFontDatabase
 from PyQt5.QtCore import Qt, QSize
-from PyQt5.QtWidgets import QWidget, QLineEdit, QHBoxLayout, QToolButton
+from PyQt5.QtWidgets import QLineEdit, QHBoxLayout, QToolButton, QLabel
 
 from .Settings import Settings
 from .colors import getBackgroundColor, getTextColor
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 
 class SearchInput(QLineEdit):
+
+    def update_count(self):
+        self.listCountLabel.setText(str(self.parent().list.count()))
+
     def __init__(self, parent=None):
         super(SearchInput, self).__init__(parent)
 
+        font_path = os.path.join(script_dir, 'assets', "sans.ttf")
+        font_id = QFontDatabase.addApplicationFont(font_path)
+        font_family = QFontDatabase.applicationFontFamilies(font_id)[0]
+        # Set the font
+        font = QFont(font_family, 10)
+
         # Create a QToolButton
         button = QToolButton()
         icon_path = os.path.join(script_dir, 'assets', 'searchIcon.svg')
         button.setIcon(QIcon(icon_path))
         button.setIconSize(QSize(32, 32))
         button.setEnabled(False)
         button.setStyleSheet("QToolButton { border: none; padding: 0px; background: transparent; }")
+        self.listCountLabel = QLabel()
+        self.setFont(font)
+        self.listCountLabel.setStyleSheet("""
+    QLabel {
+        color: %s;
+        font-size: 12px;
+        background: transparent;
+        padding-left: 5px;
+        margin: 0px;
+        font: sans;
+    }
+""" % (getTextColor())
+        )
 
         # Create a QHBoxLayout
         layout = QHBoxLayout(self)
         layout.addWidget(button, 0, Qt.AlignLeft)
+        layout.addWidget(self.listCountLabel, 0, (Qt.AlignRight | Qt.AlignBottom))
 
-        widget = QWidget()
-        layout.addWidget(widget)
-        widget.setStyleSheet("background:transparent;")
-        self.setLayout(layout)
         self.settings = Settings()
-        font_path = os.path.join(script_dir, 'assets', "sans.ttf")
-        font_id = QFontDatabase.addApplicationFont(font_path)
-        font_family = QFontDatabase.applicationFontFamilies(font_id)[0]
-        # Set the font
-        font = QFont(font_family, 10)
         self.setFont(font)
         self.setFocus()
         self.setPlaceholderText("Search for a tab")
         self.setStyleSheet("""
     QLineEdit {
         border: 2px solid gray;
         border-radius: 10px;
         padding: 0 8px;
         padding-left: 60px; 
+        padding-right: 60px; 
         height: 50px;
         background: %s;
         color: %s;
         font-size: 32px;
     }                             
 """ % (getBackgroundColor(), getTextColor())
         )
```

### Comparing `tabswitcher-0.1.0/src/tabswitcher/Settings.py` & `tabswitcher-0.1.1/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/Tab.py` & `tabswitcher-0.1.1/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/TabList.py` & `tabswitcher-0.1.1/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.1/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/actions.py` & `tabswitcher-0.1.1/src/tabswitcher/actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 
 import os
 import webbrowser
+import platform
+import subprocess
 
 from PyQt5.QtCore import Qt, QUrl
 from PyQt5.QtGui import QDesktopServices
 
 from tabswitcher.Settings import Settings
 from tabswitcher.brotab import switch_tab
 
 settings = Settings()
 
 def open_settings():
-    # Open the configuration file in the default text editor
-    os.startfile(settings.config_file)
-
+    if platform.system() == "Windows":
+        os.startfile(settings._file)
+    elif platform.system() == "Darwin":
+        subprocess.call(["open", settings._file])
+    else:
+        subprocess.call(["xdg-open", settings._file])
 
 def activate_tab(window, item):
     tab_id, tab_title, tab_url = item.data(Qt.UserRole)
     if tab_id == -1:
         webbrowser.open(tab_url)
     else:
         switch_tab(tab_id, tab_title)
```

### Comparing `tabswitcher-0.1.0/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.1/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/assets/install.bat` & `tabswitcher-0.1.1/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.1/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.1/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/brotab.py` & `tabswitcher-0.1.1/src/tabswitcher/brotab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 
 import os
+import pickle
 import subprocess
 import chardet
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QGuiApplication
 
 from tabswitcher.focusWindow import focus_window
 
 from .Settings import Settings
 from .Tab import Tab
 
 settings = Settings()
 script_dir = os.path.dirname(os.path.realpath(__file__))
+config_dir = os.path.expanduser('~/.tabswitcher')
+tab_history_path = os.path.join(config_dir, settings.get_tab_logging_file())
 
 def get_url():
     mediator_port = settings.get_mediator_port()
     if mediator_port == 0:
         return None
     elif mediator_port not in range(4625, 4627):
         raise ValueError("Mediator port must be between 4625 and 4626 or 0 for automatic selection.")
@@ -121,8 +124,9 @@
         if len(lines) == 0:
             return None
         data = lines[0].split('\t')
         if (len(data) == 5):
             return data[0]
         return None
     except:
-        return None
+        return None
+
```

### Comparing `tabswitcher-0.1.0/src/tabswitcher/colors.py` & `tabswitcher-0.1.1/src/tabswitcher/colors.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,13 @@
     return "#818181"
 
 def getWindowBackgroundColor():
     if(settings.get_show_background()):
         if(settings.get_dark_mode()):
             return "#121212"
         return "#dddddd"
-    return "transparent"
+    return "transparent"
+
+def getPlaceholderColor():
+    if(settings.get_dark_mode()):
+        return "#8a8a8b"
+    return "#8a8a8b"
```

### Comparing `tabswitcher-0.1.0/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.1/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.1/src/tabswitcher/loadBookmarks.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.1/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.1/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.0/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.1/tabswitcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -51,14 +51,20 @@
 
 ```bash
 tabswitcher --install
 ```
 
 3. Restart the browser
 
+When using Ubuntu some extra setup is required.
+
+```bash
+sudo apt-get install qtbase5-dev libxcb-xinerama0
+```
+
 ## Usage
 
 Upon opening TabSwitcher, your most recently active tabs will be displayed in the list.
 Typing in the input field will initiate a fuzzy search of all your open tabs by title.
 
 You can focus a tab by clicking an item in the list.
 Holding Shift while clicking will also bring the browser window into focus.
@@ -77,8 +83,8 @@
 Starting a input with `!` will attempt to open a new tab with the website page (requires a [Redirect Extension](https://addons.mozilla.org/de/firefox/addon/skip-redirect/)).
 
 `Ctrl + ,` will open the settings file.
 `Ctrl + q` or `Escape` will close the window.
 
 ## Known Issues
 
-- Currently, TabSwitcher only supports Windows.
+- Currently, TabSwitcher only supports Windows and limited on Ubuntu.
```

### Comparing `tabswitcher-0.1.0/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.1/tabswitcher.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/tabswitcher/focusWindow.py
 src/tabswitcher/fuzzySearch.py
 src/tabswitcher/loadBookmarks.py
 src/tabswitcher/logTabs.py
 src/tabswitcher/shortcuts.py
 src/tabswitcher/assets/Icon.ico
 src/tabswitcher/assets/install.bat
+src/tabswitcher/assets/install.sh
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
 src/tabswitcher/assets/tabswitcher_service.xml
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
 tabswitcher.egg-info/entry_points.txt
```

