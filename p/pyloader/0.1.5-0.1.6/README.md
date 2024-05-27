# Comparing `tmp/pyloader-0.1.5.tar.gz` & `tmp/pyloader-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyloader-0.1.5.tar", last modified: Mon May 11 01:45:05 2020, max compression
+gzip compressed data, was "pyloader-0.1.6.tar", last modified: Mon May 27 23:14:44 2024, max compression
```

## Comparing `pyloader-0.1.5.tar` & `pyloader-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2020-05-11 01:45:05.000000 pyloader-0.1.5/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     5922 2020-05-11 01:45:05.000000 pyloader-0.1.5/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     4585 2020-05-10 21:34:11.000000 pyloader-0.1.5/README.txt
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       42 2020-05-10 21:36:34.000000 pyloader-0.1.5/pyloader/__init__.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1353 2020-05-10 21:38:50.000000 pyloader-0.1.5/pyloader/cast.py
--rwxr-xr-x   0 jhammel   (1000) jhammel   (1000)    10382 2020-05-10 21:46:12.000000 pyloader-0.1.5/pyloader/factory.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     2138 2020-05-10 21:46:40.000000 pyloader-0.1.5/pyloader/invoke.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1228 2020-05-10 21:37:35.000000 pyloader-0.1.5/pyloader/loader.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     1144 2020-05-10 21:40:22.000000 pyloader-0.1.5/pyloader/parser.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      524 2020-05-10 21:34:11.000000 pyloader-0.1.5/pyloader/require.py
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     5922 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      348 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/SOURCES.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/dependency_links.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       99 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/entry_points.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2020-05-10 21:34:46.000000 pyloader-0.1.5/pyloader.egg-info/not-zip-safe
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        9 2020-05-11 01:45:05.000000 pyloader-0.1.5/pyloader.egg-info/top_level.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       38 2020-05-11 01:45:05.000000 pyloader-0.1.5/setup.cfg
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      886 2020-05-11 01:44:05.000000 pyloader-0.1.5/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:14:44.475859 pyloader-0.1.6/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4807 2024-05-27 23:14:44.475859 pyloader-0.1.6/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4585 2024-05-27 22:59:39.000000 pyloader-0.1.6/README.txt
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:14:44.475859 pyloader-0.1.6/pyloader/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       42 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1353 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/cast.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)    10398 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/factory.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2138 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/invoke.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1228 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/loader.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1144 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/parser.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      524 2024-05-27 22:59:39.000000 pyloader-0.1.6/pyloader/require.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:14:44.475859 pyloader-0.1.6/pyloader.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4807 2024-05-27 23:14:44.000000 pyloader-0.1.6/pyloader.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      348 2024-05-27 23:14:44.000000 pyloader-0.1.6/pyloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:14:44.000000 pyloader-0.1.6/pyloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       99 2024-05-27 23:14:44.000000 pyloader-0.1.6/pyloader.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:03:47.000000 pyloader-0.1.6/pyloader.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        9 2024-05-27 23:14:44.000000 pyloader-0.1.6/pyloader.egg-info/top_level.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-05-27 23:14:44.475859 pyloader-0.1.6/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      886 2024-05-27 23:01:06.000000 pyloader-0.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyloader-0.1.5/README.txt` & `pyloader-0.1.6/README.txt`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/pyloader/cast.py` & `pyloader-0.1.6/pyloader/cast.py`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/pyloader/factory.py` & `pyloader-0.1.6/pyloader/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     # python 3
     from configparser import InterpolationDepthError
     from configparser import InterpolationMissingOptionError
     from configparser import InterpolationSyntaxError
     from configparser import SafeConfigParser as ConfigParser
 
 
+string = (str,)
+
+
 __all__ = ['CircularReferenceError', 'PyFactory', 'IniFactory']
 
 
 class CircularReferenceError(Exception):
     """factory has detected a circular reference"""
 
 
@@ -90,23 +93,24 @@
         # invoke
         self.parsed[name] = obj(*args, **kwargs)
         return self.parsed[name]
 
     def interpolate(self, value):
 
         # only interpolate strings
-        if not isinstance(value, basestring):
+        if not isinstance(value, string):
             return value
 
         if value.startswith(self.delimeters[0]) and value.endswith(self.delimeters[1]):
             value = value[len(self.delimeters[0]):-len(self.delimeters[1])]
             if value in self.config:
                 return self.load(value)
         return value
 
+
 class IniFactory(PyFactory):
     """
     load a python object from an .ini file
     """
 
     def __init__(self, inifile, main=''):
         assert os.path.exists(inifile), "File not found: %s" % inifile
@@ -279,14 +283,15 @@
                 config[section][option] = value
 
         return cls.configuration(config, **parser.defaults())
 
 
 def main(args=sys.argv[1:]):
     """command line entry point"""
+
     usage = '%prog file1.ini -arg1 -arg2 --key1=value1 --key2=value2'
     parser = OptionParser(usage=usage, description=IniFactory.__doc__)
     options, args = parser.parse_args(args)
 
     if len(args) != 1:
         parser.print_usage()
         parser.exit()
```

### Comparing `pyloader-0.1.5/pyloader/invoke.py` & `pyloader-0.1.6/pyloader/invoke.py`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/pyloader/loader.py` & `pyloader-0.1.6/pyloader/loader.py`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/pyloader/parser.py` & `pyloader-0.1.6/pyloader/parser.py`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/pyloader/require.py` & `pyloader-0.1.6/pyloader/require.py`

 * *Files identical despite different names*

### Comparing `pyloader-0.1.5/setup.py` & `pyloader-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 try:
     here = os.path.dirname(os.path.abspath(__file__))
     description = open(os.path.join(here, 'README.txt')).read()
 except IOError:
     description = ''
 
-version = "0.1.5"
+version = "0.1.6"
 dependencies = []
 
 setup(name='pyloader',
       version=version,
       description="Load python attributes from a string",
       long_description=description,
       classifiers=[], # Get strings from http://www.python.org/pypi?%3Aaction=list_classifiers
```

