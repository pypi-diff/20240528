# Comparing `tmp/lynxy-0.0.3.tar.gz` & `tmp/lynxy-0.0.4.tar.gz`

## Comparing `lynxy-0.0.3.tar` & `lynxy-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 lynxy-0.0.3/README.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 lynxy-0.0.3/z.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 lynxy-0.0.3/.gitignore/test.txt
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/pypi/lynxy-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/pypi/lynxy-0.0.1.tar.gz
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/pypi/lynxy-0.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/pypi/lynxy-0.0.2.tar.gz
--rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0    33220 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.1.tar.gz
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.10-py3-none-any.whl
--rw-r--r--   0        0        0    39627 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.10.tar.gz
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.2.tar.gz
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.3-py3-none-any.whl
--rw-r--r--   0        0        0    34444 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.3.tar.gz
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.4-py3-none-any.whl
--rw-r--r--   0        0        0    34461 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.4.tar.gz
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.5-py3-none-any.whl
--rw-r--r--   0        0        0    34344 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.5.tar.gz
--rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.6-py3-none-any.whl
--rw-r--r--   0        0        0    34340 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.6.tar.gz
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.7-py3-none-any.whl
--rw-r--r--   0        0        0    34421 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.7.tar.gz
--rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.8-py3-none-any.whl
--rw-r--r--   0        0        0    34593 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.8.tar.gz
--rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.9-py3-none-any.whl
--rw-r--r--   0        0        0    39133 2020-02-02 00:00:00.000000 lynxy-0.0.3/_old/testpypi/lynxy-0.1.9.tar.gz
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/github/lynxy.md
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/github/lynxy_server.md
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/txt/diagram.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/txt/sources.txt
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/txt/todo.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lynxy-0.0.3/src/lynxy/__init__.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 lynxy-0.0.3/src/lynxy/lynx.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 lynxy-0.0.3/src/lynxy_server/__init__.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 lynxy-0.0.3/src/lynxy_server/lynx_server.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lynxy-0.0.3/src/lynxy_server/responses.py
--rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/new_server.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/server.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/old/lynx.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/sock/modclient.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/templates-notes/socknotes.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 lynxy-0.0.3/tests/templates-notes/sockserver.py
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 lynxy-0.0.3/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lynxy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lynxy-0.0.3/info/pypi/PyPi_info.md
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 lynxy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 lynxy-0.0.4/README.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 lynxy-0.0.4/z.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 lynxy-0.0.4/.gitignore/test.txt
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.1.tar.gz
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.2.tar.gz
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0    33220 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.1.tar.gz
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.10-py3-none-any.whl
+-rw-r--r--   0        0        0    39627 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.10.tar.gz
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.2.tar.gz
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0    34444 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.3.tar.gz
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0    34461 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.4.tar.gz
+-rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.5-py3-none-any.whl
+-rw-r--r--   0        0        0    34344 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.5.tar.gz
+-rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.6-py3-none-any.whl
+-rw-r--r--   0        0        0    34340 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.6.tar.gz
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.7-py3-none-any.whl
+-rw-r--r--   0        0        0    34421 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.7.tar.gz
+-rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.8-py3-none-any.whl
+-rw-r--r--   0        0        0    34593 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.8.tar.gz
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.9-py3-none-any.whl
+-rw-r--r--   0        0        0    39133 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.9.tar.gz
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/github/lynxy.md
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/github/lynxy_server.md
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/diagram.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/sources.txt
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/todo.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy/__init__.py
+-rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy/lynx.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/__init__.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/lynx_server.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/responses.py
+-rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/new_server.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/server.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/old/lynx.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/sock/modclient.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/templates-notes/socknotes.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/templates-notes/sockserver.py
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 lynxy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lynxy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/pypi/PyPi_info.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 lynxy-0.0.4/PKG-INFO
```

### Comparing `lynxy-0.0.3/README.md` & `lynxy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/pypi/lynxy-0.0.1-py3-none-any.whl` & `lynxy-0.0.4/_old/pypi/lynxy-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/pypi/lynxy-0.0.1.tar.gz` & `lynxy-0.0.4/_old/pypi/lynxy-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/pypi/lynxy-0.0.2-py3-none-any.whl` & `lynxy-0.0.4/_old/pypi/lynxy-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/pypi/lynxy-0.0.2.tar.gz` & `lynxy-0.0.4/_old/pypi/lynxy-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.1-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.1.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.10-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.10-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.10.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.10.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.2-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.2.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.3-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.3.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.3.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.4-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.4.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.4.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.5-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.5.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.5.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.6-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.6-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.6.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.6.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.7-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.7.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.7.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.8-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.8.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.8.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.9-py3-none-any.whl` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.9-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/_old/testpypi/lynxy-0.1.9.tar.gz` & `lynxy-0.0.4/_old/testpypi/lynxy-0.1.9.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/info/github/lynxy.md` & `lynxy-0.0.4/info/github/lynxy.md`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/info/github/lynxy_server.md` & `lynxy-0.0.4/info/github/lynxy_server.md`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/info/txt/todo.txt` & `lynxy-0.0.4/info/txt/todo.txt`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/src/lynxy/lynx.py` & `lynxy-0.0.4/src/lynxy/lynx.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/src/lynxy_server/__init__.py` & `lynxy-0.0.4/src/lynxy_server/__init__.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/src/lynxy_server/lynx_server.py` & `lynxy-0.0.4/src/lynxy_server/lynx_server.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/src/lynxy_server/responses.py` & `lynxy-0.0.4/src/lynxy_server/responses.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/new_server.py` & `lynxy-0.0.4/tests/new_server.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/server.py` & `lynxy-0.0.4/tests/server.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/old/lynx.py` & `lynxy-0.0.4/tests/old/lynx.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/sock/modclient.py` & `lynxy-0.0.4/tests/sock/modclient.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/templates-notes/socknotes.py` & `lynxy-0.0.4/tests/templates-notes/socknotes.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/tests/templates-notes/sockserver.py` & `lynxy-0.0.4/tests/templates-notes/sockserver.py`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/LICENSE` & `lynxy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.3/pyproject.toml` & `lynxy-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "src/lynxy",
     "src/lynxy_server"
 ]
 
 [project]
 name = "lynxy"
 # version = "0.1.10" # middle number 1 is currently for test pypi
-version = "0.0.3" # pypi release 
+version = "0.0.4" # pypi release 
 authors = [
   { name="Sketched Doughnut", email="sketcheddoughnut@gmail.com" },
 ]
 description = "A LAN package made for easy communication and sending of data across the same network."
 readme = "info/pypi/PyPi_info.md"
 # requires-python = ">=3.10" 
 requires-python = ">=3.9" # changing which version it needs for test pypi, might keep for release for now - do note this release version works for linux(?) (python3)
```

### Comparing `lynxy-0.0.3/PKG-INFO` & `lynxy-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: lynxy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A LAN package made for easy communication and sending of data across the same network.
 Project-URL: Homepage, https://github.com/SketchedDoughnut/lynxy
 Project-URL: Issues, https://github.com/SketchedDoughnut/lynxy/issues
 Author-email: Sketched Doughnut <sketcheddoughnut@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
-# **lynx**
-Local (yielding?) Network (eXchange?)
+# **lynxy**
+Local (yielding?) Network (eXchange?) (the y is cosmetic)
 
 # **Introduction**
 lynxy, also known as lynx, is a LAN server-client system coded in Python. It allows for easy setup of a server, as well as easy setup for clients on the same network as the server. 
 Check out the github below to learn how to use this module.
-- Github: https://github.com/SketchedDoughnut/LYNX
+- Github: https://github.com/SketchedDoughnut/lynxy
```

