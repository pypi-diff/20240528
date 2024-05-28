# Comparing `tmp/okx-sdk-1.3.5.tar.gz` & `tmp/okx-sdk-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okx-sdk-1.3.5.tar", last modified: Tue Apr 30 13:43:35 2024, max compression
+gzip compressed data, was "okx-sdk-1.3.6.tar", last modified: Tue May 28 12:51:09 2024, max compression
```

## Comparing `okx-sdk-1.3.5.tar` & `okx-sdk-1.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.570621 okx-sdk-1.3.5/
--rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.5/LICENSE
--rw-rw-rw-   0        0        0    33887 2024-04-30 13:43:35.568112 okx-sdk-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    32434 2024-04-14 07:04:21.000000 okx-sdk-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.276616 okx-sdk-1.3.5/okx/
--rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.5/okx/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.5/okx/clients.py
--rw-rw-rw-   0        0        0    21787 2024-04-14 07:02:59.000000 okx-sdk-1.3.5/okx/constants.py
--rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.5/okx/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.472712 okx-sdk-1.3.5/okx/restapi/
--rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.5/okx/restapi/Account.py
--rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.5/okx/restapi/AlgoTrading.py
--rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.5/okx/restapi/BaseClient.py
--rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.5/okx/restapi/BlockTrading.py
--rw-rw-rw-   0        0        0     8252 2024-04-14 07:02:40.000000 okx-sdk-1.3.5/okx/restapi/Broker.py
--rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.5/okx/restapi/CopyTrading.py
--rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.5/okx/restapi/Finance.py
--rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.5/okx/restapi/Funding.py
--rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.5/okx/restapi/GridTrading.py
--rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.5/okx/restapi/PublicData.py
--rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.5/okx/restapi/RecurringBuy.py
--rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.5/okx/restapi/Rubik.py
--rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.5/okx/restapi/SignalTrading.py
--rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.5/okx/restapi/SpreadTrading.py
--rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.5/okx/restapi/SubAccount.py
--rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.5/okx/restapi/Trading.py
--rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.5/okx/restapi/__init__.py
--rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.5/okx/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.528851 okx-sdk-1.3.5/okx/wsapi/
--rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.5/okx/wsapi/Factory.py
--rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.5/okx/wsapi/PrivateAsync.py
--rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.5/okx/wsapi/PublicAsync.py
--rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.5/okx/wsapi/__init__.py
--rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.5/okx/wsapi/wsutils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.566111 okx-sdk-1.3.5/okx_sdk.egg-info/
--rw-rw-rw-   0        0        0    33887 2024-04-30 13:43:35.000000 okx-sdk-1.3.5/okx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-04-30 13:43:35.000000 okx-sdk-1.3.5/okx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:43:35.000000 okx-sdk-1.3.5/okx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-30 13:43:35.000000 okx-sdk-1.3.5/okx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 13:43:35.000000 okx-sdk-1.3.5/okx_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 13:43:35.571637 okx-sdk-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1198 2024-04-30 13:43:16.000000 okx-sdk-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:43:35.564108 okx-sdk-1.3.5/tests/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.933378 okx-sdk-1.3.6/
+-rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0    33887 2024-05-28 12:51:09.931349 okx-sdk-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    32434 2024-04-14 07:04:21.000000 okx-sdk-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.713621 okx-sdk-1.3.6/okx/
+-rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.6/okx/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.6/okx/clients.py
+-rw-rw-rw-   0        0        0    21787 2024-04-14 07:02:59.000000 okx-sdk-1.3.6/okx/constants.py
+-rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.6/okx/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.863642 okx-sdk-1.3.6/okx/restapi/
+-rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.6/okx/restapi/Account.py
+-rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.6/okx/restapi/AlgoTrading.py
+-rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.6/okx/restapi/BaseClient.py
+-rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.6/okx/restapi/BlockTrading.py
+-rw-rw-rw-   0        0        0     8252 2024-04-14 07:02:40.000000 okx-sdk-1.3.6/okx/restapi/Broker.py
+-rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.6/okx/restapi/CopyTrading.py
+-rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.6/okx/restapi/Finance.py
+-rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.6/okx/restapi/Funding.py
+-rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.6/okx/restapi/GridTrading.py
+-rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.6/okx/restapi/PublicData.py
+-rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.6/okx/restapi/RecurringBuy.py
+-rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.6/okx/restapi/Rubik.py
+-rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.6/okx/restapi/SignalTrading.py
+-rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.6/okx/restapi/SpreadTrading.py
+-rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.6/okx/restapi/SubAccount.py
+-rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.6/okx/restapi/Trading.py
+-rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.6/okx/restapi/__init__.py
+-rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.6/okx/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.904724 okx-sdk-1.3.6/okx/wsapi/
+-rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.6/okx/wsapi/Factory.py
+-rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.6/okx/wsapi/PrivateAsync.py
+-rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.6/okx/wsapi/PublicAsync.py
+-rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.6/okx/wsapi/__init__.py
+-rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.6/okx/wsapi/wsutils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.931349 okx-sdk-1.3.6/okx_sdk.egg-info/
+-rw-rw-rw-   0        0        0    33887 2024-05-28 12:51:09.000000 okx-sdk-1.3.6/okx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-05-28 12:51:09.000000 okx-sdk-1.3.6/okx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:51:09.000000 okx-sdk-1.3.6/okx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-28 12:51:09.000000 okx-sdk-1.3.6/okx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 12:51:09.000000 okx-sdk-1.3.6/okx_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:51:09.933378 okx-sdk-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2024-05-28 12:50:12.000000 okx-sdk-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:51:09.929505 okx-sdk-1.3.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.6/tests/__init__.py
```

### Comparing `okx-sdk-1.3.5/LICENSE` & `okx-sdk-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/PKG-INFO` & `okx-sdk-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.5
+Version: 1.3.6
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `okx-sdk-1.3.5/README.md` & `okx-sdk-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/__init__.py` & `okx-sdk-1.3.6/okx/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/clients.py` & `okx-sdk-1.3.6/okx/clients.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/constants.py` & `okx-sdk-1.3.6/okx/constants.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/exceptions.py` & `okx-sdk-1.3.6/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Account.py` & `okx-sdk-1.3.6/okx/restapi/Account.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/AlgoTrading.py` & `okx-sdk-1.3.6/okx/restapi/AlgoTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/BaseClient.py` & `okx-sdk-1.3.6/okx/restapi/BaseClient.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/BlockTrading.py` & `okx-sdk-1.3.6/okx/restapi/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Broker.py` & `okx-sdk-1.3.6/okx/restapi/Broker.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/CopyTrading.py` & `okx-sdk-1.3.6/okx/restapi/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Finance.py` & `okx-sdk-1.3.6/okx/restapi/Finance.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Funding.py` & `okx-sdk-1.3.6/okx/restapi/Funding.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/GridTrading.py` & `okx-sdk-1.3.6/okx/restapi/GridTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/PublicData.py` & `okx-sdk-1.3.6/okx/restapi/PublicData.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/RecurringBuy.py` & `okx-sdk-1.3.6/okx/restapi/RecurringBuy.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Rubik.py` & `okx-sdk-1.3.6/okx/restapi/Rubik.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/SignalTrading.py` & `okx-sdk-1.3.6/okx/restapi/SignalTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/SpreadTrading.py` & `okx-sdk-1.3.6/okx/restapi/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/SubAccount.py` & `okx-sdk-1.3.6/okx/restapi/SubAccount.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/Trading.py` & `okx-sdk-1.3.6/okx/restapi/Trading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/restapi/__init__.py` & `okx-sdk-1.3.6/okx/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/utils.py` & `okx-sdk-1.3.6/okx/utils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/wsapi/Factory.py` & `okx-sdk-1.3.6/okx/wsapi/Factory.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/wsapi/PrivateAsync.py` & `okx-sdk-1.3.6/okx/wsapi/PrivateAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/wsapi/PublicAsync.py` & `okx-sdk-1.3.6/okx/wsapi/PublicAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx/wsapi/wsutils.py` & `okx-sdk-1.3.6/okx/wsapi/wsutils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/okx_sdk.egg-info/PKG-INFO` & `okx-sdk-1.3.6/okx_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.5
+Version: 1.3.6
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `okx-sdk-1.3.5/okx_sdk.egg-info/SOURCES.txt` & `okx-sdk-1.3.6/okx_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.5/setup.py` & `okx-sdk-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
     
-VERSION = '1.3.5'
+VERSION = '1.3.6'
 DESCRIPTION = 'Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python'
 
 setuptools.setup(
     name="okx-sdk",
     version=VERSION,
     author="Burak Öner",
     author_email="info@burakoner.com",
```

