# Comparing `tmp/uritools-4.0.2.tar.gz` & `tmp/uritools-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uritools-4.0.2.tar", last modified: Wed Aug 30 19:34:03 2023, max compression
+gzip compressed data, was "uritools-4.0.3.tar", last modified: Tue May 28 18:05:22 2024, max compression
```

## Comparing `uritools-4.0.2.tar` & `uritools-4.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.441240 uritools-4.0.2/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5460 2023-08-30 19:31:51.000000 uritools-4.0.2/CHANGELOG.rst
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1085 2022-01-02 10:31:17.000000 uritools-4.0.2/LICENSE
--rw-r--r--   0 tkem      (1000) tkem      (1000)      167 2020-08-10 17:35:07.000000 uritools-4.0.2/MANIFEST.in
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     4717 2023-08-30 19:34:03.441240 uritools-4.0.2/PKG-INFO
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     3741 2023-01-08 20:41:16.000000 uritools-4.0.2/README.rst
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.437240 uritools-4.0.2/docs/
--rw-r--r--   0 tkem      (1000) tkem      (1000)        7 2020-08-10 17:35:07.000000 uritools-4.0.2/docs/.gitignore
--rw-r--r--   0 tkem      (1000) tkem      (1000)     5572 2020-08-10 17:35:07.000000 uritools-4.0.2/docs/Makefile
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      287 2023-08-30 19:31:51.000000 uritools-4.0.2/docs/conf.py
--rw-r--r--   0 tkem      (1000) tkem      (1000)     9306 2020-08-10 17:35:07.000000 uritools-4.0.2/docs/index.rst
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      100 2021-10-11 18:18:34.000000 uritools-4.0.2/pyproject.toml
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1203 2023-08-30 19:34:03.441240 uritools-4.0.2/setup.cfg
--rw-r--r--   0 tkem      (1000) tkem      (1000)       38 2020-08-10 17:35:07.000000 uritools-4.0.2/setup.py
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.437240 uritools-4.0.2/src/
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.437240 uritools-4.0.2/src/uritools/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)    27002 2023-08-30 19:31:51.000000 uritools-4.0.2/src/uritools/__init__.py
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.437240 uritools-4.0.2/src/uritools.egg-info/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     4717 2023-08-30 19:34:03.000000 uritools-4.0.2/src/uritools.egg-info/PKG-INFO
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      481 2023-08-30 19:34:03.000000 uritools-4.0.2/src/uritools.egg-info/SOURCES.txt
--rw-rw-r--   0 tkem      (1000) tkem      (1000)        1 2023-08-30 19:34:03.000000 uritools-4.0.2/src/uritools.egg-info/dependency_links.txt
--rw-rw-r--   0 tkem      (1000) tkem      (1000)        9 2023-08-30 19:34:03.000000 uritools-4.0.2/src/uritools.egg-info/top_level.txt
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-08-30 19:34:03.437240 uritools-4.0.2/tests/
--rw-r--r--   0 tkem      (1000) tkem      (1000)        0 2020-08-10 17:35:07.000000 uritools-4.0.2/tests/__init__.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     3062 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_classify.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)    10142 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_compose.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1941 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_defrag.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     2748 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_encoding.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     4780 2023-08-30 19:31:51.000000 uritools-4.0.2/tests/test_join.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)    20747 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_split.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1071 2021-10-11 18:18:34.000000 uritools-4.0.2/tests/test_unsplit.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      781 2021-10-11 18:18:34.000000 uritools-4.0.2/tox.ini
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.811203 uritools-4.0.3/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5530 2024-05-28 18:03:50.000000 uritools-4.0.3/CHANGELOG.rst
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1085 2024-05-28 18:03:31.000000 uritools-4.0.3/LICENSE
+-rw-r--r--   0 tkem      (1000) tkem      (1000)      193 2024-05-01 18:41:31.000000 uritools-4.0.3/MANIFEST.in
+-rw-r--r--   0 tkem      (1000) tkem      (1000)     4717 2024-05-28 18:05:22.811203 uritools-4.0.3/PKG-INFO
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     3741 2023-01-08 20:41:16.000000 uritools-4.0.3/README.rst
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.807203 uritools-4.0.3/docs/
+-rw-r--r--   0 tkem      (1000) tkem      (1000)        7 2020-08-10 17:35:07.000000 uritools-4.0.3/docs/.gitignore
+-rw-r--r--   0 tkem      (1000) tkem      (1000)     5572 2020-08-10 17:35:07.000000 uritools-4.0.3/docs/Makefile
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      907 2024-05-28 18:03:31.000000 uritools-4.0.3/docs/conf.py
+-rw-r--r--   0 tkem      (1000) tkem      (1000)     9306 2020-08-10 17:35:07.000000 uritools-4.0.3/docs/index.rst
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      100 2021-10-11 18:18:34.000000 uritools-4.0.3/pyproject.toml
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1204 2024-05-28 18:05:22.811203 uritools-4.0.3/setup.cfg
+-rw-r--r--   0 tkem      (1000) tkem      (1000)       38 2020-08-10 17:35:07.000000 uritools-4.0.3/setup.py
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.803203 uritools-4.0.3/src/
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.807203 uritools-4.0.3/src/uritools/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)    27002 2024-05-28 18:03:31.000000 uritools-4.0.3/src/uritools/__init__.py
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.807203 uritools-4.0.3/src/uritools.egg-info/
+-rw-r--r--   0 tkem      (1000) tkem      (1000)     4717 2024-05-28 18:05:22.000000 uritools-4.0.3/src/uritools.egg-info/PKG-INFO
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      481 2024-05-28 18:05:22.000000 uritools-4.0.3/src/uritools.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)        1 2024-05-28 18:05:22.000000 uritools-4.0.3/src/uritools.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)        9 2024-05-28 18:05:22.000000 uritools-4.0.3/src/uritools.egg-info/top_level.txt
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2024-05-28 18:05:22.807203 uritools-4.0.3/tests/
+-rw-r--r--   0 tkem      (1000) tkem      (1000)        0 2020-08-10 17:35:07.000000 uritools-4.0.3/tests/__init__.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     3062 2021-10-11 18:18:34.000000 uritools-4.0.3/tests/test_classify.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)    10142 2021-10-11 18:18:34.000000 uritools-4.0.3/tests/test_compose.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1941 2021-10-11 18:18:34.000000 uritools-4.0.3/tests/test_defrag.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     2748 2021-10-11 18:18:34.000000 uritools-4.0.3/tests/test_encoding.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     4780 2023-08-30 19:31:51.000000 uritools-4.0.3/tests/test_join.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)    23071 2024-05-28 18:03:31.000000 uritools-4.0.3/tests/test_split.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1071 2021-10-11 18:18:34.000000 uritools-4.0.3/tests/test_unsplit.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      768 2024-05-28 18:03:31.000000 uritools-4.0.3/tox.ini
```

### Comparing `uritools-4.0.2/CHANGELOG.rst` & `uritools-4.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v4.0.3 (2024-05-28)
+===================
+
+- Prepare for Python 3.13.
+
+
 v4.0.2 (2023-08-30)
 ===================
 
 - Depend on Python >= 3.7.
 
 - Support Python 3.12.
