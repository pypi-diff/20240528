# Comparing `tmp/contenttransformer-0.3.3.tar.gz` & `tmp/contenttransformer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contenttransformer-0.3.3.tar", last modified: Thu Nov 25 20:01:35 2010, max compression, from Unix
+gzip compressed data, was "contenttransformer-0.3.5.tar", last modified: Mon May 27 23:40:53 2024, max compression
```

## Comparing `contenttransformer-0.3.3.tar` & `contenttransformer-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        2 2010-03-29 18:54:01.000000 contenttransformer-0.3.3/contenttransformer/__init__.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1811 2010-11-25 19:53:41.000000 contenttransformer-0.3.3/contenttransformer/app.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     3016 2010-10-27 16:07:35.000000 contenttransformer-0.3.3/contenttransformer/transformers.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      424 2010-03-29 18:54:01.000000 contenttransformer-0.3.3/contenttransformer/factory.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      272 2010-09-25 02:12:46.000000 contenttransformer-0.3.3/contenttransformer/utils.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1217 2010-03-29 18:54:01.000000 contenttransformer-0.3.3/contenttransformer/web.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       59 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/setup.cfg
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/dependency_links.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2010-03-29 18:58:57.000000 contenttransformer-0.3.3/contenttransformer.egg-info/not-zip-safe
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      326 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/entry_points.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       19 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/top_level.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      281 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      479 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/SOURCES.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       39 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/contenttransformer.egg-info/requires.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      281 2010-11-25 20:01:35.000000 contenttransformer-0.3.3/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1144 2010-11-25 19:54:58.000000 contenttransformer-0.3.3/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:40:53.167227 contenttransformer-0.3.5/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      268 2024-05-27 23:40:53.167227 contenttransformer-0.3.5/PKG-INFO
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:40:53.167227 contenttransformer-0.3.5/contenttransformer/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1794 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/app.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      424 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/factory.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     3002 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/transformers.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      275 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/utils.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1217 2024-05-27 23:34:17.000000 contenttransformer-0.3.5/contenttransformer/web.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:40:53.167227 contenttransformer-0.3.5/contenttransformer.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      268 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      479 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      326 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:34:23.000000 contenttransformer-0.3.5/contenttransformer.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       40 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/requires.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       19 2024-05-27 23:40:53.000000 contenttransformer-0.3.5/contenttransformer.egg-info/top_level.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-05-27 23:40:53.167227 contenttransformer-0.3.5/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1104 2024-05-27 23:39:04.000000 contenttransformer-0.3.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `contenttransformer-0.3.3/contenttransformer/app.py` & `contenttransformer-0.3.5/contenttransformer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import os
 import sys
 from fnmatch import fnmatch
 from mimetypes import guess_type
 from paste.fileapp import FileApp
 from pkg_resources import iter_entry_points
-from transformers import ContentTypeChanger
+from .transformers import ContentTypeChanger
 
 class FileTypeTransformer(object):
 
     def __init__(self, *types, **kwargs):
         """types is a list of two-tuples: glob pattern (string), transformer name (string, name of entry point)"""
         self.types = types
 
         # arguments to the xformers
         self.kwargs = kwargs
-        
+
         self.transformers = transformers()
         for pattern, transformer_name in self.types:
             if '/' in transformer_name:
                 continue
             assert transformer_name in self.transformers, '%s not in transformers' % transformer_name
 
-    def __call__(self, path): 
+    def __call__(self, path):
         """this should return something that is callable with (environ, start_response) to return a response; the transformer thing"""
         filename = os.path.basename(path)
         for pattern, transformer_name in self.types:
             if fnmatch(filename, pattern):
                 content_type, _ = guess_type(filename)
-                content = file(path).read()
+                content = open(path).read()
 
                 # transform content type
                 # XXX hack: -> refactor
                 if '/' in transformer_name:
                     return ContentTypeChanger(content, content_type, transformer_name)
-                return self.transformers[transformer_name](content, content_type, **self.kwargs.get(transformer_name, {})) 
+                return self.transformers[transformer_name](content, content_type, **self.kwargs.get(transformer_name, {}))
         return FileApp(path)
 
 
 def transformers():
     transformers = {} # XXX could cache
     for entry_point in iter_entry_points('content_transformers'):
         try:
             transformers[entry_point.name] = entry_point.load()
         except:
             raise # XXX
     return transformers
-        
+
```

### Comparing `contenttransformer-0.3.3/contenttransformer/transformers.py` & `contenttransformer-0.3.5/contenttransformer/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import docutils.core
 import subprocess
-from utils import import_path
+from .utils import import_path
 from webob import Request, Response
 
 import genshi
 from genshi.template import MarkupTemplate
 
 class Transformer(object):
     """abstract base class for transformer objects"""
@@ -31,32 +31,34 @@
     def __init__(self, content, from_type, to_type):
         self.to_type = to_type
         Transformer.__init__(self, content, from_type)
 
     def transform(self, request):
         return (self.to_type, self.content)
 
+
 class Graphviz(Transformer):
     content_types = { 'png': 'image/png',
                       'svg': 'image/svg+xml' }
-    
+
     def __init__(self, content, content_type, format='png'):
         self.format=format
         Transformer.__init__(self, content, content_type)
-    
+
     def transform(self, request):
         """create a Graphviz object"""
         _format = request.GET.get('format', self.format)
         assert _format in self.content_types, 'Unknown format: ' + _format
         process = subprocess.Popen(['dot', '-T' + _format],
                                    stdin=subprocess.PIPE,
                                    stdout=subprocess.PIPE)
         image, _ = process.communicate(self.content)
         return (self.content_types[_format], image)
 
+
 class RestructuredText(Transformer):
     settings = { 'report_level': 5 }
 
     def transform(self, request):
         """template: genshi(?) template to use (???)"""
         html = docutils.core.publish_string(self.content,
                                             writer_name='html',
@@ -72,14 +74,13 @@
         """
         self.variables = {}
         for path in modules:
             module = import_path(path)
             name = path.rsplit('.')[-1]
             self.variables[name] = module
         Transformer.__init__(self, content, content_type)
-        
+
     def transform(self, request):
         variables = dict(request=request)
         template = MarkupTemplate(self.content)
         stream = template.generate(**variables)
         return ('text/html', stream.render('html', doctype='html'))
-
```

### Comparing `contenttransformer-0.3.3/contenttransformer/web.py` & `contenttransformer-0.3.5/contenttransformer/web.py`

 * *Files identical despite different names*

### Comparing `contenttransformer-0.3.3/setup.py` & `contenttransformer-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = "0.3.3"
+version = "0.3.5"
 
 setup(name='contenttransformer',
       version=version,
       description="transform e.g. file data based on type to be served TTW",
-      long_description="""
-""",
       classifiers=[], # Get strings from http://www.python.org/pypi?%3Aaction=list_classifiers
       author='Jeff Hammel',
       author_email='k0scist@gmail.com',
       url='http://k0s.org/hg/contenttransformer',
       license="GPL",
       packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           # -*- Extra requirements: -*-
-        'WebOb',	
+        'WebOb',
         'Paste',
         'PasteScript',
         'docutils',
         'genshi',
       ],
       entry_points="""
       # -*- Entry points: -*-
@@ -31,8 +29,7 @@
 
       [content_transformers]
       Graphviz = contenttransformer.transformers:Graphviz
       ReST = contenttransformer.transformers:RestructuredText
       Genshi = contenttransformer.transformers:GenshiTransformer
       """,
       )
-
```

