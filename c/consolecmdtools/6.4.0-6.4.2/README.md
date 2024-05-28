# Comparing `tmp/consolecmdtools-6.4.0.tar.gz` & `tmp/consolecmdtools-6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolecmdtools-6.4.0.tar", last modified: Thu Feb 29 08:48:51 2024, max compression
+gzip compressed data, was "consolecmdtools-6.4.2.tar", last modified: Tue May 28 15:05:21 2024, max compression
```

## Comparing `consolecmdtools-6.4.0.tar` & `consolecmdtools-6.4.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-02-29 08:48:51.649518 consolecmdtools-6.4.0/
--rw-r--r--   0 kyan001    (501) staff       (20)     1061 2023-11-19 07:47:06.000000 consolecmdtools-6.4.0/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)    10718 2024-02-29 08:48:51.649275 consolecmdtools-6.4.0/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)     8458 2024-02-27 12:54:26.000000 consolecmdtools-6.4.0/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-02-29 08:48:51.647162 consolecmdtools-6.4.0/consolecmdtools/
--rw-r--r--   0 kyan001    (501) staff       (20)    24323 2024-02-29 08:47:13.000000 consolecmdtools-6.4.0/consolecmdtools/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2394 2024-02-25 13:49:33.000000 consolecmdtools-6.4.0/consolecmdtools/__main__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2743 2024-02-29 08:46:41.000000 consolecmdtools-6.4.0/consolecmdtools/path.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-02-29 08:48:51.648814 consolecmdtools-6.4.0/consolecmdtools.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)    10718 2024-02-29 08:48:51.000000 consolecmdtools-6.4.0/consolecmdtools.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      356 2024-02-29 08:48:51.000000 consolecmdtools-6.4.0/consolecmdtools.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-02-29 08:48:51.000000 consolecmdtools-6.4.0/consolecmdtools.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       60 2024-02-29 08:48:51.000000 consolecmdtools-6.4.0/consolecmdtools.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       21 2024-02-29 08:48:51.000000 consolecmdtools-6.4.0/consolecmdtools.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1222 2023-11-19 07:47:06.000000 consolecmdtools-6.4.0/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-02-29 08:48:51.649558 consolecmdtools-6.4.0/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-02-29 08:48:51.648563 consolecmdtools-6.4.0/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)    18409 2024-02-29 08:48:07.000000 consolecmdtools-6.4.0/tests/test_consolecmdtools.py
--rw-r--r--   0 kyan001    (501) staff       (20)      363 2023-11-19 07:47:06.000000 consolecmdtools-6.4.0/tests/test_runas.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:05:21.640058 consolecmdtools-6.4.2/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1061 2023-11-19 07:47:06.000000 consolecmdtools-6.4.2/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)    10863 2024-05-28 15:05:21.639798 consolecmdtools-6.4.2/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     8609 2024-02-29 08:50:15.000000 consolecmdtools-6.4.2/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:05:21.637828 consolecmdtools-6.4.2/consolecmdtools/
+-rw-r--r--   0 kyan001    (501) staff       (20)    24571 2024-05-28 14:44:47.000000 consolecmdtools-6.4.2/consolecmdtools/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2394 2024-02-25 13:49:33.000000 consolecmdtools-6.4.2/consolecmdtools/__main__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2743 2024-02-29 08:46:41.000000 consolecmdtools-6.4.2/consolecmdtools/path.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:05:21.639335 consolecmdtools-6.4.2/consolecmdtools.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)    10863 2024-05-28 15:05:21.000000 consolecmdtools-6.4.2/consolecmdtools.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      415 2024-05-28 15:05:21.000000 consolecmdtools-6.4.2/consolecmdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-05-28 15:05:21.000000 consolecmdtools-6.4.2/consolecmdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       54 2024-05-28 15:05:21.000000 consolecmdtools-6.4.2/consolecmdtools.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       21 2024-05-28 15:05:21.000000 consolecmdtools-6.4.2/consolecmdtools.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1291 2024-03-05 09:22:12.000000 consolecmdtools-6.4.2/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)       18 2024-03-05 09:22:12.000000 consolecmdtools-6.4.2/requirements-dev.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        7 2024-03-05 09:22:12.000000 consolecmdtools-6.4.2/requirements-opt.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       15 2024-03-05 09:22:12.000000 consolecmdtools-6.4.2/requirements.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-05-28 15:05:21.640108 consolecmdtools-6.4.2/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:05:21.639042 consolecmdtools-6.4.2/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)    18409 2024-05-28 14:45:09.000000 consolecmdtools-6.4.2/tests/test_consolecmdtools.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      363 2023-11-19 07:47:06.000000 consolecmdtools-6.4.2/tests/test_runas.py
```

### Comparing `consolecmdtools-6.4.0/LICENSE` & `consolecmdtools-6.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `consolecmdtools-6.4.0/PKG-INFO` & `consolecmdtools-6.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 6.4.0
+Version: 6.4.2
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,16 +39,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: consoleiotools
 Provides-Extra: opt
 Requires-Dist: pillow; extra == "opt"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: pycodestyle; extra == "dev"
 
 # PyConsoleCMDTools
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
 ![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
 [![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
 
 ## Installation
@@ -173,14 +173,20 @@
 './file.txt'
 
 >>> cct.get_path("./file.txt").abs  # Get the absolute path. Same as `get_path("./file.txt")` itself.
 
 >>> cct.get_path("./file.txt").exists  # Test if the path exists.
 True
 
+>>> cct.get_path("./file.txt").is_file  # Test if the path is a file.
+True
+
+>>> cct.get_path("./file.txt").is_dir  # Test if the path is a dir.
+False
+
 >>> cct.get_path("/path/to/file.txt").basename  # Get the basename of the file or dir.
 'file.txt'
 
 >>> cct.get_path("/path/to/file.txt").ext  # Get the extension of the path. If the path is a dir, return ''.
 'txt'
 
 >>> cct.get_path("/path/to/file.txt").stem  # Get the name of the path without extension. If the path is a dir, return its basename.
```

