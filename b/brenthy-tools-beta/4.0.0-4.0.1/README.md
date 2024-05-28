# Comparing `tmp/brenthy_tools_beta-4.0.0.tar.gz` & `tmp/brenthy_tools_beta-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brenthy_tools_beta-4.0.0.tar", last modified: Sat May 25 07:47:38 2024, max compression
+gzip compressed data, was "brenthy_tools_beta-4.0.1.tar", last modified: Tue May 28 15:42:00 2024, max compression
```

## Comparing `brenthy_tools_beta-4.0.0.tar` & `brenthy_tools_beta-4.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:47:38.544344 brenthy_tools_beta-4.0.0/
--rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1441 2024-05-25 07:47:38.544344 brenthy_tools_beta-4.0.0/PKG-INFO
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:47:38.540344 brenthy_tools_beta-4.0.0/brenthy_tools_beta/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      429 2024-05-07 17:25:51.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/__init__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       90 2024-05-05 11:49:49.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/__main__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1674 2024-05-11 17:23:08.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/__project__.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    13203 2024-05-22 06:43:02.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      297 2024-05-07 05:24:16.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_addresses.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:47:38.544344 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       90 2024-05-05 11:27:29.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/__main__.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1305 2024-05-07 05:23:55.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/bap_3_brenthy_tools.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6245 2024-05-11 17:36:23.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/bap_4_brenthy_tools.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6271 2024-05-22 06:43:10.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/bt_endpoints.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6940 2024-05-11 17:26:00.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/log.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     7872 2024-05-11 17:29:05.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/utils.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     2871 2024-05-11 17:26:35.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/version_utils.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      981 2024-05-22 07:57:16.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta/versions.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-25 07:47:38.544344 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/
--rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1441 2024-05-25 07:47:38.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      728 2024-05-25 07:47:38.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2024-05-25 07:47:38.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       16 2024-05-25 07:47:38.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/requires.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       60 2024-05-25 07:47:38.000000 brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2024-05-25 07:47:38.544344 brenthy_tools_beta-4.0.0/setup.cfg
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1030 2024-05-25 07:47:24.000000 brenthy_tools_beta-4.0.0/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1570 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/PKG-INFO
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/brenthy_tools_beta/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      429 2024-05-07 17:25:51.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/__init__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       90 2024-05-05 11:49:49.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/__main__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1700 2024-05-28 06:44:20.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/__project__.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    13233 2024-05-28 13:09:36.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      297 2024-05-07 05:24:16.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_addresses.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       90 2024-05-05 11:27:29.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/__main__.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1305 2024-05-07 05:23:55.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/bap_3_brenthy_tools.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6245 2024-05-11 17:36:23.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/bap_4_brenthy_tools.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6271 2024-05-22 06:43:10.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/bt_endpoints.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6940 2024-05-11 17:26:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/log.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     7872 2024-05-11 17:29:05.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/utils.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     2871 2024-05-11 17:26:35.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/version_utils.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      981 2024-05-28 14:01:30.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta/versions.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/
+-rw-r--r--   0 llearuin  (1000) llearuin  (1000)     1570 2024-05-28 15:42:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      728 2024-05-28 15:42:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2024-05-28 15:42:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       16 2024-05-28 15:42:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/requires.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       60 2024-05-28 15:42:00.000000 brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2024-05-28 15:42:00.122650 brenthy_tools_beta-4.0.1/setup.cfg
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)      985 2024-05-25 07:59:05.000000 brenthy_tools_beta-4.0.1/setup.py
```

### Comparing `brenthy_tools_beta-4.0.0/PKG-INFO` & `brenthy_tools_beta-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: brenthy_tools_beta
-Version: 4.0.0
+Version: 4.0.1
 Summary: A library for interacting with Brenthy (`brenthy_api`) and a collection of tools common to Brenthy Core and `brenthy_api`.
-Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis_Beta/Documentation/Brenthy/Meaning/Introduction.md.html
+Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
 Author: emendir
+Project-URL: IPNS, https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
+Project-URL: Github, https://github.com/emendir/BrenthyAndWalytis
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq
 Requires-Dist: termcolor
 
 # Brenthy
 Here lives the source code for Brenthy, the framework for developing and deploying new kinds of blockchain in the Python programming language.
 
 ## Learn about Brenthy:
 
 Main docs:
