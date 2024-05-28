# Comparing `tmp/wow-addon-packager-0.8.3.tar.gz` & `tmp/wow-addon-packager-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow-addon-packager-0.8.3.tar", max compression
+gzip compressed data, was "wow-addon-packager-0.9.0.tar", max compression
```

## Comparing `wow-addon-packager-0.8.3.tar` & `wow-addon-packager-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1067 2021-03-22 18:24:55.944409 wow-addon-packager-0.8.3/LICENSE
--rw-r--r--   0        0        0     4849 2021-03-22 18:24:55.944409 wow-addon-packager-0.8.3/README.rst
--rw-r--r--   0        0        0     1327 2021-03-22 18:24:55.948409 wow-addon-packager-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       22 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/__init__.py
--rw-r--r--   0        0        0     1110 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/__main__.py
--rw-r--r--   0        0        0     6554 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/addon.py
--rw-r--r--   0        0        0     1702 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/changelog.py
--rw-r--r--   0        0        0       56 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/__init__.py
--rw-r--r--   0        0        0      877 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/base.py
--rw-r--r--   0        0        0     4342 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/common.py
--rw-r--r--   0        0        0     2790 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/dev_install.py
--rw-r--r--   0        0        0     1470 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/new_config.py
--rw-r--r--   0        0        0     3143 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/package.py
--rw-r--r--   0        0        0     5860 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/quickstart.py
--rw-r--r--   0        0        0     5207 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/upload.py
--rw-r--r--   0        0        0     1020 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/validate.py
--rw-r--r--   0        0        0     2047 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/commands/watch.py
--rw-r--r--   0        0        0    10600 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/config.py
--rw-r--r--   0        0        0     4485 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/curseforge.py
--rw-r--r--   0        0        0     1407 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/exception.py
--rw-r--r--   0        0        0     3991 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/guided_config.py
--rw-r--r--   0        0        0     1664 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/log.py
--rw-r--r--   0        0        0     4067 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/toc.py
--rw-r--r--   0        0        0     1431 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/util.py
--rw-r--r--   0        0        0     2365 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/watcher.py
--rw-r--r--   0        0        0     1741 2021-03-22 18:24:55.952409 wow-addon-packager-0.8.3/wap/wowversion.py
--rw-r--r--   0        0        0     5947 2021-03-22 18:25:13.711122 wow-addon-packager-0.8.3/setup.py
--rw-r--r--   0        0        0     5711 2021-03-22 18:25:13.711678 wow-addon-packager-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-06-02 20:52:00.088383 wow-addon-packager-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4849 2021-06-02 20:52:00.088383 wow-addon-packager-0.9.0/README.rst
+-rw-r--r--   0        0        0     1327 2021-06-02 20:52:00.092383 wow-addon-packager-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/__init__.py
+-rw-r--r--   0        0        0     1110 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/__main__.py
+-rw-r--r--   0        0        0     6554 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/addon.py
+-rw-r--r--   0        0        0     1973 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/changelog.py
+-rw-r--r--   0        0        0       56 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/__init__.py
+-rw-r--r--   0        0        0      877 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/base.py
+-rw-r--r--   0        0        0     4326 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/common.py
+-rw-r--r--   0        0        0     2790 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/dev_install.py
+-rw-r--r--   0        0        0     1470 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/new_config.py
+-rw-r--r--   0        0        0     3143 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/package.py
+-rw-r--r--   0        0        0     5914 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/quickstart.py
+-rw-r--r--   0        0        0     5207 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/upload.py
+-rw-r--r--   0        0        0     1020 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/validate.py
+-rw-r--r--   0        0        0     2047 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/commands/watch.py
+-rw-r--r--   0        0        0    10842 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/config.py
+-rw-r--r--   0        0        0     4485 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/curseforge.py
+-rw-r--r--   0        0        0     1407 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/exception.py
+-rw-r--r--   0        0        0     3991 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/guided_config.py
+-rw-r--r--   0        0        0     1664 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/log.py
+-rw-r--r--   0        0        0     4085 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/toc.py
+-rw-r--r--   0        0        0     1431 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/util.py
+-rw-r--r--   0        0        0     2365 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/watcher.py
+-rw-r--r--   0        0        0     1741 2021-06-02 20:52:00.096384 wow-addon-packager-0.9.0/wap/wowversion.py
+-rw-r--r--   0        0        0     5947 2021-06-02 20:52:16.703404 wow-addon-packager-0.9.0/setup.py
+-rw-r--r--   0        0        0     5711 2021-06-02 20:52:16.703957 wow-addon-packager-0.9.0/PKG-INFO
```

### Comparing `wow-addon-packager-0.8.3/LICENSE` & `wow-addon-packager-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/README.rst` & `wow-addon-packager-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/pyproject.toml` & `wow-addon-packager-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wow-addon-packager"
-version = "0.8.3"
+version = "0.9.0"
 description = "A developer-friendly World of Warcraft addon packager"
 license = "MIT"
 authors = ["Tim Martin <tim@timmart.in>"]
 readme = "README.rst"
 homepage = "https://github.com/t-mart/wap"
 repository = "https://github.com/t-mart/wap"
 documentation = "https://wow-addon-packager.readthedocs.io/en/stable/"
