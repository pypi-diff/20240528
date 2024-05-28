# Comparing `tmp/walytis_beta_api-2.3.4.tar.gz` & `tmp/walytis_beta_api-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walytis_beta_api-2.3.4.tar", last modified: Sat May 25 07:52:14 2024, max compression
+gzip compressed data, was "walytis_beta_api-2.3.5.tar", last modified: Tue May 28 15:42:15 2024, max compression
```

## Comparing `walytis_beta_api-2.3.4.tar` & `walytis_beta_api-2.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:52:14.745763 walytis_beta_api-2.3.4/
--rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1431 2024-05-25 07:52:14.741763 walytis_beta_api-2.3.4/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2024-05-25 07:52:14.745763 walytis_beta_api-2.3.4/setup.cfg
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1051 2024-05-11 16:57:22.000000 walytis_beta_api-2.3.4/setup.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:52:14.741763 walytis_beta_api-2.3.4/walytis_beta_api/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1546 2024-05-22 06:50:12.000000 walytis_beta_api-2.3.4/walytis_beta_api/__init__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      193 2024-05-07 17:40:56.000000 walytis_beta_api-2.3.4/walytis_beta_api/__main__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1710 2024-05-25 07:51:33.000000 walytis_beta_api-2.3.4/walytis_beta_api/__project__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19287 2024-05-22 06:19:06.000000 walytis_beta_api-2.3.4/walytis_beta_api/block_model.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    22057 2024-05-25 07:00:08.000000 walytis_beta_api-2.3.4/walytis_beta_api/blockchain_model.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5511 2024-05-22 06:50:44.000000 walytis_beta_api-2.3.4/walytis_beta_api/exceptions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      793 2024-05-22 07:57:44.000000 walytis_beta_api-2.3.4/walytis_beta_api/versions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    35106 2024-05-22 06:50:12.000000 walytis_beta_api-2.3.4/walytis_beta_api/walytis_beta_interface.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:52:14.741763 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/
--rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1431 2024-05-25 07:52:14.000000 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      469 2024-05-25 07:52:14.000000 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/SOURCES.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2024-05-25 07:52:14.000000 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/dependency_links.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       69 2024-05-25 07:52:14.000000 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/requires.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       17 2024-05-25 07:52:14.000000 walytis_beta_api-2.3.4/walytis_beta_api.egg-info/top_level.txt
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:15.282797 walytis_beta_api-2.3.5/
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1540 2024-05-28 15:42:15.282797 walytis_beta_api-2.3.5/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2024-05-28 15:42:15.282797 walytis_beta_api-2.3.5/setup.cfg
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1051 2024-05-25 07:58:41.000000 walytis_beta_api-2.3.5/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:15.282797 walytis_beta_api-2.3.5/walytis_beta_api/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1546 2024-05-22 06:50:12.000000 walytis_beta_api-2.3.5/walytis_beta_api/__init__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      193 2024-05-07 17:40:56.000000 walytis_beta_api-2.3.5/walytis_beta_api/__main__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1519 2024-05-28 06:44:06.000000 walytis_beta_api-2.3.5/walytis_beta_api/__project__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19287 2024-05-22 06:19:06.000000 walytis_beta_api-2.3.5/walytis_beta_api/block_model.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    22057 2024-05-25 07:00:08.000000 walytis_beta_api-2.3.5/walytis_beta_api/blockchain_model.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5511 2024-05-22 06:50:44.000000 walytis_beta_api-2.3.5/walytis_beta_api/exceptions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      793 2024-05-28 14:01:03.000000 walytis_beta_api-2.3.5/walytis_beta_api/versions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    35211 2024-05-28 10:52:16.000000 walytis_beta_api-2.3.5/walytis_beta_api/walytis_beta_interface.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:15.282797 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1540 2024-05-28 15:42:15.000000 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      469 2024-05-28 15:42:15.000000 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2024-05-28 15:42:15.000000 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       69 2024-05-28 15:42:15.000000 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/requires.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       17 2024-05-28 15:42:15.000000 walytis_beta_api-2.3.5/walytis_beta_api.egg-info/top_level.txt
```

### Comparing `walytis_beta_api-2.3.4/PKG-INFO` & `walytis_beta_api-2.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: walytis_beta_api
-Version: 2.3.4
+Version: 2.3.5
 Summary: A library for interacting with Walytis_Beta: a lightweight, flexible, non-linear blockchain.
-Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis_Beta/Documentation/Walytis/Meaning/Introduction.md.html
+Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
 Author: emendir
-Project-URL: Github, https://github.com/emendir/Brenthy
+Project-URL: IPNS, https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
+Project-URL: Github, https://github.com/emendir/BrenthyAndWalytis
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: appdirs==1.4.3
 Requires-Dist: ipfs-toolkit>=0.5.19
 Requires-Dist: pyzmq==25.1.1
 Requires-Dist: brenthy_tools_beta
 
 # Walytis
 Here lives the source code for Walytis, a flexible, lightweight non-linear blockchain.
 
-This project is built to be run by [Brenthy](Documentation/Brenthy/Meaning/IntroductionToBrenthy.md), a framework for developing and deploying new kinds of blockchains.
+This project is built to be run by [Brenthy](/Documentation/Brenthy/Meaning/IntroductionToBrenthy.md), a framework for developing and deploying new kinds of blockchains.
 They both depend on each other, so they share the same repository. 
 
 ## Learn About Walytis
 
 Most significant docs:
 - [Introduction to Walytis](/Documentation/Walytis/Meaning/IntroductionToWalytis.md)
-- [Understanding Nonlinear Blockchain](UnderstandingNonlinearBlockchain.md)
+- [Understanding Nonlinear Blockchain](/Documentation/Walytis/Meaning/UnderstandingNonlinearBlockchain.md)
 - [Walytis Blockchain-Architecture Security](/Documentation/Walytis/Technical/WalytisBlockchainSecurity.md)
 
 Overview of all docs: [/Documentation/DocsOverview.md](/Documentation/DocsOverview.md)
```

### Comparing `walytis_beta_api-2.3.4/setup.py` & `walytis_beta_api-2.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/__init__.py` & `walytis_beta_api-2.3.5/walytis_beta_api/__init__.py`

 * *Files identical despite different names*

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/__project__.py` & `walytis_beta_api-2.3.5/walytis_beta_api/__project__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,24 +21,21 @@
 long_description = ""
 if os.path.exists("ReadMe.md"):
     with open("ReadMe.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 long_description_content_type = "text/markdown"
 url = (
     "https://ipfs.io/ipns/"
-    "k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/"
-    "BrenthyAndWalytis_Beta/Documentation/Walytis/Meaning/Introduction.md.html"
+    "k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup"
+    "/Sites/BrenthyAndWalytis/"
+    # "Documentation/Walytis/Meaning/Introduction.md.html"
 )
 project_urls = {
-    # "Source Code on IPNS": (
-    #     "ipns://k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites"
-    #     "/BrenthyAndWalytis_Beta/Documentation/"
-    #     "Walytis/Meaning/Introduction.md.html"
-    # ),
-    "Github": "https://github.com/emendir/Brenthy",
+    "IPNS": url,
+    "Github": "https://github.com/emendir/BrenthyAndWalytis",
 }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 python_requires = ">=3.6"
```

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/block_model.py` & `walytis_beta_api-2.3.5/walytis_beta_api/block_model.py`

 * *Files identical despite different names*

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/blockchain_model.py` & `walytis_beta_api-2.3.5/walytis_beta_api/blockchain_model.py`

 * *Files identical despite different names*

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/exceptions.py` & `walytis_beta_api-2.3.5/walytis_beta_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/versions.py` & `walytis_beta_api-2.3.5/walytis_beta_api/versions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 
 # the newest version of the communication protocol used by the Walytis node
 # and the walytis_beta_api library to communicate with each other
 WALYTIS_BETA_API_PROTOCOL_VERSION = (WALYTIS_BETA_PROTOCOL_VERSION, 3)
 
 # the version of the walytis_api library which is used by applications
 # to communicate with the Walytis_Beta node to interact with blockchains