-- [Introduction to Brenthy](Documentation/Brenthy/Meaning/IntroductionToBrenthy.md)
+- [Introduction to Brenthy](/Documentation/Brenthy/Meaning/IntroductionToBrenthy.md)
 - [Running from Source](/Documentation/Brenthy/User/RunningFromSource.md)
 - [Installation](/Documentation/Brenthy/User/InstallingBrenthy.md)
 - Create Blockchains for Brenthy: _coming soon..._
 
 Overview of all docs: [/Documentation/DocsOverview.md](/Documentation/DocsOverview.md)
 
 
 ## Walytis
 Walytis is the novel blockchain Brenthy was originally built for.
-Read the [Introduction to Walytis](/Documentation/Brenthy/Walytis_Beta/IntroductionToWalytis.md) to learn more.
+Read the [Introduction to Walytis](/Documentation/Walytis/Meaning/IntroductionToWalytis.md) to learn more.
 The source code for Walytis is located under [./blockchains/Walytis_Beta](./blockchains/Walytis_Beta/ReadMe.md)
```

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/__project__.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/__project__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 if os.path.exists("ReadMe.md"):
     with open("ReadMe.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 long_description_content_type = "text/markdown"
 url = (
     "https://ipfs.io/ipns/"
     "k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup"
-    "/Sites/BrenthyAndWalytis_Beta/"
-    "Documentation/Brenthy/Meaning/Introduction.md.html"
+    "/Sites/BrenthyAndWalytis/"
+    # "Documentation/Brenthy/Meaning/Introduction.md.html"
 )
 project_urls = {
-    "Source Code on IPNS": url,
-    "Github": "",
+    "IPNS": url,
+    "Github": "https://github.com/emendir/BrenthyAndWalytis",
 }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 python_requires = ">=3.6"
```

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,53 +78,55 @@
     if not isinstance(payload, bytearray):
         error_message = (
             "payload must be of type bytearray, not " f"{type(payload)}"
         )
         log.error(f"BrenthyAPI: {function_name()}: {error_message}")
         raise TypeError(error_message)
 
+    # encapsulate the request together with the blockchain type
+    # and brenthy_tools version
     request = blockchain_type.encode() + bytearray([0]) + payload
-
     request = encode_version(BRENTHY_TOOLS_VERSION) + bytearray([0]) + request
 
-    # try sending request via different protocols
     reply: bytearray = bytearray()
     # whether or not we've managed to establish communication with Brenthy-Core
     communicated = False
+    # try sending request via different protocols
     for protocol in bap_protocol_modules:
         try:
             reply = protocol.send_request(request)
-        except (CantConnectToSocketError, BrenthyReplyDecodeError):
+        except CantConnectToSocketError:
             # try next BrenthyAPI protocol
             continue
         communicated = True
-        # if we can't read the reply
+
+        # decapsulate the reply
         try:
