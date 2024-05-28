# Comparing `tmp/lynxy-0.0.4.tar.gz` & `tmp/lynxy-0.0.5.tar.gz`

## Comparing `lynxy-0.0.4.tar` & `lynxy-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 lynxy-0.0.4/README.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 lynxy-0.0.4/z.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 lynxy-0.0.4/.gitignore/test.txt
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.1.tar.gz
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/pypi/lynxy-0.0.2.tar.gz
--rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0    33220 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.1.tar.gz
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.10-py3-none-any.whl
--rw-r--r--   0        0        0    39627 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.10.tar.gz
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.2.tar.gz
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.3-py3-none-any.whl
--rw-r--r--   0        0        0    34444 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.3.tar.gz
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.4-py3-none-any.whl
--rw-r--r--   0        0        0    34461 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.4.tar.gz
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.5-py3-none-any.whl
--rw-r--r--   0        0        0    34344 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.5.tar.gz
--rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.6-py3-none-any.whl
--rw-r--r--   0        0        0    34340 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.6.tar.gz
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.7-py3-none-any.whl
--rw-r--r--   0        0        0    34421 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.7.tar.gz
--rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.8-py3-none-any.whl
--rw-r--r--   0        0        0    34593 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.8.tar.gz
--rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.9-py3-none-any.whl
--rw-r--r--   0        0        0    39133 2020-02-02 00:00:00.000000 lynxy-0.0.4/_old/testpypi/lynxy-0.1.9.tar.gz
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/github/lynxy.md
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/github/lynxy_server.md
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/diagram.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/sources.txt
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/txt/todo.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy/__init__.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy/lynx.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/__init__.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/lynx_server.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lynxy-0.0.4/src/lynxy_server/responses.py
--rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/new_server.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/server.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/old/lynx.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/sock/modclient.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/templates-notes/socknotes.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 lynxy-0.0.4/tests/templates-notes/sockserver.py
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 lynxy-0.0.4/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lynxy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 lynxy-0.0.4/info/pypi/PyPi_info.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 lynxy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 lynxy-0.0.5/README.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 lynxy-0.0.5/z.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 lynxy-0.0.5/.gitignore/test.txt
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/pypi/lynxy-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/pypi/lynxy-0.0.1.tar.gz
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/pypi/lynxy-0.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/pypi/lynxy-0.0.2.tar.gz
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0    33220 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.1.tar.gz
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.10-py3-none-any.whl
+-rw-r--r--   0        0        0    39627 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.10.tar.gz
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.2.tar.gz
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0    34444 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.3.tar.gz
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0    34461 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.4.tar.gz
+-rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.5-py3-none-any.whl
+-rw-r--r--   0        0        0    34344 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.5.tar.gz
+-rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.6-py3-none-any.whl
+-rw-r--r--   0        0        0    34340 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.6.tar.gz
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.7-py3-none-any.whl
+-rw-r--r--   0        0        0    34421 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.7.tar.gz
+-rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.8-py3-none-any.whl
+-rw-r--r--   0        0        0    34593 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.8.tar.gz
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.9-py3-none-any.whl
+-rw-r--r--   0        0        0    39133 2020-02-02 00:00:00.000000 lynxy-0.0.5/_old/testpypi/lynxy-0.1.9.tar.gz
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/github/lynxy.md
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/github/lynxy_server.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/txt/diagram.txt
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/txt/sources.txt
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/txt/todo.txt
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 lynxy-0.0.5/src/lynxy/__init__.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 lynxy-0.0.5/src/lynxy/lynx.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 lynxy-0.0.5/src/lynxy_server/__init__.py
+-rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 lynxy-0.0.5/src/lynxy_server/lynx_server.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 lynxy-0.0.5/src/lynxy_server/responses.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/new_server.py
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/server.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/old/lynx.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/sock/modclient.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/templates-notes/socknotes.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 lynxy-0.0.5/tests/templates-notes/sockserver.py
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 lynxy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 lynxy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 lynxy-0.0.5/info/pypi/PyPi_info.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 lynxy-0.0.5/PKG-INFO
```

### Comparing `lynxy-0.0.4/README.md` & `lynxy-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-<!-- Default start messages -->
-# **lynxy**
-Local (yielding?) Network (eXchange?) (the extra y is cosmetic~)
-
-# **Introduction**
-lynxy, also known as lynx, is a LAN server-client system coded in Python. It allows for easy setup of a server, as well as easy setup for clients on the same network as the server.
-The use of this module is so that if people were to make programs that require a LAN system, they can use what is provided here.
-The first section will explain instructions that apply to both, and then we will cover each individual part.
-
-# **General setup**
-Before we do anything, you should first install this module with pip. <br></br>
-`pip install (TBD)`
-`python3 -m pip install (TBD)` <br></br>
-When you do this, it will install both the modules "lynxy" and "lynxy_server". Once this is done, you are ready to read the instructions on the following sections about setting up your client, server, or both.
-
-
-
-# Server setup
-To access server setup, go [**here**](./info/github/lynxy_server.md)
-
-# Client setup
-To access client setup, go [**here**](./info/github/lynxy.md)
-
-# Etc
-You can find more info about functions by looking at the descriptions of them in your code editor.
+<!-- Default start messages -->
+# **lynxy**
+Local (yielding?) Network (eXchange?) (the extra y is cosmetic~)
+
+# **Introduction**
+lynxy, also known as lynx, is a LAN server-client system coded in Python. It allows for easy setup of a server, as well as easy setup for clients on the same network as the server.
+The use of this module is so that if people were to make programs that require a LAN system, they can use what is provided here. <br>
+This project is also named after my ~ windy ~ friend :3 <br>
+The first section will explain instructions that apply to both, and then we will cover each individual part.
+
+# **General setup**
+Before we do anything, you should first install this module with pip. <br></br>
+`pip install lynxy` <br>
+`python3 -m pip install lynxy` <br> <br>
+When you do this, it will install both the modules "lynxy" and "lynxy_server". Once this is done, you are ready to read the instructions on the following sections about setting up your client, server, or both.
+
+
+
+# Server setup
+To access server setup, go [**here**](./info/github/lynxy_server.md)
+
+# Client setup
+To access client setup, go [**here**](./info/github/lynxy.md)
+
+# Etc
+You can find more info about functions by looking at the descriptions of them in your code editor.
```

### Comparing `lynxy-0.0.4/_old/pypi/lynxy-0.0.1-py3-none-any.whl` & `lynxy-0.0.5/_old/pypi/lynxy-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/pypi/lynxy-0.0.1.tar.gz` & `lynxy-0.0.5/_old/pypi/lynxy-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/pypi/lynxy-0.0.2-py3-none-any.whl` & `lynxy-0.0.5/_old/pypi/lynxy-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/pypi/lynxy-0.0.2.tar.gz` & `lynxy-0.0.5/_old/pypi/lynxy-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.1-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.1.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.10-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.10-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.10.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.10.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.2-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.2.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.3-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.3.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.3.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.4-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.4.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.4.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.5-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.5.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.5.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.6-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.6-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.6.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.6.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.7-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.7.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.7.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.8-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.8.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.8.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.9-py3-none-any.whl` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.9-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/_old/testpypi/lynxy-0.1.9.tar.gz` & `lynxy-0.0.5/_old/testpypi/lynxy-0.1.9.tar.gz`

 * *Files identical despite different names*

### Comparing `lynxy-0.0.4/info/github/lynxy.md` & `lynxy-0.0.5/info/github/lynxy.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 
 
 ***
 # Starting your client
 To start your client, all you need to do is call one function, passing in the ip of the server. In this example, we use a loopback address: <br>
 - `lynxy.start_client('127.0.0.1')`
