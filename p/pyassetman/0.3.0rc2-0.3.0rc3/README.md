# Comparing `tmp/pyassetman-0.3.0rc2.tar.gz` & `tmp/pyassetman-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassetman-0.3.0rc2.tar", last modified: Mon May 13 18:58:31 2024, max compression
+gzip compressed data, was "pyassetman-0.3.0rc3.tar", last modified: Tue May 28 15:59:09 2024, max compression
```

## Comparing `pyassetman-0.3.0rc2.tar` & `pyassetman-0.3.0rc3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.567683 pyassetman-0.3.0rc2/
--rw-r--r--   0 josh       (504) staff       (20)    11358 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc2/LICENSE
--rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-13 18:58:31.567494 pyassetman-0.3.0rc2/PKG-INFO
--rw-r--r--   0 josh       (504) staff       (20)     5024 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc2/README.md
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.565343 pyassetman-0.3.0rc2/assetman/
--rwxr-xr-x   0 josh       (504) staff       (20)     9085 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/S3UploadThread.py
--rw-r--r--   0 josh       (504) staff       (20)      113 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/__init__.py
--rwxr-xr-x   0 josh       (504) staff       (20)    18782 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/compile.py
--rw-r--r--   0 josh       (504) staff       (20)    10542 2024-05-13 18:48:44.000000 pyassetman-0.3.0rc2/assetman/compilers.py
--rw-r--r--   0 josh       (504) staff       (20)     7083 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/managers.py
--rw-r--r--   0 josh       (504) staff       (20)     4107 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/manifest.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.565786 pyassetman-0.3.0rc2/assetman/parsers/
--rw-r--r--   0 josh       (504) staff       (20)        0 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/__init__.py
--rw-r--r--   0 josh       (504) staff       (20)     1103 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/base.py
--rw-r--r--   0 josh       (504) staff       (20)     2339 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/parsers/tornado_parser.py
--rw-r--r--   0 josh       (504) staff       (20)     2467 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/settings.py
--rw-r--r--   0 josh       (504) staff       (20)     2774 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tools.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.566546 pyassetman-0.3.0rc2/assetman/tornadoutils/
--rw-r--r--   0 josh       (504) staff       (20)      336 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/RequestHandler.py
--rw-r--r--   0 josh       (504) staff       (20)      142 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/__init__.py
--rw-r--r--   0 josh       (504) staff       (20)      651 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/helpers.py
--rw-r--r--   0 josh       (504) staff       (20)     7154 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc2/assetman/tornadoutils/static.py
-drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-13 18:58:31.567288 pyassetman-0.3.0rc2/pyassetman.egg-info/
--rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/PKG-INFO
--rw-r--r--   0 josh       (504) staff       (20)      600 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (504) staff       (20)        1 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (504) staff       (20)       29 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/requires.txt
--rw-r--r--   0 josh       (504) staff       (20)        9 2024-05-13 18:58:31.000000 pyassetman-0.3.0rc2/pyassetman.egg-info/top_level.txt
--rw-r--r--   0 josh       (504) staff       (20)      772 2024-05-13 18:48:44.000000 pyassetman-0.3.0rc2/pyproject.toml
--rw-r--r--   0 josh       (504) staff       (20)       38 2024-05-13 18:58:31.567719 pyassetman-0.3.0rc2/setup.cfg
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-28 15:59:09.290816 pyassetman-0.3.0rc3/
+-rw-r--r--   0 josh       (504) staff       (20)    11358 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc3/LICENSE
+-rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-28 15:59:09.290611 pyassetman-0.3.0rc3/PKG-INFO
+-rw-r--r--   0 josh       (504) staff       (20)     5024 2024-01-09 01:17:06.000000 pyassetman-0.3.0rc3/README.md
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-28 15:59:09.288465 pyassetman-0.3.0rc3/assetman/
+-rwxr-xr-x   0 josh       (504) staff       (20)     9085 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/S3UploadThread.py
+-rw-r--r--   0 josh       (504) staff       (20)      113 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/__init__.py
+-rwxr-xr-x   0 josh       (504) staff       (20)    18783 2024-05-28 15:41:45.000000 pyassetman-0.3.0rc3/assetman/compile.py
+-rw-r--r--   0 josh       (504) staff       (20)    10542 2024-05-13 18:48:44.000000 pyassetman-0.3.0rc3/assetman/compilers.py
+-rw-r--r--   0 josh       (504) staff       (20)     7092 2024-05-28 15:41:45.000000 pyassetman-0.3.0rc3/assetman/managers.py
+-rw-r--r--   0 josh       (504) staff       (20)     4107 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/manifest.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-28 15:59:09.288915 pyassetman-0.3.0rc3/assetman/parsers/
+-rw-r--r--   0 josh       (504) staff       (20)        0 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/parsers/__init__.py
+-rw-r--r--   0 josh       (504) staff       (20)     1103 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/parsers/base.py
+-rw-r--r--   0 josh       (504) staff       (20)     2339 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/parsers/tornado_parser.py
+-rw-r--r--   0 josh       (504) staff       (20)     2467 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/settings.py
+-rw-r--r--   0 josh       (504) staff       (20)     3357 2024-05-28 15:41:45.000000 pyassetman-0.3.0rc3/assetman/tools.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-28 15:59:09.289631 pyassetman-0.3.0rc3/assetman/tornadoutils/
+-rw-r--r--   0 josh       (504) staff       (20)      336 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/tornadoutils/RequestHandler.py
+-rw-r--r--   0 josh       (504) staff       (20)      142 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/tornadoutils/__init__.py
+-rw-r--r--   0 josh       (504) staff       (20)      651 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/tornadoutils/helpers.py
+-rw-r--r--   0 josh       (504) staff       (20)     7154 2024-02-15 23:51:52.000000 pyassetman-0.3.0rc3/assetman/tornadoutils/static.py
+drwxr-xr-x   0 josh       (504) staff       (20)        0 2024-05-28 15:59:09.290380 pyassetman-0.3.0rc3/pyassetman.egg-info/
+-rw-r--r--   0 josh       (504) staff       (20)     5577 2024-05-28 15:59:09.000000 pyassetman-0.3.0rc3/pyassetman.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (504) staff       (20)      600 2024-05-28 15:59:09.000000 pyassetman-0.3.0rc3/pyassetman.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (504) staff       (20)        1 2024-05-28 15:59:09.000000 pyassetman-0.3.0rc3/pyassetman.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (504) staff       (20)       29 2024-05-28 15:59:09.000000 pyassetman-0.3.0rc3/pyassetman.egg-info/requires.txt
+-rw-r--r--   0 josh       (504) staff       (20)        9 2024-05-28 15:59:09.000000 pyassetman-0.3.0rc3/pyassetman.egg-info/top_level.txt
+-rw-r--r--   0 josh       (504) staff       (20)      772 2024-05-28 15:41:45.000000 pyassetman-0.3.0rc3/pyproject.toml
+-rw-r--r--   0 josh       (504) staff       (20)       38 2024-05-28 15:59:09.290849 pyassetman-0.3.0rc3/setup.cfg
```

### Comparing `pyassetman-0.3.0rc2/LICENSE` & `pyassetman-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/PKG-INFO` & `pyassetman-0.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassetman
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: assetman assetmanager
 Author-email: Will McCutchen <wm@bit.ly>
 Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>, Oscar Luu <oscar.luu@bit.ly>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pyassetman-0.3.0rc2/README.md` & `pyassetman-0.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/S3UploadThread.py` & `pyassetman-0.3.0rc3/assetman/S3UploadThread.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/compile.py` & `pyassetman-0.3.0rc3/assetman/compile.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
 
 def _build_manifest_helper(static_dir, src_paths, static_url_prefix, manifest):
     assert isinstance(src_paths, (list, tuple))
     for src_path in src_paths:
         # Make sure every source path at least has the skeleton entry
         rel_src_path = make_relative_static_path(static_dir, src_path)
