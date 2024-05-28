# Comparing `tmp/cxxheaderparser-1.3.1.tar.gz` & `tmp/cxxheaderparser-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxxheaderparser-1.3.1.tar", last modified: Fri Jan 12 23:54:47 2024, max compression
+gzip compressed data, was "cxxheaderparser-1.3.2.tar", last modified: Tue May 28 03:51:29 2024, max compression
```

## Comparing `cxxheaderparser-1.3.1.tar` & `cxxheaderparser-1.3.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:47.317354 cxxheaderparser-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-12 23:54:47.317354 cxxheaderparser-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:47.309354 cxxheaderparser-1.3.1/cxxheaderparser/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:47.313354 cxxheaderparser-1.3.1/cxxheaderparser/_ply/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/_ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35252 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/_ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/gentest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24050 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    92806 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/parserstate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/tokfmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/cxxheaderparser/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:47.317354 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-12 23:54:47.000000 cxxheaderparser-1.3.1/cxxheaderparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 23:54:47.317354 cxxheaderparser-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 23:54:47.317354 cxxheaderparser-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_abv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)   127976 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_class_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33216 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_concepts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)    20107 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    45652 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_friends.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_numeric_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    31633 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)   117132 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_tokfmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_typefmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (127)    28808 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_using.py
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-01-12 23:54:39.000000 cxxheaderparser-1.3.1/tests/test_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:29.956971 cxxheaderparser-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-28 03:51:29.956971 cxxheaderparser-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:29.952971 cxxheaderparser-1.3.2/cxxheaderparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:29.952971 cxxheaderparser-1.3.2/cxxheaderparser/_ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/_ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35252 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/_ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/gentest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24050 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92836 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/parserstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/tokfmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/cxxheaderparser/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:29.956971 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 03:51:29.000000 cxxheaderparser-1.3.2/cxxheaderparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:51:29.956971 cxxheaderparser-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:51:29.956971 cxxheaderparser-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_abv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127976 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_class_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33216 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_concepts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20107 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45652 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_numeric_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31633 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117132 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_tokfmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_typefmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30483 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_using.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-28 03:51:25.000000 cxxheaderparser-1.3.2/tests/test_var.py
```

### Comparing `cxxheaderparser-1.3.1/LICENSE.txt` & `cxxheaderparser-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/PKG-INFO` & `cxxheaderparser-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxheaderparser
-Version: 1.3.1
+Version: 1.3.2
 Summary: Parse C++ header files and generate a data structure representing the class
 Home-page: https://github.com/robotpy/cxxheaderparser
 Author: Dustin Spicuzza
 Author-email: dustin@virtualroadside.com
 Maintainer: RobotPy Development Team
 Maintainer-email: robotpy@googlegroups.com
 License: BSD
```

### Comparing `cxxheaderparser-1.3.1/README.md` & `cxxheaderparser-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/_ply/lex.py` & `cxxheaderparser-1.3.2/cxxheaderparser/_ply/lex.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/dump.py` & `cxxheaderparser-1.3.2/cxxheaderparser/dump.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/gentest.py` & `cxxheaderparser-1.3.2/cxxheaderparser/gentest.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/lexer.py` & `cxxheaderparser-1.3.2/cxxheaderparser/lexer.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/options.py` & `cxxheaderparser-1.3.2/cxxheaderparser/options.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/parser.py` & `cxxheaderparser-1.3.2/cxxheaderparser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1037,15 +1037,17 @@
         self,
         tok: LexToken,
         doxygen: typing.Optional[str],
         template: typing.Optional[TemplateDecl] = None,
     ) -> None:
         self.state.location = tok.location
 
-        tok = self._next_token_must_be("NAME", "DBL_COLON", "namespace", "typename")
+        tok = self._next_token_must_be(
+            "NAME", "DBL_COLON", "namespace", "typename", "enum"
+        )
 
         if tok.type == "namespace":
             if template:
                 raise CxxParseError(
                     "unexpected using-directive when parsing alias-declaration", tok
                 )
             state = self.state