```

### Comparing `uritools-4.0.2/LICENSE` & `uritools-4.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2014-2022 Thomas Kemmer
+Copyright (c) 2014-2024 Thomas Kemmer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `uritools-4.0.2/PKG-INFO` & `uritools-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uritools
-Version: 4.0.2
+Version: 4.0.3
 Summary: URI parsing, classification and composition
 Home-page: https://github.com/tkem/uritools/
 Author: Thomas Kemmer
 Author-email: tkemmer@computer.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
```

### Comparing `uritools-4.0.2/README.rst` & `uritools-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/docs/Makefile` & `uritools-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/docs/index.rst` & `uritools-4.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/setup.cfg` & `uritools-4.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = uritools
 version = attr: uritools.__version__
 url = https://github.com/tkem/uritools/
 author = Thomas Kemmer
 author_email = tkemmer@computer.org
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 description = URI parsing, classification and composition
 long_description = file: README.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Other Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
```

### Comparing `uritools-4.0.2/src/uritools/__init__.py` & `uritools-4.0.3/src/uritools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "uridefrag",
     "uriencode",
     "urijoin",
     "urisplit",
     "uriunsplit",
 )
 
-__version__ = "4.0.2"
+__version__ = "4.0.3"
 
 
 # RFC 3986 2.2.  Reserved Characters
 #
 #   reserved    = gen-delims / sub-delims
 #
 #   gen-delims  = ":" / "/" / "?" / "#" / "[" / "]" / "@"
