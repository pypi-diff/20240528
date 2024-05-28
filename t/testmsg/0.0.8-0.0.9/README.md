# Comparing `tmp/testmsg-0.0.8.tar.gz` & `tmp/testmsg-0.0.9.tar.gz`

## Comparing `testmsg-0.0.8.tar` & `testmsg-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 testmsg-0.0.8/accomazzi.com.private
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 testmsg-0.0.8/accomazzi.com.pub
--rwxr-xr-x   0        0        0     1242 2020-02-02 00:00:00.000000 testmsg-0.0.8/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 testmsg-0.0.8/testmsg/__init__.py
--rwxr-xr-x   0        0        0     4799 2020-02-02 00:00:00.000000 testmsg-0.0.8/testmsg/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 testmsg-0.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 testmsg-0.0.8/LICENSE
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 testmsg-0.0.8/README.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 testmsg-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 testmsg-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 testmsg-0.0.9/accomazzi.com.private
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 testmsg-0.0.9/accomazzi.com.pub
+-rwxr-xr-x   0        0        0     1242 2020-02-02 00:00:00.000000 testmsg-0.0.9/setup.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 testmsg-0.0.9/testmsg/__init__.py
+-rwxr-xr-x   0        0        0     4803 2020-02-02 00:00:00.000000 testmsg-0.0.9/testmsg/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 testmsg-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 testmsg-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 testmsg-0.0.9/README.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 testmsg-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 testmsg-0.0.9/PKG-INFO
```

### Comparing `testmsg-0.0.8/accomazzi.com.private` & `testmsg-0.0.9/accomazzi.com.private`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/setup.py` & `testmsg-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/testmsg/__main__.py` & `testmsg-0.0.9/testmsg/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n" \
     "Ut enim ad minim veniam," \
     "quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.\n" \
     "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.\n" \
     "Excepteur sint occaecat cupidatat non proident, " \
     "sunt in culpa qui officia deserunt mollit anim id est laborum.\n"
 
-__version__='0.0.8'
+__version__='0.0.9'
 
 
 def attach(msg: EmailMessage, path: str):
 
     ctype, _ = mimetypes.guess_type(path)
     maintype, subtype = ctype.split('/', 1)
 
@@ -28,15 +28,15 @@
         msg.add_attachment(fp.read(),
                             maintype=maintype,
                             subtype=subtype,
                             filename=path)
 
 
 def get_args():
-    parser = argparse.ArgumentParser(description=f'Generate/Send valid RFC822 email messages for testing {version}')
+    parser = argparse.ArgumentParser(description=f'Generate/Send valid RFC822 email messages for testing {__version__}')
     parser.add_argument('-f', '--from', dest='_from', default='from@example.com', metavar='EMAIL')
     parser.add_argument('-t', '--to', default='to@example.net', metavar='EMAIL')
     parser.add_argument('-s', '--subject', metavar='Subject', default='Sent with github.com/yaroslaff/testmsg')
     parser.add_argument('-a', '--add', nargs=2, action='append', dest='headers', metavar=('HEADER', 'VALUE'), help='add header')
 
 
     g = parser.add_argument_group('Message body')
```

### Comparing `testmsg-0.0.8/.gitignore` & `testmsg-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/LICENSE` & `testmsg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/README.md` & `testmsg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/pyproject.toml` & `testmsg-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.8/PKG-INFO` & `testmsg-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmsg
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple CLI tool to generate/send valid RFC822 email messages (with DKIM optionally)
 Project-URL: Homepage, https://github.com/yaroslaff/testmsg
 Project-URL: Issues, https://github.com/yaroslaff/testmsg/issues
 Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