-        logging.info('_build_manifest_helper %s (crrent %s)', src_path, manifest.assets.get(rel_src_path))
+        logging.info('_build_manifest_helper %s (current %s)', src_path, manifest.assets.get(rel_src_path))
         manifest.assets.setdefault(rel_src_path, empty_asset_entry())
         for dep_path in iter_deps(static_dir, src_path, static_url_prefix):
             logging.info('%s > dependency %s', src_path, dep_path)
             rel_path = make_relative_static_path(static_dir, dep_path)
             manifest.assets[rel_src_path]['deps'].add(rel_path)
             _build_manifest_helper(static_dir, [dep_path], static_url_prefix, manifest)
```

### Comparing `pyassetman-0.3.0rc2/assetman/compilers.py` & `pyassetman-0.3.0rc3/assetman/compilers.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/managers.py` & `pyassetman-0.3.0rc3/assetman/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 import os
 import logging
 import functools
 import hashlib
 
-from assetman.tools import get_shard_from_list, _utf8
+from assetman.tools import get_shard_from_list, _unicode
 from assetman.manifest import Manifest
 
 class AssetManager(object):
     """AssetManager attempts to provide easy-to-use asset management and
     compilation for Tornado (or other?) templates.
 
     On the template side, assuming this `assetman` module is available in the
@@ -42,15 +42,15 @@
 
           * src_path - an optional annotation for recording where this asset
             manager originated.
 
         Any extra kwargs will be interpreted as extra HTML params to include
         on the rendered element.
         """