```

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/parserstate.py` & `cxxheaderparser-1.3.2/cxxheaderparser/parserstate.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/preprocessor.py` & `cxxheaderparser-1.3.2/cxxheaderparser/preprocessor.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/simple.py` & `cxxheaderparser-1.3.2/cxxheaderparser/simple.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/tokfmt.py` & `cxxheaderparser-1.3.2/cxxheaderparser/tokfmt.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/types.py` & `cxxheaderparser-1.3.2/cxxheaderparser/types.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser/visitor.py` & `cxxheaderparser-1.3.2/cxxheaderparser/visitor.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser.egg-info/PKG-INFO` & `cxxheaderparser-1.3.2/cxxheaderparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxheaderparser
-Version: 1.3.1
+Version: 1.3.2
 Summary: Parse C++ header files and generate a data structure representing the class
 Home-page: https://github.com/robotpy/cxxheaderparser
 Author: Dustin Spicuzza
 Author-email: dustin@virtualroadside.com
 Maintainer: RobotPy Development Team
 Maintainer-email: robotpy@googlegroups.com
 License: BSD
```

### Comparing `cxxheaderparser-1.3.1/cxxheaderparser.egg-info/SOURCES.txt` & `cxxheaderparser-1.3.2/cxxheaderparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/setup.py` & `cxxheaderparser-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_abv_template.py` & `cxxheaderparser-1.3.2/tests/test_abv_template.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_attributes.py` & `cxxheaderparser-1.3.2/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_class.py` & `cxxheaderparser-1.3.2/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_class_base.py` & `cxxheaderparser-1.3.2/tests/test_class_base.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_concepts.py` & `cxxheaderparser-1.3.2/tests/test_concepts.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_doxygen.py` & `cxxheaderparser-1.3.2/tests/test_doxygen.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_enum.py` & `cxxheaderparser-1.3.2/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_fn.py` & `cxxheaderparser-1.3.2/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_friends.py` & `cxxheaderparser-1.3.2/tests/test_friends.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_misc.py` & `cxxheaderparser-1.3.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_namespaces.py` & `cxxheaderparser-1.3.2/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_numeric_literals.py` & `cxxheaderparser-1.3.2/tests/test_numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_operators.py` & `cxxheaderparser-1.3.2/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_preprocessor.py` & `cxxheaderparser-1.3.2/tests/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_skip.py` & `cxxheaderparser-1.3.2/tests/test_skip.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_template.py` & `cxxheaderparser-1.3.2/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_tokfmt.py` & `cxxheaderparser-1.3.2/tests/test_tokfmt.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_typedef.py` & `cxxheaderparser-1.3.2/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_typefmt.py` & `cxxheaderparser-1.3.2/tests/test_typefmt.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_union.py` & `cxxheaderparser-1.3.2/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `cxxheaderparser-1.3.1/tests/test_using.py` & `cxxheaderparser-1.3.2/tests/test_using.py`

 * *Files 2% similar despite different names*

```diff
@@ -712,7 +712,68 @@
                             access="public",
                         ),
                     ],
                 )
             ]
         )
     )
+
+
+def test_using_enum_global() -> None:
+    content = """
+      namespace A {
+      using enum B::C;
+      }
+    """
+    data = parse_string(content, cleandoc=True)
+
+    assert data == ParsedData(
+        namespace=NamespaceScope(
+            namespaces={
+                "A": NamespaceScope(
+                    name="A",
+                    using=[
+                        UsingDecl(
+                            typename=PQName(
+                                segments=[
+                                    NameSpecifier(name="B"),
+                                    NameSpecifier(name="C"),
+                                ],
+                                classkey="enum",
+                            )
+                        )
+                    ],
+                )
+            }
+        )
+    )
+
+
+def test_using_enum_in_struct() -> None:
+    content = """
+      struct S {
+        using enum fruit;
+      };
+    """
+    data = parse_string(content, cleandoc=True)
+
+    assert data == ParsedData(
+        namespace=NamespaceScope(
+            classes=[
+                ClassScope(
+                    class_decl=ClassDecl(
+                        typename=PQName(
+                            segments=[NameSpecifier(name="S")], classkey="struct"
+                        )
+                    ),
+                    using=[
+                        UsingDecl(
+                            typename=PQName(
+                                segments=[NameSpecifier(name="fruit")], classkey="enum"
+                            ),
+                            access="public",
+                        )
+                    ],
+                )
+            ]
+        )
+    )
```

### Comparing `cxxheaderparser-1.3.1/tests/test_var.py` & `cxxheaderparser-1.3.2/tests/test_var.py`

 * *Files identical despite different names*

