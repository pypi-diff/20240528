# Comparing `tmp/aoirint_matvtool-0.4.2.tar.gz` & `tmp/aoirint_matvtool-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_matvtool-0.4.2.tar", max compression
+gzip compressed data, was "aoirint_matvtool-0.5.0.tar", max compression
```

## Comparing `aoirint_matvtool-0.4.2.tar` & `aoirint_matvtool-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/LICENSE
--rw-r--r--   0        0        0     6932 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/README.md
--rw-r--r--   0        0        0       22 2024-03-23 14:11:10.496213 aoirint_matvtool-0.4.2/aoirint_matvtool/__init__.py
--rw-r--r--   0        0        0       61 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/__main__.py
--rw-r--r--   0        0        0    15178 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/cli.py
--rw-r--r--   0        0        0      104 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/config.py
--rw-r--r--   0        0        0     3004 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/crop_scale.py
--rw-r--r--   0        0        0     5008 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/find_image.py
--rw-r--r--   0        0        0     1345 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/fps.py
--rw-r--r--   0        0        0     6029 2024-03-23 14:11:02.388255 aoirint_matvtool-0.4.2/aoirint_matvtool/inputs.py
--rw-r--r--   0        0        0     1975 2024-03-23 14:11:02.392255 aoirint_matvtool-0.4.2/aoirint_matvtool/key_frames.py
--rw-r--r--   0        0        0     2305 2024-03-23 14:11:02.392255 aoirint_matvtool-0.4.2/aoirint_matvtool/select_audio.py
--rw-r--r--   0        0        0     2140 2024-03-23 14:11:02.392255 aoirint_matvtool-0.4.2/aoirint_matvtool/slice.py
--rw-r--r--   0        0        0     3914 2024-03-23 14:11:02.392255 aoirint_matvtool-0.4.2/aoirint_matvtool/util.py
--rw-r--r--   0        0        0     1059 2024-03-23 14:11:10.496213 aoirint_matvtool-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 aoirint_matvtool-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6932 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-28 13:16:39.878719 aoirint_matvtool-0.5.0/aoirint_matvtool/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/__main__.py
+-rw-r--r--   0        0        0    15178 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/cli.py
+-rw-r--r--   0        0        0      104 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/config.py
+-rw-r--r--   0        0        0     3004 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/crop_scale.py
+-rw-r--r--   0        0        0     5008 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/find_image.py
+-rw-r--r--   0        0        0     1345 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/fps.py
+-rw-r--r--   0        0        0     6029 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/inputs.py
+-rw-r--r--   0        0        0     1975 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/key_frames.py
+-rw-r--r--   0        0        0     2305 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/select_audio.py
+-rw-r--r--   0        0        0     2140 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/slice.py
+-rw-r--r--   0        0        0     3914 2024-05-28 13:16:28.394607 aoirint_matvtool-0.5.0/aoirint_matvtool/util.py
+-rw-r--r--   0        0        0     1061 2024-05-28 13:16:39.878719 aoirint_matvtool-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 aoirint_matvtool-0.5.0/PKG-INFO
```

### Comparing `aoirint_matvtool-0.4.2/LICENSE` & `aoirint_matvtool-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/README.md` & `aoirint_matvtool-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/cli.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/cli.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/crop_scale.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/crop_scale.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/find_image.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/find_image.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/fps.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/fps.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/inputs.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/inputs.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/key_frames.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/key_frames.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/select_audio.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/select_audio.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/slice.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/slice.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/aoirint_matvtool/util.py` & `aoirint_matvtool-0.5.0/aoirint_matvtool/util.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.2/pyproject.toml` & `aoirint_matvtool-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.pysen]
-version = "0.10"
+version = "0.11"
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
 enable_isort = true
 enable_mypy = true
 mypy_preset = "strict"
@@ -12,40 +12,40 @@
 
   [[tool.pysen.lint.mypy_targets]]
     paths = ["."]
 
 
 [tool.poetry]
 name = "aoirint-matvtool"
-version = "0.4.2"
+version = "0.5.0"
 description = "A command line tool to handle a multi audio track video file"
 authors = ["aoirint <aoirint@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aoirint/matvtoolpy"
 packages = [{include = "aoirint_matvtool"}]
 
 [tool.poetry.scripts]
 matvtool = "aoirint_matvtool.cli:main"
 
 [tool.poetry.dependencies]
 python = "~3.11"
-pydantic = "^2.0.3"
-tqdm = "^4.65.0"
+pydantic = "^2.7.1"
+tqdm = "^4.66.4"
 
 
 [tool.poetry.group.dev.dependencies]
-types-tqdm = "^4.65.0.2"
-numpy = "^1.25.1"
-opencv-python = "^4.8.0.74"
-pysen = "^0.10.4"
-black = ">=23.7,<25.0"
-isort = "^5.12.0"
-flake8 = "^6.0.0"
-flake8-bugbear = "^23.7.10"
-mypy = "^1.4.1"
-pytest = "^7.4.0"
-pyinstaller = "^5.13.0"
+types-tqdm = "^4.66.0.20240417"
+numpy = "^1.26.4"
+opencv-python = "^4.9.0.80"
+pysen = "^0.11.0"
+black = "^24.4.2"
+isort = "^5.13.2"
+flake8 = "^7.0.0"
+flake8-bugbear = "^24.4.26"
+mypy = "^1.10.0"
+pytest = "^8.2.1"
+pyinstaller = "^6.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aoirint_matvtool-0.4.2/PKG-INFO` & `aoirint_matvtool-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aoirint-matvtool
-Version: 0.4.2
+Version: 0.5.0
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
 License: MIT
 Author: aoirint
 Author-email: aoirint@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Repository, https://github.com/aoirint/matvtoolpy
 Description-Content-Type: text/markdown
 
 # matvtoolpy / MultiAudioTrackVideoToolPy
 
 A command line tool to handle a multi audio track video file.
```

