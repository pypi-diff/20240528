# Comparing `tmp/newrl-0.3.5.tar.gz` & `tmp/newrl-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrl-0.3.5.tar", last modified: Thu Mar  2 10:08:40 2023, max compression
+gzip compressed data, was "newrl-0.3.6.tar", last modified: Tue May 28 11:26:29 2024, max compression
```

## Comparing `newrl-0.3.5.tar` & `newrl-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2023-03-02 10:08:40.294248 newrl-0.3.5/
--rw-r--r--   0 kousthub   (501) staff       (20)     1081 2021-12-09 18:19:13.000000 newrl-0.3.5/LICENSE
--rw-r--r--   0 kousthub   (501) staff       (20)     5049 2023-03-02 10:08:40.294533 newrl-0.3.5/PKG-INFO
--rw-r--r--   0 kousthub   (501) staff       (20)     4189 2022-01-25 09:12:31.000000 newrl-0.3.5/README.md
--rw-r--r--   0 kousthub   (501) staff       (20)      103 2021-12-31 14:07:40.000000 newrl-0.3.5/pyproject.toml
--rw-r--r--   0 kousthub   (501) staff       (20)      616 2023-03-02 10:08:40.294997 newrl-0.3.5/setup.cfg
--rw-r--r--   0 kousthub   (501) staff       (20)     1036 2023-03-02 10:06:58.000000 newrl-0.3.5/setup.py
-drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2023-03-02 10:08:40.289539 newrl-0.3.5/src/
-drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2023-03-02 10:08:40.292779 newrl-0.3.5/src/newrl/
--rw-r--r--   0 kousthub   (501) staff       (20)      214 2022-09-23 10:24:55.000000 newrl-0.3.5/src/newrl/__init__.py
--rw-r--r--   0 kousthub   (501) staff       (20)      560 2022-01-20 14:48:55.000000 newrl-0.3.5/src/newrl/hash.py
--rw-r--r--   0 kousthub   (501) staff       (20)     7949 2023-03-02 10:07:50.000000 newrl-0.3.5/src/newrl/node.py
--rw-r--r--   0 kousthub   (501) staff       (20)     2369 2023-01-19 11:31:25.000000 newrl-0.3.5/src/newrl/signer.py
--rw-r--r--   0 kousthub   (501) staff       (20)     5292 2022-09-23 10:24:55.000000 newrl-0.3.5/src/newrl/transaction.py
--rw-r--r--   0 kousthub   (501) staff       (20)     2047 2022-09-23 10:24:55.000000 newrl-0.3.5/src/newrl/wallet.py
-drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2023-03-02 10:08:40.294062 newrl-0.3.5/src/newrl.egg-info/
--rw-r--r--   0 kousthub   (501) staff       (20)     5049 2023-03-02 10:08:40.000000 newrl-0.3.5/src/newrl.egg-info/PKG-INFO
--rw-r--r--   0 kousthub   (501) staff       (20)      338 2023-03-02 10:08:40.000000 newrl-0.3.5/src/newrl.egg-info/SOURCES.txt
--rw-r--r--   0 kousthub   (501) staff       (20)        1 2023-03-02 10:08:40.000000 newrl-0.3.5/src/newrl.egg-info/dependency_links.txt
--rw-r--r--   0 kousthub   (501) staff       (20)       28 2023-03-02 10:08:40.000000 newrl-0.3.5/src/newrl.egg-info/requires.txt
--rw-r--r--   0 kousthub   (501) staff       (20)        6 2023-03-02 10:08:40.000000 newrl-0.3.5/src/newrl.egg-info/top_level.txt
+drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2024-05-28 11:26:29.321111 newrl-0.3.6/
+-rw-r--r--   0 kousthub   (501) staff       (20)     1081 2021-12-09 18:19:13.000000 newrl-0.3.6/LICENSE
+-rw-r--r--   0 kousthub   (501) staff       (20)     5049 2024-05-28 11:26:29.321199 newrl-0.3.6/PKG-INFO
+-rw-r--r--   0 kousthub   (501) staff       (20)     4189 2022-01-25 09:12:31.000000 newrl-0.3.6/README.md
+-rw-r--r--   0 kousthub   (501) staff       (20)      103 2021-12-31 14:07:40.000000 newrl-0.3.6/pyproject.toml
+-rw-r--r--   0 kousthub   (501) staff       (20)      616 2024-05-28 11:26:29.321456 newrl-0.3.6/setup.cfg
+-rw-r--r--   0 kousthub   (501) staff       (20)     1036 2024-05-28 11:26:20.000000 newrl-0.3.6/setup.py
+drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2024-05-28 11:26:29.318224 newrl-0.3.6/src/
+drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2024-05-28 11:26:29.320280 newrl-0.3.6/src/newrl/
+-rw-r--r--   0 kousthub   (501) staff       (20)      214 2022-09-23 10:24:55.000000 newrl-0.3.6/src/newrl/__init__.py
+-rw-r--r--   0 kousthub   (501) staff       (20)      560 2022-01-20 14:48:55.000000 newrl-0.3.6/src/newrl/hash.py
+-rw-r--r--   0 kousthub   (501) staff       (20)     8995 2024-05-28 11:09:34.000000 newrl-0.3.6/src/newrl/node.py
+-rw-r--r--   0 kousthub   (501) staff       (20)     2418 2024-05-28 09:04:36.000000 newrl-0.3.6/src/newrl/signer.py
+-rw-r--r--   0 kousthub   (501) staff       (20)     5329 2024-05-28 09:04:36.000000 newrl-0.3.6/src/newrl/transaction.py
+-rw-r--r--   0 kousthub   (501) staff       (20)     2047 2022-09-23 10:24:55.000000 newrl-0.3.6/src/newrl/wallet.py
+drwxr-xr-x   0 kousthub   (501) staff       (20)        0 2024-05-28 11:26:29.321009 newrl-0.3.6/src/newrl.egg-info/
+-rw-r--r--   0 kousthub   (501) staff       (20)     5049 2024-05-28 11:26:29.000000 newrl-0.3.6/src/newrl.egg-info/PKG-INFO
+-rw-r--r--   0 kousthub   (501) staff       (20)      338 2024-05-28 11:26:29.000000 newrl-0.3.6/src/newrl.egg-info/SOURCES.txt
+-rw-r--r--   0 kousthub   (501) staff       (20)        1 2024-05-28 11:26:29.000000 newrl-0.3.6/src/newrl.egg-info/dependency_links.txt
+-rw-r--r--   0 kousthub   (501) staff       (20)       28 2024-05-28 11:26:29.000000 newrl-0.3.6/src/newrl.egg-info/requires.txt
+-rw-r--r--   0 kousthub   (501) staff       (20)        6 2024-05-28 11:26:29.000000 newrl-0.3.6/src/newrl.egg-info/top_level.txt
```

### Comparing `newrl-0.3.5/LICENSE` & `newrl-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `newrl-0.3.5/PKG-INFO` & `newrl-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python SDK for Newrl blockchain
 Home-page: https://github.com/asqi/newrl
 Download-URL: https://github.com/asqisys/newrl-py/archive/refs/tags/v_02.tar.gz
 Author: Kousthub Raja
 Author-email: kousthub@asqi.in
 License: MIT
 Project-URL: Bug Tracker, https://github.com/asqisys/newrl-py/issues
```