```

### Comparing `wow-addon-packager-0.8.3/wap/__main__.py` & `wow-addon-packager-0.9.0/wap/__main__.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/addon.py` & `wow-addon-packager-0.9.0/wap/addon.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/changelog.py` & `wow-addon-packager-0.9.0/wap/changelog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import attr
 
 from wap import log
+from wap.exception import ChangelogException
 
 CHANGELOG_SUFFIX_MAP = {
     ".md": "markdown",
     ".markdown": "markdown",
     ".html": "html",
     ".txt": "text",
 }
@@ -44,14 +45,19 @@
         else:
             log.warn(
                 f"Unable to determine changelog type from extension for {path}, "
                 'so assuming "text"'
             )
             type = "text"
 
-        with path.open("r") as file:
-            contents = file.read()
+        with path.open("r", encoding="utf-8") as file:
+            try:
+                contents = file.read()
+            except UnicodeDecodeError as ude:
+                raise ChangelogException(
+                    f'Changelog file "{path}" cannot be decoded to utf-8: {ude}'
+                )
 
         return cls(
             type=type,
             contents=contents,
         )
```

### Comparing `wow-addon-packager-0.8.3/wap/commands/base.py` & `wow-addon-packager-0.9.0/wap/commands/base.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/common.py` & `wow-addon-packager-0.9.0/wap/commands/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 WAP_CURSEFORGE_TOKEN_ENVVAR_NAME = "WAP_CURSEFORGE_TOKEN"
 WAP_CONFIG_PATH_ENVVAR_NAME = "WAP_CONFIG_PATH"
 WAP_WOW_ADDONS_PATH_ENVVAR_NAME = "WAP_WOW_ADDONS_PATH"
 
 _DECORATED_FUNC_TYPE = TypeVar("_DECORATED_FUNC_TYPE", bound=Callable[..., Any])
 
 
-def config_path_option() -> Callable[[_DECORATED_FUNC_TYPE], _DECORATED_FUNC_TYPE]:
-    def wrapper(func: _DECORATED_FUNC_TYPE) -> _DECORATED_FUNC_TYPE:
+def config_path_option() -> Callable[[_DECORATED_FUNC_TYPE], Callable[..., Any]]:
+    def wrapper(func: _DECORATED_FUNC_TYPE) -> Callable[..., Any]:
         decorated = click.option(
             "-c",
             "--config-path",
             type=PATH_TYPE,
             default=str(DEFAULT_CONFIG_PATH),
             envvar=WAP_CONFIG_PATH_ENVVAR_NAME,
             show_default=str(DEFAULT_CONFIG_PATH),
@@ -54,16 +54,16 @@
         return update_wrapper(decorated, func)
 
     return wrapper
 
 
 def version_option(
     *, help: str, required: bool = False
-) -> Callable[[_DECORATED_FUNC_TYPE], _DECORATED_FUNC_TYPE]:
-    def wrapper(func: _DECORATED_FUNC_TYPE) -> _DECORATED_FUNC_TYPE:
+) -> Callable[[_DECORATED_FUNC_TYPE], Callable[..., Any]]:
+    def wrapper(func: _DECORATED_FUNC_TYPE) -> Callable[..., Any]:
         decorated = click.option(
             "-v",
             "--version",
             required=required,
             default=None if required else DEFAULT_PROJECT_VERSION,
             show_default=not required,
             help=help,
@@ -72,38 +72,38 @@
         return update_wrapper(decorated, func)
 
     return wrapper
 
 
 def json_option(
     *, help: Optional[str] = None
-) -> Callable[[_DECORATED_FUNC_TYPE], _DECORATED_FUNC_TYPE]:
+) -> Callable[[_DECORATED_FUNC_TYPE], Callable[..., Any]]:
     if help is None:
         help = (
             "Output json to stdout of the operations wap performed (so it can be "
             "written to files or piped to other programs)"
         )
 