```

### Comparing `uritools-4.0.2/src/uritools.egg-info/PKG-INFO` & `uritools-4.0.3/src/uritools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uritools
-Version: 4.0.2
+Version: 4.0.3
 Summary: URI parsing, classification and composition
 Home-page: https://github.com/tkem/uritools/
 Author: Thomas Kemmer
 Author-email: tkemmer@computer.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
```

### Comparing `uritools-4.0.2/tests/test_classify.py` & `uritools-4.0.3/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tests/test_compose.py` & `uritools-4.0.3/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tests/test_defrag.py` & `uritools-4.0.3/tests/test_defrag.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tests/test_encoding.py` & `uritools-4.0.3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tests/test_join.py` & `uritools-4.0.3/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tests/test_split.py` & `uritools-4.0.3/tests/test_split.py`

 * *Files 19% similar despite different names*

```diff
@@ -402,60 +402,141 @@
             parts = urisplit(query)
             self.assertEqual(
                 parts.getquerylist(sep),
                 querylist,
                 "Error parsing query list for %r" % query,
             )
 
-    def test_ip_literal(self):
+    def test_ipv4_literal(self):
         cases = [
-            ("http://Test.python.org:5432/foo/", "test.python.org", 5432),
+            ("http://12.34.56.78/foo/", "12.34.56.78", None),
+            ("http://12.34.56.78:/foo/", "12.34.56.78", None),
             ("http://12.34.56.78:5432/foo/", "12.34.56.78", 5432),
-            ("http://[::1]:5432/foo/", "::1", 5432),
-            ("http://[dead:beef::1]:5432/foo/", "dead:beef::1", 5432),
-            ("http://[dead:beef::]:5432/foo/", "dead:beef::", 5432),
+        ]
+        for uri, host, port in cases:
+            for parts in (urisplit(uri), urisplit(uri.encode("ascii"))):
+                self.assertEqual(host, str(parts.gethost()))
+                self.assertEqual(port, parts.getport())
+
+    def test_ipv6_literal(self):
+        cases = [
+            ("http://[::1]:5432/foo/", "0000:0000:0000:0000:0000:0000:0000:0001", 5432),
+            (
+                "http://[dead:beef::1]:5432/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0001",
+                5432,
+            ),
+            (
+                "http://[dead:beef::]:5432/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0000",
+                5432,
+            ),
             (
                 "http://[dead:beef:cafe:5417:affe:8FA3:deaf:feed]:5432/foo/",
                 "dead:beef:cafe:5417:affe:8fa3:deaf:feed",
                 5432,
             ),
-            ("http://[::12.34.56.78]:5432/foo/", "::c22:384e", 5432),
-            ("http://[::ffff:12.34.56.78]:5432/foo/", "::ffff:c22:384e", 5432),
-            ("http://Test.python.org/foo/", "test.python.org", None),
-            ("http://12.34.56.78/foo/", "12.34.56.78", None),
-            ("http://[::1]/foo/", "::1", None),
-            ("http://[dead:beef::1]/foo/", "dead:beef::1", None),
-            ("http://[dead:beef::]/foo/", "dead:beef::", None),
+            ("http://[::1]/foo/", "0000:0000:0000:0000:0000:0000:0000:0001", None),
+            (
+                "http://[dead:beef::1]/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0001",
+                None,
+            ),
+            (
+                "http://[dead:beef::]/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0000",
+                None,
+            ),
             (
                 "http://[dead:beef:cafe:5417:affe:8FA3:deaf:feed]/foo/",
                 "dead:beef:cafe:5417:affe:8fa3:deaf:feed",
                 None,
             ),
-            ("http://[::12.34.56.78]/foo/", "::c22:384e", None),
-            ("http://[::ffff:12.34.56.78]/foo/", "::ffff:c22:384e", None),
-            ("http://Test.python.org:/foo/", "test.python.org", None),
-            ("http://12.34.56.78:/foo/", "12.34.56.78", None),
-            ("http://[::1]:/foo/", "::1", None),
-            ("http://[dead:beef::1]:/foo/", "dead:beef::1", None),
-            ("http://[dead:beef::]:/foo/", "dead:beef::", None),
+            ("http://[::1]:/foo/", "0000:0000:0000:0000:0000:0000:0000:0001", None),
+            (
+                "http://[dead:beef::1]:/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0001",
+                None,
+            ),
+            (
+                "http://[dead:beef::]:/foo/",
+                "dead:beef:0000:0000:0000:0000:0000:0000",
+                None,
+            ),
             (
                 "http://[dead:beef:cafe:5417:affe:8FA3:deaf:feed]:/foo/",
                 "dead:beef:cafe:5417:affe:8fa3:deaf:feed",
                 None,
             ),
-            ("http://[::12.34.56.78]:/foo/", "::c22:384e", None),
-            ("http://[::ffff:12.34.56.78]:/foo/", "::ffff:c22:384e", None),
         ]
         for uri, host, port in cases:
+            for parts in (urisplit(uri), urisplit(uri.encode("ascii"))):
+                self.assertEqual(host, parts.gethost().exploded)
+                self.assertEqual(port, parts.getport())
+
+    def test_ipv4_mapped_literal(self):
+        # since Python 3.13, the "alternative form" is used for
+        # IPv4-mapped addresses, see RFC 4291 2.2 p.3
+        cases = [
+            (
+                "http://[::12.34.56.78]:5432/foo/",
+                [
+                    "0000:0000:0000:0000:0000:0000:0c22:384e",
+                    "0000:0000:0000:0000:0000:0000:12.34.56.78",
+                ],
+                5432,
+            ),
+            (
+                "http://[::ffff:12.34.56.78]:5432/foo/",
+                [
+                    "0000:0000:0000:0000:0000:ffff:0c22:384e",
+                    "0000:0000:0000:0000:0000:ffff:12.34.56.78",
+                ],
+                5432,
+            ),
+            (
+                "http://[::12.34.56.78]/foo/",
+                [
+                    "0000:0000:0000:0000:0000:0000:0c22:384e",
+                    "0000:0000:0000:0000:0000:0000:12.34.56.78",
+                ],
+                None,
+            ),
+            (
+                "http://[::ffff:12.34.56.78]/foo/",
+                [
+                    "0000:0000:0000:0000:0000:ffff:0c22:384e",
+                    "0000:0000:0000:0000:0000:ffff:12.34.56.78",
+                ],
+                None,
+            ),
+            (
+                "http://[::12.34.56.78]:/foo/",
+                [
+                    "0000:0000:0000:0000:0000:0000:0c22:384e",
+                    "0000:0000:0000:0000:0000:0000:12.34.56.78",
+                ],
+                None,
+            ),
+            (
+                "http://[::ffff:12.34.56.78]:/foo/",
+                [
+                    "0000:0000:0000:0000:0000:ffff:0c22:384e",
+                    "0000:0000:0000:0000:0000:ffff:12.34.56.78",
+                ],
+                None,
+            ),
+        ]
+        for uri, hosts, port in cases:
             parts = urisplit(uri)
-            self.assertEqual(host, str(parts.gethost()))
-            self.assertEqual(port, parts.getport())
+            self.assertIn(parts.gethost().exploded, hosts)
+            self.assertEqual(parts.getport(), port)
             parts = urisplit(uri.encode("ascii"))
-            self.assertEqual(host, str(parts.gethost()))
-            self.assertEqual(port, parts.getport())
+            self.assertIn(parts.gethost().exploded, hosts)
+            self.assertEqual(parts.getport(), port)
 
     def test_invalid_ip_literal(self):
         uris = [
             "http://::12.34.56.78]/",
             "http://[::1/foo/",
             "ftp://[::1/foo/bad]/bad",
             "http://[::1/foo/bad]/bad",
```

### Comparing `uritools-4.0.2/tests/test_unsplit.py` & `uritools-4.0.3/tests/test_unsplit.py`

 * *Files identical despite different names*

### Comparing `uritools-4.0.2/tox.ini` & `uritools-4.0.3/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tox]
 envlist = check-manifest,docs,doctest,flake8,py
 
 [testenv]
 deps =
-    coverage
     pytest
     pytest-cov
 commands =
     py.test --basetemp={envtmpdir} --cov=uritools {posargs}
 
 [testenv:check-manifest]
 deps =
```