### Comparing `consolecmdtools-6.4.0/README.md` & `consolecmdtools-6.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -125,14 +125,20 @@
 './file.txt'
 
 >>> cct.get_path("./file.txt").abs  # Get the absolute path. Same as `get_path("./file.txt")` itself.
 
 >>> cct.get_path("./file.txt").exists  # Test if the path exists.
 True
 
+>>> cct.get_path("./file.txt").is_file  # Test if the path is a file.
+True
+
+>>> cct.get_path("./file.txt").is_dir  # Test if the path is a dir.
+False
+
 >>> cct.get_path("/path/to/file.txt").basename  # Get the basename of the file or dir.
 'file.txt'
 
 >>> cct.get_path("/path/to/file.txt").ext  # Get the extension of the path. If the path is a dir, return ''.
 'txt'
 
 >>> cct.get_path("/path/to/file.txt").stem  # Get the name of the path without extension. If the path is a dir, return its basename.
```

### Comparing `consolecmdtools-6.4.0/consolecmdtools/__init__.py` & `consolecmdtools-6.4.2/consolecmdtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 # -*- coding: utf-8 -*-
 import os
 import sys
 import platform
 import urllib.request
+import urllib.parse
 import json
 import io
 import pathlib
 import typing
 # !! some imports are lazy-loaded
 
 import consoleiotools as cit
 
 from .path import Path
 
 
-__version__ = '6.4.0'
+__version__ = '6.4.2'
 
 
 def banner(text: str) -> str:
     """Generate a banner of 3 lines"""
     FILLER = "#"
     text = text.strip()
     middle_line = FILLER + text.center(int(len(text) / 0.618)) + FILLER
     top_line = bottom_line = FILLER * len(middle_line)
     return "\n".join([top_line, middle_line, bottom_line])
 
 