-    def wrapper(func: _DECORATED_FUNC_TYPE) -> _DECORATED_FUNC_TYPE:
+    def wrapper(func: _DECORATED_FUNC_TYPE) -> Callable[..., Any]:
         decorated = click.option(
             "-j",
             "--json",
             "show_json",
             is_flag=True,
             default=False,
             help=help,
         )(func)
 
         return update_wrapper(decorated, func)
 
     return wrapper
 
 
-def wow_addons_path_option() -> Callable[[_DECORATED_FUNC_TYPE], _DECORATED_FUNC_TYPE]:
-    def wrapper(func: _DECORATED_FUNC_TYPE) -> _DECORATED_FUNC_TYPE:
+def wow_addons_path_option() -> Callable[[_DECORATED_FUNC_TYPE], Callable[..., Any]]:
+    def wrapper(func: _DECORATED_FUNC_TYPE) -> Callable[..., Any]:
         decorated = click.option(
             "-w",
             "--wow-addons-path",
             envvar=WAP_WOW_ADDONS_PATH_ENVVAR_NAME,
             required=True,
             type=WOW_ADDONS_PATH_TYPE,
             help=(
```

### Comparing `wow-addon-packager-0.8.3/wap/commands/dev_install.py` & `wow-addon-packager-0.9.0/wap/commands/dev_install.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/new_config.py` & `wow-addon-packager-0.9.0/wap/commands/new_config.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/package.py` & `wow-addon-packager-0.9.0/wap/commands/package.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/quickstart.py` & `wow-addon-packager-0.9.0/wap/commands/quickstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from wap.util import default_wow_addons_path_for_system
 from wap.wowversion import WoWVersion
 
 LATEST_RETAIL_VERSION = WoWVersion.from_dot_version("9.0.2")
 
 
 def write_changelog(path: Path, name: str) -> None:
-    with path.open("w") as changelog_file:
+    with path.open("w", encoding="utf-8") as changelog_file:
         changelog_file.write(f"# {name} Changelog\n\n")
         changelog_file.write(
             "This file is used by *wap* when you upload to Curseforge. It should "
             "contain a record of changes over time to your project.\n\n"
         )
         changelog_file.write("## Example Version 0.0.1\n\n")
         changelog_file.write("- Added feature X\n")
         changelog_file.write("- Fixed bug Y\n")
 
 
 def write_readme(path: Path, name: str) -> None:
-    with path.open("w") as readme_file:
+    with path.open("w", encoding="utf-8") as readme_file:
         readme_file.write(f"# {name}\n\n")
         readme_file.write(
             "(This file is not required to run *wap*. It is here as a suggestion to "
             "document your project.)\n\n"
         )
         readme_file.write(
             'This file is written in Markdown, "a lightweight and easy-to-use syntax '
@@ -47,15 +47,15 @@
         readme_file.write("- Boosts your DPS!\n")
         readme_file.write(
             "- Did someone say Thunderfury, Blessed Blade of the Windseeker?\n"
         )
 
 
 def write_lua_file(path: Path, name: str) -> None:
-    with path.open("w") as lua_file:
+    with path.open("w", encoding="utf-8") as lua_file:
         lua_file.write("-- Your code can go here.\n")
         lua_file.write("-- Here's something to get you started,\n")
         lua_file.write("-- but you can erase it if you wish.\n\n")
         lua_file.write(f'local title = GetAddOnMetadata("{name}", "Title")\n')
         lua_file.write(f'local version = GetAddOnMetadata("{name}", "Version")\n')
         lua_file.write('print(title .. " version " .. version .. " has loaded.")\n')
```

### Comparing `wow-addon-packager-0.8.3/wap/commands/upload.py` & `wow-addon-packager-0.9.0/wap/commands/upload.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/validate.py` & `wow-addon-packager-0.9.0/wap/commands/validate.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/commands/watch.py` & `wow-addon-packager-0.9.0/wap/commands/watch.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/config.py` & `wow-addon-packager-0.9.0/wap/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,20 @@
         return obj
 
     @classmethod
     def from_path(cls, path: Path) -> Config:
         if not path.is_file():
             raise ConfigFileException(f'No such config file "{path}"')
 
-        with path.open("r") as file:
-            contents = file.read()
+        with path.open("r", encoding="utf-8") as file:
+            try:
+                contents = file.read()
+            except UnicodeDecodeError as ude:
+                raise ConfigFileException(
+                    f'Config file "{path}" cannot be decoded to utf-8: {ude}'
+                )
 
         return cls.from_yaml(yaml=contents, label=str(path))
 
     def to_path(self, path: Path) -> None:
-        with path.open("w") as file:
+        with path.open("w", encoding="utf-8") as file:
             file.write(self.to_yaml())
```

### Comparing `wow-addon-packager-0.8.3/wap/curseforge.py` & `wow-addon-packager-0.9.0/wap/curseforge.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/exception.py` & `wow-addon-packager-0.9.0/wap/exception.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/guided_config.py` & `wow-addon-packager-0.9.0/wap/guided_config.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/log.py` & `wow-addon-packager-0.9.0/wap/log.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/toc.py` & `wow-addon-packager-0.9.0/wap/toc.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,10 +131,10 @@
 
     lines = [
         *[_create_tag_line(tag, value) for tag, value in tag_map.items()],
         "\n",
         *[_create_file_line(file) for file in toc_config.files],
     ]
 
-    with write_path.open("w") as toc_file:
+    with write_path.open("w", encoding="utf-8") as toc_file:
         for line in lines:
             toc_file.write(line)
```

### Comparing `wow-addon-packager-0.8.3/wap/util.py` & `wow-addon-packager-0.9.0/wap/util.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/watcher.py` & `wow-addon-packager-0.9.0/wap/watcher.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/wap/wowversion.py` & `wow-addon-packager-0.9.0/wap/wowversion.py`

 * *Files identical despite different names*

### Comparing `wow-addon-packager-0.8.3/setup.py` & `wow-addon-packager-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'strictyaml>=1.3.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['wap = wap.__main__:main']}
 
 setup_kwargs = {
     'name': 'wow-addon-packager',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'A developer-friendly World of Warcraft addon packager',
     'long_description': 'wap (WoW Addon Packager)\n========================\n\n.. teaser-begin\n\n.. image:: https://github.com/t-mart/wap/actions/workflows/ci.yml/badge.svg?branch=master\n   :target: https://github.com/t-mart/wap/actions/workflows/ci.yml\n   :alt: GitHub Actions status for master branch\n\n.. image:: https://codecov.io/gh/t-mart/wap/branch/master/graph/badge.svg?token=AVOA4QWTBL\n   :target: https://codecov.io/gh/t-mart/wap\n   :alt: Code Coverage on codecov.io\n\n.. image:: https://img.shields.io/pypi/v/wow-addon-packager\n   :target: https://pypi.org/project/wow-addon-packager/\n   :alt: Latest release on PyPI\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Code styled with black\n\n.. image:: https://img.shields.io/github/license/t-mart/wap\n   :target: https://github.com/t-mart/wap/blob/master/LICENSE\n   :alt: MIT licensed\n\n.. image:: https://readthedocs.org/projects/wow-addon-packager/badge/?version=latest\n   :target: https://wow-addon-packager.readthedocs.io/en/latest\n   :alt: Documentation Status\n\n|\n\n``wap`` is a developer-friendly World of Warcraft addon packager.\n\n.. image:: https://raw.githubusercontent.com/t-mart/wap/master/docs/_static/images/demo.gif\n   :alt: wap demo\n\nFeatures\n--------\n\n- Packages retail or classic WoW addons (or both!)\n- Uploads your addons to CurseForge\n- Automatically installs your addons to your AddOns folder when a file changes in your project\n- Generates valid TOC files automagically\n- Sets up new addon projects quickly, ready to go with one command\n- Consolidates all configuration in one easy-to-edit file\n- Supports and is tested on Windows, macOS, and Linux\n- Has awesome `documentation`_\n\n.. _`documentation`: https://wow-addon-packager.readthedocs.io/en/stable\n\n.. teaser-end\n\n\n``wap`` in 5 minutes\n--------------------\n\n.. five-minutes-begin\n\nThis entire set of instructions is runnable without editing a single line of code!\n\n1. `Download Python 3.9 or greater`_ and install it.\n\n2. Install ``wap`` with pip:\n\n   .. code-block:: console\n\n      $ pip install --upgrade --user wow-addon-packager\n\n3. Create a new project:\n\n   .. code-block:: console\n\n      $ wap quickstart MyAddon  # or whatever name you\'d like!\n\n   and answer the prompted questions. Don\'t worry too much about your answers -- you can\n   always change them later in your configuration file.\n\n   Then change to your new project\'s directory\n\n   .. code-block:: console\n\n      $ cd "MyAddon"\n\n4. Package your addon\n\n   .. code-block:: console\n\n      $ wap package\n\n5. Install your addon so you can test it out in your local WoW installation:\n\n   Windows\n      .. code-block:: console\n\n         $ wap dev-install --wow-addons-path "C:\\Program Files (x86)\\World of Warcraft\\_retail_\\Interface\\AddOns"\n\n   macOS\n      .. code-block:: console\n\n         $ wap dev-install --wow-addons-path "/Applications/World of Warcraft/_retail_/Interface/AddOns"\n\n   .. note::\n\n      Also check out the ``watch`` command for automatic repackage and re-dev-installation!\n\n6. Upload your project to CurseForge\n\n   .. code-block:: console\n\n      $ wap upload --addon-version "dev" --curseforge-token "<your-token>"\n\n   You can generate a new token at Curseforge\'s `My API Tokens`_ page.\n\n.. _`My API Tokens`: https://authors.curseforge.com/account/api-tokens\n.. _`Download Python 3.9 or greater`: https://www.python.org/downloads/\n\n.. five-minutes-end\n\n\nFurther Help\n------------\n\nSee the `official documentation site`_. There\'s a lot more information there!\n\nAlso, the ``wap`` command is fully documented in its help text. View it with:\n\n.. code-block:: console\n\n   $ wap --help\n   $ wap build --help\n   $ wap upload --help\n   ... etc\n\n.. badge-begin\n\nBadge\n-----\n\nIf you\'d like to show others in your documentation that you are using ``wap`` to package\nyour addon, you can include the following official badge (hosted by https://shields.io/):\n\n.. image:: https://img.shields.io/badge/packaged%20by-wap-d33682\n   :target: https://github.com/t-mart/wap\n   :alt: Packaged by wap\n\nMarkdown\n   .. code-block:: markdown\n\n      [![Packaged by wap](https://img.shields.io/badge/packaged%20by-wap-d33682)](https://github.com/t-mart/wap)\n\nreStructuredText\n   .. code-block:: rst\n\n      .. image:: https://img.shields.io/badge/packaged%20by-wap-d33682\n         :target: https://github.com/t-mart/wap\n         :alt: Packaged by wap\n\n.. badge-end\n\nContributing\n------------\n\nSee `how to contribute`_ in the official docs.\n\nTODOs\n-----\n\n- localization via curseforge?\n- Dockerfile github action `<https://docs.github.com/en/actions/creating-actions/creating-a-docker-container-action>`_\n\n.. _`how to contribute`: https://wow-addon-packager.readthedocs.io/en/stable/contributing.html\n.. _`official documentation site`: https://wow-addon-packager.readthedocs.io/en/stable\n\nCopyright (c) 2021 Tim Martin\n',
     'author': 'Tim Martin',
     'author_email': 'tim@timmart.in',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/t-mart/wap',
```

### Comparing `wow-addon-packager-0.8.3/PKG-INFO` & `wow-addon-packager-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-addon-packager
-Version: 0.8.3
+Version: 0.9.0
 Summary: A developer-friendly World of Warcraft addon packager
 Home-page: https://github.com/t-mart/wap
 License: MIT
 Keywords: World of Warcraft,WoW,Addons
 Author: Tim Martin
 Author-email: tim@timmart.in
 Requires-Python: >=3.9,<4.0
```

