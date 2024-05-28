# Comparing `tmp/reprec-2021.34.0.tar.gz` & `tmp/reprec-2021.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprec-2021.34.0.tar", last modified: Sat Mar 19 13:00:48 2022, max compression
+gzip compressed data, was "reprec-2021.37.0.tar", last modified: Tue May 28 20:39:54 2024, max compression
```

## Comparing `reprec-2021.34.0.tar` & `reprec-2021.37.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2022-03-19 13:00:48.476735 reprec-2021.34.0/
--rw-rw-r--   0 guettli   (1000) guettli   (1000)     5937 2022-03-19 13:00:48.476735 reprec-2021.34.0/PKG-INFO
--rw-rw-r--   0 guettli   (1000) guettli   (1000)     3901 2022-03-19 12:55:08.000000 reprec-2021.34.0/README.rst
-drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2022-03-19 13:00:48.476735 reprec-2021.34.0/reprec/
--rwxrwxr-x   0 guettli   (1000) guettli   (1000)    19257 2022-03-19 12:55:51.000000 reprec-2021.34.0/reprec/__init__.py
-drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2022-03-19 13:00:48.476735 reprec-2021.34.0/reprec.egg-info/
--rw-rw-r--   0 guettli   (1000) guettli   (1000)     5937 2022-03-19 13:00:48.000000 reprec-2021.34.0/reprec.egg-info/PKG-INFO
--rw-rw-r--   0 guettli   (1000) guettli   (1000)      210 2022-03-19 13:00:48.000000 reprec-2021.34.0/reprec.egg-info/SOURCES.txt
--rw-rw-r--   0 guettli   (1000) guettli   (1000)        1 2022-03-19 13:00:48.000000 reprec-2021.34.0/reprec.egg-info/dependency_links.txt
--rw-rw-r--   0 guettli   (1000) guettli   (1000)       61 2022-03-19 13:00:48.000000 reprec-2021.34.0/reprec.egg-info/entry_points.txt
--rw-rw-r--   0 guettli   (1000) guettli   (1000)       14 2022-03-19 13:00:48.000000 reprec-2021.34.0/reprec.egg-info/top_level.txt
-drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2022-03-19 13:00:48.476735 reprec-2021.34.0/setops/
--rw-rw-r--   0 guettli   (1000) guettli   (1000)     2329 2021-01-01 13:29:51.000000 reprec-2021.34.0/setops/__init__.py
--rw-rw-r--   0 guettli   (1000) guettli   (1000)       38 2022-03-19 13:00:48.476735 reprec-2021.34.0/setup.cfg
--rw-rw-r--   0 guettli   (1000) guettli   (1000)     2010 2022-03-19 13:00:48.000000 reprec-2021.34.0/setup.py
+drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2024-05-28 20:39:54.060910 reprec-2021.37.0/
+-rw-r--r--   0 guettli   (1000) guettli   (1000)     4403 2024-05-28 20:39:54.060910 reprec-2021.37.0/PKG-INFO
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)     3901 2022-03-19 12:55:08.000000 reprec-2021.37.0/README.rst
+drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2024-05-28 20:39:54.060910 reprec-2021.37.0/reprec/
+-rwxrwxr-x   0 guettli   (1000) guettli   (1000)    19149 2024-05-28 20:11:05.000000 reprec-2021.37.0/reprec/__init__.py
+drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2024-05-28 20:39:54.060910 reprec-2021.37.0/reprec.egg-info/
+-rw-r--r--   0 guettli   (1000) guettli   (1000)     4403 2024-05-28 20:39:54.000000 reprec-2021.37.0/reprec.egg-info/PKG-INFO
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)      210 2024-05-28 20:39:54.000000 reprec-2021.37.0/reprec.egg-info/SOURCES.txt
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)        1 2024-05-28 20:39:54.000000 reprec-2021.37.0/reprec.egg-info/dependency_links.txt
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)       60 2024-05-28 20:39:54.000000 reprec-2021.37.0/reprec.egg-info/entry_points.txt
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)       14 2024-05-28 20:39:54.000000 reprec-2021.37.0/reprec.egg-info/top_level.txt
+drwxrwxr-x   0 guettli   (1000) guettli   (1000)        0 2024-05-28 20:39:54.060910 reprec-2021.37.0/setops/
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)     2244 2024-05-28 20:19:33.000000 reprec-2021.37.0/setops/__init__.py
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)       38 2024-05-28 20:39:54.060910 reprec-2021.37.0/setup.cfg
+-rw-rw-r--   0 guettli   (1000) guettli   (1000)     1619 2024-05-28 20:39:53.000000 reprec-2021.37.0/setup.py
```

### Comparing `reprec-2021.34.0/PKG-INFO` & `reprec-2021.37.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,151 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: reprec
-Version: 2021.34.0
+Version: 2021.37.0
 Summary: reprec: Recursively replace strings in files and other goodies
 Home-page: https://github.com/guettli/reprec/
 Author: Thomas Guettler
 Author-email: info.reprec@thomas-guettler.de
 License: Apache Software License 2.0
