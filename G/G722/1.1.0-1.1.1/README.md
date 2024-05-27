# Comparing `tmp/g722-1.1.0.tar.gz` & `tmp/g722-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g722-1.1.0.tar", last modified: Mon Apr 22 23:46:45 2024, max compression
+gzip compressed data, was "g722-1.1.1.tar", last modified: Mon May 27 22:37:37 2024, max compression
```

## Comparing `g722-1.1.0.tar` & `g722-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:46:45.297491 g722-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:46:45.297491 g722-1.1.0/G722.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-22 23:46:45.000000 g722-1.1.0/G722.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 23:46:45.000000 g722-1.1.0/G722.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:46:45.000000 g722-1.1.0/G722.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:46:45.000000 g722-1.1.0/G722.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:46:45.000000 g722-1.1.0/G722.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 23:46:36.000000 g722-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 23:46:36.000000 g722-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-22 23:46:45.297491 g722-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-22 23:46:36.000000 g722-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-22 23:46:36.000000 g722-1.1.0/g722.h
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 23:46:36.000000 g722-1.1.0/g722_codec.h
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-22 23:46:36.000000 g722-1.1.0/g722_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-22 23:46:36.000000 g722-1.1.0/g722_decode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:46:36.000000 g722-1.1.0/g722_decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-22 23:46:36.000000 g722-1.1.0/g722_encode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:46:36.000000 g722-1.1.0/g722_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 23:46:36.000000 g722-1.1.0/g722_private.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:46:45.297491 g722-1.1.0/python/
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-04-22 23:46:36.000000 g722-1.1.0/python/G722_mod.c
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:46:36.000000 g722-1.1.0/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 23:46:36.000000 g722-1.1.0/python/symbols.map
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:46:45.297491 g722-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-22 23:46:36.000000 g722-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:37:37.107379 g722-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:37:37.107379 g722-1.1.1/G722.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-27 22:37:37.000000 g722-1.1.1/G722.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 22:37:37.000000 g722-1.1.1/G722.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:37:37.000000 g722-1.1.1/G722.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 22:37:37.000000 g722-1.1.1/G722.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 22:37:37.000000 g722-1.1.1/G722.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-27 22:37:27.000000 g722-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 22:37:27.000000 g722-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-27 22:37:37.107379 g722-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-27 22:37:27.000000 g722-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-27 22:37:27.000000 g722-1.1.1/g722.h
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 22:37:27.000000 g722-1.1.1/g722_codec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-27 22:37:27.000000 g722-1.1.1/g722_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-27 22:37:27.000000 g722-1.1.1/g722_decode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-27 22:37:27.000000 g722-1.1.1/g722_decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-27 22:37:27.000000 g722-1.1.1/g722_encode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-27 22:37:27.000000 g722-1.1.1/g722_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-27 22:37:27.000000 g722-1.1.1/g722_private.h
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 22:37:27.000000 g722-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:37:37.107379 g722-1.1.1/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-27 22:37:27.000000 g722-1.1.1/python/G722_mod.c
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 22:37:27.000000 g722-1.1.1/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 22:37:27.000000 g722-1.1.1/python/symbols.map
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:37:37.107379 g722-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-27 22:37:27.000000 g722-1.1.1/setup.py
```

### Comparing `g722-1.1.0/G722.egg-info/PKG-INFO` & `g722-1.1.1/G722.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: G722
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a package for G.722 module
 Home-page: https://github.com/sippy/libg722
 Author: Maksym Sobolyev
 Author-email: sobomax@sippysoft.com
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
```

### Comparing `g722-1.1.0/LICENSE` & `g722-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/PKG-INFO` & `g722-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: G722
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a package for G.722 module
 Home-page: https://github.com/sippy/libg722
 Author: Maksym Sobolyev
 Author-email: sobomax@sippysoft.com
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
```

### Comparing `g722-1.1.0/README.md` & `g722-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722.h` & `g722-1.1.1/g722.h`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_common.h` & `g722-1.1.1/g722_common.h`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_decode.c` & `g722-1.1.1/g722_decode.c`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_decoder.h` & `g722-1.1.1/g722_decoder.h`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_encode.c` & `g722-1.1.1/g722_encode.c`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_encoder.h` & `g722-1.1.1/g722_encoder.h`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/g722_private.h` & `g722-1.1.1/g722_private.h`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/python/G722_mod.c` & `g722-1.1.1/python/G722_mod.c`

 * *Files identical despite different names*

### Comparing `g722-1.1.0/setup.py` & `g722-1.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,67 @@
-from sys import exit
+from sys import exit, argv
 from distutils.core import setup, Extension
 from setuptools.command.test import test as TestCommand
 from os.path import exists, realpath, dirname, join as path_join
 from sys import argv as sys_argv