-        self.rel_urls = [_f for _f in _utf8(rel_url_text).split() if _f]
+        self.rel_urls = [_f for _f in _unicode(rel_url_text).split() if _f]
         self.local = local
         self.include_tag = include_tag
         self.src_path = src_path
         self.attrs = attrs
         self._manifest = None
         assert settings
         self.settings = settings
@@ -96,15 +96,15 @@
             prefix = get_shard_from_list(self.settings['cdn_url_prefix'], os.path.basename(rel_url))
         return prefix.rstrip('/') + '/' + rel_url.lstrip('/')
 
     def render_attrs(self):
         """Returns this asset block's attrs as an HTML string. Includes a
         leading space.
         """
-        attrs = ' '.join('%s=%r' % (attr, _utf8(val))
+        attrs = ' '.join('%s=%r' % (attr, _unicode(val))
                          for attr, val in self.attrs.items())
         return ' ' + attrs if attrs else ''
 
     def render_asset(self, url):
         """Renders an individual asset at the given URL. The given URL should
         be the full URL to of the asset.
         """
```

### Comparing `pyassetman-0.3.0rc2/assetman/manifest.py` & `pyassetman-0.3.0rc3/assetman/manifest.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/parsers/base.py` & `pyassetman-0.3.0rc3/assetman/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/parsers/tornado_parser.py` & `pyassetman-0.3.0rc3/assetman/parsers/tornado_parser.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/settings.py` & `pyassetman-0.3.0rc3/assetman/settings.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/tools.py` & `pyassetman-0.3.0rc3/assetman/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,35 @@
     return settings_list[bucket]
 
 def _crc(key):
     """crc32 hash a string"""
     return binascii.crc32(_utf8(key)) & 0xffffffff
 
 def _utf8(s):
-    """encode a unicode string as utf-8"""
+    """encode a string as utf-8, returning bytes"""
     if isinstance(s, str):
-        return s.encode("utf-8").decode()
+        return s.encode("utf-8")
     if isinstance(s, bytes):
-        return s.decode("utf-8")
-    assert isinstance(s, str), "_utf8 expected a str, not %r" % type(s)
+        try:
+            s.decode("utf-8")
+        except UnicodeDecodeError:
+            raise AssertionError("Invalid encoding. _utf8 expected a str or utf-8 encoded bytes")
+    assert isinstance(s, bytes), "_utf8 expected a str or utf-8 encoded bytes, not %r" % type(s)
     return s
 
+def _unicode(value):
+    """decode utf-8 bytes, returning string"""
+    if isinstance(value, bytes):
+        try:
+            return value.decode("utf-8")
+        except UnicodeDecodeError:
+            raise AssertionError("Invalid encoding. _unicode expected a str or utf-8 encoded bytes")
+    assert isinstance(value, str), "_unicode expected a str or utf-8 encoded bytes, not %r" % type(value)
+    return value
+
 def iter_template_paths(template_dirs, template_ext):
     """Walks each directory in the given list of template directories,
     yielding the path to each template found.
     """
     # We only try to parse files that match this pattern as Tornado templates
     template_file_matcher = re.compile(r'\.' + re.escape(template_ext) + '$').search
```

### Comparing `pyassetman-0.3.0rc2/assetman/tornadoutils/helpers.py` & `pyassetman-0.3.0rc3/assetman/tornadoutils/helpers.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/assetman/tornadoutils/static.py` & `pyassetman-0.3.0rc3/assetman/tornadoutils/static.py`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/pyassetman.egg-info/PKG-INFO` & `pyassetman-0.3.0rc3/pyassetman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassetman
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: assetman assetmanager
 Author-email: Will McCutchen <wm@bit.ly>
 Maintainer-email: Jehiah Czebotar <jehiah@gmail.com>, Josh Harshman <josh.harshman@bit.ly>, Oscar Luu <oscar.luu@bit.ly>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pyassetman-0.3.0rc2/pyassetman.egg-info/SOURCES.txt` & `pyassetman-0.3.0rc3/pyassetman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyassetman-0.3.0rc2/pyproject.toml` & `pyassetman-0.3.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyassetman"
 description = "assetman assetmanager"
-version = "0.3.0rc2"
+version = "0.3.0rc3"
 authors = [
   { name="Will McCutchen", email="wm@bit.ly" },
 ]
 maintainers = [
   { name="Jehiah Czebotar", email="jehiah@gmail.com"},
   { name="Josh Harshman", email="josh.harshman@bit.ly"},
   { name="Oscar Luu", email="oscar.luu@bit.ly"}
```