-Description: reprec: Recursively replace strings in files and other goodies
-        ==================================================================
-        
-        Command line tool for text files.
-        
-        https://github.com/guettli/reprec
-        
-        Tools
-        =====
-        
-        Up to now there are these tools:
-        
-         * reprec: Replace strings in text files. Can work recursive in a directory tree
-         * setops: Set operations (union, intersection, ...) for line based files.
-         
-        reprec
-        ======
-        
-        The tool reprec replaces strings in text files::
-        
-            ===> reprec --help
-            Usage: reprec
-                     [-p|--pattern] p
-                     [-i|--insert] i
-                     [-f|--filename regex]
-                     [-n|--no-regex]
-                     [-v|--verbose]
-                     [-a|--ask]
-                     [--print-lines]
-                     [--dotall]
-                     [--ignorecase]
-                     [--no-std-exclude]
-                     [--files-from file|-]
-                     [--ignore regex]
-                     [--print-std-exclude]
-        
-                     dirs
-        
-                dirs:        Directories or files for replacing. Use is '.' for current dir.
-        
-                pattern:     Regex pattern.
-        
-                insert:      Text which gets inserted
-        
-                filename:    Regex matching the filename. E.g. '.*\.py'
-        
-                no-regex:    Normal string replacement will be used.
-                             This means you can use '.', '*', '[' without quoting
-        
-                verbose:     Print the number of changes for each file
-        
-                print-lines: Print the old and the new line for each change.
-                             Not available if --dotall is used.
-        
-                dotall:      In regular expressions '.' matches newlines, too.
-                             Not supported with --ask and --print-lines.
-        
-                ignorecase:  ...
-        
-                no-std-exclude: Don't exclude the directories called '.git' or '.tox'.
-                             By default they get ignored.
-        
-                ask:         Aks before replacing (interactive).
-        
-                files-from:  Read filenames from file or stdin if '-'.
-                             Skip directories.
-        
-                ignore:      Ignore lines that match a regular expression.
-                             This options can be given several times.
-        
-                print-std-exclude: print the directories which get ignored (use --no-std-exclude to
-                             not ignore them)
-        
-                Example:
-                 reprec --pattern '(xml)' --insert '\1\1' .
-                 -->This will replace all 'xml' with 'xmlxml'
-        
-                 Or, shorter:
-                 reprec '(xml)' '\1\1'
-        
-                Example2:
-                 find -mtime -1 -name '*.py' | reprec --files-from=- foo bar
-        
-        
-                The Perl Compatible Regular Expresssions are explained here:
-                  http://docs.python.org/lib/re-syntax.html
-        
-                The files are created by moving (os.rename()) FILE_RANDOMINTEGER
-                to FILE. This way no half written files will be left, if the
-                process gets killed. If the process gets killed one FILE_RANDOMINTEGER
-                may be left in the filesystem.
-        
-        
-        
-        setops
-        ======
-        The tool setops provides set operations (union, intersection, ...) for line based files::
-        
-            usage: setops [-h] set1 operator set2
-        
-            Operators:
-              union Aliases: | + or
-              intersection Aliases: & and
-              difference Aliases: - minus
-              symmetric_difference Aliases: ^
-        
-            Examples
-        
-            #Show all files in directory "a" which are not in directory "b":
-            setops <(cd a; find ) - <(cd b; find )
-        
-            # Create some files for testing
-            echo foo > foo.txt
-            echo bar > bar.txt
-            echo foobar > foobar.txt
-        
-            # All files minus files containing "foo"
-            user@host$ setops <(ls *.txt) - <(grep -l foo *.txt)
-        
-            # All files containing "foo" or "bar" minus files which contain "foobar"
-            setops <(setops <(grep -l bar *.txt) + <(grep -l foo *.txt)) - <(grep -l foobar *.txt)
-        
-        
-        
-            positional arguments:
-              set1
-              operator
-              set2
-        
-            optional arguments:
-              -h, --help  show this help message and exit
-        
-        Install
-        =======
-        
-        Install from `pypi <https://pypi.python.org/pypi/reprec/>`_::
-        
-            pip install reprec
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+
+reprec: Recursively replace strings in files and other goodies
+==================================================================
+
+Command line tool for text files.
+
+https://github.com/guettli/reprec
+
+Tools
+=====
+
+Up to now there are these tools:
+
+ * reprec: Replace strings in text files. Can work recursive in a directory tree
+ * setops: Set operations (union, intersection, ...) for line based files.
+ 
+reprec
+======
+
+The tool reprec replaces strings in text files::
+
+    ===> reprec --help
+    Usage: reprec
+             [-p|--pattern] p
+             [-i|--insert] i
+             [-f|--filename regex]
+             [-n|--no-regex]
+             [-v|--verbose]
+             [-a|--ask]
+             [--print-lines]
+             [--dotall]
+             [--ignorecase]
+             [--no-std-exclude]
+             [--files-from file|-]
+             [--ignore regex]
+             [--print-std-exclude]
+
+             dirs
+
+        dirs:        Directories or files for replacing. Use is '.' for current dir.
+
+        pattern:     Regex pattern.
+
+        insert:      Text which gets inserted
+
+        filename:    Regex matching the filename. E.g. '.*\.py'
+
+        no-regex:    Normal string replacement will be used.
+                     This means you can use '.', '*', '[' without quoting
+
+        verbose:     Print the number of changes for each file
+
+        print-lines: Print the old and the new line for each change.
+                     Not available if --dotall is used.
+
+        dotall:      In regular expressions '.' matches newlines, too.
+                     Not supported with --ask and --print-lines.
+
+        ignorecase:  ...
+
+        no-std-exclude: Don't exclude the directories called '.git' or '.tox'.
+                     By default they get ignored.
+
+        ask:         Aks before replacing (interactive).
+
+        files-from:  Read filenames from file or stdin if '-'.
+                     Skip directories.
+
+        ignore:      Ignore lines that match a regular expression.
+                     This options can be given several times.
+
+        print-std-exclude: print the directories which get ignored (use --no-std-exclude to
+                     not ignore them)
+
+        Example:
+         reprec --pattern '(xml)' --insert '\1\1' .
+         -->This will replace all 'xml' with 'xmlxml'
+
+         Or, shorter:
+         reprec '(xml)' '\1\1'
+
+        Example2:
+         find -mtime -1 -name '*.py' | reprec --files-from=- foo bar
+
+
+        The Perl Compatible Regular Expresssions are explained here:
+          http://docs.python.org/lib/re-syntax.html
+
+        The files are created by moving (os.rename()) FILE_RANDOMINTEGER
+        to FILE. This way no half written files will be left, if the
+        process gets killed. If the process gets killed one FILE_RANDOMINTEGER
+        may be left in the filesystem.
+
+
+
+setops
+======
+The tool setops provides set operations (union, intersection, ...) for line based files::
+
+    usage: setops [-h] set1 operator set2
+
+    Operators:
+      union Aliases: | + or
+      intersection Aliases: & and
+      difference Aliases: - minus
+      symmetric_difference Aliases: ^
+
+    Examples
+
+    #Show all files in directory "a" which are not in directory "b":
+    setops <(cd a; find ) - <(cd b; find )
+
+    # Create some files for testing
+    echo foo > foo.txt
+    echo bar > bar.txt
+    echo foobar > foobar.txt
+
+    # All files minus files containing "foo"
+    user@host$ setops <(ls *.txt) - <(grep -l foo *.txt)
+
+    # All files containing "foo" or "bar" minus files which contain "foobar"
+    setops <(setops <(grep -l bar *.txt) + <(grep -l foo *.txt)) - <(grep -l foobar *.txt)
+
+
+
+    positional arguments:
+      set1
+      operator
+      set2
+
+    optional arguments:
+      -h, --help  show this help message and exit
+
+Install
+=======
+
+Install from `pypi <https://pypi.python.org/pypi/reprec/>`_::
+
+    pip install reprec
```

### Comparing `reprec-2021.34.0/README.rst` & `reprec-2021.37.0/README.rst`

 * *Files identical despite different names*

### Comparing `reprec-2021.34.0/reprec/__init__.py` & `reprec-2021.37.0/reprec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, division, print_function, unicode_literals
+#!/usr/bin/env python3
 
 import getopt
 import io
 import os
 import random
 import re
 import sys
