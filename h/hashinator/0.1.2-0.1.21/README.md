# Comparing `tmp/hashinator-0.1.2.tar.gz` & `tmp/hashinator-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashinator-0.1.2.tar", last modified: Tue May 28 19:21:01 2024, max compression
+gzip compressed data, was "hashinator-0.1.21.tar", last modified: Tue May 28 20:14:53 2024, max compression
```

## Comparing `hashinator-0.1.2.tar` & `hashinator-0.1.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.799077 hashinator-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-05-28 18:52:44.000000 hashinator-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      241 2024-05-28 19:21:01.783469 hashinator-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-28 19:20:49.000000 hashinator-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 19:21:01.799077 hashinator-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.735890 hashinator-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.747494 hashinator-0.1.2/src/hashinator/
--rw-rw-rw-   0        0        0        0 2024-05-28 18:24:57.000000 hashinator-0.1.2/src/hashinator/__init__.py
--rw-rw-rw-   0        0        0    12452 2024-05-28 18:25:39.000000 hashinator-0.1.2/src/hashinator/hashes.py
--rw-rw-rw-   0        0        0     3306 2024-05-28 18:22:10.000000 hashinator-0.1.2/src/hashinator/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 19:21:01.783469 hashinator-0.1.2/src/hashinator.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-28 19:21:01.000000 hashinator-0.1.2/src/hashinator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 20:14:53.713022 hashinator-0.1.21/
+-rw-rw-rw-   0        0        0     1091 2024-05-28 18:52:44.000000 hashinator-0.1.21/LICENSE
+-rw-rw-rw-   0        0        0      263 2024-05-28 20:14:53.713022 hashinator-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-05-28 20:14:44.000000 hashinator-0.1.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 20:14:53.713022 hashinator-0.1.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 20:14:53.687100 hashinator-0.1.21/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 20:14:53.691662 hashinator-0.1.21/src/hashinator/
+-rw-rw-rw-   0        0        0        0 2024-05-28 18:24:57.000000 hashinator-0.1.21/src/hashinator/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-05-28 20:13:57.000000 hashinator-0.1.21/src/hashinator/hashes.py
+-rw-rw-rw-   0        0        0     3306 2024-05-28 18:22:10.000000 hashinator-0.1.21/src/hashinator/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:14:53.713022 hashinator-0.1.21/src/hashinator.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-05-28 20:14:53.000000 hashinator-0.1.21/src/hashinator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-28 20:14:53.000000 hashinator-0.1.21/src/hashinator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 20:14:53.000000 hashinator-0.1.21/src/hashinator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-28 20:14:53.000000 hashinator-0.1.21/src/hashinator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-28 20:14:53.000000 hashinator-0.1.21/src/hashinator.egg-info/top_level.txt
```

### Comparing `hashinator-0.1.2/LICENSE` & `hashinator-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `hashinator-0.1.2/src/hashinator/hashes.py` & `hashinator-0.1.21/src/hashinator/hashes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 
 import numpy
 from PIL import Image, ImageFilter
 from scipy.fftpack import dct
 
-import utils
+from hashinator import utils
 
 __all__ = [
     'ahash',
     'mhash',
     'phash',
     'dhash',
     'whash',
@@ -317,20 +317,7 @@
             blocks[block_bottom][block_left] += value * weight_bottom * weight_left
             blocks[block_bottom][block_right] += value * weight_bottom * weight_right
 
     result = [blocks[row][col] for row in range(bits) for col in range(bits)]
 
     _translate_blocks_to_bits(result, block_width * block_height)
     return "".join(map(str, result))
-    # return bits_to_hexhash(result)
-
-
-if __name__ == "__main__":
-    print(utils.compare_hashes(crop_resistant_hash(Image.open("images/img1.jpg")), crop_resistant_hash(Image.open("images/img3.jpg"))))
-    # print(imagehash.crop_resistant_hash(Image.open("images/img1.jpg")) - imagehash.crop_resistant_hash(Image.open(
-    #     "images/img3.jpg")))
-    # print(imagehash.crop_resistant_hash(Image.open("images/img1.jpg")) - imagehash.crop_resistant_hash(Image.open(
-    #     "images/img4.jpg")))
-    # print(imagehash.crop_resistant_hash(Image.open("images/img1.jpg")) - imagehash.crop_resistant_hash(Image.open(
-    #     "images/img5.jpg")))
-    # print(imagehash.crop_resistant_hash(Image.open("images/img1.jpg")) - imagehash.crop_resistant_hash(Image.open(
-    #     "images/img6.jpg")))
```

### Comparing `hashinator-0.1.2/src/hashinator/utils.py` & `hashinator-0.1.21/src/hashinator/utils.py`

 * *Files identical despite different names*