-def md5(target: any, force_text: bool = False) -> str:
+def md5(target: str | bytes, force_text: bool = False) -> str:
     """Generate MD5 hash for bytes, str, int, file, etc."""
     import hashlib
 
     if not target:
-        return None
+        return ""
     if not force_text and os.path.isfile(target):  # if target is a file
         with open(target, 'rb') as f:
             content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
             return hashlib.md5(content).hexdigest()
     if not isinstance(target, bytes):  # the input of hashlib.md5() should be type of bytes
         target = str(target).encode()
     return hashlib.md5(target).hexdigest()
 
 
-def crc32(target: any, force_text: bool = False) -> int:
+def crc32(target: str | bytes, force_text: bool = False) -> int:
     """Generate CRC32 hash for bytes, str, int, file, etc."""
     import binascii
 
     if not target:
         return 0
     if not force_text and os.path.isfile(target):  # if target is a file
         with open(target, 'rb') as f:
             content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
             return binascii.crc32(content)
     if not isinstance(target, bytes):  # if target is str/int/float, the input of binascii.crc32() should be type of bytes
         target = str(target).encode()
     return binascii.crc32(target)
 
 
-def main_color(source: str, scale: int = 200, triplet: str = "rgb", is_url: bool = False) -> str:
+def main_color(source: str, scale: int = 200, triplet: str = "rgb", is_url: bool = False) -> str | tuple[int, int, int] | None:
     """Get a representative color from the source-pointed image
 
     Imports:
         colorsys: Shipped with python.
         PIL: Use `pip install pillow` or install by package manager (apt, apk, etc).
 
     Args:
@@ -82,24 +83,24 @@
         return None
     if is_url:
         img_buffer = io.BytesIO(read_url(source))
         img = Image.open(img_buffer).convert("RGBA")
     else:  # source is an image file
         img = Image.open(source).convert("RGBA")
     img.thumbnail((scale, scale))
-    statistics = {
+    statistics: dict = {
         "r": 0,
         "g": 0,
         "b": 0,
         "coef": 0
     }
     for count, (r, g, b, a) in img.getcolors(img.size[0] * img.size[1]):  # get each color used in image with its count, maxcolors = the size of the image.
         _h, s, _v = colorsys.rgb_to_hsv(r / 255, g / 255, b / 255)
         saturation = s * 255  # extend the range from 0~1 to 0~255
-        coefficient = (saturation * count * a) or 0.01  # get how important this color is. Should not be 0.
+        coefficient: float = (saturation * count * a) or 0.01  # get how important this color is. Should not be 0.
         statistics["r"] += coefficient * r  # raise the importance of red of this image.
         statistics["g"] += coefficient * g
         statistics["b"] += coefficient * b
         statistics["coef"] += coefficient
     color = (
         int(statistics["r"] / statistics["coef"]),  # normalize to 0~255
         int(statistics["g"] / statistics["coef"]),
@@ -181,51 +182,51 @@
     else:  # Linux, Unix, macOS
         proc = os.popen("command -v {}".format(cmd))
         result = proc.read()
         proc.close()
         return (result != "")
 
 
-def install_package(name: typing.Union[str, dict], manager: typing.Union[str, dict] = {"Windows": "scoop", "Linux": "apt", "Darwin": "brew", "*": "pip3"}) -> bool:
+def install_package(name: str | dict, manager: str | dict = {"Windows": "scoop", "Linux": "apt", "Darwin": "brew", "*": "pip3"}) -> bool:
     """Install package using package manager
 
     Args:
         package (str|dict): The package name or a dict of package names for different platforms. If this is a dict, the key should be the platform name from `platform.system()` or `*` for default, and the value should be the package name.
         manager (str|dict): The package manager or a dict of package managers for different platforms. If is a dict, the key should be the platform name from `platform.system()` or `*` for default, and the value should be the package manager name. Defaults to `{"Windows": "scoop", "Linux": "apt", "Darwin": "brew", "*": "pip3"}`.
 
     Returns:
         bool: Does this command run successfully
     """
-    def extract_package_info(data: typing.Union[str, dict], title: str) -> str:
+    def extract_package_info(data: str | dict, title: str) -> str | None:
         """Extract package info from input data
 
         Args:
             data (str|dict): The package data or a dict of package datas for different platforms.
             title (str): The title of the data, such as "package name" or "package manager".
 
         Returns:
-            str: The package name or package manager name.
+            str or None: The package name or package manager name. Return None if no package name found.
         """
         if isinstance(data, dict):
             result = data.get(platform.system())
             if result:
                 return result
             cit.warn(f"No {title} found for {platform.system()}")
             result = data.get("*")
             if result:
                 cit.warn(f"Using default {title}: {result}")
                 return result
             cit.err(f"No default {title} found!")
             cit.info(f"Supported {title} platforms: {data.keys()}")
-            return False
+            return None
         elif isinstance(data, str):
             return data
         else:
             cit.err(f"Unsupported type of {title} data: {type(data)}")
-            return False
+            return None
 
     # check inputs
     if not name:
         cit.err("No package name provided!")
         return False
     cit.info(f"Platform: {platform.system()}")
     manager_name = extract_package_info(manager, "package manager")
@@ -267,15 +268,16 @@
             "commandline": "pip3 install --user {}",
         },
         "npm": {  # npm (Node.js)
             "command": "npm",
             "commandline": "npm install -g {}",
         },
     }
-    current_manager = available_managers.get(manager_name)
+    if manager_name:
+        current_manager = available_managers.get(manager_name)
     if not current_manager:
         cit.err(f"Unsupported package manager: {manager_name}!")
         return False
     if not is_cmd_exist(current_manager["command"]):
         cit.err(f"{manager_name} is not installed!")
         return False
     return run_cmd(current_manager["commandline"].format(package_name))
@@ -333,15 +335,15 @@
     while queue:
         path = queue.pop(0)
         yield path
         if path.is_dir():  # path included `~` returns False
             queue = [p for p in path.iterdir()] + queue  # insert into the front of the queue
 
 
-def get_paths(root: str, filter: callable = None) -> list:
+def get_paths(root: str, filter: typing.Callable | None = None) -> list:
     """List folders and files under `root` folder with filter.
 
     Args:
         root (str): root folder to list.
         filter (callable): a function to indicate if the folder or file should be returned. Defaults to return every path. `filter(path: str) -> bool`.
 
     Returns:
@@ -351,20 +353,19 @@
     for path in bfs_walk(root):
         if (not filter) or filter(path):
             paths.append(str(path))
     return paths
 
 
 @cit.deprecated_by(get_paths)
-def get_files(root: str, filter: callable = None) -> list:
+def get_files(root: str, filter: typing.Callable | None = None):
     pass
 
 