@@ -33,15 +31,15 @@
 
         dirs:        Directories or files for replacing. Use is '.' for current dir.
 
         pattern:     Regex pattern.
 
         insert:      Text which gets inserted
 
-        filename:    Regex matching the filename. E.g. '.*\.py'
+        filename:    Regex matching the filename. E.g. '.*\\.py'
 
         no-regex:    Normal string replacement will be used.
                      This means you can use '.', '*', '[' without quoting
 
         verbose:     Print the number of changes for each file
 
         print-lines: Print the old and the new line for each change.
@@ -59,15 +57,15 @@
 
         files-from:  Read filenames from file or stdin if '-'.
                      Skip directories.
 
         ignore:      Ignore lines that match a regular expression.
                      This options can be given several times.
 
-        print-std-exclude: print the directories which get ignored (use --no-std-exclude to 
+        print-std-exclude: print the directories which get ignored (use --no-std-exclude to
                      not ignore them)
 
         Example:
          %s --pattern '(xml)' --insert '\\1\\1' .
          -->This will replace all 'xml' with 'xmlxml'
 
          Or, shorter:
@@ -102,15 +100,15 @@
     if dotall and ignore_lines:
         raise Exception("You can't use --dotall and --ignore together")
 
     if isinstance(pattern, str):
         pattern = pattern.encode('utf8')
     if isinstance(text, str):
         text = text.encode('utf8')
-    
+
     rr = ReplaceRecursive(pattern, text, filename_regex,
                           no_regex, verbose, dotall,
                           print_lines, no_std_exclude, ask, ignorecase, ignore_lines)
 
     if files_from:
         assert not dirname, dirname
         for line in files_from:
@@ -331,15 +329,15 @@
             return False
         if self.always_yes:
             return True
         print('Replace in %s:' % file_name)
         print(line)
         print('with:')
         print(line_replaced)
-        if line.endswith('\n') and not line_replaced.endswith('\n'):
+        if line.endswith(b'\n') and not line_replaced.endswith(b'\n'):
             print('WARNING: Newline at the end of line was stripped!')
         while True:
             user_input = self.do_ask_one_time()
             if user_input is None:
                 continue
             return user_input
```

### Comparing `reprec-2021.34.0/reprec.egg-info/PKG-INFO` & `reprec-2021.37.0/reprec.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,151 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: reprec
-Version: 2021.34.0
+Version: 2021.37.0
 Summary: reprec: Recursively replace strings in files and other goodies
 Home-page: https://github.com/guettli/reprec/
 Author: Thomas Guettler
 Author-email: info.reprec@thomas-guettler.de
 License: Apache Software License 2.0
-Description: reprec: Recursively replace strings in files and other goodies
-        ==================================================================
-        
-        Command line tool for text files.
-        
-        https://github.com/guettli/reprec
-        
-        Tools
-        =====
-        
-        Up to now there are these tools:
-        
-         * reprec: Replace strings in text files. Can work recursive in a directory tree
-         * setops: Set operations (union, intersection, ...) for line based files.
-         
-        reprec
-        ======
-        
-        The tool reprec replaces strings in text files::
-        
-            ===> reprec --help
-            Usage: reprec
-                     [-p|--pattern] p
-                     [-i|--insert] i
-                     [-f|--filename regex]
-                     [-n|--no-regex]
-                     [-v|--verbose]
-                     [-a|--ask]
-                     [--print-lines]
-                     [--dotall]
-                     [--ignorecase]
-                     [--no-std-exclude]
-                     [--files-from file|-]
-                     [--ignore regex]
-                     [--print-std-exclude]
-        
-                     dirs
-        
-                dirs:        Directories or files for replacing. Use is '.' for current dir.
-        
-                pattern:     Regex pattern.
-        
-                insert:      Text which gets inserted
-        
-                filename:    Regex matching the filename. E.g. '.*\.py'
-        
-                no-regex:    Normal string replacement will be used.
-                             This means you can use '.', '*', '[' without quoting
-        
-                verbose:     Print the number of changes for each file
-        
-                print-lines: Print the old and the new line for each change.
-                             Not available if --dotall is used.
-        
-                dotall:      In regular expressions '.' matches newlines, too.
-                             Not supported with --ask and --print-lines.
-        
-                ignorecase:  ...
-        
-                no-std-exclude: Don't exclude the directories called '.git' or '.tox'.
-                             By default they get ignored.
-        
-                ask:         Aks before replacing (interactive).
-        
-                files-from:  Read filenames from file or stdin if '-'.
-                             Skip directories.
-        
-                ignore:      Ignore lines that match a regular expression.
-                             This options can be given several times.
-        
-                print-std-exclude: print the directories which get ignored (use --no-std-exclude to
-                             not ignore them)
-        
-                Example:
-                 reprec --pattern '(xml)' --insert '\1\1' .
-                 -->This will replace all 'xml' with 'xmlxml'
-        
-                 Or, shorter:
-                 reprec '(xml)' '\1\1'
-        
-                Example2:
-                 find -mtime -1 -name '*.py' | reprec --files-from=- foo bar
-        
-        
-                The Perl Compatible Regular Expresssions are explained here:
-                  http://docs.python.org/lib/re-syntax.html
-        
-                The files are created by moving (os.rename()) FILE_RANDOMINTEGER
-                to FILE. This way no half written files will be left, if the
-                process gets killed. If the process gets killed one FILE_RANDOMINTEGER
-                may be left in the filesystem.
-        
-        
-        
-        setops
-        ======
-        The tool setops provides set operations (union, intersection, ...) for line based files::
-        
-            usage: setops [-h] set1 operator set2
-        
-            Operators:
-              union Aliases: | + or
-              intersection Aliases: & and
-              difference Aliases: - minus
-              symmetric_difference Aliases: ^
-        
-            Examples
-        
-            #Show all files in directory "a" which are not in directory "b":
-            setops <(cd a; find ) - <(cd b; find )
-        
-            # Create some files for testing
-            echo foo > foo.txt
-            echo bar > bar.txt
-            echo foobar > foobar.txt
-        
-            # All files minus files containing "foo"
-            user@host$ setops <(ls *.txt) - <(grep -l foo *.txt)
-        
-            # All files containing "foo" or "bar" minus files which contain "foobar"
-            setops <(setops <(grep -l bar *.txt) + <(grep -l foo *.txt)) - <(grep -l foobar *.txt)
-        
-        
-        
-            positional arguments:
-              set1
-              operator
-              set2
-        
-            optional arguments:
-              -h, --help  show this help message and exit
-        
-        Install
-        =======
-        
-        Install from `pypi <https://pypi.python.org/pypi/reprec/>`_::
-        
-            pip install reprec
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+
+reprec: Recursively replace strings in files and other goodies
+==================================================================
+
+Command line tool for text files.
+
+https://github.com/guettli/reprec
+
+Tools
+=====
+
+Up to now there are these tools:
+
+ * reprec: Replace strings in text files. Can work recursive in a directory tree
+ * setops: Set operations (union, intersection, ...) for line based files.
+ 
+reprec
+======
+
+The tool reprec replaces strings in text files::
+
+    ===> reprec --help
+    Usage: reprec
+             [-p|--pattern] p
+             [-i|--insert] i
+             [-f|--filename regex]
+             [-n|--no-regex]
+             [-v|--verbose]
+             [-a|--ask]
+             [--print-lines]
+             [--dotall]
+             [--ignorecase]
+             [--no-std-exclude]
+             [--files-from file|-]
+             [--ignore regex]
+             [--print-std-exclude]
+
+             dirs
+
+        dirs:        Directories or files for replacing. Use is '.' for current dir.
+
+        pattern:     Regex pattern.
+
+        insert:      Text which gets inserted
+
+        filename:    Regex matching the filename. E.g. '.*\.py'
+
+        no-regex:    Normal string replacement will be used.
+                     This means you can use '.', '*', '[' without quoting
+
+        verbose:     Print the number of changes for each file
+
+        print-lines: Print the old and the new line for each change.
+                     Not available if --dotall is used.
+
+        dotall:      In regular expressions '.' matches newlines, too.
+                     Not supported with --ask and --print-lines.
+
+        ignorecase:  ...
+
+        no-std-exclude: Don't exclude the directories called '.git' or '.tox'.
+                     By default they get ignored.
+
+        ask:         Aks before replacing (interactive).
+
+        files-from:  Read filenames from file or stdin if '-'.
+                     Skip directories.
+
+        ignore:      Ignore lines that match a regular expression.
+                     This options can be given several times.
+
+        print-std-exclude: print the directories which get ignored (use --no-std-exclude to
+                     not ignore them)
+
+        Example:
+         reprec --pattern '(xml)' --insert '\1\1' .
+         -->This will replace all 'xml' with 'xmlxml'
+
+         Or, shorter:
+         reprec '(xml)' '\1\1'
+
+        Example2:
+         find -mtime -1 -name '*.py' | reprec --files-from=- foo bar
+
+
+        The Perl Compatible Regular Expresssions are explained here:
+          http://docs.python.org/lib/re-syntax.html
+
+        The files are created by moving (os.rename()) FILE_RANDOMINTEGER
+        to FILE. This way no half written files will be left, if the
+        process gets killed. If the process gets killed one FILE_RANDOMINTEGER
+        may be left in the filesystem.
+
+
+
+setops
+======
+The tool setops provides set operations (union, intersection, ...) for line based files::
+
+    usage: setops [-h] set1 operator set2
+
+    Operators:
+      union Aliases: | + or
+      intersection Aliases: & and
+      difference Aliases: - minus
+      symmetric_difference Aliases: ^
+
+    Examples
+
+    #Show all files in directory "a" which are not in directory "b":
+    setops <(cd a; find ) - <(cd b; find )
+
+    # Create some files for testing
+    echo foo > foo.txt
+    echo bar > bar.txt
+    echo foobar > foobar.txt
+
+    # All files minus files containing "foo"
+    user@host$ setops <(ls *.txt) - <(grep -l foo *.txt)
+
+    # All files containing "foo" or "bar" minus files which contain "foobar"
+    setops <(setops <(grep -l bar *.txt) + <(grep -l foo *.txt)) - <(grep -l foobar *.txt)
+
+
+
+    positional arguments:
+      set1
+      operator
+      set2
+
+    optional arguments:
+      -h, --help  show this help message and exit
+
+Install
+=======
+
+Install from `pypi <https://pypi.python.org/pypi/reprec/>`_::
+
+    pip install reprec
```

### Comparing `reprec-2021.34.0/setops/__init__.py` & `reprec-2021.37.0/setops/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 import argparse
 
 
 def string_to_set(string_value):
     return set(open(string_value).read().splitlines())
 
 
@@ -43,15 +41,15 @@
 
 
 def description():
     return '''Operators: \n%s
 
 Examples
 
-#Show all files in directory "a" which are not in directory "b": 
+#Show all files in directory "a" which are not in directory "b":
 setops <(cd a; find ) - <(cd b; find )
 
 
 
 # Create some files for testing
 echo foo > foo.txt
 echo bar > bar.txt
```

### Comparing `reprec-2021.34.0/setup.py` & `reprec-2021.37.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 setup(
     name='reprec',
 
     # Updated via travisd: https://travis-ci.com/guettli/reprec
     # See .travis.yml
-    version='2021.34.0',
+    version='2021.37.0',
 
     description='reprec: Recursively replace strings in files and other goodies',
     long_description=long_description,
 
     url='https://github.com/guettli/reprec/',
 
     author='Thomas Guettler',
@@ -39,23 +39,15 @@
         'Intended Audience :: Information Technology',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: Apache Software License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
     ],
 
     packages=setuptools.find_packages(),
 
     entry_points={
         'console_scripts': [
             'reprec=reprec:main',
```

