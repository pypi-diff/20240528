# Comparing `tmp/easy_gui_jupyter-2024.5.28.tar.gz` & `tmp/easy_gui_jupyter-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gui_jupyter-2024.5.28.tar", max compression
+gzip compressed data, was "easy_gui_jupyter-2024.5.8.tar", max compression
```

## Comparing `easy_gui_jupyter-2024.5.28.tar` & `easy_gui_jupyter-2024.5.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.28/LICENSE.txt
--rw-r--r--   0        0        0     3017 2024-05-24 13:22:50.689908 easy_gui_jupyter-2024.5.28/README.md
--rw-r--r--   0        0        0      115 2024-05-19 16:20:30.033036 easy_gui_jupyter-2024.5.28/easy_gui_jupyter/__init__.py
--rw-r--r--   0        0        0     9951 2024-05-28 10:56:38.684056 easy_gui_jupyter-2024.5.28/easy_gui_jupyter/easy_gui_jupyter.py
--rw-r--r--   0        0        0     1021 2024-05-28 11:03:11.718381 easy_gui_jupyter-2024.5.28/pyproject.toml
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.28/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.8/LICENSE.txt
+-rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.8/README.md
+-rw-r--r--   0        0        0       52 2024-05-08 11:08:51.866358 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/__init__.py
+-rw-r--r--   0        0        0     9311 2024-05-08 11:08:51.867208 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py
+-rw-r--r--   0        0        0      840 2024-05-08 14:12:51.366763 easy_gui_jupyter-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.8/PKG-INFO
```

### Comparing `easy_gui_jupyter-2024.5.28/LICENSE.txt` & `easy_gui_jupyter-2024.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-2024.5.28/README.md` & `easy_gui_jupyter-2024.5.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # Easy GUI Jupyter
 