-
-def ls_tree(root: str, show_icon: bool = True, ascii: bool = False, to_visible: callable = lambda path: True, to_highlight: callable = lambda path: False, add_suffix: callable = None):
+def ls_tree(root: str, show_icon: bool = True, ascii: bool = False, to_visible: typing.Callable | None = lambda path: True, to_highlight: typing.Callable | None = lambda path: False, add_suffix: typing.Callable | None = None):
     """Print folders and files under `root` folder in tree structure.
 
     Args:
         root (str): root folder to list.
         show_icon (bool): show icon for folders and files. Defaults to True.
         ascii (bool): use ascii characters for tree structure. Defaults to False.
         to_visible (callable): a function to indicate if the folder or file should be visible. Default to show every path. `to_visible(path: str) -> bool`.
@@ -380,38 +381,37 @@
             return True
         if path.is_dir():
             for child_path in path.iterdir():  # only direct folders and files in path
                 if is_visible(child_path):
                     return True
         return False
 
+    cit_ascii, cit.__ascii__  = cit.__ascii__, ascii
     for path in bfs_walk(root):
         # construct text
         path_text = path.name
         # add prefix
-        depth = len(path.relative_to(root).parts)
+        level = len(path.relative_to(root).parts)
         icon = " " if not show_icon else ("📁" if path.is_dir() else "📄")
-        indent_char = f"[dim]{'|' if ascii else '│'}[/]   "
-        dash_char = f"{'|--' if ascii else '├──'}{icon}"
-        prefix = (indent_char * (depth - 1) + dash_char) if depth > 0 else "📂"  # add tree branchs characters
         # add suffix
         suffix = add_suffix(path) if add_suffix else ""
         # style hightlights
         if to_highlight and to_highlight(path):  # highlight the path if needed
             path_text = f"[u]{path_text}[/]"
         # style hiddens
         if path.name.startswith("."):  # dim hidden files and folders
             path_text = f"[dim]{path_text}[/]"
         # style dirs
         path_text = f"{path_text}{os.sep if path.is_dir() else ''}"  # add "/" or "\" to the end of the folder name
         # assemble
-        full_text = f"{prefix} {path_text} {suffix}"
+        full_text = f"{icon} {path_text} {suffix}"
         # print
         if is_visible(path):  # check if the path is visible, or the path include visible files or folders
-            cit.print(full_text)
+            cit.echo(full_text, indent=level, bar="")
+    cit.__ascii__ = cit_ascii
 
 
 def show_in_file_manager(path: str, ask: bool = False):
     """Show file in Explorer/Finder/File Manager."""
     import subprocess
     import platform
     if ask:
@@ -478,14 +478,17 @@
     def compare(s1, s2):
         return s1 == s2, len(s2) - len(s1)
 
     if not url or not filename:
         return False
     try:
         raw_codes = read_url(url)
+        if not raw_codes:
+            cit.err("Failed to get remote file content.")
+            return False
         with open(filename, "rb") as f:
             current_codes = f.read().replace(b"\r", b"")
         is_same, diff = compare(current_codes, raw_codes)
         if is_same:
             cit.info("{} is already up-to-date.".format(filename))
             return False
         else:
@@ -525,15 +528,15 @@
     Args:
         source (str|Request): The target url.
 
     Returns:
         bytes: The content of the request's response.
     """
     response = urllib.request.urlopen(source)
-    return response.read() if response else None
+    return response.read() if response else b""
 
 
 def copy_file(*args, **kwargs) -> str:
     """Copy file from one place to another.
 
     Args:
         *args, **kwargs: All the arguments and keyword arguments will be passed to `move_file` function, except `copy` is set to `True`. Copying when moving is logical, moving when copying is not.
@@ -541,15 +544,15 @@
     Returns:
         Returns whatever `move_file` returns.
     """
     kwargs['copy'] = True  # Override the `copy` argument to `True`
     return move_file(*args, **kwargs)
 
 
-def move_file(src: str, dst: str, copy: bool = False, backup: bool = False, ensure: bool = False, msgout: callable = None) -> str:
+def move_file(src: str, dst: str, copy: bool = False, backup: bool = False, ensure: bool = False, msgout: typing.Callable | None = None) -> str:
     """Move or copy file from one place to another.
 
     Args:
         src (str): Source file path.
         dst (str): Destination file path.
         copy (bool): Copy or move source file to destination.
         backup (bool): Backup destination file or not. `True` means try to backup destination file, pass if destination file does not exist.
@@ -604,20 +607,20 @@
         param (dict): The parameters in the request payload.
         method (str): The method of request, "get" or "post".
     Returns:
         dict: The responsed json decoded into a dict.
     """
     if method.lower() == "get":
         if param:
-            param = urllib.parse.urlencode(param)
-            url += "?" + param
+            param_enc = urllib.parse.urlencode(param)
+            url += "?" + param_enc
         req = urllib.request.Request(url)
     elif method.lower() == "post":
-        param = json.dumps(param).encode("utf-8")
-        req = urllib.request.Request(url, data=param)
+        param_enc = json.dumps(param).encode("utf-8")
+        req = urllib.request.Request(url, data=param_enc)
     else:
         raise Exception("invalid method '{}' (GET/POST)".format(method))
     rsp_bytes = read_url(req)
     if rsp_bytes:
         rsp_str = rsp_bytes.decode("utf-8")
         try:
             return json.loads(rsp_str)
@@ -627,35 +630,37 @@
 
 
 def is_python3() -> bool:
     """Check does the script is running in python3"""
     return sys.version_info[0] == 3
 
 
-def is_admin() -> bool:
+def is_admin() -> bool | None:
     """Check does the script has admin privileges."""
     import ctypes
-    try:
+    if platform.system() == "Windows":  # Windows only
         return ctypes.windll.shell32.IsUserAnAdmin()
-    except AttributeError:  # Windows only
-        return None
+    return None
 
 
 def runas_admin(py_file: str) -> bool:
     """Execute a python script with admin privileges.
 
     Links:
         Syntax of ShellExecuteW: https://docs.microsoft.com/en-us/windows/win32/api/shellapi/nf-shellapi-shellexecutew
 
     Args:
         py_file (str): The command line arguments passed to python. It should be the script path, such as `__file__`.
+
     Returns:
         bool: Command run success.
     """
     import ctypes
+    if not platform.system() == 'Windows':
+        return False
     parent_window_handle = None  # no UI
     operation = "runas"  # run as admin
     executor = sys.executable  # python.exe
     parameter = py_file
     directory = None  # using current working directory.
     SHOWNORMAL = 1  # SW_SHOWNORMAL
     if not os.path.isfile(parameter):
```

### Comparing `consolecmdtools-6.4.0/consolecmdtools/__main__.py` & `consolecmdtools-6.4.2/consolecmdtools/__main__.py`

 * *Files identical despite different names*

### Comparing `consolecmdtools-6.4.0/consolecmdtools/path.py` & `consolecmdtools-6.4.2/consolecmdtools/path.py`

 * *Files identical despite different names*

### Comparing `consolecmdtools-6.4.0/consolecmdtools.egg-info/PKG-INFO` & `consolecmdtools-6.4.2/consolecmdtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 6.4.0
+Version: 6.4.2
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,16 +39,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: consoleiotools
 Provides-Extra: opt
 Requires-Dist: pillow; extra == "opt"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: pycodestyle; extra == "dev"
 
 # PyConsoleCMDTools
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
 ![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
 [![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
 
 ## Installation
@@ -173,14 +173,20 @@
 './file.txt'
 
 >>> cct.get_path("./file.txt").abs  # Get the absolute path. Same as `get_path("./file.txt")` itself.
 
 >>> cct.get_path("./file.txt").exists  # Test if the path exists.
 True
 
+>>> cct.get_path("./file.txt").is_file  # Test if the path is a file.
+True
+
+>>> cct.get_path("./file.txt").is_dir  # Test if the path is a dir.
+False
+
 >>> cct.get_path("/path/to/file.txt").basename  # Get the basename of the file or dir.
 'file.txt'
 
 >>> cct.get_path("/path/to/file.txt").ext  # Get the extension of the path. If the path is a dir, return ''.
 'txt'
 
 >>> cct.get_path("/path/to/file.txt").stem  # Get the name of the path without extension. If the path is a dir, return its basename.
```

### Comparing `consolecmdtools-6.4.0/tests/test_consolecmdtools.py` & `consolecmdtools-6.4.2/tests/test_consolecmdtools.py`

 * *Files identical despite different names*

