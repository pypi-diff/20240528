# Comparing `tmp/download-center-5.4.0.tar.gz` & `tmp/download-center-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\download-center-5.4.0.tar", last modified: Tue May 28 06:02:46 2024, max compression
+gzip compressed data, was "dist\download-center-5.4.1.tar", last modified: Tue May 28 06:12:46 2024, max compression
```

## Comparing `download-center-5.4.0.tar` & `download-center-5.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.295795 download-center-5.4.0/
--rw-rw-rw-   0        0        0     1829 2024-05-28 06:02:46.294798 download-center-5.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      914 2024-05-16 07:40:34.000000 download-center-5.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.249361 download-center-5.4.0/download_center/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/config.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.268342 download-center-5.4.0/download_center/new_spider/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.270305 download-center-5.4.0/download_center/new_spider/downloader/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/downloader/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/downloader/config.py
--rw-rw-rw-   0        0        0     9318 2024-05-28 03:21:13.000000 download-center-5.4.0/download_center/new_spider/downloader/html_local_downloader.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.273297 download-center-5.4.0/download_center/new_spider/spider/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/spider/__init__.py
--rw-rw-rw-   0        0        0    18441 2024-05-28 05:34:10.000000 download-center-5.4.0/download_center/new_spider/spider/basespider.py
--rw-rw-rw-   0        0        0     4832 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/spider/spider.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.280278 download-center-5.4.0/download_center/new_spider/util/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/__init__.py
--rw-rw-rw-   0        0        0    38181 2024-05-16 08:40:14.000000 download-center-5.4.0/download_center/new_spider/util/util_baidu.py
--rw-rw-rw-   0        0        0    12892 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_baidu_relate.py
--rw-rw-rw-   0        0        0      344 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_md5.py
--rw-rw-rw-   0        0        0      558 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_ping.py
--rw-rw-rw-   0        0        0      804 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_url.py
--rw-rw-rw-   0        0        0      741 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_useragent.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.289808 download-center-5.4.0/download_center/store/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/__init__.py
--rw-rw-rw-   0        0        0     3254 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/baidu_cookies.py
--rw-rw-rw-   0        0        0      802 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/config.py
--rw-rw-rw-   0        0        0     9397 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/py_store_mysql_pool.py
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_cache.py
--rw-rw-rw-   0        0        0     3398 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_es.py
--rw-rw-rw-   0        0        0     4163 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_es_v2.py
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_file.py
--rw-rw-rw-   0        0        0      764 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_mongo.py
--rw-rw-rw-   0        0        0     2082 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_oss.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.293800 download-center-5.4.0/download_center/util/
--rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/__init__.py
--rw-rw-rw-   0        0        0     6299 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/py_util_basestore.py
--rw-rw-rw-   0        0        0     2490 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/util_log.py
--rw-rw-rw-   0        0        0     2563 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/util_log_v2.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.266317 download-center-5.4.0/download_center.egg-info/
--rw-rw-rw-   0        0        0     1829 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1440 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 06:02:46.295795 download-center-5.4.0/setup.cfg
--rw-rw-rw-   0        0        0     4169 2024-05-28 05:46:24.000000 download-center-5.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.367892 download-center-5.4.1/
+-rw-rw-rw-   0        0        0     1829 2024-05-28 06:12:46.367892 download-center-5.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-05-16 07:40:34.000000 download-center-5.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.325007 download-center-5.4.1/download_center/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/config.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.334981 download-center-5.4.1/download_center/new_spider/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.337972 download-center-5.4.1/download_center/new_spider/downloader/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/downloader/config.py
+-rw-rw-rw-   0        0        0     9940 2024-05-28 06:09:52.000000 download-center-5.4.1/download_center/new_spider/downloader/html_local_downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.341963 download-center-5.4.1/download_center/new_spider/spider/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/spider/__init__.py
+-rw-rw-rw-   0        0        0    18441 2024-05-28 05:34:10.000000 download-center-5.4.1/download_center/new_spider/spider/basespider.py
+-rw-rw-rw-   0        0        0     4832 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/spider/spider.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.348944 download-center-5.4.1/download_center/new_spider/util/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/__init__.py
+-rw-rw-rw-   0        0        0    38181 2024-05-16 08:40:14.000000 download-center-5.4.1/download_center/new_spider/util/util_baidu.py
+-rw-rw-rw-   0        0        0    12892 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/util_baidu_relate.py
+-rw-rw-rw-   0        0        0      344 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/util_md5.py
+-rw-rw-rw-   0        0        0      558 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/util_ping.py
+-rw-rw-rw-   0        0        0      804 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/util_url.py
+-rw-rw-rw-   0        0        0      741 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/new_spider/util/util_useragent.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.361909 download-center-5.4.1/download_center/store/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/baidu_cookies.py
+-rw-rw-rw-   0        0        0      802 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/config.py
+-rw-rw-rw-   0        0        0     9397 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/py_store_mysql_pool.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_cache.py
+-rw-rw-rw-   0        0        0     3398 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_es.py
+-rw-rw-rw-   0        0        0     4163 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_es_v2.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_file.py
+-rw-rw-rw-   0        0        0      764 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_mongo.py
+-rw-rw-rw-   0        0        0     2082 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/store/store_oss.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.365898 download-center-5.4.1/download_center/util/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/util/__init__.py
+-rw-rw-rw-   0        0        0     6299 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/util/py_util_basestore.py
+-rw-rw-rw-   0        0        0     2490 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/util/util_log.py
+-rw-rw-rw-   0        0        0     2563 2024-05-16 07:40:34.000000 download-center-5.4.1/download_center/util/util_log_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:12:46.333984 download-center-5.4.1/download_center.egg-info/
+-rw-rw-rw-   0        0        0     1829 2024-05-28 06:12:46.000000 download-center-5.4.1/download_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2024-05-28 06:12:46.000000 download-center-5.4.1/download_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:12:46.000000 download-center-5.4.1/download_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-28 06:12:46.000000 download-center-5.4.1/download_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 06:12:46.000000 download-center-5.4.1/download_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:12:46.368890 download-center-5.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     4169 2024-05-28 06:11:35.000000 download-center-5.4.1/setup.py
```

### Comparing `download-center-5.4.0/PKG-INFO` & `download-center-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.4.0
+Version: 5.4.1
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Description: 
         ##版本说明：