-WALYTIS_BETA_API_VERSION = (*WALYTIS_BETA_API_PROTOCOL_VERSION, 4)
+WALYTIS_BETA_API_VERSION = (*WALYTIS_BETA_API_PROTOCOL_VERSION, 5)
 
 # the version of the Walytis node software, which runs blockchains
-WALYTIS_BETA_CORE_VERSION = (*WALYTIS_BETA_API_PROTOCOL_VERSION, 3)
+WALYTIS_BETA_CORE_VERSION = (*WALYTIS_BETA_API_PROTOCOL_VERSION, 4)
```

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api/walytis_beta_interface.py` & `walytis_beta_api-2.3.5/walytis_beta_api/walytis_beta_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,14 +803,17 @@
 
         self.event_listener = brenthy_api.EventListener(
             "Walytis_Beta", self._eventhandler, f"{blockchain_id}-NewBlocks"
         )
 
     def _eventhandler(self, data: dict, topic: str) -> None:
         """Handle new block messages, calling the user's eventhandler."""
+        # decapsulate topic for documentation purposes
+        blockchain_topic = topic.strip(f"{self.blockchain_id}-")
+
         block_id = string_to_bytes(data["block_id"])
         block = get_block(self.blockchain_id, block_id)
         log.info(
             "Walytis_BetaAPI: BlocksListener: got block: "
             f"{(self.topics, block.topics)}"
         )
         try:
@@ -997,17 +1000,15 @@
                                 needs to process our request, its arguments
 
     Returns:
         bytearray: the reply from the function we called in
                                 walytis_beta_api_terminal
     """
     request = (
-        encode_version(WALYTIS_BETA_API_PROTOCOL_VERSION)
-        + bytearray([0])
-        + function_name.encode()
-        + bytearray([0])
+        encode_version(WALYTIS_BETA_API_PROTOCOL_VERSION) + bytearray([0])
+        + function_name.encode() + bytearray([0])
         + payload
     )
     reply = brenthy_api.send_request("Walytis_Beta", request)
     walytis_api_version = decode_version(reply[: reply.index(bytearray([0]))])
     reply = reply[reply.index(bytearray([0])) + 1:]
     return reply
```

### Comparing `walytis_beta_api-2.3.4/walytis_beta_api.egg-info/PKG-INFO` & `walytis_beta_api-2.3.5/walytis_beta_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: walytis_beta_api
-Version: 2.3.4
+Version: 2.3.5
 Summary: A library for interacting with Walytis_Beta: a lightweight, flexible, non-linear blockchain.
-Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis_Beta/Documentation/Walytis/Meaning/Introduction.md.html
+Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
 Author: emendir
-Project-URL: Github, https://github.com/emendir/Brenthy
+Project-URL: IPNS, https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
+Project-URL: Github, https://github.com/emendir/BrenthyAndWalytis
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: appdirs==1.4.3
 Requires-Dist: ipfs-toolkit>=0.5.19
 Requires-Dist: pyzmq==25.1.1
 Requires-Dist: brenthy_tools_beta
 
 # Walytis
 Here lives the source code for Walytis, a flexible, lightweight non-linear blockchain.
 
-This project is built to be run by [Brenthy](Documentation/Brenthy/Meaning/IntroductionToBrenthy.md), a framework for developing and deploying new kinds of blockchains.
+This project is built to be run by [Brenthy](/Documentation/Brenthy/Meaning/IntroductionToBrenthy.md), a framework for developing and deploying new kinds of blockchains.
 They both depend on each other, so they share the same repository. 
 
 ## Learn About Walytis
 
 Most significant docs:
 - [Introduction to Walytis](/Documentation/Walytis/Meaning/IntroductionToWalytis.md)
-- [Understanding Nonlinear Blockchain](UnderstandingNonlinearBlockchain.md)
+- [Understanding Nonlinear Blockchain](/Documentation/Walytis/Meaning/UnderstandingNonlinearBlockchain.md)
 - [Walytis Blockchain-Architecture Security](/Documentation/Walytis/Technical/WalytisBlockchainSecurity.md)
 
 Overview of all docs: [/Documentation/DocsOverview.md](/Documentation/DocsOverview.md)
```