+  **ARGS: None -> returns bool on status of connection**
     - To get the servers ip, please refer to the server setup page, specifically the section named ["Starting the server"](lynxy_server.md#starting-the-server). This IP should be distributed to anyone with the code containing the lynxy client code.
  
 ***
 # Client communication function explanations
 This section is dedicated towards explaining the functions that the lynxy module has.
 - `lynxy.submit_username_data()` 
   - **ARGS: username: str -> returns string from server**
```

### Comparing `lynxy-0.0.4/info/github/lynxy_server.md` & `lynxy-0.0.5/info/github/lynxy_server.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-# Table of contents
-[Server setup](./lynxy_server.md#server-setup) <br>
-[Configuring your server](./lynxy_server.md#configuring-your-server) <br>
-[Starting the server](./lynxy_server.md#starting-the-server) <br>
-[Server response key](./lynxy_server.md#server-response-key) <br>
-[Server functions key](./lynxy_server.md#server-functions-key) <br>
-[Other functions](./lynxy_server.md#other-functions) 
-***
-
-
-
-
-# Server setup
-To set up the server module, you first need to import it. <br>
-`import lynxy_server` <br>
-Next, there is some customization you can do. However, if you want to just start the server, skip to "Starting your server"
-
-
-
-
-
-
-
-
-
-
-
-<!-- Instructions on how to configure the server -->
-***
-# Configuring your server <br>
-The server has a couple of parameters that can be overriden. These are: 
-- the ports it attempts to connect to
-- the IP it tries to run on 
-- whether the program prints or not
-
-
-**Overriding ports** <br>
-The server has a default list of ports it will try to connect to. These ports are:
-1.  11111 
-2.  12111 
-3.  11211 
-4.  11121 
-5.  11112 
-6.  22111 
-7.  12211 
-8.  11221 
-9.  11122 
-10. 22222 
-
-It cycles through these ports so that if one is not available, it can still launch itself. You can override these ports by running the function below, and passing in a list with one or more ports (in integer form). There is no limit for how many ports you can pass into it. In this example, we use three random ports: <br>
-`lynxy_server.override_ports([12345, 67890, 17390])` <br>
-**NOTE**: YOU MUST HAVE PORTS ON THE CLIENT AND THE SERVER THAT ARE THE SAME, SO THAT THEY CAN FIND EACH OTHER
-
-
-**Overriding IP** <br>
-The server uses the ipv4 IP of the device it is running on. It is advised to not change this. However, if you want to override the IP, you can use the following function, inputting a string. <br>
-`lynxy_server.override_ip("123.456.789.0")`
-
-
-**Overriding prints** <br>
-If you don't want any console message to be printed, use the following command: <br>
-`lynxy_server.disable_print()` <br>
-If you want to enable printing, use the following command: <br>
-`lynxy_server.enable_print()` <br>
-**NOTE**: Prints are enabled by default.
-
-
-
-
-
-
-
-
-
-
-<!-- Instructions on how to start the server -->
-***
-# Starting the server
-To start your server, you have a couple of options. Here is the rundown: <br>
-- `lynxy_server.start_server()`
-  - This option will not block your code, as it will run the server in a seperate thread. This allows for use of functions such as `lynxy_server.get_data()`, and more.
-  - If you disable print and then call on this function, absolutely nothing will be printed. You can get the IP the server is on, the port the server is on, and the session token from `lynxy_server.get_data()`. Alternatively, `lynxy_server.start_server()` returns a tuple containing all of these (in respective order) which you can also use to get data from. Clients will need the IP address to connect to the server, and if you want to remotely control the server then you will also need the session token. Usage of this token is elaborated on more in the client setup page.
-  - **PLEASE NOTE**: If you use this function, and there is no code continuing after it, the file will finish. This means that the server will get terminated. To prevent this, please include some sort of loop system AFTER calling the function that keeps the file in which you called on this function active, as to not close the server.
-- `lynxy_server.no_thread_start_server()`
-  - This option will block your code, as it is directly running the server. This does not allow for any code to run after this function is called, until the server goes offline. The server will only go offline if it crashes, or if someone remotely shuts it down by authorizing their user, and then commanding the server to shut down. This is explained more in the client setup page, and the shutdown feature is explained below. <br>
-
-**BEFORE CONTINUING**: Check the IP your server is on. If it is on an ip such as 127.0.0.1, then it will not work. You need the public ipv4 address of the device running the server, typically labeled with "LAN" or something of the sort.
- 
-***
-# Server response key
-The server has a variety of numbers it will return as responses to actions. Codes from 0 to 99 are status codes. Codes from 100 to 199 is regarding invalid messages from the clients. Codes from 200 to 299 are regarding system settings, set by an authorized client. These include being denied if you do not have the right permissions.
-The key is below. 
-- 000
-  - the operation was successful
-- 001
-  - the server failed to do an operation
-- 002
-  - the client requested to end the communication channel with the server
-- 003
-  - the message the the client sent to the server is not connected to any command, and so it did nothing
-- 004
-  - The session between the server and client crashed
-- 100
-  - the client requested data associated with a username that does not exist
-- 101
-  - the user tried to authorize themself, but had an invalid auth token
-- 102
-  - the user has not been authorized, and can not do what they just tried to
-- 103
-  - The message is invalid (meaning it is empty or corrupt in some way)
-- 200
-  - the server has been commanded to deny every client that connects to it
-
-
-
-
-
-***
-# Server functions key
-There are set commands that one can send to the server, from the client. They are as follows. <br>
-**NOTE**: The functions used here are: `lynxy.submit_username_data()`, `lynxy.request_username_data()`, `lynxy.send_msg()`.
-These functions are elaborated on more in the client setup page, but what you do need to know is that they all return data.
-
-- **username (name)**
-  - This argument submits a username to the server database. Example usage is below.
-    - `lynxy.submit_username_data('SketchedDoughnut')`
-    - or `lynxy.send_msg('username SketchedDougnut')`
-  - **NOTE**: NO SPACES ARE ALLOWED, AND WILL BE REMOVED FROM YOUR USERNAME UPON SUBMISSION
-
-- **request_by_user (name)**
-  - This argument requests the data (data being IP, port) associated with a username that is pre-existing in the servers database. Example usage is below.
-    - `lynxy.request_username_data('SketchedDoughnut')`
-    - or `lynxy.send_msg('request_by_user SketchedDougnut' )`
-  - **NOTE**: NO SPACES ARE ALLOWED, AND WILL BE REMOVED FROM YOUR USERNAME UPON SUBMISSION
-
-- **auth (token)**
-  - This argument attempts to authorize the client. If the token is equal to the session token generated on the servers start, then the client will be authorized. Example usage is below.
-    - `lynxy.send_msg('auth (token)' )`
-
-- **clear_client**
-  - If the user is authorized, this argument will clear the client dictionary. This is helpful if, for some reason, you would need to reset it. Example usage is below.
-    - `lynxy.send_msg('clear_client' )`
-
-- **freeze_server**
-  - If the user is authorized, this function will freeze the server. This will either make the server not exist for new clients, and/or severe the current connections with the clients. This function is intended for use if someone does not have direct access to the computer itself, or if you are running the server with `lynxy_server.no_thread_start_server()`. The reason why is because if you run the server directly instead of via a thread, you would not be able to call on the dedicated function for freezing the server, as your code would be blocked. This is a get-around to that. Example usage is below.
-    - `lynxy.send_msg('freeze_server' )`
-
-- **end_session**
-  - This argument ends the session between the client and the server. Example usage is below.
-    - `lynxy.send_msg('end_session' )`
-
-
-
-
-
-
-
-
-
-***
-# Other functions
-- `lynxy_server.get_data()` -> This function will only work if you are using the threaded start function, and will return the following data in a dictionary:
-  - server info
-    - if the server is alive or not (bool)
-    - the ip the server is on (string)
-    - the port the server is on (int)
-  - client info (dict)
-    - example username (str)
-      - (example ip, example port) (tuple)
-- `lynxy_server.freeze_server()` -> will freeze the server, and return a reponse telling you whether it worked or not. Freezing the server means it will render the server unusable, but the file will still be running. This is meant to disable the server until a person can physically access the computer and disable it from there. 
-- `lynxy_server.help()` -> has an optional argument, if it is set to True it will open a link to the Github page for this project. Otherwise, it will return a link to that page.
-- `lynxy_server.license()` -> has an optional argument, if it is set to True it will open a link to the license page on the Github for this project. Otherwise, it will return a link to that page.
+# Table of contents
+[Server setup](./lynxy_server.md#server-setup) <br>
+[Configuring your server](./lynxy_server.md#configuring-your-server) <br>
+[Starting the server](./lynxy_server.md#starting-the-server) <br>
+[Server response key](./lynxy_server.md#server-response-key) <br>
+[Server functions key](./lynxy_server.md#server-functions-key) <br>
+[Other functions](./lynxy_server.md#other-functions) 
+***
+
+
+
+
+# Server setup
+To set up the server module, you first need to import it. <br>
+`import lynxy_server` <br>
+Next, there is some customization you can do. However, if you want to just start the server, skip to "Starting your server"
+
+
+
+
+
+
+
+
+
+
+
+<!-- Instructions on how to configure the server -->
+***
+# Configuring your server <br>
+The server has a couple of parameters that can be overriden. These are: 
+- the ports it attempts to connect to
+- the IP it tries to run on 
+- whether the program prints or not
+
+
+**Overriding ports** <br>
+The server has a default list of ports it will try to connect to. These ports are:
+1.  11111 
+2.  12111 
+3.  11211 
+4.  11121 
+5.  11112 
+6.  22111 
+7.  12211 
+8.  11221 
+9.  11122 
+10. 22222 
+
+It cycles through these ports so that if one is not available, it can still launch itself. You can override these ports by running the function below, and passing in a list with one or more ports (in integer form). There is no limit for how many ports you can pass into it. In this example, we use three random ports: <br>
+`lynxy_server.override_ports([12345, 67890, 17390])` <br>
+**NOTE**: YOU MUST HAVE PORTS ON THE CLIENT AND THE SERVER THAT ARE THE SAME, SO THAT THEY CAN FIND EACH OTHER
+
+
+**Overriding IP** <br>
+The server uses the ipv4 IP of the device it is running on. It is advised to not change this. However, if you want to override the IP, you can use the following function, inputting a string. <br>
+`lynxy_server.override_ip("123.456.789.0")`
+
+
+**Overriding prints** <br>
+If you don't want any console message to be printed, use the following command: <br>
+`lynxy_server.disable_print()` <br>
+If you want to enable printing, use the following command: <br>
+`lynxy_server.enable_print()` <br>
+**NOTE**: Prints are enabled by default.
+
+
+
+
+
+
+
+
+
+
+<!-- Instructions on how to start the server -->
+***
+# Starting the server
+To start your server, you have a couple of options. Here is the rundown: <br>
+- `lynxy_server.start_server()`
+  - This option will not block your code, as it will run the server in a seperate thread. This allows for use of functions such as `lynxy_server.get_data()`, and more.
+  - If you disable print and then call on this function, absolutely nothing will be printed. You can get the IP the server is on, the port the server is on, and the session token from `lynxy_server.get_data()`. Alternatively, `lynxy_server.start_server()` returns a tuple containing all of these (in respective order) which you can also use to get data from. Clients will need the IP address to connect to the server, and if you want to remotely control the server then you will also need the session token. Usage of this token is elaborated on more in the client setup page.
+  - **PLEASE NOTE**: If you use this function, and there is no code continuing after it, the file will finish. This means that the server will get terminated. To prevent this, please include some sort of loop system AFTER calling the function that keeps the file in which you called on this function active, as to not close the server.
+- `lynxy_server.no_thread_start_server()`
+  - This option will block your code, as it is directly running the server. This does not allow for any code to run after this function is called, until the server goes offline. The server will only go offline if it crashes, or if someone remotely shuts it down by authorizing their user, and then commanding the server to shut down. This is explained more in the client setup page, and the shutdown feature is explained below. <br>
+
+**BEFORE CONTINUING**: Check the IP your server is on. If it is on an ip such as 127.0.0.1, then it will not work. You need the public ipv4 address of the device running the server, typically labeled with "LAN" or something of the sort.
+ 
+***
+# Server response key
+The server has a variety of numbers it will return as responses to actions. Codes from 0 to 99 are status codes. Codes from 100 to 199 is regarding invalid messages from the clients. Codes from 200 to 299 are regarding system settings, set by an authorized client. These include being denied if you do not have the right permissions.
+The key is below. 
+- 000
+  - the operation was successful
+- 001
+  - the server failed to do an operation
+- 002
+  - the client requested to end the communication channel with the server
+- 003
+  - the message the the client sent to the server is not connected to any command, and so it did nothing
+- 004
+  - The session between the server and client crashed
+- 100
+  - the client requested data associated with a username that does not exist
+- 101
+  - the user tried to authorize themself, but had an invalid auth token
+- 102
+  - the user has not been authorized, and can not do what they just tried to
+- 103
+  - The message is invalid (meaning it is empty or corrupt in some way)
+- 200
+  - the server has been commanded to deny every client that connects to it
+
+
+
+
+
+***
+# Server functions key
+There are set commands that one can send to the server, from the client. They are as follows. <br>
+**NOTE**: The functions used here are: `lynxy.submit_username_data()`, `lynxy.request_username_data()`, `lynxy.send_msg()`.
+These functions are elaborated on more in the client setup page, but what you do need to know is that they all return data.
+
+- **username (name)**
+  - This argument submits a username to the server database. Example usage is below.
+    - `lynxy.submit_username_data('SketchedDoughnut')`
+    - or `lynxy.send_msg('username SketchedDougnut')`
+  - **NOTE**: NO SPACES ARE ALLOWED, AND WILL BE REMOVED FROM YOUR USERNAME UPON SUBMISSION
+
+- **request_by_user (name)**
+  - This argument requests the data (data being IP, port) associated with a username that is pre-existing in the servers database. Example usage is below.
+    - `lynxy.request_username_data('SketchedDoughnut')`
+    - or `lynxy.send_msg('request_by_user SketchedDougnut' )`
+  - **NOTE**: NO SPACES ARE ALLOWED, AND WILL BE REMOVED FROM YOUR USERNAME UPON SUBMISSION
+
+- **auth (token)**
+  - This argument attempts to authorize the client. If the token is equal to the session token generated on the servers start, then the client will be authorized. Example usage is below.
+    - `lynxy.send_msg('auth (token)' )`
+
+- **clear_client**
+  - If the user is authorized, this argument will clear the client dictionary. This is helpful if, for some reason, you would need to reset it. Example usage is below.
+    - `lynxy.send_msg('clear_client' )`
+
+- **freeze_server**
+  - If the user is authorized, this function will freeze the server. This will either make the server not exist for new clients, and/or severe the current connections with the clients. This function is intended for use if someone does not have direct access to the computer itself, or if you are running the server with `lynxy_server.no_thread_start_server()`. The reason why is because if you run the server directly instead of via a thread, you would not be able to call on the dedicated function for freezing the server, as your code would be blocked. This is a get-around to that. Example usage is below.
+    - `lynxy.send_msg('freeze_server' )`
+
+- **end_session**
+  - This argument ends the session between the client and the server. Example usage is below.
+    - `lynxy.send_msg('end_session' )`
+
+
+
+
+
+
+
+
+
+***
+# Other functions
+- `lynxy_server.get_data()` -> This function will only work if you are using the threaded start function, and will return the following data in a dictionary:
+  - server info
+    - if the server is alive or not (bool)
+    - the ip the server is on (string)
+    - the port the server is on (int)
+  - client info (dict)
+    - example username (str)
+      - (example ip, example port) (tuple)
+- `lynxy_server.freeze_server()` -> will freeze the server, and return a reponse telling you whether it worked or not. Freezing the server means it will render the server unusable, but the file will still be running. This is meant to disable the server until a person can physically access the computer and disable it from there. 
+- `lynxy_server.help()` -> has an optional argument, if it is set to True it will open a link to the Github page for this project. Otherwise, it will return a link to that page.
+- `lynxy_server.license()` -> has an optional argument, if it is set to True it will open a link to the license page on the Github for this project. Otherwise, it will return a link to that page.
 - `lynxy_server.credits()` -> will return a string containing information about the credits for this project.
```

### Comparing `lynxy-0.0.4/info/txt/todo.txt` & `lynxy-0.0.5/info/txt/todo.txt`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-This is the goal for how we want this to work.
-
-THINGS THE USER DOES NOT HAVE ACCESS TO: 
-- __cycle_port__
-
-THINGS THE USER DOES HAVE ACCESS TO: 
-- valid_ports
-- HOST
-- submit_username_data()
-- request_username_data()
-- general_send()
-- start_connection()
-
-
-    
-WORKFLOW
-- MOST IMPORTANTLY, the user chooses if they want to use the server option or the client option
-- FOR THE CLIENT:
-    - WHAT THEY CAN OVERRIDE:
-        - if the user wants, they can override the valid ports (ONLY IF THEY KNOW WHAT THEY ARE DOING)
-        - if the user wants, they can override the default ip (empty) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
-        - if the user wants, they can override the selected port (THIS IS HIGHLY NOT RECOMMENDED)
-        - if the user wants, they can override the main_client (socket object) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
-    
-    - WHAT THEY CAN SET UP:
-        - The user starts a connection to the server 
-            - start_connection()
-        - The user sets their username (no spaces)
-        - The user submits their username data to the server 
-            - submit_username_data(username)
-        - The user requests data assigned to the other players username from the server
-            - request_data(username)
-    
-    - TO BE DONE:
-        - The user runs a function to attempt to connect to the other client
-            - if succeeds, closes server connection
-            - if fails after 3 tries, returns failed
-
-- FOR THE SERVER:
-    - WHAT THEY CAN OVERRIDE:
-        - if the user wants, they can override the valid ports (ONLY IF THEY KNOW WHAT THEY ARE DOING)
-        - if the user wants, they can override the default ip (empty) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
-        - if the user wants, they can override the selected port (THIS IS HIGHLY NOT RECOMMENDED)
-
-    - WHAT THEY CAN SET UP:
-        - the user starts the server
-
-    - TO BE DONE:
+This is the goal for how we want this to work.
+
+THINGS THE USER DOES NOT HAVE ACCESS TO: 
+- __cycle_port__
+
+THINGS THE USER DOES HAVE ACCESS TO: 
+- valid_ports
+- HOST
+- submit_username_data()
+- request_username_data()
+- general_send()
+- start_connection()
+
+
+    
+WORKFLOW
+- MOST IMPORTANTLY, the user chooses if they want to use the server option or the client option
+- FOR THE CLIENT:
+    - WHAT THEY CAN OVERRIDE:
+        - if the user wants, they can override the valid ports (ONLY IF THEY KNOW WHAT THEY ARE DOING)
+        - if the user wants, they can override the default ip (empty) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
+        - if the user wants, they can override the selected port (THIS IS HIGHLY NOT RECOMMENDED)
+        - if the user wants, they can override the main_client (socket object) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
+    
+    - WHAT THEY CAN SET UP:
+        - The user starts a connection to the server 
+            - start_connection()
+        - The user sets their username (no spaces)
+        - The user submits their username data to the server 
+            - submit_username_data(username)
+        - The user requests data assigned to the other players username from the server
+            - request_data(username)
+    
+    - TO BE DONE:
+        - The user runs a function to attempt to connect to the other client
+            - if succeeds, closes server connection
+            - if fails after 3 tries, returns failed
+
+- FOR THE SERVER:
+    - WHAT THEY CAN OVERRIDE:
+        - if the user wants, they can override the valid ports (ONLY IF THEY KNOW WHAT THEY ARE DOING)
+        - if the user wants, they can override the default ip (empty) (ONLY IF THEY KNOW WHAT THEY ARE DOING)
+        - if the user wants, they can override the selected port (THIS IS HIGHLY NOT RECOMMENDED)
+
+    - WHAT THEY CAN SET UP:
+        - the user starts the server
+
+    - TO BE DONE:
         - Add more features to the server?
```

### Comparing `lynxy-0.0.4/src/lynxy/lynx.py` & `lynxy-0.0.5/src/lynxy/lynx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,254 +1,257 @@
-# this below code has been contributed to by chat gpt
-import socket
-import time
-
-_valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112,
-    22111,
-    12211,
-    11221,
-    11122,
-    22222
-]
-
-# define all global vars
-_HOST, _PORT = '', _valid_ports[0] # local_HOST
-_main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-
-# override info
-_ov_ports = []
-_do_print = False
-
-# status vars
-_connected = False
-
-
-
-## FUNCTIONS - overrides, features
-def override_ports(ports: list) -> None:
-    ''' 
-    Overrides what ports the client will attempt to connect to
-    '''
-    global _ov_ports
-    _ov_ports = ports
-
-# disable prints
-def disable_print() -> None:
-    '''
-    Disables the client from printing messages
-    '''
-    global _do_print
-    _do_print = False
-
-# enable prints
-def enable_print() -> None:
-    '''
-    Enables the client to print messages
-    '''
-    global _do_print
-    _do_print = True
-
-# function to handle printing
-def pprint(msg: str) -> None:
-    '''
-    A function meant for filtering prints based on if it is enabled or disabled - This is meant for internal use
-    '''
-    if _do_print:
-        print(msg)
-    else:
-        pass
-
-# function to display current data
-def get_data() -> dict:
-    '''
-    Returns data about the current client in the form of a dictionary
-    '''
-    return {
-        'client info': {
-            'ip': _HOST,
-            'port': _PORT
-        },
-        'sillies': 'sillies :3'
-    }
-
-
-
-
-
-## FUNCTIONS - operations
-# cycles port connection
-def _cycle_port(client: socket.socket) -> socket.socket:
-    global _connected
-    '''
-    An internal function used to cycle through the ports in _valid_ports to try and find a connection
-    '''
-    _connected = False
-    for port in _valid_ports:
-        try:
-            pprint(f'[PORT CYCLE] Client trying port: {port}')
-            client.connect((_HOST, port))
-            pprint(f'[PORT CYCLE] Client connected to: {port}')
-            pprint('----------------------------------------------')
-            _connected = True
-            break
-        except IndexError:
-            port = _valid_ports[0]
-            pprint(f'[PORT CYCLE - RESET 1] Client resetting port to: {port}')
-        except:
-            try:
-                pprint(f'[PORT CYCLE] Client port cycling: {port} -> {_valid_ports[_valid_ports.index(port) + 1]}')
-            except IndexError:
-                port = _valid_ports[0]
-                pprint(f'[PORT CYCLE - RESET 2] Client resetting port to: {port}')
-    if _connected == True:
-        return client, port
-    else:
-        pprint('[PORT CYCLE] the client can not find a open valid server port, exiting')
-        # exit()
-        return client, _PORT
-
-
-
-# a function to fully recieve the message from server (to try and prevent loss)
-# def full_recieve(client: socket.socket) -> str:
-#     message_length = len(client.recv(1024).decode('utf-8'))
-#     incoming_message = ''
-#     local_length = 0
-#     while local_length <= message_length:
-#         incoming_message += client.recv(1024).decode('utf-8')
-#         local_length = len(incoming_message)
-#     return incoming_message
-
-# a function for submitting username data to the server
-def submit_username_data(username: str) -> str:
-    '''
-    Submits a username to the server, which the server will associate with your IP and port.
-    Returns a message that confirms that the action has happened.
-    '''
-    # local override for package form
-    client = _main_client
-    message = username
-    # encoded_message = message.encode('utf-8')
-    message2 = f'username {message}'
-    encoded_message = message2.encode('utf-8') # added username prefix by default
-    client.sendall(encoded_message)
-    pprint(f"Sent:     {message2}")
-    incoming_data = client.recv(1024).decode('utf-8')
-    pprint(f"Received: {incoming_data}")
-    return incoming_data
-
-# requests ip and port from server
-def request_username_data(username: str) -> any:
-    '''
-    requests data associated with a username from the server, and either returns a status code, meaning you entered an invalid username, 
-    or returns the IP and port of the user in a list.
-    '''
-    # local override for package form
-    client = _main_client
-    message = username
-    # encoded_message = message.encode('utf-8')
-    message2 = f'request_by_user {message}'
-    encoded_message = message2.encode('utf-8') # added request_by_user prefix by default
-    client.sendall(encoded_message)
-    pprint(f"Sent:     {message2}")
-    # incoming_data = full_recieve(client)
-    incoming_data = client.recv(1024).decode('utf-8')
-    pprint(f"Received: {incoming_data}")
-    if incoming_data == '100':
-        return incoming_data
-
-    # parse into list
-    address_str = incoming_data.strip('()')
-    ip_str, port_str = address_str.split(',')
-    ip_str = ip_str.strip().strip("'")
-    port_int = int(port_str.strip())
-    incoming_data = [ip_str, port_int]
-    return incoming_data
-
-# a general message sender
-def send_msg(message: str, recieve: bool = True) -> str:
-    '''
-    A general tool function for sending messages to the recipient (server, other client, etc)
-    '''
-    # local override for package form
-    client = _main_client
-    encoded_message = message.encode('utf-8')
-    client.sendall(encoded_message)
-    pprint(f"Sent:     {message}")
-    # incoming_data = full_recieve(client)
-    if recieve:
-        incoming_data = client.recv(1024).decode('utf-8')
-        pprint(f"Received: {incoming_data}")
-        return incoming_data
-
-# def send_file(file, recieve: bool = False) -> any:
-#     '''
-#     A general tool function for sending files to the recipient (server, other client, etc)
-#     '''
-#     client = _main_client
-#     encoded_file =
-
-# def target_client(client_ip: str, client_port: int, mode: str) -> bool:
-#     '''
-#     Takes in the target clients ip and port, and will attempt to connect to them. If this fails, 
-#     then it is possible the other client is not available.
-#     This function returns a boolean, telling you whether it worked or not.
-#     '''
-#     global _HOST, _PORT, _valid_ports
-#     global _main_client
-#     global _do_print
-#     # reset main_client
-#     _main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-#     # overwrite host
-#     _HOST = client_ip
-#     # overwrite valid ports list
-#     override_ports([client_port])
-#     # overwrite port
-#     _PORT = _valid_ports[0]
-#     # setup other vars
-#     save = _do_print
-
-#     for i in range(30):
-#         print(f'attempt {i}')
-#         disable_print()
-#         _main_client, _PORT = _cycle_port(_main_client)
-#         _do_print = save
-#         if _connected == True:
-#             return True
-#         time.sleep(1)
-#     return False
-
-
-
-# function for shutting down the client
-def shutdown_client() -> bool:
-    '''
-    A function to shut down the client: returns a bool telling you whether it worked or not.
-    '''
-    global _main_client
-    try:
-        _main_client.close()
-        pprint('[CLIENT SHUTDOWN] Shutting down client...')
-        return True
-    except:
-        return False
-
-def start_client(connection_ip: str) -> None:
-    '''
-    Starts the connection to the server, taking in an IP
-    '''
-    global _main_client, _valid_ports, _PORT, _HOST
-    _HOST = connection_ip
-
-    # overrides
-    if len(_ov_ports) > 0:
-        _valid_ports = _ov_ports
-        _PORT = _valid_ports[0]
-        pprint(f'[OVERRIDE] Overrided ports to: {_valid_ports}')
-    
-    # establish the connection to a port that the server is on
-    _main_client, _PORT = _cycle_port(_main_client)
+# this below code has been contributed to by chat gpt
+import socket
+import time
+
+_valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112,
+    22111,
+    12211,
+    11221,
+    11122,
+    22222
+]
+
+# define all global vars
+_HOST, _PORT = '', _valid_ports[0] # local_HOST
+_main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+# override info
+_ov_ports = []
+_do_print = False
+
+# status vars
+_connected = False
+
+
+
+## FUNCTIONS - overrides, features
+def override_ports(ports: list) -> None:
+    ''' 
+    Overrides what ports the client will attempt to connect to
+    '''
+    global _ov_ports
+    _ov_ports = ports
+
+# disable prints
+def disable_print() -> None:
+    '''
+    Disables the client from printing messages
+    '''
+    global _do_print
+    _do_print = False
+
+# enable prints
+def enable_print() -> None:
+    '''
+    Enables the client to print messages
+    '''
+    global _do_print
+    _do_print = True
+
+# function to handle printing
+def pprint(msg: str) -> None:
+    '''
+    A function meant for filtering prints based on if it is enabled or disabled - This is meant for internal use
+    '''
+    if _do_print:
+        print(msg)
+    else:
+        pass
+
+# function to display current data
+def get_data() -> dict:
+    '''
+    Returns data about the current client in the form of a dictionary
+    '''
+    return {
+        'client info': {
+            'ip': _HOST,
+            'port': _PORT
+        },
+        'sillies': 'sillies :3'
+    }
+
+
+
+
+
+## FUNCTIONS - operations
+# cycles port connection
+def _cycle_port(client: socket.socket) -> tuple[socket.socket, int, bool]:
+    global _connected
+    '''
+    An internal function used to cycle through the ports in _valid_ports to try and find a connection
+    '''
+    _connected = False
+    out_port = 0
+    for port in _valid_ports:
+        out_port = port
+        try:
+            pprint(f'[PORT CYCLE] Client trying port: {port}')
+            client.connect((_HOST, port))
+            pprint(f'[PORT CYCLE] Client connected to: {port}')
+            pprint('----------------------------------------------')
+            _connected = True
+            break
+        except IndexError:
+            port = _valid_ports[0]
+            pprint(f'[PORT CYCLE - RESET 1] Client resetting port to: {port}')
+        except:
+            try:
+                pprint(f'[PORT CYCLE] Client port cycling: {port} -> {_valid_ports[_valid_ports.index(port) + 1]}')
+            except IndexError:
+                port = _valid_ports[0]
+                pprint(f'[PORT CYCLE - RESET 2] Client resetting port to: {port}')
+    if _connected == True:
+        return client, out_port, True
+    elif _connected == False:
+        pprint('[PORT CYCLE] the client can not find a open valid server port, exiting')
+        return client, _PORT, False
+
+
+
+# a function to fully recieve the message from server (to try and prevent loss)
+# def full_recieve(client: socket.socket) -> str:
+#     message_length = len(client.recv(1024).decode('utf-8'))
+#     incoming_message = ''
+#     local_length = 0
+#     while local_length <= message_length:
+#         incoming_message += client.recv(1024).decode('utf-8')
+#         local_length = len(incoming_message)
+#     return incoming_message
+
+# a function for submitting username data to the server
+def submit_username_data(username: str) -> str:
+    '''
+    Submits a username to the server, which the server will associate with your IP and port.
+    Returns a message that confirms that the action has happened.
+    '''
+    # local override for package form
+    client = _main_client
+    message = username
+    # encoded_message = message.encode('utf-8')
+    message2 = f'username {message}'
+    encoded_message = message2.encode('utf-8') # added username prefix by default
+    client.sendall(encoded_message)
+    pprint(f"Sent:     {message2}")
+    incoming_data = client.recv(1024).decode('utf-8')
+    pprint(f"Received: {incoming_data}")
+    return incoming_data
+
+# requests ip and port from server
+def request_username_data(username: str) -> any:
+    '''
+    requests data associated with a username from the server, and either returns a status code, meaning you entered an invalid username, 
+    or returns the IP and port of the user in a list.
+    '''
+    # local override for package form
+    client = _main_client
+    message = username
+    # encoded_message = message.encode('utf-8')
+    message2 = f'request_by_user {message}'
+    encoded_message = message2.encode('utf-8') # added request_by_user prefix by default
+    client.sendall(encoded_message)
+    pprint(f"Sent:     {message2}")
+    # incoming_data = full_recieve(client)
+    incoming_data = client.recv(1024).decode('utf-8')
+    pprint(f"Received: {incoming_data}")
+    if incoming_data == '100':
+        return incoming_data
+
+    # parse into list
+    address_str = incoming_data.strip('()')
+    ip_str, port_str = address_str.split(',')
+    ip_str = ip_str.strip().strip("'")
+    port_int = int(port_str.strip())
+    incoming_data = [ip_str, port_int]
+    return incoming_data
+
+# a general message sender
+def send_msg(message: str, recieve: bool = True) -> str:
+    '''
+    A general tool function for sending messages to the recipient (server, other client, etc)
+    '''
+    # local override for package form
+    client = _main_client
+    encoded_message = message.encode('utf-8')
+    client.sendall(encoded_message)
+    pprint(f"Sent:     {message}")
+    # incoming_data = full_recieve(client)
+    if recieve:
+        incoming_data = client.recv(1024).decode('utf-8')
+        pprint(f"Received: {incoming_data}")
+        return incoming_data
+
+# def send_file(file, recieve: bool = False) -> any:
+#     '''
+#     A general tool function for sending files to the recipient (server, other client, etc)
+#     '''
+#     client = _main_client
+#     encoded_file =
+
+# def target_client(client_ip: str, client_port: int, mode: str) -> bool:
+#     '''
+#     Takes in the target clients ip and port, and will attempt to connect to them. If this fails, 
+#     then it is possible the other client is not available.
+#     This function returns a boolean, telling you whether it worked or not.
+#     '''
+#     global _HOST, _PORT, _valid_ports
+#     global _main_client
+#     global _do_print
+#     # reset main_client
+#     _main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+#     # overwrite host
+#     _HOST = client_ip
+#     # overwrite valid ports list
+#     override_ports([client_port])
+#     # overwrite port
+#     _PORT = _valid_ports[0]
+#     # setup other vars
+#     save = _do_print
+
+#     for i in range(30):
+#         print(f'attempt {i}')
+#         disable_print()
+#         _main_client, _PORT = _cycle_port(_main_client)
+#         _do_print = save
+#         if _connected == True:
+#             return True
+#         time.sleep(1)
+#     return False
+
+
+
+# function for shutting down the client
+def shutdown_client() -> bool:
+    '''
+    A function to shut down the client: returns a bool telling you whether it worked or not.
+    '''
+    global _main_client
+    try:
+        _main_client.close()
+        pprint('[CLIENT SHUTDOWN] Shutting down client...')
+        return True
+    except:
+        return False
+
+def start_client(connection_ip: str) -> bool:
+    '''
+    Starts the connection to the server, taking in an IP. 
+    This function returns a bool, telling you whether it worked or not.
+    '''
+    global _main_client, _valid_ports, _PORT, _HOST
+    _HOST = connection_ip
+
+    # overrides
+    if len(_ov_ports) > 0:
+        _valid_ports = _ov_ports
+        _PORT = _valid_ports[0]
+        pprint(f'[OVERRIDE] Overrided ports to: {_valid_ports}')
+    
+    # establish the connection to a port that the server is on
+    _main_client, _PORT, state = _cycle_port(_main_client)
+    return state
```

### Comparing `lynxy-0.0.4/src/lynxy_server/__init__.py` & `lynxy-0.0.5/src/lynxy_server/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-'''
-This is the lynxy server module. To find documentation, go to the github~!
-- Github: https://github.com/SketchedDoughnut//lynxy
-'''
-
-# extending main lynx file
-from .lynx_server import *
-
-def help(open_tab: bool = False) -> str:
-    '''
-    A function that returns a link to the Github page
-    '''
-    if open_tab == True:
-        import webbrowser
-        webbrowser.open_new_tab('https://github.com/SketchedDoughnut/lynxy')
-    else:
-        return 'https://github.com/SketchedDoughnut/lynxy'
-    
-def license(open_tab: bool = False) -> str:
-    '''
-    A function that returns a link to the license this project is under
-    '''
-    if open_tab == True:
-        import webbrowser
-        webbrowser.open_new_tab('https://github.com/SketchedDoughnut/lynxy/blob/master/LICENSE')
-    else:
-        return 'https://github.com/SketchedDoughnut/lynxy/blob/master/LICENSE'
-    
-def credits() -> str:
-    '''
-    A function that returns a string containing the credits for this project
-    '''
-    return 'This project is developed and maintained by SketchedDoughnut'
+'''
+This is the lynxy server module. To find documentation, go to the github~!
+- Github: https://github.com/SketchedDoughnut//lynxy
+'''
+
+# extending main lynx file
+from .lynx_server import *
+
+def help(open_tab: bool = False) -> str:
+    '''
+    A function that returns a link to the Github page
+    '''
+    if open_tab == True:
+        import webbrowser
+        webbrowser.open_new_tab('https://github.com/SketchedDoughnut/lynxy')
+    else:
+        return 'https://github.com/SketchedDoughnut/lynxy'
+    
+def license(open_tab: bool = False) -> str:
+    '''
+    A function that returns a link to the license this project is under
+    '''
+    if open_tab == True:
+        import webbrowser
+        webbrowser.open_new_tab('https://github.com/SketchedDoughnut/lynxy/blob/master/LICENSE')
+    else:
+        return 'https://github.com/SketchedDoughnut/lynxy/blob/master/LICENSE'
+    
+def credits() -> str:
+    '''
+    A function that returns a string containing the credits for this project
+    '''
+    return 'This project is developed and maintained by SketchedDoughnut'
```

### Comparing `lynxy-0.0.4/src/lynxy_server/lynx_server.py` & `lynxy-0.0.5/src/lynxy_server/lynx_server.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-import socketserver
-import socket
-import threading
-import time
-import random
-
-# file imports
-from .responses import *
-
-# where client data is stored
-_client_dict = {
-    'default': 0
-}
-
-# all valid ports it will attempt to connect to
-_valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112,
-    22111,
-    12211,
-    11221,
-    11122,
-    22222
-]
-
-# _HOST and _PORT info for connections
-_HOST = socket.gethostbyname(socket.gethostname())
-_PORT = _valid_ports[0]
-
-# override info
-_ov_ip = ''
-_ov_ports = []
-_do_print = True
-
-# status vars
-_connected = False
-_shutdown = False
-_kill_all = False
-
-# server obj for shutting down
-_server = 0
-
-# starting thread object
-_starting_thread = 0
-
-# server token
-_token = 'x'
-_verified = False
-
-
-
-
-
-
-
-## OVERRIDE FUNCTIONS
-# override ports
-def override_ports(ports: list) -> None:
-    ''' 
-    Overrides what ports the server will attempt to connect to
-    '''
-    global _valid_ports, _ov_ports
-    _ov_ports = ports
-
-# override ip
-def override_ip(ip_in: str) -> None:
-    '''
-    Overrides what IP the server will attempt to connect to
-    '''
-    global _ov_ip
-    _ov_ip = ip_in
-
-# disable prints
-def disable_print() -> None:
-    '''
-    Disables the server from printing messages
-    '''
-    global _do_print
-    _do_print = False
-
-# enable prints
-def enable_print() -> None:
-    '''
-    Enables the server to print messages
-    '''
-    global _do_print
-    _do_print = True
-
-
-## FEATURE FUNCTIONS
-# function to handle printing
-def pprint(msg: str) -> None:
-    '''
-    A function meant for filtering prints based on if it is enabled or disabled - This is meant for internal use
-    '''
-    if _do_print:
-        print(msg)
-    else:
-        pass
-
-# function to display current data
-def get_data() -> dict:
-    '''
-    Returns data about the current server in the form of a dictionary
-    '''
-    return {
-        'server info': {
-            'is_alive': _connected,
-            'ip': _HOST,
-            'port': _PORT,
-            'token': _token
-        },
-        'client info': _client_dict
-    }
-
-# function for shutting down the server
-def freeze_server(do_print: bool = True) -> str:
-    '''
-    A function to shut down the server: returns a status code.
-    '''
-    global _server, _kill_all
-    try:
-        _server.shutdown()
-        _kill_all = True
-        if do_print == True:
-            pprint('[SERVER SHUTDOWN] Shutting down server...')
-        return OPERATION_SUCCESS.decode()
-    except:
-        return OPERATION_FAIL.decode()
-    
-# function to poll shutdown var, if it is enabled then shutdown
-def _poll_shutdown() -> None:
-    global _kill_all
-    while True:
-        if _shutdown == True:
-            pprint('[SERVER SHUTDOWN] request to shutdown detected, shutting down server...')
-            freeze_server(False)
-            pprint('[SERVER SHUTDOWN] Enabling _kill_all...')
-            _kill_all = True
-            pprint('[SERVER SHUTDOWN] Server shut down, exiting...')
-            break
-        time.sleep(5)
-    exit()
-
-## SAFETY FUNCTIONS
-# function to generate an auth token that someone can use to remotely control the server
-def _gen_auth_token() -> str:
-    '''
-    A function that generates an auth token for the user to use to remotely connect and control the server
-    '''
-    lower_alpha = 'abcdefghijklmnopqrstuvwxyz'
-    upper_alpha = lower_alpha.upper()
-    letter_list = [lower_alpha, upper_alpha]
-    token = ''
-    for i in range(6): # length of your sign-in token
-        letter_or_num = random.randint(0, 1)
-        if letter_or_num == 0:
-            letter_type = random.randint(0, 1)
-            letter_range = letter_list[letter_type]
-            letter_index = random.randint(0, len(letter_range) - 1)
-            token += letter_range[letter_index]
-        elif letter_or_num == 1:
-            token += str(random.randint(0, 9))
-    return token
-
-
-# MAIN CLASS
-class _myTCPserver(socketserver.BaseRequestHandler):
-    def handle(self) -> None:
-        global _client_dict, _verified, _shutdown
-
-        while True:
-            # establish client address
-            addr = self.client_address[0]
-            addr = self.client_address[1]
-
-            # kill client communication if is true (will kill before msg)
-            if _kill_all == True:
-                # self.request.sendall('the server has been commanded to kill all client instances'.encode())
-                self.request.sendall(KILL_ALL)
-                pprint(f'[{addr}] Killing this instance, due to _kill_all being True...')
-                break
-
-            # format incoming message
-            try:
-                msg = bytes(self.request.recv(1024)).decode('utf-8')
-                split_msg = msg.split()
-                prefix = split_msg[0]
-                split_msg.remove(prefix)
-                joined_msg = "".join(split_msg)
-            except:
-                try:
-                    self.request.sendall(INVALID_MESSAGE) # try to send message telling them what they gave is invalid
-                    continue
-                except Exception as e:
-                    pprint(f'[{addr}] - crash - ending this instance')
-                    pprint('----------------------------------------------')
-                    break
-
-            # if prefix is username, log their username and their device info (ip, port) associated with it
-            if prefix == 'username':
-                if joined_msg: # if not empty
-                    _client_dict[joined_msg] = self.client_address
-                    pprint(f'[{addr}] {prefix} - logging {self.client_address} to {joined_msg}')
-                    # self.request.sendall('logged username, data'.encode())
-                    self.request.sendall(OPERATION_SUCCESS)
-                else:
-                    self.request.sendall(INVALID_MESSAGE)
-
-            # if prefix is request_by_user, attempt to return the data associated with that username. If it does not exist, send back "None"
-            elif prefix == 'request_by_user':
-                try:
-                    self.request.sendall(str(_client_dict[joined_msg]).encode())
-                    pprint(f'[{addr}] {prefix} - return {joined_msg} data: {_client_dict[joined_msg]}')
-                except:
-                    pprint(f'[{addr}] {prefix} - return {joined_msg} data: None')
-                    # self.request.sendall('None'.encode())
-                    self.request.sendall(INVALID_USERNAME_DATA)
-
-            # if prefix is auth, check if token is matching, then allow user to use dev features
-            elif prefix == 'auth':
-                if joined_msg == _token:
-                    _verified = True
-                    # self.request.sendall('client session authorized'.encode())
-                    self.request.sendall(OPERATION_SUCCESS)
-                    pprint(f'[{addr}] {prefix} - authed client')
-                else:
-                    # self.request.sendall('invalid auth token'.encode())
-                    self.request.sendall(INVALID_AUTH_TOKEN)
-
-            # if msg is clear_client, check if this client is authorized and then clear the client_dict
-            elif msg == 'clear_client':
-                if _verified == True:
-                    _client_dict = {
-                        'default': 0
-                    }
-                    # self.request.sendall('cleared client dictionary')
-                    self.request.sendall(OPERATION_SUCCESS)
-                    pprint(f'[{addr}] {msg} - clearing client_dict')
-                else:
-                    # self.request.sendall('user not authorized'.encode())
-                    self.request.sendall(USER_NOT_AUTHORIZED)
-
-
-            # if msg is freeze_server, check if this client is authorized and then raise the flag to shutdown srever
-            elif msg == 'freeze_server':
-                if _verified == True:
-                    _shutdown = True
-                    # self.request.sendall('shutdown of server requested, raising flag'.encode())
-                    self.request.sendall(OPERATION_SUCCESS)
-                    pprint(f'[{addr}] {msg} - shutdown of server requested, raising flag')
-                else:
-                    # self.request.sendall('user not authorized'.encode())
-                    self.request.sendall(USER_NOT_AUTHORIZED)
-
-            # if msg is end_session, end the current session the server and the client have
-            elif msg == 'end_session':
-                # self.request.sendall('ending'.encode())
-                self.request.sendall(END_SESSION)
-                pprint(f'[{addr}] {msg} - ending this instance')
-                pprint('----------------------------------------------')
-                break
-            
-            # ignore their message if otherwise
-            else:
-                # self.request.sendall(msg.upper().encode())  # Send response back to the client
-                # self.request.sendall('invalid command'.encode())
-                self.request.sendall(INVALID_COMMAND)
-                pass
-
-
-# main function for starting, does not use a thread and will block code
-def no_thread_start_server(is_threaded: bool = False) -> None:
-    '''
-    If you want to start the server without it running in a thread, you can call this function. However, this will block your code until the server goes offline.
-    This won't happen unless it crashes, or you remotely raise the shutdown flag (refer to the server setup page of documentation on Github)
-    '''
-    global _HOST, _PORT, _valid_ports, _connected, _server, _token
-    ## apply overrides
-    # override ip
-    if _ov_ip:
-        _HOST = _ov_ip
-        pprint(f'[OVERRIDE] IP overrided to: {_HOST}')
-    if len(_ov_ports) > 0:
-        _valid_ports = _ov_ports
-        _PORT = _valid_ports[0]
-        pprint(f'[OVERRIDE] Valid ports overrided to: {_valid_ports}')
-
-    # pre-loop variables
-    _connected = False
-    
-    # generate unique session token for remote controlling the server
-    _token = _gen_auth_token()
-
-    # loop, trying to find a free port
-    for port in _valid_ports:
-
-        try:
-            pprint(f'[PORT CYCLE] Server trying port: {port}')
-            with socketserver.ThreadingTCPServer((_HOST, port), _myTCPserver) as _server:
-                pprint(f'[PORT CYCLE] Server found port for startup: {port}')
-                # start server shutdown poll
-                threading.Thread(target=lambda:_poll_shutdown()).start()    # , daemon=True).start()
-                pprint('[SERVER] Started scan for shutdown requests')
-                if is_threaded: 
-                    pprint(f'[SERVER] Server IP: {_HOST}')
-                    pprint(f'[SERVER] Control token: {_token}')
-                else: 
-                    print(f'[SERVER] Server IP: {_HOST}')
-                    print(f'[SERVER] Session token: {_token}')
-                pprint('[SERVER] Server is ready for communication~!')
-                if is_threaded:
-                    pprint('----------------------------------------------')
-                else: 
-                    print('----------------------------------------------')
-                _connected = True
-                _PORT = port
-                _server.serve_forever()
-                break
-        except:
-            try:
-                pprint(f'[PORT CYCLE] Server port cycling: {port} -> {_valid_ports[_valid_ports.index(port) + 1]}')
-            except IndexError:
-                port = _valid_ports[0]
-                pprint(f'[PORT CYCLE - RESET 2] Server resetting port to: {port}')
-    
-    if _connected == False:
-        pprint('[PORT CYCLE - ERROR 0] Server failed to find an open valid port, exiting')
-        exit()
-    else:
-        pprint('[PORT CYCLE - ERROR 1] It is assumed server has been shutdown, ignoring error')
-
-
-
-
-
-# starts the server via a thread, to let the code calling this function continue running instead of blocking
-def start_server() -> tuple:
-    global _starting_thread
-    '''
-    Starts the server in a thread, which means this will not block the rest of your code if you have more things done after this function is called. 
-    This function also returns the IP that the server is on, the port the server is on, and the authorization token in a tuple.
-    '''
-    _starting_thread = threading.Thread(target=lambda:no_thread_start_server(True)) #, daemon=True)
-    _starting_thread.start()
-    time.sleep(0.25) # this is to not get false information if they request data later on 
+import socketserver
+import socket
+import threading
+import time
+import random
+
+# file imports
+from .responses import *
+
+# where client data is stored
+_client_dict = {
+    'default': 0
+}
+
+# all valid ports it will attempt to connect to
+_valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112,
+    22111,
+    12211,
+    11221,
+    11122,
+    22222
+]
+
+# _HOST and _PORT info for connections
+_HOST = socket.gethostbyname(socket.gethostname())
+_PORT = _valid_ports[0]
+
+# override info
+_ov_ip = ''
+_ov_ports = []
+_do_print = True
+
+# status vars
+_connected = False
+_shutdown = False
+_kill_all = False
+
+# server obj for shutting down
+_server = 0
+
+# starting thread object
+_starting_thread = 0
+
+# server token
+_token = 'x'
+_verified = False
+
+
+
+
+
+
+
+## OVERRIDE FUNCTIONS
+# override ports
+def override_ports(ports: list) -> None:
+    ''' 
+    Overrides what ports the server will attempt to connect to
+    '''
+    global _valid_ports, _ov_ports
+    _ov_ports = ports
+
+# override ip
+def override_ip(ip_in: str) -> None:
+    '''
+    Overrides what IP the server will attempt to connect to
+    '''
+    global _ov_ip
+    _ov_ip = ip_in
+
+# disable prints
+def disable_print() -> None:
+    '''
+    Disables the server from printing messages
+    '''
+    global _do_print
+    _do_print = False
+
+# enable prints
+def enable_print() -> None:
+    '''
+    Enables the server to print messages
+    '''
+    global _do_print
+    _do_print = True
+
+
+## FEATURE FUNCTIONS
+# function to handle printing
+def pprint(msg: str) -> None:
+    '''
+    A function meant for filtering prints based on if it is enabled or disabled - This is meant for internal use
+    '''
+    if _do_print:
+        print(msg)
+    else:
+        pass
+
+# function to display current data
+def get_data() -> dict:
+    '''
+    Returns data about the current server in the form of a dictionary
+    '''
+    return {
+        'server info': {
+            'is_alive': _connected,
+            'ip': _HOST,
+            'port': _PORT,
+            'token': _token
+        },
+        'client info': _client_dict
+    }
+
+# function for shutting down the server
+def freeze_server(do_print: bool = True) -> str:
+    '''
+    A function to shut down the server: returns a status code.
+    '''
+    global _server, _kill_all
+    try:
+        _server.shutdown()
+        _kill_all = True
+        if do_print == True:
+            pprint('[SERVER SHUTDOWN] Shutting down server...')
+        return OPERATION_SUCCESS.decode()
+    except:
+        return OPERATION_FAIL.decode()
+    
+# function to poll shutdown var, if it is enabled then shutdown
+def _poll_shutdown() -> None:
+    global _kill_all
+    while True:
+        if _shutdown == True:
+            pprint('[SERVER SHUTDOWN] request to shutdown detected, shutting down server...')
+            freeze_server(False)
+            pprint('[SERVER SHUTDOWN] Enabling _kill_all...')
+            _kill_all = True
+            pprint('[SERVER SHUTDOWN] Server shut down, exiting...')
+            break
+        time.sleep(5)
+    exit()
+
+## SAFETY FUNCTIONS
+# function to generate an auth token that someone can use to remotely control the server
+def _gen_auth_token() -> str:
+    '''
+    A function that generates an auth token for the user to use to remotely connect and control the server
+    '''
+    lower_alpha = 'abcdefghijklmnopqrstuvwxyz'
+    upper_alpha = lower_alpha.upper()
+    letter_list = [lower_alpha, upper_alpha]
+    token = ''
+    for i in range(6): # length of your sign-in token
+        letter_or_num = random.randint(0, 1)
+        if letter_or_num == 0:
+            letter_type = random.randint(0, 1)
+            letter_range = letter_list[letter_type]
+            letter_index = random.randint(0, len(letter_range) - 1)
+            token += letter_range[letter_index]
+        elif letter_or_num == 1:
+            token += str(random.randint(0, 9))
+    return token
+
+
+# MAIN CLASS
+class _myTCPserver(socketserver.BaseRequestHandler):
+    def handle(self) -> None:
+        global _client_dict, _verified, _shutdown
+
+        while True:
+            # establish client address
+            addr = self.client_address[0]
+            addr = self.client_address[1]
+
+            # kill client communication if is true (will kill before msg)
+            if _kill_all == True:
+                # self.request.sendall('the server has been commanded to kill all client instances'.encode())
+                self.request.sendall(KILL_ALL)
+                pprint(f'[{addr}] Killing this instance, due to _kill_all being True...')
+                break
+
+            # format incoming message
+            try:
+                msg = bytes(self.request.recv(1024)).decode('utf-8')
+                split_msg = msg.split()
+                prefix = split_msg[0]
+                split_msg.remove(prefix)
+                joined_msg = "".join(split_msg)
+            except:
+                try:
+                    self.request.sendall(INVALID_MESSAGE) # try to send message telling them what they gave is invalid
+                    continue
+                except Exception as e:
+                    pprint(f'[{addr}] - crash - ending this instance')
+                    pprint('----------------------------------------------')
+                    break
+
+            # if prefix is username, log their username and their device info (ip, port) associated with it
+            if prefix == 'username':
+                if joined_msg: # if not empty
+                    _client_dict[joined_msg] = self.client_address
+                    pprint(f'[{addr}] {prefix} - logging {self.client_address} to {joined_msg}')
+                    # self.request.sendall('logged username, data'.encode())
+                    self.request.sendall(OPERATION_SUCCESS)
+                else:
+                    self.request.sendall(INVALID_MESSAGE)
+
+            # if prefix is request_by_user, attempt to return the data associated with that username. If it does not exist, send back "None"
+            elif prefix == 'request_by_user':
+                try:
+                    self.request.sendall(str(_client_dict[joined_msg]).encode())
+                    pprint(f'[{addr}] {prefix} - return {joined_msg} data: {_client_dict[joined_msg]}')
+                except:
+                    pprint(f'[{addr}] {prefix} - return {joined_msg} data: None')
+                    # self.request.sendall('None'.encode())
+                    self.request.sendall(INVALID_USERNAME_DATA)
+
+            # if prefix is auth, check if token is matching, then allow user to use dev features
+            elif prefix == 'auth':
+                if joined_msg == _token:
+                    _verified = True
+                    # self.request.sendall('client session authorized'.encode())
+                    self.request.sendall(OPERATION_SUCCESS)
+                    pprint(f'[{addr}] {prefix} - authed client')
+                else:
+                    # self.request.sendall('invalid auth token'.encode())
+                    self.request.sendall(INVALID_AUTH_TOKEN)
+
+            # if msg is clear_client, check if this client is authorized and then clear the client_dict
+            elif msg == 'clear_client':
+                if _verified == True:
+                    _client_dict = {
+                        'default': 0
+                    }
+                    # self.request.sendall('cleared client dictionary')
+                    self.request.sendall(OPERATION_SUCCESS)
+                    pprint(f'[{addr}] {msg} - clearing client_dict')
+                else:
+                    # self.request.sendall('user not authorized'.encode())
+                    self.request.sendall(USER_NOT_AUTHORIZED)
+
+
+            # if msg is freeze_server, check if this client is authorized and then raise the flag to shutdown srever
+            elif msg == 'freeze_server':
+                if _verified == True:
+                    _shutdown = True
+                    # self.request.sendall('shutdown of server requested, raising flag'.encode())
+                    self.request.sendall(OPERATION_SUCCESS)
+                    pprint(f'[{addr}] {msg} - shutdown of server requested, raising flag')
+                else:
+                    # self.request.sendall('user not authorized'.encode())
+                    self.request.sendall(USER_NOT_AUTHORIZED)
+
+            # if msg is end_session, end the current session the server and the client have
+            elif msg == 'end_session':
+                # self.request.sendall('ending'.encode())
+                self.request.sendall(END_SESSION)
+                pprint(f'[{addr}] {msg} - ending this instance')
+                pprint('----------------------------------------------')
+                break
+            
+            # ignore their message if otherwise
+            else:
+                # self.request.sendall(msg.upper().encode())  # Send response back to the client
+                # self.request.sendall('invalid command'.encode())
+                self.request.sendall(INVALID_COMMAND)
+                pass
+
+
+# main function for starting, does not use a thread and will block code
+def no_thread_start_server(is_threaded: bool = False) -> None:
+    '''
+    If you want to start the server without it running in a thread, you can call this function. However, this will block your code until the server goes offline.
+    This won't happen unless it crashes, or you remotely raise the shutdown flag (refer to the server setup page of documentation on Github)
+    '''
+    global _HOST, _PORT, _valid_ports, _connected, _server, _token
+    ## apply overrides
+    # override ip
+    if _ov_ip:
+        _HOST = _ov_ip
+        pprint(f'[OVERRIDE] IP overrided to: {_HOST}')
+    if len(_ov_ports) > 0:
+        _valid_ports = _ov_ports
+        _PORT = _valid_ports[0]
+        pprint(f'[OVERRIDE] Valid ports overrided to: {_valid_ports}')
+
+    # pre-loop variables
+    _connected = False
+    
+    # generate unique session token for remote controlling the server
+    _token = _gen_auth_token()
+
+    # loop, trying to find a free port
+    for port in _valid_ports:
+
+        try:
+            pprint(f'[PORT CYCLE] Server trying port: {port}')
+            with socketserver.ThreadingTCPServer((_HOST, port), _myTCPserver) as _server:
+                pprint(f'[PORT CYCLE] Server found port for startup: {port}')
+                # start server shutdown poll
+                threading.Thread(target=lambda:_poll_shutdown()).start()    # , daemon=True).start()
+                pprint('[SERVER] Started scan for shutdown requests')
+                if is_threaded: 
+                    pprint(f'[SERVER] Server IP: {_HOST}')
+                    pprint(f'[SERVER] Control token: {_token}')
+                else: 
+                    print(f'[SERVER] Server IP: {_HOST}')
+                    print(f'[SERVER] Session token: {_token}')
+                pprint('[SERVER] Server is ready for communication~!')
+                if is_threaded:
+                    pprint('----------------------------------------------')
+                else: 
+                    print('----------------------------------------------')
+                _connected = True
+                _PORT = port
+                _server.serve_forever()
+                break
+        except:
+            try:
+                pprint(f'[PORT CYCLE] Server port cycling: {port} -> {_valid_ports[_valid_ports.index(port) + 1]}')
+            except IndexError:
+                port = _valid_ports[0]
+                pprint(f'[PORT CYCLE - RESET 2] Server resetting port to: {port}')
+    
+    if _connected == False:
+        pprint('[PORT CYCLE - ERROR 0] Server failed to find an open valid port, exiting')
+        exit()
+    else:
+        pprint('[PORT CYCLE - ERROR 1] It is assumed server has been shutdown, ignoring error')
+
+
+
+
+
+# starts the server via a thread, to let the code calling this function continue running instead of blocking
+def start_server() -> tuple:
+    global _starting_thread
+    '''
+    Starts the server in a thread, which means this will not block the rest of your code if you have more things done after this function is called. 
+    This function also returns the IP that the server is on, the port the server is on, and the authorization token in a tuple.
+    '''
+    _starting_thread = threading.Thread(target=lambda:no_thread_start_server(True)) #, daemon=True)
+    _starting_thread.start()
+    time.sleep(0.25) # this is to not get false information if they request data later on 
     return _HOST, _PORT, _token
```

### Comparing `lynxy-0.0.4/tests/new_server.py` & `lynxy-0.0.5/tests/new_server.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,322 +1,322 @@
-import socket
-import random
-import time
-import threading
-
-# all valid ports to cycle through
-valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112
-]
-
-# set limit for server instances
-INSTANCE_LIMIT = 5
-initial_limit_print = False
-alive_bound_instance = 0
-alive_searching_instance = 0
-
-# set port limits, defaults
-not_inclusive_max_port_amount = len(valid_ports) - 1
-default_port = valid_ports[0]
-
-# set up client dict, storing username to ip correlation
-client_dict = {
-    'default': 0
-}
-
-# a dictionary where a port number is associated with [State of living (bool), server_socket, client_socket] NOTE: server_socket is not used
-unique_server_instance_dict = {}
-for port in valid_ports:
-    unique_server_instance_dict[port] = [False, 'x', 'x']
-
-
-
-
-
-### FUNCTIONS
-
-## TOOlS
-
-# a function that is ran and evaluates all sockets, killing them if neccesary (thread) (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
-def check_alive() -> None:
-    global unique_server_instance_dict
-    import time
-    while True:
-        for port in valid_ports:
-            try:
-                data = unique_server_instance_dict[port]
-                state = data[0]
-                server_obj = data[1]
-                client_obj = data[2]
-                closed = is_socket_closed(client_obj)
-                if closed == True:
-                    print(f'[ALIVE SCANNER] the client for port {port} is not responsive, so the connection will be terminated.')
-                    unique_server_instance_dict[port] = [False, server_obj, client_obj]
-                    print(f'[ALIVE SCANNER] closing associated server and client...')
-                    server_obj.close()
-                    client_obj.close()
-                # else:
-                    # print(f'{por} is connected to a client and healthy')
-            except:
-                pass
-                # print('not checking this port as they have not signed on yet')
-        time.sleep(5)
-
-
-
-# A function to check if the socket is closed (not sure how it works, though)
-# https://stackoverflow.com/questions/48024720/python-how-to-check-if-socket-is-still-connected
-def is_socket_closed(sock: socket.socket) -> bool:
-    try:
-        # this will try to read bytes without blocking and also without removing them from buffer (peek only)
-        data = sock.recv(16, socket.MSG_DONTWAIT | socket.MSG_PEEK)
-        # data = sock.recv(16)
-        if len(data) == 0:
-            return True
-        
-    except BlockingIOError:
-        return False  # socket is open and reading from it would block
-    except ConnectionResetError:
-        return True  # socket was closed for some other reason
-    except Exception as e:
-        #logger.exception("unexpected exception when checking if a socket is closed")
-        return False
-    return False
-
-
-
-
-
-
-
-
-
-## CORE FUNCTIONS
-# connect to client
-def connect_to_client(server: socket.socket, port_override: int = 0, return_port: bool = False) -> list:
-    # access global
-    #local_port = default_port
-
-
-    try:
-        # iterate through valid ports, check if any are not alive in unique_server_instance_dict
-        found_open = False
-        if port_override == 0:
-            for port in valid_ports:
-                data = unique_server_instance_dict[port]
-                is_alive = data[0]
-                server_obj = data[1]
-                client_obj = data[2]
-                if is_alive == False:
-                    found_open = True
-                    open_port = port
-                    break
-            if found_open == True:
-                print(f'[unbound] open port found: {open_port}')
-                #server.bind(('', open_port))
-                server.bind(('localhost', open_port))
-                print(f'[{open_port}] server binded to port {open_port}')
-            else:
-                print('[unbound] all ports are being used, cancelling attempt')
-                exit()
-        else:
-            open_port = port_override
-            print(f'[unbound] port overrided to: {open_port}')
-            #server.bind(('', open_port))
-            server.bind(('localhost', open_port))
-            print(f'[{open_port}] server binded to port {open_port}')
-    except Exception as e:
-        print(f'[unbound] an error occured when trying to bind to ports: {e}')
-
-
-
-    # print(f'[{local_port}] cycling port ({default_port}) to local_port ({local_port})')
-    # default_port = local_port
-
-    # listen for an incoming connection
-    print(f'[{open_port}] server listening for a connection...')
-    server.listen(5)
-
-    # set client, client address
-    client, client_address = server.accept()
-    print(f'[{open_port}] connected to client at address {client_address}')
-
-    # waits for verification message
-    msg = client.recv(1024).decode('utf-8')
-
-    # if verification message contains "verify", return "verify_confirm"
-    if 'verify' in msg:
-        print(f'[{open_port}] recieved "verify" message, sending "verify_confirm"')
-        msg = "verify_confirm".encode('utf-8')
-        client.sendall(msg)
-        print(f'[{open_port}] verify_confirm sent')
-        if return_port == True:
-            return [client, client_address , open_port] # if port requested, return client, client_address, and the port used for this instance
-        else:
-            return [client, client_address] # if no port requested, return client, client_address
-        
-
-
-# logs username data into client_dict (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
-def log_username_data(username: str, address: str, port: int) -> None:
-    global client_dict
-    client_dict[username] = address
-    print(f'[{port}] logged username ({username})  and address ({address}) to client dict')
-
-
-
-# answer requests with a username with the data assigned to that username -> ip, port
-def answer_request_by_username(client: socket.socket, client_address: str, port: int, client_dict: dict, username: str) -> None:
-    # if string not empty, continue
-    if username:
-        print(f'[{port}] client requested data associated with "{username}", searching for in client_dict...')
-        # try to search for that username in the databse
-        try:
-            req_details = str(client_dict[username])
-            print(f'[{port}] data acquired by username: {req_details}')
-            msg = req_details.encode('utf-8')
-            # client.sendall(msg)
-            #client.sendto(msg, client_address)
-            print(f'[{port}] address found')
-
-        # if failed, then there is no person of that username, send that back
-        except:
-            print(f'[{port}] username does not exist in database, returning null')
-            msg = 'null'.encode('utf-8')
-        client.sendall(msg)
-        print(f'[{port}] request results sent back to client')
-
-
-
-# handles inputs while scanning for messages (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
-def input_handler(client: socket.socket, client_address: str, server: socket.socket, server_port: int) -> None:
-    global client_dict, alive_bound_instance
-    # starts
-    print(f'----------------------\n[{server_port}] INPUT HANDLER STARTED\n----------------------')
-
-    # starts thread to check for what sockets are alive (disabled, currently) 
-    print(f'[{server_port}] starting alive check loop...') ################################################
-    threading.Thread(target=lambda:check_alive(), daemon=True).start() ################################################
-
-    # internal loop
-    while True: 
-        # see if the current server is supposed to be alive
-        is_alive = unique_server_instance_dict[server_port][0]
-        if is_alive == False:
-            print(f'[{server_port}] this server on port {server_port} has no active client, and will therefore terminate its process')
-            # close client and server if this port is not connected to a client
-            server.close()
-            client.close()
-            # lower how many are considered alive and bound so a new instance can be made 
-            alive_bound_instance -= 1
-            break
-
-        # try to recieve a message from the client
-        try:
-            msg = client.recv(1024).decode('utf-8')
-
-        # failed due to lack of connection, or whatnot -> close server and client
-        except Exception as e:
-            # print(f'[{server_port}] the client on port {server_port} has been closed, and the server will therefore terminate its process')
-            print(f'[{server_port} - ERROR] server has recieved an error, terminating: {e}')
-            server.close()
-            client.close()
-            # lower how many are considered alive and bound so a new instance can be made 
-            alive_bound_instance -= 1
-            break
-        
-        # if message is not empty, continue
-        if msg:
-            # split message into a list, see command (list[0], assigned to "prefix")
-            split_msg = str(msg).split()
-            print('---------------- MSG:', msg)
-            print('----------------SPLIT MSG:', split_msg)
-            prefix = split_msg[0]
-
-            # if prefix is username, remove the prefix from the string and re-connect it together
-            if prefix == 'username':
-                print(f'[{server_port}] -- username prefix detected')
-                split_msg.remove(prefix)
-                username = "".join(split_msg)
-                # call on the function to log username data, passing in -> username, client_address, server_port (just for printing)
-                log_username_data(username, client_address, server_port)
-
-            # elif prefix is request_ip_by_user, remove the prefix from the string and re-connect it together
-            elif prefix == 'request_ip_by_user':
-                print(f'[{server_port}] -- request_ip_by_user prefix detected')
-                split_msg.remove(prefix)
-                username = "".join(split_msg)
-                # call on the function to answer this request, passing in -> client, client_address, server_port, client_dict, username
-                answer_request_by_username(client, client_address, server_port, client_dict, username)
-
-    # exit if the code broke out of the loop
-    exit()
-
-
-
-# this function is called on to set up the initial server instance (thread) (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
-def start_server_instance(instance_at_start: int) -> None:
-    global alive_searching_instance, alive_bound_instance, unique_server_instance_dict
-
-    # initially make server binded before loop
-    server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    # server = socket.socket(socket.AF_INET, socket.TCP_NODELAY)
-
-    # set the client object, the clients address, and the servers binded port from connect_to_client, passing in a server socket
-    print(f'[SERVER STARTER-{instance_at_start}] starting a new searching server instance with num: {instance_at_start}')
-    client, client_address, server_port = connect_to_client(server, return_port=True)
-    print(f'[SERVER STARTER-{instance_at_start}] server instance {instance_at_start} binded to client')
-
-    # sign into the dictionary, passing in -> alive or dead (bool, default is True as we are starting), server socket, client_socket
-    print(f'[SERVER STARTER-{instance_at_start}] client address, server port: {client_address}, {server_port}')
-    unique_server_instance_dict[server_port] = [True, server, client]
-    print(f'[SERVER STARTER-{instance_at_start}] signing in to active dict with port, logging True and main_client')
-
-    # lower searching as server instance has found client, increase bound (will trigger a new instance creation)
-    print(f'[SERVER STARTER-{instance_at_start}] decreasing search and increasing bound')
-    alive_searching_instance -= 1
-    alive_bound_instance += 1
-    print(f'[SERVER STARTER-{instance_at_start}] searching is now:', alive_searching_instance)
-    print(f'[SERVER STARTER-{instance_at_start}] bound is now:', alive_bound_instance)
-
-    # start the input handler, this thread has now finished its task
-    print(f'[SERVER STARTER-{instance_at_start}] transferring to input handler') 
-    input_handler(client, client_address, server, server_port)
-
-
-
-# the manager for starting server instances (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
-def start_instance_handler() -> None:
-    global alive_searching_instance, alive_bound_instance, initial_limit_print
-    
-    # main loop
-    while True:
-        # if no instances are searching, continue
-        if alive_searching_instance == 0:
-            # if the amount of bound instances is below the limit, start a new instance (assigned a cosmetic num which is alive_bound_instance + 1)
-            if alive_bound_instance < INSTANCE_LIMIT:
-                initial_limit_print = False
-                # increment alive_bound_instance
-                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (before)')
-                alive_searching_instance += 1
-                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (after)')
-                
-                # create a var, then immediately start, this gets overwritten when a new one is created
-                new_server_thread = threading.Thread(target=lambda:start_server_instance(alive_bound_instance + 1), daemon=True)
-                new_server_thread.start()
-
-            # if we are the limit, print taht we are (initial_limit_print used to not spam console) and finish
-            else:
-                if initial_limit_print == False:
-                    time.sleep(3) # time for other things to calm down
-                    print(f'[SERVER HANDLER] INSTANCE LIMIT REACHED, NO MORE INSTANCES WILL BE MADE\n[SERVER HANDLER] BOUND COUNT: {alive_bound_instance}')
-                    initial_limit_print = True
-
-
-
-
-# the only acting line, calling on the handler which handles everything
+import socket
+import random
+import time
+import threading
+
+# all valid ports to cycle through
+valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112
+]
+
+# set limit for server instances
+INSTANCE_LIMIT = 5
+initial_limit_print = False
+alive_bound_instance = 0
+alive_searching_instance = 0
+
+# set port limits, defaults
+not_inclusive_max_port_amount = len(valid_ports) - 1
+default_port = valid_ports[0]
+
+# set up client dict, storing username to ip correlation
+client_dict = {
+    'default': 0
+}
+
+# a dictionary where a port number is associated with [State of living (bool), server_socket, client_socket] NOTE: server_socket is not used
+unique_server_instance_dict = {}
+for port in valid_ports:
+    unique_server_instance_dict[port] = [False, 'x', 'x']
+
+
+
+
+
+### FUNCTIONS
+
+## TOOlS
+
+# a function that is ran and evaluates all sockets, killing them if neccesary (thread) (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
+def check_alive() -> None:
+    global unique_server_instance_dict
+    import time
+    while True:
+        for port in valid_ports:
+            try:
+                data = unique_server_instance_dict[port]
+                state = data[0]
+                server_obj = data[1]
+                client_obj = data[2]
+                closed = is_socket_closed(client_obj)
+                if closed == True:
+                    print(f'[ALIVE SCANNER] the client for port {port} is not responsive, so the connection will be terminated.')
+                    unique_server_instance_dict[port] = [False, server_obj, client_obj]
+                    print(f'[ALIVE SCANNER] closing associated server and client...')
+                    server_obj.close()
+                    client_obj.close()
+                # else:
+                    # print(f'{por} is connected to a client and healthy')
+            except:
+                pass
+                # print('not checking this port as they have not signed on yet')
+        time.sleep(5)
+
+
+
+# A function to check if the socket is closed (not sure how it works, though)
+# https://stackoverflow.com/questions/48024720/python-how-to-check-if-socket-is-still-connected
+def is_socket_closed(sock: socket.socket) -> bool:
+    try:
+        # this will try to read bytes without blocking and also without removing them from buffer (peek only)
+        data = sock.recv(16, socket.MSG_DONTWAIT | socket.MSG_PEEK)
+        # data = sock.recv(16)
+        if len(data) == 0:
+            return True
+        
+    except BlockingIOError:
+        return False  # socket is open and reading from it would block
+    except ConnectionResetError:
+        return True  # socket was closed for some other reason
+    except Exception as e:
+        #logger.exception("unexpected exception when checking if a socket is closed")
+        return False
+    return False
+
+
+
+
+
+
+
+
+
+## CORE FUNCTIONS
+# connect to client
+def connect_to_client(server: socket.socket, port_override: int = 0, return_port: bool = False) -> list:
+    # access global
+    #local_port = default_port
+
+
+    try:
+        # iterate through valid ports, check if any are not alive in unique_server_instance_dict
+        found_open = False
+        if port_override == 0:
+            for port in valid_ports:
+                data = unique_server_instance_dict[port]
+                is_alive = data[0]
+                server_obj = data[1]
+                client_obj = data[2]
+                if is_alive == False:
+                    found_open = True
+                    open_port = port
+                    break
+            if found_open == True:
+                print(f'[unbound] open port found: {open_port}')
+                #server.bind(('', open_port))
+                server.bind(('localhost', open_port))
+                print(f'[{open_port}] server binded to port {open_port}')
+            else:
+                print('[unbound] all ports are being used, cancelling attempt')
+                exit()
+        else:
+            open_port = port_override
+            print(f'[unbound] port overrided to: {open_port}')
+            #server.bind(('', open_port))
+            server.bind(('localhost', open_port))
+            print(f'[{open_port}] server binded to port {open_port}')
+    except Exception as e:
+        print(f'[unbound] an error occured when trying to bind to ports: {e}')
+
+
+
+    # print(f'[{local_port}] cycling port ({default_port}) to local_port ({local_port})')
+    # default_port = local_port
+
+    # listen for an incoming connection
+    print(f'[{open_port}] server listening for a connection...')
+    server.listen(5)
+
+    # set client, client address
+    client, client_address = server.accept()
+    print(f'[{open_port}] connected to client at address {client_address}')
+
+    # waits for verification message
+    msg = client.recv(1024).decode('utf-8')
+
+    # if verification message contains "verify", return "verify_confirm"
+    if 'verify' in msg:
+        print(f'[{open_port}] recieved "verify" message, sending "verify_confirm"')
+        msg = "verify_confirm".encode('utf-8')
+        client.sendall(msg)
+        print(f'[{open_port}] verify_confirm sent')
+        if return_port == True:
+            return [client, client_address , open_port] # if port requested, return client, client_address, and the port used for this instance
+        else:
+            return [client, client_address] # if no port requested, return client, client_address
+        
+
+
+# logs username data into client_dict (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
+def log_username_data(username: str, address: str, port: int) -> None:
+    global client_dict
+    client_dict[username] = address
+    print(f'[{port}] logged username ({username})  and address ({address}) to client dict')
+
+
+
+# answer requests with a username with the data assigned to that username -> ip, port
+def answer_request_by_username(client: socket.socket, client_address: str, port: int, client_dict: dict, username: str) -> None:
+    # if string not empty, continue
+    if username:
+        print(f'[{port}] client requested data associated with "{username}", searching for in client_dict...')
+        # try to search for that username in the databse
+        try:
+            req_details = str(client_dict[username])
+            print(f'[{port}] data acquired by username: {req_details}')
+            msg = req_details.encode('utf-8')
+            # client.sendall(msg)
+            #client.sendto(msg, client_address)
+            print(f'[{port}] address found')
+
+        # if failed, then there is no person of that username, send that back
+        except:
+            print(f'[{port}] username does not exist in database, returning null')
+            msg = 'null'.encode('utf-8')
+        client.sendall(msg)
+        print(f'[{port}] request results sent back to client')
+
+
+
+# handles inputs while scanning for messages (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
+def input_handler(client: socket.socket, client_address: str, server: socket.socket, server_port: int) -> None:
+    global client_dict, alive_bound_instance
+    # starts
+    print(f'----------------------\n[{server_port}] INPUT HANDLER STARTED\n----------------------')
+
+    # starts thread to check for what sockets are alive (disabled, currently) 
+    print(f'[{server_port}] starting alive check loop...') ################################################
+    threading.Thread(target=lambda:check_alive(), daemon=True).start() ################################################
+
+    # internal loop
+    while True: 
+        # see if the current server is supposed to be alive
+        is_alive = unique_server_instance_dict[server_port][0]
+        if is_alive == False:
+            print(f'[{server_port}] this server on port {server_port} has no active client, and will therefore terminate its process')
+            # close client and server if this port is not connected to a client
+            server.close()
+            client.close()
+            # lower how many are considered alive and bound so a new instance can be made 
+            alive_bound_instance -= 1
+            break
+
+        # try to recieve a message from the client
+        try:
+            msg = client.recv(1024).decode('utf-8')
+
+        # failed due to lack of connection, or whatnot -> close server and client
+        except Exception as e:
+            # print(f'[{server_port}] the client on port {server_port} has been closed, and the server will therefore terminate its process')
+            print(f'[{server_port} - ERROR] server has recieved an error, terminating: {e}')
+            server.close()
+            client.close()
+            # lower how many are considered alive and bound so a new instance can be made 
+            alive_bound_instance -= 1
+            break
+        
+        # if message is not empty, continue
+        if msg:
+            # split message into a list, see command (list[0], assigned to "prefix")
+            split_msg = str(msg).split()
+            print('---------------- MSG:', msg)
+            print('----------------SPLIT MSG:', split_msg)
+            prefix = split_msg[0]
+
+            # if prefix is username, remove the prefix from the string and re-connect it together
+            if prefix == 'username':
+                print(f'[{server_port}] -- username prefix detected')
+                split_msg.remove(prefix)
+                username = "".join(split_msg)
+                # call on the function to log username data, passing in -> username, client_address, server_port (just for printing)
+                log_username_data(username, client_address, server_port)
+
+            # elif prefix is request_ip_by_user, remove the prefix from the string and re-connect it together
+            elif prefix == 'request_ip_by_user':
+                print(f'[{server_port}] -- request_ip_by_user prefix detected')
+                split_msg.remove(prefix)
+                username = "".join(split_msg)
+                # call on the function to answer this request, passing in -> client, client_address, server_port, client_dict, username
+                answer_request_by_username(client, client_address, server_port, client_dict, username)
+
+    # exit if the code broke out of the loop
+    exit()
+
+
+
+# this function is called on to set up the initial server instance (thread) (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
+def start_server_instance(instance_at_start: int) -> None:
+    global alive_searching_instance, alive_bound_instance, unique_server_instance_dict
+
+    # initially make server binded before loop
+    server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    # server = socket.socket(socket.AF_INET, socket.TCP_NODELAY)
+
+    # set the client object, the clients address, and the servers binded port from connect_to_client, passing in a server socket
+    print(f'[SERVER STARTER-{instance_at_start}] starting a new searching server instance with num: {instance_at_start}')
+    client, client_address, server_port = connect_to_client(server, return_port=True)
+    print(f'[SERVER STARTER-{instance_at_start}] server instance {instance_at_start} binded to client')
+
+    # sign into the dictionary, passing in -> alive or dead (bool, default is True as we are starting), server socket, client_socket
+    print(f'[SERVER STARTER-{instance_at_start}] client address, server port: {client_address}, {server_port}')
+    unique_server_instance_dict[server_port] = [True, server, client]
+    print(f'[SERVER STARTER-{instance_at_start}] signing in to active dict with port, logging True and main_client')
+
+    # lower searching as server instance has found client, increase bound (will trigger a new instance creation)
+    print(f'[SERVER STARTER-{instance_at_start}] decreasing search and increasing bound')
+    alive_searching_instance -= 1
+    alive_bound_instance += 1
+    print(f'[SERVER STARTER-{instance_at_start}] searching is now:', alive_searching_instance)
+    print(f'[SERVER STARTER-{instance_at_start}] bound is now:', alive_bound_instance)
+
+    # start the input handler, this thread has now finished its task
+    print(f'[SERVER STARTER-{instance_at_start}] transferring to input handler') 
+    input_handler(client, client_address, server, server_port)
+
+
+
+# the manager for starting server instances (ONE OF THE FEW FUNCTIONS WITH GLOBAL ACCESS TO VARS)
+def start_instance_handler() -> None:
+    global alive_searching_instance, alive_bound_instance, initial_limit_print
+    
+    # main loop
+    while True:
+        # if no instances are searching, continue
+        if alive_searching_instance == 0:
+            # if the amount of bound instances is below the limit, start a new instance (assigned a cosmetic num which is alive_bound_instance + 1)
+            if alive_bound_instance < INSTANCE_LIMIT:
+                initial_limit_print = False
+                # increment alive_bound_instance
+                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (before)')
+                alive_searching_instance += 1
+                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (after)')
+                
+                # create a var, then immediately start, this gets overwritten when a new one is created
+                new_server_thread = threading.Thread(target=lambda:start_server_instance(alive_bound_instance + 1), daemon=True)
+                new_server_thread.start()
+
+            # if we are the limit, print taht we are (initial_limit_print used to not spam console) and finish
+            else:
+                if initial_limit_print == False:
+                    time.sleep(3) # time for other things to calm down
+                    print(f'[SERVER HANDLER] INSTANCE LIMIT REACHED, NO MORE INSTANCES WILL BE MADE\n[SERVER HANDLER] BOUND COUNT: {alive_bound_instance}')
+                    initial_limit_print = True
+
+
+
+
+# the only acting line, calling on the handler which handles everything
 start_instance_handler()
```

### Comparing `lynxy-0.0.4/tests/server.py` & `lynxy-0.0.5/tests/server.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,375 +1,375 @@
-import socket
-import random
-import time
-import threading
-
-valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112
-]
-
-
-# set limit for server instances
-INSTANCE_LIMIT = 5
-initial_limit_print = False
-alive_bound_instance = 0
-alive_searching_instance = 0
-
-# create server object, set port
-#main_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-# port = 11111
-# port_iter = 0 
-# valid_ports = v.valid_ports
-not_inclusive_max_port_amount = len(valid_ports) - 1
-port = valid_ports[0]
-
-# set up client dict, storing name to ip correlation
-client_dict = {
-    'default': 0
-}
-
-unique_server_instance_dict = {}
-message_lookup = {}
-
-
-
-
-# def recv_all(client_socket, n): ################################################
-#     # Helper function to receive n bytes or return None if EOF is hit
-#     data = bytearray()
-#     while len(data) < n:
-#         packet = client_socket.recv(n - len(data))
-#         if not packet:
-#             return None
-#         data.extend(packet)
-#     return data
-
-
-
-
-
-# connect to client
-def connect_to_client(server: socket.socket, return_port: bool = False) -> list[socket.socket, str, int]:
-    global port
-    local_port = port
-    # bind to first incoming ip, and port
-    #server.bind(('', port))
-    #print(f'server binded to port {port}')
-    while True:
-        try:
-            print(f'[unbound] attempting to bind to port:', local_port)
-            server.bind(('', local_port))
-            print(f'[{local_port}] server binded to port {local_port}')
-            break
-        except:
-            if valid_ports.index(local_port) < not_inclusive_max_port_amount:
-                print('[unbound] port bind failed, cycling')
-                local_port = valid_ports[valid_ports.index(local_port) + 1]
-                print('[unbound] swapped to port', local_port)
-            else:
-                print('[unbound] all ports are being used, cancelling attempt')
-                exit()
-    print(f'[{local_port}] cycling port ({port}) to local_port ({local_port})')
-    port = local_port
-
-    # listen for an incoming connection
-    print(f'[{local_port}] server listening for a connection...')
-    server.listen(5)
-
-    # set client, client address
-    client, addr = server.accept()
-    print(f'[{local_port}] connected to client at address {addr}')
-
-
-
-
-    # waits for verification message
-    msg = client.recv(1024).decode('utf-8')
-    # msg = recv_all(client, 4) ################################################
-    # message_length = int.from_bytes(msg, byteorder='big') ################################################
-    # msg = recv_all(client, message_length).decode('utf-8') ################################################
-
-
-
-
-    if 'verify' in msg:
-        print(f'[{local_port}] recieved "verify" message, sending "verify_confirm"')
-        msg = "verify_confirm".encode('utf-8')
-        client.sendall(msg)
-        print(f'[{local_port}] message sent')
-        if return_port == True:
-            return [client, addr, local_port]
-        else:
-            return [client, addr]
-
-# intake username data
-# def recieve_username_data(client: socket.socket, msg: str) -> str:
-#     # msg = client.recv(1024).decode('utf-8')
-#     split_msg = msg.split()
-#     if msg:
-#         if split_msg[0] == "username":
-#             split_msg.remove("username")
-#             username = "".join(split_msg)
-#             print(f'username recieved: {username}')
-#             return username
-
-
-
-
-
-
-
-
-
-
-def check_alive() -> None:
-    global unique_server_instance_dict
-    import time
-    while True:
-        for por in valid_ports:
-            try:
-                data = unique_server_instance_dict[port]
-                state = data[0]
-                server_obj = data[1]
-                client_obj = data[2]
-                closed = is_socket_closed(client_obj)
-                if closed == True:
-                    print(f'[ALIVE SCANNER] the client for port {por} is not responsive, so the connection will be terminated.')
-                    unique_server_instance_dict[por] = [False, server_obj, client_obj]
-                # else:
-                    # print(f'{por} is connected to a client and healthy')
-            except:
-                pass
-                # print('not checking this port as they have not signed on yet')
-        time.sleep(5)
-        
-
-
-
-
-
-
-
-# https://stackoverflow.com/questions/48024720/python-how-to-check-if-socket-is-still-connected
-def is_socket_closed(sock: socket.socket) -> bool:
-    try:
-        # this will try to read bytes without blocking and also without removing them from buffer (peek only)
-        #data = sock.recv(16, socket.MSG_DONTWAIT | socket.MSG_PEEK)
-        data = sock.recv(16)
-        if len(data) == 0:
-            return True
-        
-    except BlockingIOError:
-        return False  # socket is open and reading from it would block
-    except ConnectionResetError:
-        return True  # socket was closed for some other reason
-    except Exception as e:
-        #logger.exception("unexpected exception when checking if a socket is closed")
-        return False
-    return False
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# log username data into client_dict
-#def log_username_data(username: str, address: str, c_dict: dict) -> dict:
-def log_username_data(username: str, address: str, po: int) -> None:
-    global client_dict
-    client_dict[username] = address
-    print(f'[{po}] logged username ({username})  and address ({address}) to client dict')
-    #return client_dict
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-def answer_request_by_username(client: socket.socket, client_addr: str, server_po: int, c_dict: dict, cmd: str) -> None:
-    # cmd = client.recv(1024).decode('utf-8')
-    # split_cmd = cmd.split()
-    if cmd:
-        # if split_cmd[0] == 'request_ip_by_user':
-        #     split_cmd.remove('request_ip_by_user')
-            # username = "".join(split_cmd)
-            username = cmd
-            print(f'[{server_po}] client requested data associated with "{username}", searching for in client_dict...')
-            try:
-                req_details = str(c_dict[username])
-                print(f'[{server_po}] data acquired by username: {req_details}')
-                msg = req_details.encode('utf-8')
-                # client.sendall(msg)
-                client.sendto(msg, client_addr)
-                print(f'[{server_po}] address sent back to client')
-            except:
-                print(f'[{server_po}] username does not exist in database, returning None.')
-                msg = 'null'.encode('utf-8')
-                client.sendall(msg)
-
-
-
-
-
-
-# def log_message(client: socket.socket, sport: int) -> None:
-#     global message_lookup
-#     client.settimeout(5)
-#     while True:
-#         try:
-#             msg = client.recv(1024).decode('utf-8')
-#             message_lookup[sport] = msg
-#             print('picked up and logged msg')
-#             print('-------------------', msg)
-#         except:
-#             # print('timed out')
-#             pass
-
-
-
-
-
-
-
-# MAIN MESSAGE HANDLER
-def input_handler(client: socket.socket, client_address: str, server: socket.socket, server_port: int) -> None:
-    global client_dict, alive_bound_instance #, message_lookup
-    print('----------------------')
-    print(f'[{server_port}] INPUT HANDLER STARTED')
-    print('----------------------')
-    print(f'[{server_port}] starting alive check loop...')
-    threading.Thread(target=lambda:check_alive(), daemon=True).start()
-    #threading.Thread(target=lambda:log_message(client, server_port), daemon=True).start()
-    while True: 
-        if unique_server_instance_dict[server_port][0] == False:
-            print(f'[{server_port}] this server on port {server_port} has no active client, and will therefore terminate its process')
-            # try:
-            #     server.shutdown(socket.SHUT_RDWR)
-            #     client.shutdown(socket.SHUT_RDWR)
-            # except:
-            #     pass
-            # server.detach()
-            # client.detach()
-            server.close()
-            client.close()
-            alive_bound_instance -= 1
-            break
-        try:
-            msg = client.recv(1024).decode('utf-8')
-        except:
-            print(f'[{server_port}] client has been closed on port {server_port}, server instance terminating')
-            # try:
-            #     server.shutdown(socket.SHUT_RDWR)
-            #     client.shutdown(socket.SHUT_RDWR)
-            # except:
-            #     pass
-            # server.detach()
-            # client.detach()
-            server.close()
-            client.close()
-            alive_bound_instance -= 1
-            break
-        # try:
-            #msg = message_lookup[server_port]
-        if msg:
-            split_msg = str(msg).split()
-            print('---------------- MSG', msg)
-            print('----------------SPLIT MSG', split_msg)
-            prefix = split_msg[0]
-            if prefix == 'username':
-                print(f'[{server_port}] -- username prefix detected')
-                split_msg.remove(prefix)
-                username = "".join(split_msg)
-                #client_dict = log_username_data(username, client_address, client_dict)
-                log_username_data(username, client_address, server_port)
-                # message_lookup[server_port] = ''
-            elif prefix == 'request_ip_by_user':
-                print(f'[{server_port}] -- request_ip_by_user prefix detected')
-                split_msg.remove(prefix)
-                username = "".join(split_msg)
-                answer_request_by_username(client, client_address, server_port, client_dict, username)
-                # message_lookup[server_port] = ''
-        # except:
-            # pass
-    exit()
-
-
-
-
-
-
-
-def start_server_instance(server: socket.socket, instance_at_start: int) -> None:
-    global alive_searching_instance, alive_bound_instance, unique_server_instance_dict
-    print(f'[SERVER STARTER] starting a new searching instance with num: {instance_at_start}')
-    main_client, client_address, server_port = connect_to_client(server, return_port=True)
-    print('[SERVER STARTER] binded to client, decreasing search and increasing bound')
-    alive_searching_instance -= 1
-    alive_bound_instance += 1
-    print('[SERVER STARTER] bound is now:', alive_bound_instance)
-    print('[SERVER STARTER] signing in to active dict with port, logging True and main_client')
-    print(f'[SERVER STARTER] client address, server port: {client_address}, {server_port}')
-    # active_instance_dict[server_port] = [True, main_client]
-    unique_server_instance_dict[server_port] = [True, server, main_client]
-    # print('logging client address to detect if closed later')
-    # unique_server_instance_dict[main_client] = True
-    print('[SERVER STARTER] transferring to input handler') 
-    input_handler(main_client, client_address, server, server_port)
-
-
-
-
-
-
-
-def start_instance_handler() -> None:
-    global alive_searching_instance, alive_bound_instance, initial_limit_print
-    while True:
-        if alive_searching_instance == 0:
-            if alive_bound_instance < INSTANCE_LIMIT:
-                initial_limit_print = False
-                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (before)')
-                alive_searching_instance += 1
-                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (after)')
-
-                main_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-                # main_server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1) # 1
-                threading.Thread(target=lambda:start_server_instance(main_server, alive_bound_instance + 1), daemon=True).start()
-            else:
-                if initial_limit_print == False:
-                    time.sleep(3) # time for other things to calm down
-                    print('[SERVER HANDLER] INSTANCE LIMIT REACHED, NO MORE INSTANCES WILL BE MADE')
-                    print('[SERVER HANDLER] BOUND COUNT:', alive_bound_instance)
-                    initial_limit_print = True
-
-
-
-
-
-
-
-
-
-# start normal handler
+import socket
+import random
+import time
+import threading
+
+valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112
+]
+
+
+# set limit for server instances
+INSTANCE_LIMIT = 5
+initial_limit_print = False
+alive_bound_instance = 0
+alive_searching_instance = 0
+
+# create server object, set port
+#main_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+# port = 11111
+# port_iter = 0 
+# valid_ports = v.valid_ports
+not_inclusive_max_port_amount = len(valid_ports) - 1
+port = valid_ports[0]
+
+# set up client dict, storing name to ip correlation
+client_dict = {
+    'default': 0
+}
+
+unique_server_instance_dict = {}
+message_lookup = {}
+
+
+
+
+# def recv_all(client_socket, n): ################################################
+#     # Helper function to receive n bytes or return None if EOF is hit
+#     data = bytearray()
+#     while len(data) < n:
+#         packet = client_socket.recv(n - len(data))
+#         if not packet:
+#             return None
+#         data.extend(packet)
+#     return data
+
+
+
+
+
+# connect to client
+def connect_to_client(server: socket.socket, return_port: bool = False) -> list[socket.socket, str, int]:
+    global port
+    local_port = port
+    # bind to first incoming ip, and port
+    #server.bind(('', port))
+    #print(f'server binded to port {port}')
+    while True:
+        try:
+            print(f'[unbound] attempting to bind to port:', local_port)
+            server.bind(('', local_port))
+            print(f'[{local_port}] server binded to port {local_port}')
+            break
+        except:
+            if valid_ports.index(local_port) < not_inclusive_max_port_amount:
+                print('[unbound] port bind failed, cycling')
+                local_port = valid_ports[valid_ports.index(local_port) + 1]
+                print('[unbound] swapped to port', local_port)
+            else:
+                print('[unbound] all ports are being used, cancelling attempt')
+                exit()
+    print(f'[{local_port}] cycling port ({port}) to local_port ({local_port})')
+    port = local_port
+
+    # listen for an incoming connection
+    print(f'[{local_port}] server listening for a connection...')
+    server.listen(5)
+
+    # set client, client address
+    client, addr = server.accept()
+    print(f'[{local_port}] connected to client at address {addr}')
+
+
+
+
+    # waits for verification message
+    msg = client.recv(1024).decode('utf-8')
+    # msg = recv_all(client, 4) ################################################
+    # message_length = int.from_bytes(msg, byteorder='big') ################################################
+    # msg = recv_all(client, message_length).decode('utf-8') ################################################
+
+
+
+
+    if 'verify' in msg:
+        print(f'[{local_port}] recieved "verify" message, sending "verify_confirm"')
+        msg = "verify_confirm".encode('utf-8')
+        client.sendall(msg)
+        print(f'[{local_port}] message sent')
+        if return_port == True:
+            return [client, addr, local_port]
+        else:
+            return [client, addr]
+
+# intake username data
+# def recieve_username_data(client: socket.socket, msg: str) -> str:
+#     # msg = client.recv(1024).decode('utf-8')
+#     split_msg = msg.split()
+#     if msg:
+#         if split_msg[0] == "username":
+#             split_msg.remove("username")
+#             username = "".join(split_msg)
+#             print(f'username recieved: {username}')
+#             return username
+
+
+
+
+
+
+
+
+
+
+def check_alive() -> None:
+    global unique_server_instance_dict
+    import time
+    while True:
+        for por in valid_ports:
+            try:
+                data = unique_server_instance_dict[port]
+                state = data[0]
+                server_obj = data[1]
+                client_obj = data[2]
+                closed = is_socket_closed(client_obj)
+                if closed == True:
+                    print(f'[ALIVE SCANNER] the client for port {por} is not responsive, so the connection will be terminated.')
+                    unique_server_instance_dict[por] = [False, server_obj, client_obj]
+                # else:
+                    # print(f'{por} is connected to a client and healthy')
+            except:
+                pass
+                # print('not checking this port as they have not signed on yet')
+        time.sleep(5)
+        
+
+
+
+
+
+
+
+# https://stackoverflow.com/questions/48024720/python-how-to-check-if-socket-is-still-connected
+def is_socket_closed(sock: socket.socket) -> bool:
+    try:
+        # this will try to read bytes without blocking and also without removing them from buffer (peek only)
+        #data = sock.recv(16, socket.MSG_DONTWAIT | socket.MSG_PEEK)
+        data = sock.recv(16)
+        if len(data) == 0:
+            return True
+        
+    except BlockingIOError:
+        return False  # socket is open and reading from it would block
+    except ConnectionResetError:
+        return True  # socket was closed for some other reason
+    except Exception as e:
+        #logger.exception("unexpected exception when checking if a socket is closed")
+        return False
+    return False
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# log username data into client_dict
+#def log_username_data(username: str, address: str, c_dict: dict) -> dict:
+def log_username_data(username: str, address: str, po: int) -> None:
+    global client_dict
+    client_dict[username] = address
+    print(f'[{po}] logged username ({username})  and address ({address}) to client dict')
+    #return client_dict
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+def answer_request_by_username(client: socket.socket, client_addr: str, server_po: int, c_dict: dict, cmd: str) -> None:
+    # cmd = client.recv(1024).decode('utf-8')
+    # split_cmd = cmd.split()
+    if cmd:
+        # if split_cmd[0] == 'request_ip_by_user':
+        #     split_cmd.remove('request_ip_by_user')
+            # username = "".join(split_cmd)
+            username = cmd
+            print(f'[{server_po}] client requested data associated with "{username}", searching for in client_dict...')
+            try:
+                req_details = str(c_dict[username])
+                print(f'[{server_po}] data acquired by username: {req_details}')
+                msg = req_details.encode('utf-8')
+                # client.sendall(msg)
+                client.sendto(msg, client_addr)
+                print(f'[{server_po}] address sent back to client')
+            except:
+                print(f'[{server_po}] username does not exist in database, returning None.')
+                msg = 'null'.encode('utf-8')
+                client.sendall(msg)
+
+
+
+
+
+
+# def log_message(client: socket.socket, sport: int) -> None:
+#     global message_lookup
+#     client.settimeout(5)
+#     while True:
+#         try:
+#             msg = client.recv(1024).decode('utf-8')
+#             message_lookup[sport] = msg
+#             print('picked up and logged msg')
+#             print('-------------------', msg)
+#         except:
+#             # print('timed out')
+#             pass
+
+
+
+
+
+
+
+# MAIN MESSAGE HANDLER
+def input_handler(client: socket.socket, client_address: str, server: socket.socket, server_port: int) -> None:
+    global client_dict, alive_bound_instance #, message_lookup
+    print('----------------------')
+    print(f'[{server_port}] INPUT HANDLER STARTED')
+    print('----------------------')
+    print(f'[{server_port}] starting alive check loop...')
+    threading.Thread(target=lambda:check_alive(), daemon=True).start()
+    #threading.Thread(target=lambda:log_message(client, server_port), daemon=True).start()
+    while True: 
+        if unique_server_instance_dict[server_port][0] == False:
+            print(f'[{server_port}] this server on port {server_port} has no active client, and will therefore terminate its process')
+            # try:
+            #     server.shutdown(socket.SHUT_RDWR)
+            #     client.shutdown(socket.SHUT_RDWR)
+            # except:
+            #     pass
+            # server.detach()
+            # client.detach()
+            server.close()
+            client.close()
+            alive_bound_instance -= 1
+            break
+        try:
+            msg = client.recv(1024).decode('utf-8')
+        except:
+            print(f'[{server_port}] client has been closed on port {server_port}, server instance terminating')
+            # try:
+            #     server.shutdown(socket.SHUT_RDWR)
+            #     client.shutdown(socket.SHUT_RDWR)
+            # except:
+            #     pass
+            # server.detach()
+            # client.detach()
+            server.close()
+            client.close()
+            alive_bound_instance -= 1
+            break
+        # try:
+            #msg = message_lookup[server_port]
+        if msg:
+            split_msg = str(msg).split()
+            print('---------------- MSG', msg)
+            print('----------------SPLIT MSG', split_msg)
+            prefix = split_msg[0]
+            if prefix == 'username':
+                print(f'[{server_port}] -- username prefix detected')
+                split_msg.remove(prefix)
+                username = "".join(split_msg)
+                #client_dict = log_username_data(username, client_address, client_dict)
+                log_username_data(username, client_address, server_port)
+                # message_lookup[server_port] = ''
+            elif prefix == 'request_ip_by_user':
+                print(f'[{server_port}] -- request_ip_by_user prefix detected')
+                split_msg.remove(prefix)
+                username = "".join(split_msg)
+                answer_request_by_username(client, client_address, server_port, client_dict, username)
+                # message_lookup[server_port] = ''
+        # except:
+            # pass
+    exit()
+
+
+
+
+
+
+
+def start_server_instance(server: socket.socket, instance_at_start: int) -> None:
+    global alive_searching_instance, alive_bound_instance, unique_server_instance_dict
+    print(f'[SERVER STARTER] starting a new searching instance with num: {instance_at_start}')
+    main_client, client_address, server_port = connect_to_client(server, return_port=True)
+    print('[SERVER STARTER] binded to client, decreasing search and increasing bound')
+    alive_searching_instance -= 1
+    alive_bound_instance += 1
+    print('[SERVER STARTER] bound is now:', alive_bound_instance)
+    print('[SERVER STARTER] signing in to active dict with port, logging True and main_client')
+    print(f'[SERVER STARTER] client address, server port: {client_address}, {server_port}')
+    # active_instance_dict[server_port] = [True, main_client]
+    unique_server_instance_dict[server_port] = [True, server, main_client]
+    # print('logging client address to detect if closed later')
+    # unique_server_instance_dict[main_client] = True
+    print('[SERVER STARTER] transferring to input handler') 
+    input_handler(main_client, client_address, server, server_port)
+
+
+
+
+
+
+
+def start_instance_handler() -> None:
+    global alive_searching_instance, alive_bound_instance, initial_limit_print
+    while True:
+        if alive_searching_instance == 0:
+            if alive_bound_instance < INSTANCE_LIMIT:
+                initial_limit_print = False
+                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (before)')
+                alive_searching_instance += 1
+                print(f'[SERVER HANDLER] starting instance, searching count is {alive_searching_instance} (after)')
+
+                main_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                # main_server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1) # 1
+                threading.Thread(target=lambda:start_server_instance(main_server, alive_bound_instance + 1), daemon=True).start()
+            else:
+                if initial_limit_print == False:
+                    time.sleep(3) # time for other things to calm down
+                    print('[SERVER HANDLER] INSTANCE LIMIT REACHED, NO MORE INSTANCES WILL BE MADE')
+                    print('[SERVER HANDLER] BOUND COUNT:', alive_bound_instance)
+                    initial_limit_print = True
+
+
+
+
+
+
+
+
+
+# start normal handler
 start_instance_handler()
```

### Comparing `lynxy-0.0.4/tests/old/lynx.py` & `lynxy-0.0.5/tests/old/lynx.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import socket
-import time
-import threading
-import json
-
-valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112
-]
-
-# set up server ip, port to connect to
-server_ip = input('enter ip: ')
-# valid_ports = v.valid_ports
-not_inclusive_max_port_amount = len(valid_ports) - 1
-server_port = valid_ports[0]
-
-# start client timeout
-# connection_timeout = False
-
-
-
-
-
-
-
-
-# def timeout_connection(timeout_time: int = 5) -> None:
-#     global connection_timeout
-#     init_time = time.time()
-#     while True:
-#         new_time = time.time()
-#         dif = new_time - init_time
-#         if dif >= timeout_time:
-#             connection_timeout = True
-#             print('timed out')
-#             exit()
-
-
-
-
-
-
-
-
-
-# def info_connect() -> dict:
-#     # attempt to connect to the data server object
-#     info_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-#     info_client.connect((server_ip, 22222))
-#     active_data = info_client.recv(1024).decode('utf-8')
-
-#     active_data = active_data.strip('{}')
-#     # Split by commas to get individual key-value pairs
-#     pairs = active_data.split(',')
-
-#     # Initialize an empty dictionary to store the parsed data
-#     data_dict = {}
-
-#     # Iterate over each pair and split by colon to get key and value
-#     for pair in pairs:
-#         key, value = pair.split(':')
-#         # Strip spaces and convert key to integer
-#         key = int(key.strip())
-#         # Evaluate value and store it in the dictionary
-#         value = eval(value.strip())
-#         data_dict[key] = value
-
-#     return data_dict
-
-
-
-
-# connects to server
-def connect_to_server(client: socket.socket):
-    global server_port, connection_timeout
-    '''sets up the initial connection to the server, verifies it can send data over'''
-    
-    # connect to server ip, server port
-    print('cycling connection to server until succeed / fail...')
-    attempt_count = 0
-    while True:
-        print(f'attempt: {attempt_count}')
-        try:
-            print('trying port:', server_port)
-            # con_thread = threading.Thread(target=lambda:client.connect((server_ip, server_port)))
-            # con_thread.start()
-            # tm_thread = threading.Thread(target=lambda:timeout_connection())
-            # tm_thread.start()
-            # if connection_timeout == True:
-            #     print('timed out - main')
-            # if con_thread.is_alive() == False:
-            #client.connect((server_ip, server_port))
-            client.connect(('localhost', server_port))
-            break
-        except Exception as e:
-            # print('error:', e)
-            # exit()
-            attempt_count += 1
-            if attempt_count > 0:
-                print('failed, moving to next port')
-                if valid_ports.index(server_port) < not_inclusive_max_port_amount:
-                    server_port = valid_ports[valid_ports.index(server_port) + 1]
-                    print('swapped to port', server_port)
-                else:
-                    print('all ports exhausted, exiting')
-                    exit()
-                attempt_count = 0
-            # attempt_count += 1
-            # if attempt_count > 9:
-            #     print('connection failed 10 times, exiting')
-            #     exit()
-
-    # loop until get verify back
-    while True:
-        msg = "verify"
-        # message_length = len(msg) ################################################ 
-        # client.sendall(message_length.to_bytes(4, byteorder='big'))  # Send the length of the message ################################################
-        client.sendall(msg.encode('utf-8')) # send message  
-        print('sent verify message, waiting for return')
-        incoming = client.recv(1024).decode('utf-8') # recieve message 
-        if incoming == 'verify_confirm': # message to confirm verify = "verify_confirm"
-            print('recieved verify_confirm')
-            break # breaks out of loop when it recieves
-    print('connection made, verified connection')
-
-
-
-
-
-
-
-
-
-def submit_username_data(client: socket.socket, username: str) -> None:
-    '''submits username to the server that gets associated with this clients ip address
-    NOTE: USERNAME CAN HAVE NO SPACES, ANY SPACES WILL BE REMOVED'''
-    msg = f'username {username}'.encode('utf-8')
-    # message_length = len(msg) # chatty
-    # client.sendall(message_length.to_bytes(4, byteorder='big')) # chatty
-    client.sendall(msg)
-    print(f'submitted username to server: {username}')
-
-
-
-
-
-
-
-
-
-
-def request_by_username(client: socket.socket, username: str) -> tuple:
-    '''requests an address from the server, getting back an ip address and port'''
-    msg = f'request_ip_by_user {username}'.encode('utf-8')
-    # print('senttoff msg:', msg)
-    client.sendall(msg)
-    target_data = client.recv(1024).decode('utf-8')
-    if target_data == 'null':
-        print('request failed, there is not currently anyone using that username')
-        return ('x', 0)
-    else:
-        # ????????????????????????????????????????
-        target_data = target_data.strip('()')
-        target_ip, target_port = target_data.split(',')
-        target_ip = target_ip.strip().strip("'")
-        target_port = target_port.strip()
-        target_port = int(target_port)
-        print(f'acquired ip and port of {username}, respectively: {target_ip}, {target_port}')
-        return (target_ip, target_port)
-
-
-
-
-
-
-
-# port = valid_ports[0]
-for port in valid_ports:
-    server_port = port
-    main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    print('CLIENT: CONNECTING TO PORT', port)
-    connect_to_server(main_client)
-    submit_username_data(main_client, 'SketchedDoughnut')
-    time.sleep(1) # NECESSARY OR MESSAGES GET SCRAMBLED AND CUT OFF BY EACHOTHER
-    target_ip, target_port = request_by_username(main_client, 'SketchedDoughnut')
+import socket
+import time
+import threading
+import json
+
+valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112
+]
+
+# set up server ip, port to connect to
+server_ip = input('enter ip: ')
+# valid_ports = v.valid_ports
+not_inclusive_max_port_amount = len(valid_ports) - 1
+server_port = valid_ports[0]
+
+# start client timeout
+# connection_timeout = False
+
+
+
+
+
+
+
+
+# def timeout_connection(timeout_time: int = 5) -> None:
+#     global connection_timeout
+#     init_time = time.time()
+#     while True:
+#         new_time = time.time()
+#         dif = new_time - init_time
+#         if dif >= timeout_time:
+#             connection_timeout = True
+#             print('timed out')
+#             exit()
+
+
+
+
+
+
+
+
+
+# def info_connect() -> dict:
+#     # attempt to connect to the data server object
+#     info_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+#     info_client.connect((server_ip, 22222))
+#     active_data = info_client.recv(1024).decode('utf-8')
+
+#     active_data = active_data.strip('{}')
+#     # Split by commas to get individual key-value pairs
+#     pairs = active_data.split(',')
+
+#     # Initialize an empty dictionary to store the parsed data
+#     data_dict = {}
+
+#     # Iterate over each pair and split by colon to get key and value
+#     for pair in pairs:
+#         key, value = pair.split(':')
+#         # Strip spaces and convert key to integer
+#         key = int(key.strip())
+#         # Evaluate value and store it in the dictionary
+#         value = eval(value.strip())
+#         data_dict[key] = value
+
+#     return data_dict
+
+
+
+
+# connects to server
+def connect_to_server(client: socket.socket):
+    global server_port, connection_timeout
+    '''sets up the initial connection to the server, verifies it can send data over'''
+    
+    # connect to server ip, server port
+    print('cycling connection to server until succeed / fail...')
+    attempt_count = 0
+    while True:
+        print(f'attempt: {attempt_count}')
+        try:
+            print('trying port:', server_port)
+            # con_thread = threading.Thread(target=lambda:client.connect((server_ip, server_port)))
+            # con_thread.start()
+            # tm_thread = threading.Thread(target=lambda:timeout_connection())
+            # tm_thread.start()
+            # if connection_timeout == True:
+            #     print('timed out - main')
+            # if con_thread.is_alive() == False:
+            #client.connect((server_ip, server_port))
+            client.connect(('localhost', server_port))
+            break
+        except Exception as e:
+            # print('error:', e)
+            # exit()
+            attempt_count += 1
+            if attempt_count > 0:
+                print('failed, moving to next port')
+                if valid_ports.index(server_port) < not_inclusive_max_port_amount:
+                    server_port = valid_ports[valid_ports.index(server_port) + 1]
+                    print('swapped to port', server_port)
+                else:
+                    print('all ports exhausted, exiting')
+                    exit()
+                attempt_count = 0
+            # attempt_count += 1
+            # if attempt_count > 9:
+            #     print('connection failed 10 times, exiting')
+            #     exit()
+
+    # loop until get verify back
+    while True:
+        msg = "verify"
+        # message_length = len(msg) ################################################ 
+        # client.sendall(message_length.to_bytes(4, byteorder='big'))  # Send the length of the message ################################################
+        client.sendall(msg.encode('utf-8')) # send message  
+        print('sent verify message, waiting for return')
+        incoming = client.recv(1024).decode('utf-8') # recieve message 
+        if incoming == 'verify_confirm': # message to confirm verify = "verify_confirm"
+            print('recieved verify_confirm')
+            break # breaks out of loop when it recieves
+    print('connection made, verified connection')
+
+
+
+
+
+
+
+
+
+def submit_username_data(client: socket.socket, username: str) -> None:
+    '''submits username to the server that gets associated with this clients ip address
+    NOTE: USERNAME CAN HAVE NO SPACES, ANY SPACES WILL BE REMOVED'''
+    msg = f'username {username}'.encode('utf-8')
+    # message_length = len(msg) # chatty
+    # client.sendall(message_length.to_bytes(4, byteorder='big')) # chatty
+    client.sendall(msg)
+    print(f'submitted username to server: {username}')
+
+
+
+
+
+
+
+
+
+
+def request_by_username(client: socket.socket, username: str) -> tuple:
+    '''requests an address from the server, getting back an ip address and port'''
+    msg = f'request_ip_by_user {username}'.encode('utf-8')
+    # print('senttoff msg:', msg)
+    client.sendall(msg)
+    target_data = client.recv(1024).decode('utf-8')
+    if target_data == 'null':
+        print('request failed, there is not currently anyone using that username')
+        return ('x', 0)
+    else:
+        # ????????????????????????????????????????
+        target_data = target_data.strip('()')
+        target_ip, target_port = target_data.split(',')
+        target_ip = target_ip.strip().strip("'")
+        target_port = target_port.strip()
+        target_port = int(target_port)
+        print(f'acquired ip and port of {username}, respectively: {target_ip}, {target_port}')
+        return (target_ip, target_port)
+
+
+
+
+
+
+
+# port = valid_ports[0]
+for port in valid_ports:
+    server_port = port
+    main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    print('CLIENT: CONNECTING TO PORT', port)
+    connect_to_server(main_client)
+    submit_username_data(main_client, 'SketchedDoughnut')
+    time.sleep(1) # NECESSARY OR MESSAGES GET SCRAMBLED AND CUT OFF BY EACHOTHER
+    target_ip, target_port = request_by_username(main_client, 'SketchedDoughnut')
     time.sleep(1)
```

### Comparing `lynxy-0.0.4/tests/sock/modclient.py` & `lynxy-0.0.5/tests/sock/modclient.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# this below code has been contributed to by chat gpt
-import socket
-import time
-
-valid_ports = [
-    11111,
-    12111,
-    11211,
-    11121,
-    11112,
-    22111,
-    12211,
-    11221,
-    11122
-]
-
-# define all global vars
-HOST, PORT = '', valid_ports[0] # localhost
-main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-
-
-
-## FUNCTIONS
-# cycles port connection
-def cycle_port(client: socket.socket) -> socket.socket:
-    connected = False
-    for port in valid_ports:
-        try:
-            print(f'[PORT CYCLE] Client trying port: {port}')
-            client.connect((HOST, port))
-            print(f'[PORT CYCLE] Client connected to: {port}')
-            print('----------------------------------------------')
-            connected = True
-            break
-        except IndexError:
-            port = valid_ports[0]
-            print(f'[PORT CYCLE - RESET 1] Client resetting port to: {port}')
-        except:
-            try:
-                print(f'[PORT CYCLE] Client port cycling: {port} -> {valid_ports[valid_ports.index(port) + 1]}')
-            except IndexError:
-                port = valid_ports[0]
-                print(f'[PORT CYCLE - RESET 2] Client resetting port to: {port}')
-    if connected == True:
-        return client, port
-    else:
-        print('[PORT CYCLE] the client can not find a open valid server port, exiting')
-        exit()
-
-
-
-# a function to fully recieve the message from server (to try and prevent loss)
-def full_recieve(client: socket.socket) -> str:
-    message_length = len(client.recv(1024).decode('utf-8'))
-    incoming_message = ''
-    local_length = 0
-    while local_length <= message_length:
-        incoming_message += client.recv(1024).decode('utf-8')
-        local_length = len(incoming_message)
-    return incoming_message
-
-
-
-# a function for submitting username data to the server
-def submit_username_data(client: socket.socket, message: str) -> None:
-    encoded_message  = message.encode('utf-8')
-    client.sendall(encoded_message)
-    print(f"Sent:     {message}")
-    incoming_data = client.recv(1024).decode('utf-8')
-    print(f"Received: {incoming_data}")
-
-
-# requests ip and port from server
-def request_data(client: socket.socket, message: str) -> socket.socket:
-    encoded_message = message.encode('utf-8')
-    client.sendall(encoded_message)
-    print(f"Sent:     {message}")
-    # incoming_data = full_recieve(client)
-    incoming_data = client.recv(1024).decode('utf-8')
-    print(f"Received: {incoming_data}")
-
-
-
-# a general message sender
-def general_send(client: socket.socket, message: str) -> None:
-    encoded_message = message.encode('utf-8')
-    client.sendall(encoded_message)
-    print(f"Sent:     {message}")
-    # incoming_data = full_recieve(client)
-    incoming_data = client.recv(1024).decode('utf-8')
-    print(f"Received: {incoming_data}")
-
-
-
-
-# establish the connection to a port that the server is on
-main_client, PORT = cycle_port(main_client)
-
-# next, send a send a message to the server
-submit_username_data(main_client, 'username SketchedDoughnut')
-
-# necessary delay
-time.sleep(1)
-
-# next, request username data
-request_data(main_client, 'request_by_user SketchedDoughnut')
-
-# necessary delay
-time.sleep(1)
-
-# finally, end the session
+# this below code has been contributed to by chat gpt
+import socket
+import time
+
+valid_ports = [
+    11111,
+    12111,
+    11211,
+    11121,
+    11112,
+    22111,
+    12211,
+    11221,
+    11122
+]
+
+# define all global vars
+HOST, PORT = '', valid_ports[0] # localhost
+main_client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+
+
+## FUNCTIONS
+# cycles port connection
+def cycle_port(client: socket.socket) -> socket.socket:
+    connected = False
+    for port in valid_ports:
+        try:
+            print(f'[PORT CYCLE] Client trying port: {port}')
+            client.connect((HOST, port))
+            print(f'[PORT CYCLE] Client connected to: {port}')
+            print('----------------------------------------------')
+            connected = True
+            break
+        except IndexError:
+            port = valid_ports[0]
+            print(f'[PORT CYCLE - RESET 1] Client resetting port to: {port}')
+        except:
+            try:
+                print(f'[PORT CYCLE] Client port cycling: {port} -> {valid_ports[valid_ports.index(port) + 1]}')
+            except IndexError:
+                port = valid_ports[0]
+                print(f'[PORT CYCLE - RESET 2] Client resetting port to: {port}')
+    if connected == True:
+        return client, port
+    else:
+        print('[PORT CYCLE] the client can not find a open valid server port, exiting')
+        exit()
+
+
+
+# a function to fully recieve the message from server (to try and prevent loss)
+def full_recieve(client: socket.socket) -> str:
+    message_length = len(client.recv(1024).decode('utf-8'))
+    incoming_message = ''
+    local_length = 0
+    while local_length <= message_length:
+        incoming_message += client.recv(1024).decode('utf-8')
+        local_length = len(incoming_message)
+    return incoming_message
+
+
+
+# a function for submitting username data to the server
+def submit_username_data(client: socket.socket, message: str) -> None:
+    encoded_message  = message.encode('utf-8')
+    client.sendall(encoded_message)
+    print(f"Sent:     {message}")
+    incoming_data = client.recv(1024).decode('utf-8')
+    print(f"Received: {incoming_data}")
+
+
+# requests ip and port from server
+def request_data(client: socket.socket, message: str) -> socket.socket:
+    encoded_message = message.encode('utf-8')
+    client.sendall(encoded_message)
+    print(f"Sent:     {message}")
+    # incoming_data = full_recieve(client)
+    incoming_data = client.recv(1024).decode('utf-8')
+    print(f"Received: {incoming_data}")
+
+
+
+# a general message sender
+def general_send(client: socket.socket, message: str) -> None:
+    encoded_message = message.encode('utf-8')
+    client.sendall(encoded_message)
+    print(f"Sent:     {message}")
+    # incoming_data = full_recieve(client)
+    incoming_data = client.recv(1024).decode('utf-8')
+    print(f"Received: {incoming_data}")
+
+
+
+
+# establish the connection to a port that the server is on
+main_client, PORT = cycle_port(main_client)
+
+# next, send a send a message to the server
+submit_username_data(main_client, 'username SketchedDoughnut')
+
+# necessary delay
+time.sleep(1)
+
+# next, request username data
+request_data(main_client, 'request_by_user SketchedDoughnut')
+
+# necessary delay
+time.sleep(1)
+
+# finally, end the session
 general_send(main_client, 'end_session')
```

### Comparing `lynxy-0.0.4/tests/templates-notes/socknotes.py` & `lynxy-0.0.5/tests/templates-notes/socknotes.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# import socket
-
-# ip = '' # localhost
-# port = 1111
-
-# client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-# input('input to start: ')
-# client.connect((ip, port))
-# client.sendall('message from client!'.encode('utf-8'))
-# print(client.recv(1024).decode('utf-8'))
-
-import socket
-
-HOST, PORT = "localhost", 11111
-
-for i in range(2):
-    # data = f"Hello, World: {i}"
-    data = f'request_by_user SketchedDoughnut-{i}'
-    # Create a socket (SOCK_STREAM means a TCP socket)
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-        # Connect to server and send data
-        sock.connect((HOST, PORT))
-        sock.sendall(data.encode('utf-8'))
-
-        # Receive data from the server and shut down
-        received = sock.recv(1024)
-
-    print(f"Sent:     {data}")
+# import socket
+
+# ip = '' # localhost
+# port = 1111
+
+# client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+# input('input to start: ')
+# client.connect((ip, port))
+# client.sendall('message from client!'.encode('utf-8'))
+# print(client.recv(1024).decode('utf-8'))
+
+import socket
+
+HOST, PORT = "localhost", 11111
+
+for i in range(2):
+    # data = f"Hello, World: {i}"
+    data = f'request_by_user SketchedDoughnut-{i}'
+    # Create a socket (SOCK_STREAM means a TCP socket)
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+        # Connect to server and send data
+        sock.connect((HOST, PORT))
+        sock.sendall(data.encode('utf-8'))
+
+        # Receive data from the server and shut down
+        received = sock.recv(1024)
+
+    print(f"Sent:     {data}")
     print(f"Received: {received.decode('utf-8')}")
```

### Comparing `lynxy-0.0.4/tests/templates-notes/sockserver.py` & `lynxy-0.0.5/tests/templates-notes/sockserver.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import socketserver
-
-# https://nora.codes/tutorial/socketserver-the-python-networking-module-you-didnt-know-you-needed/
-class CaaSHandler(socketserver.StreamRequestHandler):
-    def handle(self):
-        self.wfile.write(b"Enter some data to be capitalized:\n")
-        data = self.rfile.readline()
-        self.wfile.write(data.upper())
-
-if __name__ == "__main__":
-    server = socketserver.TCPServer(('', 11111), CaaSHandler)
-    server.serve_forever()
-
-
-'''
-https://pymotw.com/2/SocketServer/
-https://stackoverflow.com/questions/37689518/python-socketserver-or-socket-with-thread
-https://docs.python.org/3/library/socketserver.html
-https://gist.github.com/pklaus/c4c37152e261a9e9331f
-https://www.bogotobogo.com/python/python_network_programming_socketserver_framework_for_network_servers.php#google_vignette
-https://stackoverflow.com/questions/18563664/socketserver-python
-https://realpython.com/courses/python-sockets-part-1/
+import socketserver
+
+# https://nora.codes/tutorial/socketserver-the-python-networking-module-you-didnt-know-you-needed/
+class CaaSHandler(socketserver.StreamRequestHandler):
+    def handle(self):
+        self.wfile.write(b"Enter some data to be capitalized:\n")
+        data = self.rfile.readline()
+        self.wfile.write(data.upper())
+
+if __name__ == "__main__":
+    server = socketserver.TCPServer(('', 11111), CaaSHandler)
+    server.serve_forever()
+
+
+'''
+https://pymotw.com/2/SocketServer/
+https://stackoverflow.com/questions/37689518/python-socketserver-or-socket-with-thread
+https://docs.python.org/3/library/socketserver.html
+https://gist.github.com/pklaus/c4c37152e261a9e9331f
+https://www.bogotobogo.com/python/python_network_programming_socketserver_framework_for_network_servers.php#google_vignette
+https://stackoverflow.com/questions/18563664/socketserver-python
+https://realpython.com/courses/python-sockets-part-1/
 '''
```

### Comparing `lynxy-0.0.4/LICENSE` & `lynxy-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2024 Sketched Doughnut
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2024 Sketched Doughnut
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lynxy-0.0.4/pyproject.toml` & `lynxy-0.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[build-system]
-requires = [
-    "hatchling",
-    "requests"
-]
-build-backend = "hatchling.build"
-
-[tool.hatch.build.targets.wheel]
-packages = [
-    "src/lynxy",
-    "src/lynxy_server"
-]
-
-[project]
-name = "lynxy"
-# version = "0.1.10" # middle number 1 is currently for test pypi
-version = "0.0.4" # pypi release 
-authors = [
-  { name="Sketched Doughnut", email="sketcheddoughnut@gmail.com" },
-]
-description = "A LAN package made for easy communication and sending of data across the same network."
-readme = "info/pypi/PyPi_info.md"
-# requires-python = ">=3.10" 
-requires-python = ">=3.9" # changing which version it needs for test pypi, might keep for release for now - do note this release version works for linux(?) (python3)
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-  "requests"
-]
-
-[project.urls]
-Homepage = "https://github.com/SketchedDoughnut/lynxy"
-Issues = "https://github.com/SketchedDoughnut/lynxy/issues"
+[build-system]
+requires = [
+    "hatchling",
+    "requests"
+]
+build-backend = "hatchling.build"
+
+[tool.hatch.build.targets.wheel]
+packages = [
+    "src/lynxy",
+    "src/lynxy_server"
+]
+
+[project]
+name = "lynxy"
+# version = "0.1.10" # test pypi release
+version = "0.0.5" # pypi release 
+authors = [
+  { name="Sketched Doughnut", email="sketcheddoughnut@gmail.com" },
+]
+description = "A LAN package made for easy communication and sending of data across the same network."
+readme = "info/pypi/PyPi_info.md"
+# requires-python = ">=3.10" 
+requires-python = ">=3.9" # changing which version it needs for test pypi, might keep for release for now - do note this release version works for linux(?) (python3)
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+  "requests"
+]
+
+[project.urls]
+Homepage = "https://github.com/SketchedDoughnut/lynxy"
+Issues = "https://github.com/SketchedDoughnut/lynxy/issues"
```

### Comparing `lynxy-0.0.4/PKG-INFO` & `lynxy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lynxy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A LAN package made for easy communication and sending of data across the same network.
 Project-URL: Homepage, https://github.com/SketchedDoughnut/lynxy
 Project-URL: Issues, https://github.com/SketchedDoughnut/lynxy/issues
 Author-email: Sketched Doughnut <sketcheddoughnut@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