-import numpy as np
+from sysconfig import get_platform
 
-mod_name = 'G722'
-mod_name_dbg = mod_name + '_debug'
+def main():
 
-mod_dir = dirname(realpath(sys_argv[0]))
-src_dir = './' if exists('g722_decode.c') else '../'
-mod_fname = mod_name + '_mod.c'
-mod_dir = '' if exists(mod_fname) else 'python/'
-
-compile_args = [f'-I{src_dir}', '-flto', f'-I{np.get_include()}']
-smap_fname = f'{mod_dir}symbols.map'
-link_args = ['-flto', f'-Wl,--version-script={smap_fname}']
-debug_cflags = ['-g3', '-O0', '-DDEBUG_MOD']
-debug_link_args = ['-g3', '-O0']
-mod_common_args = {
-    'sources': [mod_dir + mod_fname, src_dir + 'g722_decode.c', src_dir + 'g722_encode.c'],
-    'extra_compile_args': compile_args,
-    'extra_link_args': link_args
-}
-mod_debug_args = mod_common_args.copy()
-mod_debug_args['extra_compile_args'] = mod_debug_args['extra_compile_args'] + debug_cflags
-mod_debug_args['extra_link_args'] = mod_debug_args['extra_link_args'] + debug_link_args
-
-module1 = Extension(mod_name, **mod_common_args)
-module2 = Extension(mod_name_dbg, **mod_debug_args)
-
-requirements = [x.strip() for x in open(mod_dir + "requirements.txt", "r").readlines()]
-with open(src_dir + "README.md", "r") as fh:
-    long_description = fh.read()
-
-kwargs = {
-      'name':mod_name,
-      'version':'1.1.0',
-      'description':'This is a package for G.722 module',
-      'long_description': long_description,
-      'long_description_content_type': "text/markdown",
-      'author':'Maksym Sobolyev',
-      'author_email':'sobomax@sippysoft.com',
-      'url':'https://github.com/sippy/libg722',
-      'ext_modules': [module1, module2],
-      'python_requires': '>=3.10',
-      'install_requires': requirements,
-      'classifiers': [
-            'License :: Public Domain',
-            'Operating System :: OS Independent',
-            'Programming Language :: C',
-            'Programming Language :: Python'
-      ]
-}
+    mod_name = 'G722'
+    mod_name_dbg = mod_name + '_debug'
 
-setup (**kwargs)
+    mod_dir = dirname(realpath(sys_argv[0]))
+    src_dir = './' if exists('g722_decode.c') else '../'
+    mod_fname = mod_name + '_mod.c'
+    mod_dir = '' if exists(mod_fname) else 'python/'
+
+    def np_include():
+        import numpy as np
+        return f'-I{np.get_include()}'
+
+    compile_args = [f'-I{src_dir}', '-flto', np_include()]
+    smap_fname = f'{mod_dir}symbols.map'
+    link_args = ['-flto',]
+    if not get_platform().startswith('macosx-'):
+        link_args.append(f'-Wl,--version-script={smap_fname}')
+    debug_cflags = ['-g3', '-O0', '-DDEBUG_MOD']
+    debug_link_args = ['-g3', '-O0']
+    mod_common_args = {
+        'sources': [mod_dir + mod_fname, src_dir + 'g722_decode.c', src_dir + 'g722_encode.c'],
+        'extra_compile_args': compile_args,
+        'extra_link_args': link_args
+    }
+    mod_debug_args = mod_common_args.copy()
+    mod_debug_args['extra_compile_args'] = mod_debug_args['extra_compile_args'] + debug_cflags
+    mod_debug_args['extra_link_args'] = mod_debug_args['extra_link_args'] + debug_link_args
+
+    module1 = Extension(mod_name, **mod_common_args)
+    module2 = Extension(mod_name_dbg, **mod_debug_args)
+
+    requirements = [x.strip() for x in open(mod_dir + "requirements.txt", "r").readlines()]
+    with open(src_dir + "README.md", "r") as fh:
+        long_description = fh.read()
+
+    kwargs = {
+        'name':mod_name,
+        'version':'1.1.1',
+        'description':'This is a package for G.722 module',
+        'long_description': long_description,
+        'long_description_content_type': "text/markdown",
+        'author':'Maksym Sobolyev',
+        'author_email':'sobomax@sippysoft.com',
+        'url':'https://github.com/sippy/libg722',
+        'ext_modules': [module1, module2],
+        'python_requires': '>=3.10',
+        'install_requires': requirements,
+        'classifiers': [
+                'License :: Public Domain',
+                'Operating System :: OS Independent',
+                'Programming Language :: C',
+                'Programming Language :: Python'
+        ]
+    }
+
+    setup (**kwargs)
+
+if __name__ == '__main__': main()
```

