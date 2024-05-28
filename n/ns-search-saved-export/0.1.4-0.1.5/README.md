# Comparing `tmp/ns_search_saved_export-0.1.4.tar.gz` & `tmp/ns_search_saved_export-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.4.tar", last modified: Sun May 26 18:25:04 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.5.tar", last modified: Tue May 28 00:44:40 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.4.tar` & `ns_search_saved_export-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:25:04.020800 ns_search_saved_export-0.1.4/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-05-26 18:25:04.018242 ns_search_saved_export-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 18:25:04.014750 ns_search_saved_export-0.1.4/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.4/Tests/__init__.py
--rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.4/Tests/test_main.py
--rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.4/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.4/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:25:03.998186 ns_search_saved_export-0.1.4/ns_search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.4/ns_search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.4/ns_search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.4/ns_search_saved_export/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:25:04.017031 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-05-26 18:25:03.000000 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-05-26 18:25:03.000000 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:25:03.000000 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-26 18:25:03.000000 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-26 18:25:03.000000 ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 18:25:04.021306 ns_search_saved_export-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-05-26 18:24:41.000000 ns_search_saved_export-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.569929 ns_search_saved_export-0.1.5/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-05-28 00:44:40.568782 ns_search_saved_export-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.565870 ns_search_saved_export-0.1.5/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.5/Tests/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.5/Tests/test_main.py
+-rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.5/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.5/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.550929 ns_search_saved_export-0.1.5/ns_search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     4812 2024-05-28 00:38:23.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.567611 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:44:40.570486 ns_search_saved_export-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-28 00:38:40.000000 ns_search_saved_export-0.1.5/setup.py
```

### Comparing `ns_search_saved_export-0.1.4/PKG-INFO` & `ns_search_saved_export-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.4/README.md` & `ns_search_saved_export-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/Tests/test_main.py` & `ns_search_saved_export-0.1.5/Tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/Tests/test_ns_search_saved_export.py` & `ns_search_saved_export-0.1.5/Tests/test_ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/Tests/test_utils.py` & `ns_search_saved_export-0.1.5/Tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/ns_search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.5/ns_search_saved_export/ns_search_saved_export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 import oauth2 as oauth
 import requests
 import pandas as pd
 from .utils import SignatureMethod_HMAC_SHA256
 
 class NsSearchSavedExport:
-    def __init__(self, url: str, consumer_key: str, consumer_secret: str, token_key: str, token_secret: str, realm: str):
+    def __init__(self, url: str, consumer_key: str, consumer_secret: str, token_key: str, token_secret: str, realm: str, search_id: str = ''):
         """Class constructor
 
         Args:
             url (str): RESTlet service URL to export saved search
             consumer_key (str): Netsuite integration client key
             consumer_secret (str): Netsuite integration client secret key
             token_key (str): NetSuite Access Key Token
             token_secret (str): NetSuite Access Secret Token
             realm (str): NetSuite domain environment ID. Example: 123456
+            searchID (str): search ID of the search saved in NetSuite
         """
         self.url = url
         self.consumer = oauth.Consumer(key=consumer_key, secret=consumer_secret)
         self.token = oauth.Token(key=token_key, secret=token_secret)
         self.realm = realm
+        self.search_id = search_id
+        self.payload = {'searchID': search_id}
 
     def _generate_oauth_params(self):
         """Returns the structured oauth parameters
 
         Returns:
             dict: Oauth params
         """
@@ -32,62 +35,66 @@
             'oauth_nonce': oauth.generate_nonce(),
             'oauth_timestamp': str(oauth.generate_timestamp()),
             'oauth_token': self.token.key,
             'oauth_consumer_key': self.consumer.key,
             'oauth_signature_method': 'HMAC-SHA256'
         }
 
-    def send_request(self, payload: dict):
+    def send_request(self):
         """POST request to obtain saved search data
 
-        Args:
-            payload (dict): Saved Search ID JSON
-
         Returns:
             dict: POST request response
         """
         params = self._generate_oauth_params()
         req = oauth.Request(method='POST', url=self.url, parameters=params)
         signature_method = SignatureMethod_HMAC_SHA256()
         req.sign_request(signature_method, self.consumer, self.token)
         header = req.to_header(self.realm)
         headers = {'Authorization': header['Authorization'].encode('ascii', 'ignore'), 'Content-Type': 'application/json'}
         
-        response = requests.post(url=self.url, headers=headers, data=json.dumps(payload))
+        response = requests.post(url=self.url, headers=headers, data=json.dumps(self.payload))
         response.raise_for_status()
         return response.json()
 
     def extract_data(self, json_data: dict):
         """Structured data obtained from the saved search
 
         Args:
             json_data (dict): Data obtained in the POST response
 
         Returns:
             list: List of saved search data
         """
+        # Export original JSON data to a JSON file
+        with open(self.search_id, 'w', encoding='utf-8') as json_file:
+            json.dump(json_data, self.search_id, ensure_ascii=False, indent=4)
+        
         matrix = []
         headers = set()
         for index, data in enumerate(json_data['results']):
             row = []
             values = data['values']
             
             if index == 0:
                 headers = list(values.keys())
-                
+                matrix.append(headers)
             
             for key in headers:
                 value = values.get(key, "")
                 if isinstance(value, list) and key == 'internalid':
                     row.append(value[0]['value'])
+                elif isinstance(value, list) and value and 'text' in value[0]:
+                    row.append(value[0]['text'])
+                elif isinstance(value, dict) and 'text' in value:
+                    row.append(value['text'])
                 else:
                     row.append(value)
             matrix.append(row)
         
-        matrix.insert(0, headers)
         return matrix
 
     @staticmethod
     def save_to_excel(matrix: list, filename: str, sheet_name: str):
         """Save data in Excel format
 
         Args:
```

### Comparing `ns_search_saved_export-0.1.4/ns_search_saved_export/utils.py` & `ns_search_saved_export-0.1.5/ns_search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/PKG-INFO` & `ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.4/ns_search_saved_export.egg-info/SOURCES.txt` & `ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.4/setup.py` & `ns_search_saved_export-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.4',
+    version='0.1.5',
     description='A library for interacting with NetSuite API and exporting data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
```

