# Comparing `tmp/asciiscape-0.0.1.tar.gz` & `tmp/asciiscape-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciiscape-0.0.1.tar", last modified: Mon May 27 21:20:23 2024, max compression
+gzip compressed data, was "asciiscape-0.1.0.tar", max compression
```

## Comparing `asciiscape-0.0.1.tar` & `asciiscape-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 21:20:23.857236 asciiscape-0.0.1/
--rw-rw-rw-   0        0        0      591 2024-05-27 21:20:23.855248 asciiscape-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 21:20:23.802238 asciiscape-0.0.1/asciiscape/
--rw-rw-rw-   0        0        0       81 2024-05-27 20:55:45.000000 asciiscape-0.0.1/asciiscape/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-05-27 21:14:10.000000 asciiscape-0.0.1/asciiscape/console.py
--rw-rw-rw-   0        0        0     5292 2024-05-27 20:52:02.000000 asciiscape-0.0.1/asciiscape/imgUtils.py
--rw-rw-rw-   0        0        0      643 2024-05-27 18:35:30.000000 asciiscape-0.0.1/asciiscape/main.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:20:23.853253 asciiscape-0.0.1/asciiscape.egg-info/
--rw-rw-rw-   0        0        0      591 2024-05-27 21:20:23.000000 asciiscape-0.0.1/asciiscape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-05-27 21:20:23.000000 asciiscape-0.0.1/asciiscape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 21:20:23.000000 asciiscape-0.0.1/asciiscape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 21:20:23.000000 asciiscape-0.0.1/asciiscape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 21:20:23.000000 asciiscape-0.0.1/asciiscape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 21:20:23.857236 asciiscape-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-27 21:18:33.000000 asciiscape-0.0.1/setup.py
+-rw-r--r--   0        0        0        0 2024-05-28 03:34:12.242744 asciiscape-0.1.0/asciiscape/__init__.py
+-rw-r--r--   0        0        0     4394 2024-05-27 21:14:10.147623 asciiscape-0.1.0/asciiscape/console.py
+-rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.0/asciiscape/imgUtils.py
+-rw-r--r--   0        0        0      643 2024-05-27 18:35:30.430600 asciiscape-0.1.0/asciiscape/main.py
+-rw-r--r--   0        0        0      496 2024-05-28 03:40:12.529850 asciiscape-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.0/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.0/PKG-INFO
```

### Comparing `asciiscape-0.0.1/asciiscape/console.py` & `asciiscape-0.1.0/asciiscape/console.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.0.1/asciiscape/imgUtils.py` & `asciiscape-0.1.0/asciiscape/imgUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PIL import Image
 import numpy
 
 grayscale91=[' ','`', '.', '-', "'", ':', '_', ',', '^', '=', ';', '>', '<', '+', '!', 'r', 'c', '*', '/', 'z', '?', 's', 'L', 'T', 'v', ')', 'J', '7', '(', '|', 'F', 'i', '{', 'C', '}', 'f', 'I', '3', '1', 't', 'l', 'u', '[', 'n', 'e', 'o', 'Z', '5', 'Y', 'x', 'j', 'y', 'a', ']', '2', 'E', 'S', 'w', 'q', 'k', 'P', '6', 'h', '9', 'd', '4', 'V', 'p', 'O', 'G', 'b', 'U', 'A', 'K', 'X', 'H', 'm', '8', 'R', 'D', '#', '$', 'B', 'g', '0', 'M', 'N', 'W', 'Q', '%', '&', '@']
-grayscaleCharBrightness91=[0,0.0751, 0.0829, 0.0848, 0.1227, 0.1403, 0.1559, 0.185, 0.2183, 0.2417, 0.2571, 0.2852, 0.2902, 0.2919, 0.3099, 0.3192, 0.3232, 0.3294, 0.3384, 0.3609, 0.3619, 0.3667, 0.3737, 0.3747, 0.3838, 0.3921, 0.396, 0.3984, 0.3993, 0.4075, 0.4091, 0.4101, 0.42, 0.423, 0.4247, 0.4274, 0.4293, 0.4328, 0.4382, 0.4385, 0.442, 0.4473, 0.4477, 0.4503, 0.4562, 0.458, 0.461, 0.4638, 0.4667, 0.4686, 0.4693, 0.4703, 0.4833, 0.4881, 0.4944, 0.4953, 0.4992, 0.5509, 0.5567, 0.5569, 0.5591, 0.5602, 0.5602, 0.565, 0.5776, 0.5777, 0.5818, 0.587, 0.5972, 0.5999, 0.6043, 0.6049, 0.6093, 0.6099, 0.6465, 0.6561, 0.6595, 0.6631, 0.6714, 0.6759, 0.6809, 0.6816, 0.6925, 0.7039, 0.7086, 0.7235, 0.7302, 0.7332, 0.7602, 0.7834, 0.8037, 0.1]
+grayscaleCharBrightness91=[0.0751, 0.0829, 0.0848, 0.1227, 0.1403, 0.1559, 0.185, 0.2183, 0.2417, 0.2571, 0.2852, 0.2902, 0.2919, 0.3099, 0.3192, 0.3232, 0.3294, 0.3384, 0.3609, 0.3619, 0.3667, 0.3737, 0.3747, 0.3838, 0.3921, 0.396, 0.3984, 0.3993, 0.4075, 0.4091, 0.4101, 0.42, 0.423, 0.4247, 0.4274, 0.4293, 0.4328, 0.4382, 0.4385, 0.442, 0.4473, 0.4477, 0.4503, 0.4562, 0.458, 0.461, 0.4638, 0.4667, 0.4686, 0.4693, 0.4703, 0.4833, 0.4881, 0.4944, 0.4953, 0.4992, 0.5509, 0.5567, 0.5569, 0.5591, 0.5602, 0.5602, 0.565, 0.5776, 0.5777, 0.5818, 0.587, 0.5972, 0.5999, 0.6043, 0.6049, 0.6093, 0.6099, 0.6465, 0.6561, 0.6595, 0.6631, 0.6714, 0.6759, 0.6809, 0.6816, 0.6925, 0.7039, 0.7086, 0.7235, 0.7302, 0.7332, 0.7602, 0.7834, 0.8037]
 grayscale10=[' ', '.', ':', '-', '=', '+', '*', '#', '%', '@']
 grayscaleCharBrightness10=[0,0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9]
 braileeDots = [
     (0x01, 0x08),
     (0x02, 0x10),
     (0x04, 0x20),
     (0x40, 0x80)
```

### Comparing `asciiscape-0.0.1/asciiscape/main.py` & `asciiscape-0.1.0/asciiscape/main.py`

 * *Files identical despite different names*

