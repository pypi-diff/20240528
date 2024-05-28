# Comparing `tmp/tc-wikipedia-lib-1.0.0.tar.gz` & `tmp/tc-wikipedia-lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-wikipedia-lib-1.0.0.tar", last modified: Tue May 21 12:41:07 2024, max compression
+gzip compressed data, was "tc-wikipedia-lib-1.0.1.tar", last modified: Tue May 28 12:14:12 2024, max compression
```

## Comparing `tc-wikipedia-lib-1.0.0.tar` & `tc-wikipedia-lib-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-21 12:41:07.942994 tc-wikipedia-lib-1.0.0/
--rw-r--r--   0 equinox   (1000) equinox   (1000)     1057 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/LICENSE
--rw-r--r--   0 equinox   (1000) equinox   (1000)       43 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/MANIFEST.in
--rw-r--r--   0 equinox   (1000) equinox   (1000)     4577 2024-05-21 12:41:07.942994 tc-wikipedia-lib-1.0.0/PKG-INFO
--rw-r--r--   0 equinox   (1000) equinox   (1000)     3966 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/README.rst
--rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/requirements.txt
--rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-21 12:41:07.942994 tc-wikipedia-lib-1.0.0/setup.cfg
--rw-r--r--   0 equinox   (1000) equinox   (1000)     1134 2024-05-21 12:07:51.000000 tc-wikipedia-lib-1.0.0/setup.py
-drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-21 12:41:07.942994 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/
--rw-r--r--   0 equinox   (1000) equinox   (1000)     4577 2024-05-21 12:41:07.000000 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/PKG-INFO
--rw-r--r--   0 equinox   (1000) equinox   (1000)      342 2024-05-21 12:41:07.000000 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/SOURCES.txt
--rw-r--r--   0 equinox   (1000) equinox   (1000)        1 2024-05-21 12:41:07.000000 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/dependency_links.txt
--rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-21 12:41:07.000000 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/requires.txt
--rw-r--r--   0 equinox   (1000) equinox   (1000)       10 2024-05-21 12:41:07.000000 tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/top_level.txt
-drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-21 12:41:07.942994 tc-wikipedia-lib-1.0.0/wikipedia/
--rw-r--r--   0 equinox   (1000) equinox   (1000)       76 2024-05-21 12:39:47.000000 tc-wikipedia-lib-1.0.0/wikipedia/__init__.py
--rw-r--r--   0 equinox   (1000) equinox   (1000)     2280 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/wikipedia/exceptions.py
--rw-r--r--   0 equinox   (1000) equinox   (1000)      985 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.0/wikipedia/util.py
--rw-r--r--   0 equinox   (1000) equinox   (1000)    20796 2024-05-16 16:58:13.000000 tc-wikipedia-lib-1.0.0/wikipedia/wikipedia.py
+drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-28 12:14:12.897768 tc-wikipedia-lib-1.0.1/
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     1057 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/LICENSE
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       43 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/MANIFEST.in
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     4577 2024-05-28 12:14:12.897768 tc-wikipedia-lib-1.0.1/PKG-INFO
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     3966 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/README.rst
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/requirements.txt
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-28 12:14:12.897768 tc-wikipedia-lib-1.0.1/setup.cfg
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     1134 2024-05-21 12:07:51.000000 tc-wikipedia-lib-1.0.1/setup.py
+drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-28 12:14:12.897768 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     4577 2024-05-28 12:14:12.000000 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/PKG-INFO
+-rw-r--r--   0 equinox   (1000) equinox   (1000)      342 2024-05-28 12:14:12.000000 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 equinox   (1000) equinox   (1000)        1 2024-05-28 12:14:12.000000 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       38 2024-05-28 12:14:12.000000 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/requires.txt
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       10 2024-05-28 12:14:12.000000 tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/top_level.txt
+drwxr-xr-x   0 equinox   (1000) equinox   (1000)        0 2024-05-28 12:14:12.897768 tc-wikipedia-lib-1.0.1/wikipedia/
+-rw-r--r--   0 equinox   (1000) equinox   (1000)       76 2024-05-28 12:12:25.000000 tc-wikipedia-lib-1.0.1/wikipedia/__init__.py
+-rw-r--r--   0 equinox   (1000) equinox   (1000)     2280 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/wikipedia/exceptions.py
+-rw-r--r--   0 equinox   (1000) equinox   (1000)      985 2024-05-16 16:56:37.000000 tc-wikipedia-lib-1.0.1/wikipedia/util.py
+-rw-r--r--   0 equinox   (1000) equinox   (1000)    21672 2024-05-28 11:28:50.000000 tc-wikipedia-lib-1.0.1/wikipedia/wikipedia.py
```

### Comparing `tc-wikipedia-lib-1.0.0/LICENSE` & `tc-wikipedia-lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tc-wikipedia-lib-1.0.0/PKG-INFO` & `tc-wikipedia-lib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-wikipedia-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wikimedia API for Python
 Home-page: https://github.com/polux0/Wikipedia
 Author: Jonathan Goldsmith, modified by Aleksa Stojanović
 Author-email: alexusnavas@gmail.com
 License: MIT
 Keywords: python wikimedia API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tc-wikipedia-lib-1.0.0/README.rst` & `tc-wikipedia-lib-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tc-wikipedia-lib-1.0.0/setup.py` & `tc-wikipedia-lib-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tc-wikipedia-lib-1.0.0/tc_wikipedia_lib.egg-info/PKG-INFO` & `tc-wikipedia-lib-1.0.1/tc_wikipedia_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-wikipedia-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wikimedia API for Python
 Home-page: https://github.com/polux0/Wikipedia
 Author: Jonathan Goldsmith, modified by Aleksa Stojanović
 Author-email: alexusnavas@gmail.com
 License: MIT
 Keywords: python wikimedia API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tc-wikipedia-lib-1.0.0/wikipedia/exceptions.py` & `tc-wikipedia-lib-1.0.1/wikipedia/exceptions.py`

 * *Files identical despite different names*

### Comparing `tc-wikipedia-lib-1.0.0/wikipedia/util.py` & `tc-wikipedia-lib-1.0.1/wikipedia/util.py`

 * *Files identical despite different names*

### Comparing `tc-wikipedia-lib-1.0.0/wikipedia/wikipedia.py` & `tc-wikipedia-lib-1.0.1/wikipedia/wikipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,29 +457,50 @@
     return self._html
 
   @property
   def content(self):
     '''
     Plain text content of the page, excluding images, tables, and other data.
     '''