### Comparing `newrl-0.3.5/README.md` & `newrl-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `newrl-0.3.5/setup.cfg` & `newrl-0.3.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = newrl
-version = 0.3.5
+version = 0.3.6
 author = Kousthub Raja
 author_email = kousthub@asqi.in
 description = Python SDK for Newrl blockchain
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asqisys/newrl-py
 project_urls =
```

### Comparing `newrl-0.3.5/setup.py` & `newrl-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'newrl',
   packages = ['newrl'],
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'Python SDK for Newrl blockchain',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Kousthub Raja',
   author_email = 'kousthub@asqi.in',
   url = 'https://github.com/asqi/newrl',
```

### Comparing `newrl-0.3.5/src/newrl/hash.py` & `newrl-0.3.6/src/newrl/hash.py`

 * *Files identical despite different names*

### Comparing `newrl-0.3.5/src/newrl/signer.py` & `newrl-0.3.6/src/newrl/signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     sk = ecdsa.SigningKey.from_string(private_key_bytes, curve=ecdsa.SECP256k1)
     msgsignbytes = sk.sign(msg)
     msgsign = msgsignbytes.hex()
     signatures = transaction_data['signatures'] if 'signatures' in transaction_data else [
     ]
     signatures.append({'wallet_address': address, 'msgsign': msgsign})
 
+    transaction_data['signatures'] = signatures
+
     return transaction_data
 
 
 def addresschecker(transaction, address):
     #	trans=trandata['transaction']
     #	signatures = trandata['signatures']
     validadds = getvalidadds(transaction)
```

### Comparing `newrl-0.3.5/src/newrl/transaction.py` & `newrl-0.3.6/src/newrl/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 def add_smart_contract_transaction(
     sc_address: str,
     sc_name: str,
     version: str,
     creator: str,
     signatories: dict,
     contractspecs: dict,
+    sc_function : str = 'setup',
     actmode: str = "hybrid",
     legalparams: dict = {},
 ) -> dict:
     smart_contract_data = {
         "creator": creator,
         "name": sc_name,
         "version": version,
@@ -157,15 +158,15 @@
         "parent": None,
         "oracleids": None,
         "selfdestruct": 1,
     }
 
     transaction_data = {
         "address": sc_address,
-        "function": "setup",
+        "function": sc_function,
         "signers": [creator],
         "params": smart_contract_data
     }
 
     transaction = {
         'timestamp': int(time.time() * 1000),
         'type': 3,
```

### Comparing `newrl-0.3.5/src/newrl/wallet.py` & `newrl-0.3.6/src/newrl/wallet.py`

 * *Files identical despite different names*

### Comparing `newrl-0.3.5/src/newrl.egg-info/PKG-INFO` & `newrl-0.3.6/src/newrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python SDK for Newrl blockchain
 Home-page: https://github.com/asqi/newrl
 Download-URL: https://github.com/asqisys/newrl-py/archive/refs/tags/v_02.tar.gz
 Author: Kousthub Raja
 Author-email: kousthub@asqi.in
 License: MIT
 Project-URL: Bug Tracker, https://github.com/asqisys/newrl-py/issues
```

