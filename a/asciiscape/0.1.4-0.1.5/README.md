# Comparing `tmp/asciiscape-0.1.4.tar.gz` & `tmp/asciiscape-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciiscape-0.1.4.tar", max compression
+gzip compressed data, was "asciiscape-0.1.5.tar", max compression
```

## Comparing `asciiscape-0.1.4.tar` & `asciiscape-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.4/asciiscape/__init__.py
--rw-r--r--   0        0        0      690 2024-05-28 04:08:35.711513 asciiscape-0.1.4/asciiscape/__main__.py
--rw-r--r--   0        0        0     4394 2024-05-28 04:08:31.637091 asciiscape-0.1.4/asciiscape/console.py
--rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.4/asciiscape/imgUtils.py
--rw-r--r--   0        0        0      496 2024-05-28 04:08:48.540221 asciiscape-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.4/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.5/asciiscape/__init__.py
+-rw-r--r--   0        0        0      690 2024-05-28 04:08:35.711513 asciiscape-0.1.5/asciiscape/__main__.py
+-rw-r--r--   0        0        0     4410 2024-05-28 04:10:11.855019 asciiscape-0.1.5/asciiscape/console.py
+-rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.5/asciiscape/imgUtils.py
+-rw-r--r--   0        0        0      496 2024-05-28 04:10:26.768643 asciiscape-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.5/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.5/PKG-INFO
```

### Comparing `asciiscape-0.1.4/asciiscape/__main__.py` & `asciiscape-0.1.5/asciiscape/__main__.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.4/asciiscape/console.py` & `asciiscape-0.1.5/asciiscape/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rich.console import Console
 from rich.panel import Panel
 from rich.prompt import Confirm, IntPrompt, Prompt
-import imgUtils as iu
+from asciiscape import imgUtils as iu
 
 console=Console()
 def renderTitle():
     title=r'''
 ╔═╗╔═╗╔═╗╦╦┌─┐┌─┐┌─┐┌─┐┌─┐
 ╠═╣╚═╗║  ║║└─┐│  ├─┤├─┘├┤ 
 ╩ ╩╚═╝╚═╝╩╩└─┘└─┘┴ ┴┴  └─┘
```

### Comparing `asciiscape-0.1.4/asciiscape/imgUtils.py` & `asciiscape-0.1.5/asciiscape/imgUtils.py`

 * *Files identical despite different names*