-
     if not getattr(self, '_content', False):
-      query_params = {
-        'prop': 'extracts|revisions',
-        'explaintext': '',
-        'rvprop': 'ids'
-      }
-      if not getattr(self, 'title', None) is None:
-         query_params['titles'] = self.title
-      else:
-         query_params['pageids'] = self.pageid
-      request = _wiki_request(query_params)
-      self._content     = request['query']['pages'][self.pageid]['extract']
-      self._revision_id = request['query']['pages'][self.pageid]['revisions'][0]['revid']
-      self._parent_id   = request['query']['pages'][self.pageid]['revisions'][0]['parentid']
+        query_params = {
+            'prop': 'extracts|revisions',
+            'explaintext': '',
+            'rvprop': 'ids|content'
+        }
+        if not getattr(self, 'title', None) is None:
+            query_params['titles'] = self.title
+        else:
+            query_params['pageids'] = self.pageid
+        # Check if the API is for Wikitravel
+        if "wikitravel.org" in API_URL:
+            query_params = {
+                'prop': 'revisions',
+                'rvprop': 'content',
+                'rvlimit': 1,
+            }
+            if not getattr(self, 'title', None) is None:
+                query_params['titles'] = self.title
+            else:
+                query_params['pageids'] = self.pageid
+        request = _wiki_request(query_params)
+        try:
+            if "wikitravel.org" in API_URL:
+                self._content = request['query']['pages'][self.pageid]['revisions'][0]['*']
+            else:
+                self._content = request['query']['pages'][self.pageid]['extract']
+        except KeyError:
+            # Handle case where 'extract' is not present
+            self._content = "Content not available."
+        try:
+            self._revision_id = request['query']['pages'][self.pageid]['revisions'][0]['revid']
+            self._parent_id = request['query']['pages'][self.pageid]['revisions'][0]['parentid']
+        except KeyError:
+            self._revision_id = None
+            self._parent_id = None
 
     return self._content
 
   @property
   def revision_id(self):
     '''
     Revision ID of the page.
```