-            brenthy_core_version = decode_version(  # pylint: disable=unused-variable
+            brenthy_core_version = decode_version(
                 reply[: reply.index(bytearray([0]))]
             )
             reply = reply[reply.index(bytearray([0])) + 1:]
+            if not reply:
+                continue
+            # Request was processed successfully by Brenthy.
+            success = reply[0] == 1
+            reply = reply[1:]
+
+            break  # request sent, got reply,so move on
         except:
             continue
-        if not reply:
-            continue
-        # log.debug(f"Used BAP-{protocol.BAP_VERSION}")
-        break  # request sent, got reply,so move on
     if not reply:
         if communicated:
             raise BrenthyReplyDecodeError()
         else:
             raise BrenthyNotRunningError()
-    # Request was processed successfully by Brenthy.
-
-    success = reply[0] == 1
-    reply = reply[1:]
     if success:
         return reply
-    # Brenthy failed to process our request.
+
+    # Brenthy/blockchain failed to process our request.
     raise _analyse_no_success_reply(reply)
 
 
 def _analyse_no_success_reply(reply: bytearray) -> Exception:
     """Get the appropriate Exception for the given reply from Brenthy.
 
     Assumes the reply is from a request which Brenthy (not its blockchains)
@@ -318,15 +320,15 @@
 class BrenthyReplyDecodeError(Exception):
     """When Brenthy's reply can't be decoded."""
 
     def_message = (
         "error parsing the reply from Brenthy. " "This is probably a bug."
     )
 
-    def __init__(self, message: str = def_message, reply: bytearray = ""):
+    def __init__(self, message: str = def_message, reply: bytearray | None = None):
         """Raise a BrenthyReplyDecodeError exception.
 
         Args:
             message (str): the error message to store in this Exception
             reply (str): the reply received from Brenthy
         """
         self.message = message
```

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/bap_3_brenthy_tools.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/bap_3_brenthy_tools.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/brenthy_api_protocols/bap_4_brenthy_tools.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/brenthy_api_protocols/bap_4_brenthy_tools.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/bt_endpoints.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/bt_endpoints.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/log.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/log.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/utils.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/utils.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/version_utils.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/version_utils.py`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta/versions.py` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta/versions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # the brenthy_tools_beta library to communicate with each other
 BRENTHY_API_PROTOCOL_VERSION = 4
 
 # the version of the core Brenthy software which runs blockchains
 BRENTHY_CORE_VERSION = (
     BRENTHY_API_PROTOCOL_VERSION,  # major: the BrenthyAPI Protocol version
     1,  # minor: significant changes to Brenthy since the last major update
-    1,  # patch: minor changes to Brenthy since the last minor update
+    2,  # patch: minor changes to Brenthy since the last minor update
 )
 
 
 # the version of the brenthy_api library which is used by applications
 # to communicate with Brenthy Core to interact with blockchains
 BRENTHY_TOOLS_VERSION = (
     BRENTHY_API_PROTOCOL_VERSION,  # major: the BrenthyAPI Protocol version
     0,  # minor: changes to brenthy_api but not BAP since the last major update
-    0,  # patch: changes outside brenthy_api since the last minor update
+    1,  # patch: changes outside brenthy_api since the last minor update
 )
```

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/PKG-INFO` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: brenthy_tools_beta
-Version: 4.0.0
+Version: 4.0.1
 Summary: A library for interacting with Brenthy (`brenthy_api`) and a collection of tools common to Brenthy Core and `brenthy_api`.
-Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis_Beta/Documentation/Brenthy/Meaning/Introduction.md.html
+Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
 Author: emendir
+Project-URL: IPNS, https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup/Sites/BrenthyAndWalytis/
+Project-URL: Github, https://github.com/emendir/BrenthyAndWalytis
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq
 Requires-Dist: termcolor
 
 # Brenthy
 Here lives the source code for Brenthy, the framework for developing and deploying new kinds of blockchain in the Python programming language.
 
 ## Learn about Brenthy:
 
 Main docs:
-- [Introduction to Brenthy](Documentation/Brenthy/Meaning/IntroductionToBrenthy.md)
+- [Introduction to Brenthy](/Documentation/Brenthy/Meaning/IntroductionToBrenthy.md)
 - [Running from Source](/Documentation/Brenthy/User/RunningFromSource.md)
 - [Installation](/Documentation/Brenthy/User/InstallingBrenthy.md)
 - Create Blockchains for Brenthy: _coming soon..._
 
 Overview of all docs: [/Documentation/DocsOverview.md](/Documentation/DocsOverview.md)
 
 
 ## Walytis
 Walytis is the novel blockchain Brenthy was originally built for.
-Read the [Introduction to Walytis](/Documentation/Brenthy/Walytis_Beta/IntroductionToWalytis.md) to learn more.
+Read the [Introduction to Walytis](/Documentation/Walytis/Meaning/IntroductionToWalytis.md) to learn more.
 The source code for Walytis is located under [./blockchains/Walytis_Beta](./blockchains/Walytis_Beta/ReadMe.md)
```

### Comparing `brenthy_tools_beta-4.0.0/brenthy_tools_beta.egg-info/SOURCES.txt` & `brenthy_tools_beta-4.0.1/brenthy_tools_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brenthy_tools_beta-4.0.0/setup.py` & `brenthy_tools_beta-4.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,24 @@
         long_description_content_type,
         project_name,
         project_urls,
         python_requires,
         url,
         version,
     )
+
 setuptools.setup(
     name=project_name,
     version=version,
     author=author,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     url=url,
-    # homepage=url,
-    # download_url=url,
-    # project_urls=project_urls,
+    project_urls=project_urls,
     classifiers=classifiers,
     packages=[
         "brenthy_tools_beta",
         "brenthy_tools_beta/brenthy_api_protocols",
     ],
     python_requires=python_requires,
     install_requires=install_requires,
```

