# Comparing `tmp/morpheus-cypher-0.1.4.tar.gz` & `tmp/morpheus_cypher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morpheus-cypher-0.1.4.tar", last modified: Tue Feb 22 21:24:30 2022, max compression
+gzip compressed data, was "morpheus_cypher-0.2.0.tar", last modified: Tue May 28 14:04:53 2024, max compression
```

## Comparing `morpheus-cypher-0.1.4.tar` & `morpheus_cypher-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 21:24:30.494246 morpheus-cypher-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-22 21:24:29.000000 morpheus-cypher-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-02-22 21:24:30.494246 morpheus-cypher-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-02-22 21:24:29.000000 morpheus-cypher-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 21:24:30.494246 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-02-22 21:24:30.000000 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-02-22 21:24:30.000000 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 21:24:30.000000 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-22 21:24:30.000000 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-22 21:24:30.000000 morpheus-cypher-0.1.4/morpheus_cypher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 21:24:30.494246 morpheus-cypher-0.1.4/morpheuscypher/
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-02-22 21:24:29.000000 morpheus-cypher-0.1.4/morpheuscypher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-22 21:24:29.000000 morpheus-cypher-0.1.4/morpheuscypher/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-22 21:24:30.494246 morpheus-cypher-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-22 21:24:29.000000 morpheus-cypher-0.1.4/setup.py
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2024-05-28 14:04:52.999354 morpheus_cypher-0.2.0/
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)    11358 2021-09-28 15:00:11.000000 morpheus_cypher-0.2.0/LICENSE.txt
+-rw-r--r--   0 ncelebic  (1000) ncelebic  (1001)      300 2024-05-28 14:04:52.999354 morpheus_cypher-0.2.0/PKG-INFO
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     1724 2024-05-24 18:16:43.000000 morpheus_cypher-0.2.0/README.md
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2024-05-28 14:04:52.998354 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/
+-rw-r--r--   0 ncelebic  (1000) ncelebic  (1001)      300 2024-05-28 14:04:52.000000 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/PKG-INFO
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      306 2024-05-28 14:04:52.000000 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/SOURCES.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)        1 2024-05-28 14:04:52.000000 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/dependency_links.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       17 2024-05-28 14:04:52.000000 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/requires.txt
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       15 2024-05-28 14:04:52.000000 morpheus_cypher-0.2.0/morpheus_cypher.egg-info/top_level.txt
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2024-05-28 14:04:52.998354 morpheus_cypher-0.2.0/morpheuscypher/
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)     6688 2024-05-24 18:16:43.000000 morpheus_cypher-0.2.0/morpheuscypher/__init__.py
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       22 2024-05-28 13:51:24.000000 morpheus_cypher-0.2.0/morpheuscypher/version.py
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)       79 2024-05-28 14:04:53.004354 morpheus_cypher-0.2.0/setup.cfg
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      707 2022-02-22 21:23:31.000000 morpheus_cypher-0.2.0/setup.py
+drwxrwxr-x   0 ncelebic  (1000) ncelebic  (1001)        0 2024-05-28 14:04:52.998354 morpheus_cypher-0.2.0/test/
+-rw-rw-r--   0 ncelebic  (1000) ncelebic  (1001)      228 2022-02-22 17:39:41.000000 morpheus_cypher-0.2.0/test/testcypher.py
```

### Comparing `morpheus-cypher-0.1.4/LICENSE.txt` & `morpheus_cypher-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morpheus-cypher-0.1.4/morpheuscypher/__init__.py` & `morpheus_cypher-0.2.0/morpheuscypher/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -129,7 +129,54 @@
         if secret_path == '':
             return data['data']
         try:
             return self._get_item(data['data'], secret_path)
         except:
             raise Exception("The secret %s does not contain the path '%s'. for cypher lookup" %
                             (secret, ":".join(secret_path)))
+    def write(self, secret_key, secret_value=None, ttl=0):
+        appliance_url = self.url
+        url = appliance_url + self.cypher_endpoint + secret_key
+        headers = {'content-type': 'application/json', 'X-Cypher-Token': self.token}
+        generating_cypher_types = [
+            'uuid',
+            'key',
+            'password'
+        ]
+        cypher_mount_type = secret_key.split('/')[0].lower()
+        if cypher_mount_type in generating_cypher_types:
+            params = {
+                "ttl": ttl
+            }
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", category=Warning)
+                r = requests.post(url=url, params=params, headers=headers, verify=self.ssl_verify)
+        else:
+            params = {
+                "type": "string",
+                "ttl": ttl
+            }
+            json = {
+                "value": secret_value
+            }
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", category=Warning)
+                r = requests.post(url=url, params=params, headers=headers, json=json, verify=self.ssl_verify)
+        response = r.json()
+        if response is None:
+            raise Exception("The secret %s did not write correctly, no response data was returned" % secret_key)
+        if not response['success']:
+            raise Exception(response['msg'])
+        return response['data']
+    def delete(self, secret_key):
+        appliance_url = self.url
+        url = appliance_url + self.cypher_endpoint + secret_key
+        headers = {'content-type': 'application/json', 'X-Cypher-Token': self.token}
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=Warning)
+            r = requests.delete(url=url, headers=headers, verify=self.ssl_verify)
+        response = r.json()
+        if response is None:
+            raise Exception("The secret %s did not delete correctly, no response data was returned" % secret_key)
+        if not response['success']:
+            raise Exception(response['msg'])
+        return response['success']
```

### Comparing `morpheus-cypher-0.1.4/setup.py` & `morpheus_cypher-0.2.0/setup.py`

 * *Files identical despite different names*

