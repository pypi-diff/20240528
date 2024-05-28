# Comparing `tmp/1password-1.0.7.tar.gz` & `tmp/1password-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1password-1.0.7.tar", last modified: Fri Dec 22 12:49:48 2023, max compression
+gzip compressed data, was "1password-1.0.8.tar", last modified: Tue May 28 14:19:48 2024, max compression
```

## Comparing `1password-1.0.7.tar` & `1password-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:49:48.824385 1password-1.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:49:48.824385 1password-1.0.7/1password.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2023-12-22 12:49:48.000000 1password-1.0.7/1password.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-22 12:49:48.000000 1password-1.0.7/1password.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 12:49:48.000000 1password-1.0.7/1password.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 12:49:48.000000 1password-1.0.7/1password.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-22 12:49:48.000000 1password-1.0.7/1password.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-22 12:49:37.000000 1password-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-22 12:49:37.000000 1password-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2023-12-22 12:49:48.824385 1password-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2023-12-22 12:49:37.000000 1password-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 12:49:42.000000 1password-1.0.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2023-12-22 12:49:37.000000 1password-1.0.7/install_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:49:48.824385 1password-1.0.7/onepassword/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-22 12:49:37.000000 1password-1.0.7/onepassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2023-12-22 12:49:37.000000 1password-1.0.7/onepassword/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-22 12:49:37.000000 1password-1.0.7/onepassword/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2023-12-22 12:49:37.000000 1password-1.0.7/onepassword/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 12:49:48.824385 1password-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-22 12:49:37.000000 1password-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 12:49:48.824385 1password-1.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2023-12-22 12:49:37.000000 1password-1.0.7/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:19:48.876937 1password-1.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:19:48.872937 1password-1.0.8/1password.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-28 14:19:48.000000 1password-1.0.8/1password.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 14:19:48.000000 1password-1.0.8/1password.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:19:48.000000 1password-1.0.8/1password.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 14:19:48.000000 1password-1.0.8/1password.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 14:19:48.000000 1password-1.0.8/1password.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 14:19:39.000000 1password-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 14:19:39.000000 1password-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-28 14:19:48.876937 1password-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-28 14:19:39.000000 1password-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 14:19:46.000000 1password-1.0.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-28 14:19:39.000000 1password-1.0.8/install_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:19:48.872937 1password-1.0.8/onepassword/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 14:19:39.000000 1password-1.0.8/onepassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19514 2024-05-28 14:19:39.000000 1password-1.0.8/onepassword/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 14:19:39.000000 1password-1.0.8/onepassword/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-28 14:19:39.000000 1password-1.0.8/onepassword/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:19:48.876937 1password-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-28 14:19:39.000000 1password-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:19:48.872937 1password-1.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 14:19:39.000000 1password-1.0.8/test/test_client.py
```

### Comparing `1password-1.0.7/1password.egg-info/PKG-INFO` & `1password-1.0.8/1password.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python client and wrapper around the 1Password CLI.
 Home-page: https://github.com/wandera/1password-client
 Author: David Pryce
 Author-email: david.prycecompson@jamf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `1password-1.0.7/LICENSE.txt` & `1password-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `1password-1.0.7/PKG-INFO` & `1password-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python client and wrapper around the 1Password CLI.
 Home-page: https://github.com/wandera/1password-client
 Author: David Pryce
 Author-email: david.prycecompson@jamf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `1password-1.0.7/README.md` & `1password-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `1password-1.0.7/install_op.py` & `1password-1.0.8/install_op.py`

 * *Files identical despite different names*

### Comparing `1password-1.0.7/onepassword/client.py` & `1password-1.0.8/onepassword/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,7 +441,17 @@
             item = {
                 fields: read_bash_return(
                     "op item get {} --fields label={}".format(uuid, fields), single=False).rstrip('\n')
             }
         else:
             item = json.loads(read_bash_return("op item get {} --format=json".format(uuid), single=False))
         return item
+
+    @staticmethod
+    def get_item_otp(uuid: str | bytes):
+        """
+        Helper function to get the item otp, you can find the UUID you need using list_items
+
+        :param uuid: Uuid of the item you wish to get, no vault needed
+        :return: the otp of the item, if it exists
+        """
+        return read_bash_return("op item get {} --otp".format(uuid), single=False).rstrip('\n')
```

### Comparing `1password-1.0.7/onepassword/utils.py` & `1password-1.0.8/onepassword/utils.py`

 * *Files identical despite different names*

### Comparing `1password-1.0.7/setup.py` & `1password-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `1password-1.0.7/test/test_client.py` & `1password-1.0.8/test/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,10 +107,16 @@
 
     def test_get_items(self):
         """
         Without user interaction will not be signed in and be unable to list anything
         """
         pass
 
+    def test_get_item_otp(self):
+        """
+        Without user interaction will not be signed in and be unable to list anything
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