-[![PyPI version](https://badge.fury.io/py/easy_gui_jupyter.svg)](https://badge.fury.io/py/easy_gui_jupyter)
-[![Python versions](https://img.shields.io/pypi/pyversions/easy_gui_jupyter.svg)](https://pypi.org/project/easy_gui_jupyter/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
 Easy GUI Jupyter is a Python library that simplifies the creation of graphical user interfaces (GUIs) in Jupyter notebooks using ipywidgets. It provides a convenient way to add various types of widgets to your Jupyter notebooks, making it easier to interact with your code and visualize results.
 
 ## Features
 
 - Simplifies the creation of GUIs in Jupyter notebooks
 - Supports a variety of widget types, including labels, buttons, text inputs, sliders, checkboxes, and dropdowns
 - Allows saving and loading widget values to maintain user settings across sessions
```

### Comparing `easy_gui_jupyter-2024.5.28/easy_gui_jupyter/easy_gui_jupyter.py` & `easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,321 +1,244 @@
-import yaml
-from ipyfilechooser import FileChooser
-import ipywidgets as widgets
-from IPython.display import display, clear_output
-from pathlib import Path
-
 """
 A module to help simplify the create of GUIs in Jupyter notebooks using ipywidgets.
 """
 
-CONFIG_PATH = Path.home() / ".config" / "easy_gui"
-
-
-def get_config(title: str) -> dict:
-    """
-    Get the configuration dictionary without needing to initialize the GUI.
-
-    Args:
-        title (str): The title of the GUI.
-
-    Returns:
-        dict: The configuration dictionary.
-    """
-
-    config_file = CONFIG_PATH / f"{title}.yml"
-
-    if not config_file.exists():
-        return {}
-
-    with open(config_file, "r") as f:
-        cfg = yaml.load(f, Loader=yaml.SafeLoader)
+import os
+import yaml
+from ipyfilechooser import FileChooser
 
-    if title is None:
-        return cfg
-    elif title in cfg:
-        return cfg[title]
-    else:
-        return {}
+import ipywidgets as widgets
+from IPython.display import display, clear_output
 
 
-def save_config(title: str, cfg: dict):
+class EasyGUI:
     """
-    Save the configuration dictionary to file.
+    A class to simplify the creation of GUIs in Jupyter notebooks using ipywidgets.
 
     Args:
         title (str): The title of the GUI.
-        cfg (dict): The configuration dictionary.
-    """
-    config_file = CONFIG_PATH / f"{title}.yml"
-    config_file.parent.mkdir(exist_ok=True)
-
-    base_config = get_config(None)  # loads the config file
-    base_config[title] = cfg
-
-    with open(config_file, "w") as f:
-        yaml.dump(base_config, f)
+        width (str): The width of the widget container (e.g., "50%").
 
+    Attributes:
+        _layout (ipywidgets.Layout): The layout for widgets.
+        _style (dict): Style configuration for widgets.
+        _widgets (dict): A dictionary to store widgets.
+        _nLabels (int): The number of labels added to the GUI.
+        _main_display (ipywidgets.VBox): The main output widget for the GUI.
+        _title (str): The title of the GUI.
+        _cfg (dict): Configuration dictionary to store widget values.
+        cfg (dict): Alias for the _cfg dictionary associated with the GUI.
+
+    Methods:
+        add_label: Add a label widget to the GUI.
+        add_button: Add a button widget to the GUI.
+        add_text: Add a text widget to the GUI.
+        add_int_slider: Add an integer slider widget to the GUI.
+        add_float_slider: Add a float slider widget to the GUI.
+        add_checkbox: Add a checkbox widget to the GUI.
+        add_int_text: Add an integer text widget to the GUI.
+        add_float_text: Add a float text widget to the GUI.
+        add_dropdown: Add a dropdown widget to the GUI.
+        add_file_upload: Add a file upload widget to the GUI.
+        save_settings: Save widget values to a configuration file.
+        show: Display the GUI with its widgets.
+        clear: Clear all widgets from the GUI.
 
-class EasyGUI:
-    """
-    A class to help simplify the creation of GUIs in Jupyter notebooks using ipywidgets.
+    Note:
+        This class simplifies the creation of GUIs in Jupyter notebooks using ipywidgets. It provides a variety of methods for adding different types of widgets to the GUI, and it allows for saving and loading widget values to maintain user settings across sessions.
     """
 
     def __init__(self, title="basic_gui", width="50%"):
         """
         Container for widgets.
-
-        Args:
-            title (str): The title of the widget container, used to store settings.
-            width (str): The width of the widget container.
+        :param width: width of the widget container
         """
         self._layout = widgets.Layout(width=width)
         self._style = {"description_width": "initial"}
         self._widgets = {}
         self._nLabels = 0
         self._main_display = widgets.VBox()
         self._title = title
-        self._cfg = get_config(title)
-
-    def __getitem__(self, tag: str) -> widgets.Widget:
-        """
-        Get a widget by tag.
+        self._cfg = {title: {}}
+        self.cfg = self._cfg[title]
 
-        Args:
-            tag (str): The tag of the widget.
+        # Get the user's home folder
+        self._home_folder = os.path.expanduser("~")
+        self._config_folder = os.path.join(self._home_folder, ".nanopyx")
+        if not os.path.exists(self._config_folder):
+            os.makedirs(self._config_folder)
+
+        self._config_file = os.path.join(self._config_folder, "easy_gui.yml")
+        if os.path.exists(self._config_file):
+            with open(self._config_file, "r") as f:
+                self._cfg = yaml.load(f, Loader=yaml.FullLoader)
+                if title in self._cfg:
+                    self.cfg = self._cfg[title]
 
-        Returns:
-            widgets.Widget: The widget.
-        """
+    def __getitem__(self, tag: str) -> widgets.Widget:
         return self._widgets[tag]
 
     def __len__(self) -> int:
-        """
-        Get the number of widgets.
-
-        Returns:
-            int: The number of widgets.
-        """
         return len(self._widgets)
 
     def add_label(self, *args, **kwargs):
         """
         Add a label widget to the container.
-
-        Args:
-            args: Args for the widget.
-            kwargs: Kwargs for the widget.
+        :param args: args for the widget
+        :param kwargs: kwargs for the widget
         """
         self._nLabels += 1
         self._widgets[f"label_{self._nLabels}"] = widgets.Label(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_button(self, tag, *args, **kwargs):
         """
         Add a button widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param kwargs: kwargs for the widget
         """
         self._widgets[tag] = widgets.Button(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
-    def add_text(self, tag, *args, remember_value=False, **kwargs):
+    def add_text(self, tag, *args, **kwargs):
         """
         Add a text widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param kwargs: kwargs for the widget
 
         Example:
-            The following example demonstrates how to add a text widget to the GUI:
-
             >>> gui = EasyGUI()
-            >>> gui.add_text("text", "Enter some text:")
-            >>> gui.show()
+            >>> gui.add_text("text", value="Hello, world!")
         """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = str(self._cfg[tag])
-
         self._widgets[tag] = widgets.Text(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
-    def add_textarea(self, tag, *args, remember_value=False, **kwargs):
-        """
-        Add a textarea widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
-        """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = str(self._cfg[tag])
-        self._widgets[tag] = widgets.Textarea(
-            *args, **kwargs, layout=self._layout, style=self._style
-        )
-
-        self._widgets[tag] = widgets.Textarea(
-            *args, **kwargs, layout=self._layout, style=self._style
-        )
-
     def add_int_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer slider widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
         if (
             remember_value
-            and tag in self._cfg
-            and kwargs["min"] <= self._cfg[tag] <= kwargs["max"]
+            and tag in self.cfg
+            and kwargs["min"] <= self.cfg[tag] <= kwargs["max"]
         ):
-            kwargs["value"] = int(self._cfg[tag])
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.IntSlider(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_float_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float slider widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = self._cfg[tag]
+        if remember_value and tag in self.cfg:
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.FloatSlider(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_checkbox(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a checkbox widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = self._cfg[tag]
+        if remember_value and tag in self.cfg:
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.Checkbox(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_int_text(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer text widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = self._cfg[tag]
+        if remember_value and tag in self.cfg:
+            kwargs["value"] = self.cfg[tag]
 
         self._widgets[tag] = widgets.IntText(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_float_text(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float text widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self._cfg:
-            kwargs["value"] = self._cfg[tag]
+        if remember_value and tag in self.cfg:
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.FloatText(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_dropdown(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a dropdown widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            remember_value (bool): Remember the last value.
-            kwargs: Kwargs for the widget.
-
-        Example:
-            >>> gui = EasyGUI()
-            >>> gui.add_dropdown("dropdown", options=["A", "B", "C"])
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param remember_value: remember the last value
+        :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self._cfg and self._cfg[tag] in kwargs["options"]:
-            kwargs["value"] = self._cfg[tag]
+        if remember_value and tag in self.cfg and self.cfg[tag] in kwargs["options"]:
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.Dropdown(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_file_upload(self, tag, *args, accept=None, multiple=False, **kwargs):
         """
         Add a file upload widget to the container.
-
-        Args:
-            tag (str): The tag to identify the widget.
-            args: Args for the widget.
-            accept: The file types to accept.
-            multiple (bool): Allow multiple files to be uploaded.
-            kwargs: Kwargs for the widget.
+        :param tag: tag to identify the widget
+        :param args: args for the widget
+        :param accept: file types to accept
+        :param multiple: allow multiple files to be uploaded
+        :param kwargs: kwargs for the widget
         """
         self._widgets[tag] = FileChooser()
         if accept is not None:
             self._widgets[tag].filter_pattern = accept
 
     def save_settings(self):
-        """
-        Save the widget values to the configuration file.
-        """
+        # remember widget values for next time and store them in a config file
         for tag in self._widgets:
             if tag.startswith("label_"):
                 pass
             elif hasattr(self._widgets[tag], "value"):
-                self._cfg[tag] = self._widgets[tag].value
-
-        save_config(self._title, self._cfg)
-
-    def restore_default_settings(self):
-        """
-        Restore the default settings and clear the widgets.
-        """
-        save_config(self._title, {})
-        self.clear()
-        self.show()
+                self.cfg[tag] = self._widgets[tag].value
+        self._cfg[self._title] = self.cfg
+        with open(self._config_file, "w") as f:
+            yaml.dump(self._cfg, f)
 
     def show(self):
         """
         Show the widgets in the container.
         """
+        # display the widgets
         self._main_display.children = tuple(self._widgets.values())
         clear_output()
         display(self._main_display)
 
     def clear(self):
         """
         Clear the widgets in the container.
```

### Comparing `easy_gui_jupyter-2024.5.28/pyproject.toml` & `easy_gui_jupyter-2024.5.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = [ "poetry-core",]
-build-backend = "poetry.core.masonry.api"
-
 [tool.poetry]
 name = "easy_gui_jupyter"
-version = "2024.05.28"
+version = "2024.05.08"
 description = "Simplify the creation of GUI elements in Jupyter notebooks"
-license = "MIT"
-repository = "https://github.com/HenriquesLab/easy-gui-jupyter"
-documentation = "https://github.com/HenriquesLab/easy-gui-jupyter/tree/main/docs"
-authors = [ "Ricardo Henriques <ricardo@henriqueslab.org>", "Bruno Saraiva <bruno.msaraiva2@gmail.com>", "António Brito <antmsbrito95@gmail.com>",]
+authors = [    
+    "Ricardo Henriques <ricardo@henriqueslab.org>", 
+    "Bruno Saraiva <bruno.msaraiva2@gmail.com>",
+    "António Brito <antmsbrito95@gmail.com>"
+    ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ipython = "^8.24.0"
 ipywidgets = "^8.1.2"
 ipyfilechooser = "^0.6.0"
 pyyaml = "^6.0.1"
-toml = "^0.10.2"
-
-[tool.pytest.ini_options]
-testpaths = [ "tests",]
-addopts = "--nbmake -n=auto"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 ipykernel = "^6.29.4"
 ruff = "^0.4.3"
-lazydocs = "^0.4.8"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 pytest-xdist = "^3.6.1"
 nbmake = "^1.5.3"
 gptrepo = "^1.0.3"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = "--nbmake -n=auto"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
```

### Comparing `easy_gui_jupyter-2024.5.28/PKG-INFO` & `easy_gui_jupyter-2024.5.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 Metadata-Version: 2.1
 Name: easy_gui_jupyter
-Version: 2024.5.28
+Version: 2024.5.8
 Summary: Simplify the creation of GUI elements in Jupyter notebooks
-Home-page: https://github.com/HenriquesLab/easy-gui-jupyter
-License: MIT
 Author: Ricardo Henriques
 Author-email: ricardo@henriqueslab.org
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipyfilechooser (>=0.6.0,<0.7.0)
 Requires-Dist: ipython (>=8.24.0,<9.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Project-URL: Documentation, https://github.com/HenriquesLab/easy-gui-jupyter/tree/main/docs
-Project-URL: Repository, https://github.com/HenriquesLab/easy-gui-jupyter
 Description-Content-Type: text/markdown
 
 # Easy GUI Jupyter
 
-[![PyPI version](https://badge.fury.io/py/easy_gui_jupyter.svg)](https://badge.fury.io/py/easy_gui_jupyter)
-[![Python versions](https://img.shields.io/pypi/pyversions/easy_gui_jupyter.svg)](https://pypi.org/project/easy_gui_jupyter/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
 Easy GUI Jupyter is a Python library that simplifies the creation of graphical user interfaces (GUIs) in Jupyter notebooks using ipywidgets. It provides a convenient way to add various types of widgets to your Jupyter notebooks, making it easier to interact with your code and visualize results.
 
 ## Features
 
 - Simplifies the creation of GUIs in Jupyter notebooks
 - Supports a variety of widget types, including labels, buttons, text inputs, sliders, checkboxes, and dropdowns
 - Allows saving and loading widget values to maintain user settings across sessions
```