```

### Comparing `download-center-5.4.0/README.md` & `download-center-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/config.py` & `download-center-5.4.1/download_center/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/downloader/config.py` & `download-center-5.4.1/download_center/new_spider/downloader/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/downloader/html_local_downloader.py` & `download-center-5.4.1/download_center/new_spider/downloader/html_local_downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -236,7 +236,29 @@
         for t in tlist:
             content = content.replace("<link" + t + ">", "")
         content = re.sub(' +', ' ', content)
         content = re.sub('\\t+', ' ', content)
         content = re.sub('\\r+', ' ', content)
         return content
 
+
+class SpiderRequest(object):
+
+    __slots__ = ['user_id', 'headers', 'config', 'urls']    # save memory
+
+    def __init__(self, user_id=None, headers=dict(), config=dict(), urls=list()):
+        self.user_id = user_id
+        self.headers = headers
+        self.config = config
+        self.urls = urls
+
+    def set_headers_key(self, key, value):
+        self.headers[key] = value
+
+    def set_headers(self, header):
+        self.headers = header
+
+    def set_config_key(self, key, value):
+        self.headers[key] = value
+
+    def set_config(self, set_configs):
+        self.headers = set_configs
```

### Comparing `download-center-5.4.0/download_center/new_spider/spider/basespider.py` & `download-center-5.4.1/download_center/new_spider/spider/basespider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/spider/spider.py` & `download-center-5.4.1/download_center/new_spider/spider/spider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/util/util_baidu.py` & `download-center-5.4.1/download_center/new_spider/util/util_baidu.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/util/util_baidu_relate.py` & `download-center-5.4.1/download_center/new_spider/util/util_baidu_relate.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/util/util_ping.py` & `download-center-5.4.1/download_center/new_spider/util/util_ping.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/util/util_url.py` & `download-center-5.4.1/download_center/new_spider/util/util_url.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/new_spider/util/util_useragent.py` & `download-center-5.4.1/download_center/new_spider/util/util_useragent.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/baidu_cookies.py` & `download-center-5.4.1/download_center/store/baidu_cookies.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/config.py` & `download-center-5.4.1/download_center/store/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/py_store_mysql_pool.py` & `download-center-5.4.1/download_center/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/store_es.py` & `download-center-5.4.1/download_center/store/store_es.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/store_es_v2.py` & `download-center-5.4.1/download_center/store/store_es_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/store_mongo.py` & `download-center-5.4.1/download_center/store/store_mongo.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/store/store_oss.py` & `download-center-5.4.1/download_center/store/store_oss.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/util/py_util_basestore.py` & `download-center-5.4.1/download_center/util/py_util_basestore.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/util/util_log.py` & `download-center-5.4.1/download_center/util/util_log.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center/util/util_log_v2.py` & `download-center-5.4.1/download_center/util/util_log_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/download_center.egg-info/PKG-INFO` & `download-center-5.4.1/download_center.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.4.0
+Version: 5.4.1
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Description: 
         ##版本说明：
```

### Comparing `download-center-5.4.0/download_center.egg-info/SOURCES.txt` & `download-center-5.4.1/download_center.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.4.0/setup.py` & `download-center-5.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'download-center'
 DESCRIPTION = 'spider framework for winndoo.'
 URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
 EMAIL = 'baozhu.zhang@winndoo.com'
 AUTHOR = 'Welcome#1'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '5.4.0'
+VERSION = '5.4.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo',
     'oss2',
     'redis',
     'DBUtils',
```

