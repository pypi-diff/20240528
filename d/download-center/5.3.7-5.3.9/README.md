# Comparing `tmp/download-center-5.3.7.tar.gz` & `tmp/download-center-5.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download-center-5.3.7.tar", last modified: Thu May 16 10:00:07 2024, max compression
+gzip compressed data, was "download-center-5.3.9.tar", last modified: Tue May 28 03:54:23 2024, max compression
```

## Comparing `download-center-5.3.7.tar` & `download-center-5.3.9.tar`

### file list

```diff
@@ -1,56 +1,52 @@
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.847679 download-center-5.3.7/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1870 2024-05-16 10:00:07.847494 download-center-5.3.7/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)      935 2024-05-16 10:00:03.000000 download-center-5.3.7/README.md
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842227 download-center-5.3.7/download_center/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/config.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842904 download-center-5.3.7/download_center/new_spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/__init__.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.843814 download-center-5.3.7/download_center/new_spider/downloader/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     7982 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      254 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_capture.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      260 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9176 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_local_downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      251 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_render.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.844174 download-center-5.3.7/download_center/new_spider/spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    16634 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/basespider.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/spider.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.845536 download-center-5.3.7/download_center/new_spider/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_mobile_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_pc_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_spider_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    37369 2024-05-16 09:59:13.000000 download-center-5.3.7/download_center/new_spider/util/util_baidu.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_baidu_relate.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_md5.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_ping.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_url.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_useragent.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/requirements.txt
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.846807 download-center-5.3.7/download_center/store/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/baidu_cookies.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/py_store_mysql_pool.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_cache.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_es.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_es_v2.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_file.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_mongo.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_oss.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.847277 download-center-5.3.7/download_center/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/py_util_basestore.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/util_log.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/util_log_v2.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842776 download-center-5.3.7/download_center.egg-info/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1870 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1838 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/SOURCES.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/dependency_links.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/requires.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       16 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/top_level.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-16 10:00:07.847728 download-center-5.3.7/setup.cfg
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4025 2024-05-16 10:00:03.000000 download-center-5.3.7/setup.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.703291 download-center-5.3.9/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1823 2024-05-28 03:54:23.703105 download-center-5.3.9/PKG-INFO
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      888 2024-05-28 03:53:33.000000 download-center-5.3.9/README.md
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695105 download-center-5.3.9/download_center/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/config.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695960 download-center-5.3.9/download_center/new_spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/__init__.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.696285 download-center-5.3.9/download_center/new_spider/downloader/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/downloader/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/downloader/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9076 2024-05-28 03:53:36.000000 download-center-5.3.9/download_center/new_spider/downloader/html_local_downloader.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.697023 download-center-5.3.9/download_center/new_spider/spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/spider/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    16614 2024-05-28 03:53:36.000000 download-center-5.3.9/download_center/new_spider/spider/basespider.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/spider/spider.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.700951 download-center-5.3.9/download_center/new_spider/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_mobile_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_pc_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_spider_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    37369 2024-05-16 09:59:13.000000 download-center-5.3.9/download_center/new_spider/util/util_baidu.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_baidu_relate.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_md5.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_ping.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_url.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_useragent.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/requirements.txt
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.702271 download-center-5.3.9/download_center/store/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/baidu_cookies.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/py_store_mysql_pool.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_cache.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_es.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_es_v2.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_file.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_mongo.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_oss.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.702884 download-center-5.3.9/download_center/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/py_util_basestore.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/util_log.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/util_log_v2.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695838 download-center-5.3.9/download_center.egg-info/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1823 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/PKG-INFO
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1622 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/SOURCES.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/dependency_links.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/requires.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       16 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/top_level.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-28 03:54:23.703377 download-center-5.3.9/setup.cfg
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4025 2024-05-28 03:54:22.000000 download-center-5.3.9/setup.py
```

### Comparing `download-center-5.3.7/PKG-INFO` & `download-center-5.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.3.7
+Version: 5.3.9
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -43,15 +43,14 @@
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
 - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
 - 5.3.5: 添加本地模式代理
-- 5.3.7: config 配置文件路径错误问题
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.7/README.md` & `download-center-5.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
 - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
 - 5.3.5: 添加本地模式代理
-- 5.3.7: config 配置文件路径错误问题
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.7/download_center/config.py` & `download-center-5.3.9/download_center/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/downloader/config.py` & `download-center-5.3.9/download_center/new_spider/downloader/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/downloader/html_local_downloader.py` & `download-center-5.3.9/download_center/new_spider/downloader/html_local_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 # -*- coding: utf-8 -*-
 """
  @Time: 2019/6/10 13:21
 """
-import time
-import os
-import sys
 import traceback
 import hashlib
-import urllib
-import pymysql
-import json
-import time
-import base64
 from pymysql.converters import escape_string
 
 from datetime import datetime
 
 import re
 import urllib3
 urllib3.disable_warnings()
```

### Comparing `download-center-5.3.7/download_center/new_spider/spider/basespider.py` & `download-center-5.3.9/download_center/new_spider/spider/basespider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf8 -*-
 import json
 
 import requests
-from download_center.new_spider.downloader.downloader import Downloader
 from download_center.new_spider.downloader.downloader import SpiderRequest
 from download_center.new_spider.downloader.html_local_downloader import HtmlLocalDownloader
 from download_center.new_spider.util.util_useragent import UtilUseragent
 from download_center.new_spider.downloader import config
 # from Queue import LifoQueue
 from queue import Queue
 from queue import Empty
@@ -73,23 +72,23 @@
                 raise RuntimeError('用户验证失败')
                 sys.exit()
         else:
             pass
 
     def get_downloader(self):
         """
-        设置下载器类型，默认为Downloader
+        # 设置下载器类型，默认为Downloader
+        由原默认为Downloader下载中心更改为proxy代理模式
         Return:
             SpiderDownloader
         """
-        if self.remote:
-            return Downloader()
-        else:
-            print("local downloader")
-            return HtmlLocalDownloader()
+        # if self.remote:
+        #     return Downloader()
+        print("local downloader")
+        return HtmlLocalDownloader()
 
     def start_requests(self):
         """
         初始化待发送请求队列，由子类实现。拼装一串SpiderRequest对象并送到sending_queue队列中
         """
         raise NotImplementedError()
 
@@ -160,15 +159,15 @@
         获取url爬取结果。将sended_queue队列中的SpiderRequest对象通过downloader到下载中心去获取抓取到的html
         """
         start_time = time.time()
         while True:
             try:
                 if self.response_queue.qsize() < self.response_queue_max:
                     request = self.sended_queue.get(timeout=1)
-                    if not self.remote:
+                    if self.remote:
                         user, password = self.get_user_password()
                         data = {"user": user, "password": password}
                         # 获取代理 ip
                         r = requests.post(config.AGENCYIP_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]),
                                           data=data, timeout=config.REQUEST_TIMEOUT)
                         request.config["proxies"] = json.loads(r.text)["proxy"]
                     results = self.downloader.get(request)
```

### Comparing `download-center-5.3.7/download_center/new_spider/spider/spider.py` & `download-center-5.3.9/download_center/new_spider/spider/spider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/ua_mobile_list.txt` & `download-center-5.3.9/download_center/new_spider/util/ua_mobile_list.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/ua_pc_list.txt` & `download-center-5.3.9/download_center/new_spider/util/ua_pc_list.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/util_baidu.py` & `download-center-5.3.9/download_center/new_spider/util/util_baidu.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/util_baidu_relate.py` & `download-center-5.3.9/download_center/new_spider/util/util_baidu_relate.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/util_ping.py` & `download-center-5.3.9/download_center/new_spider/util/util_ping.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/util_url.py` & `download-center-5.3.9/download_center/new_spider/util/util_url.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/new_spider/util/util_useragent.py` & `download-center-5.3.9/download_center/new_spider/util/util_useragent.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/baidu_cookies.py` & `download-center-5.3.9/download_center/store/baidu_cookies.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/config.py` & `download-center-5.3.9/download_center/store/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/py_store_mysql_pool.py` & `download-center-5.3.9/download_center/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/store_es.py` & `download-center-5.3.9/download_center/store/store_es.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/store_es_v2.py` & `download-center-5.3.9/download_center/store/store_es_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/store_mongo.py` & `download-center-5.3.9/download_center/store/store_mongo.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/store/store_oss.py` & `download-center-5.3.9/download_center/store/store_oss.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/util/py_util_basestore.py` & `download-center-5.3.9/download_center/util/py_util_basestore.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/util/util_log.py` & `download-center-5.3.9/download_center/util/util_log.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center/util/util_log_v2.py` & `download-center-5.3.9/download_center/util/util_log_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.7/download_center.egg-info/PKG-INFO` & `download-center-5.3.9/download_center.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-center
-Version: 5.3.7
+Version: 5.3.9
 Summary: spider framework for winndoo.
 Home-page: http://git.winndoo.cn:82/python/download_center/downloader_client.git
 Author: Welcome#1
 Author-email: baozhu.zhang@winndoo.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -43,15 +43,14 @@
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
 - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
 - 5.3.5: 添加本地模式代理
-- 5.3.7: config 配置文件路径错误问题
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.7/download_center.egg-info/SOURCES.txt` & `download-center-5.3.9/download_center.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 download_center.egg-info/SOURCES.txt
 download_center.egg-info/dependency_links.txt
 download_center.egg-info/requires.txt
 download_center.egg-info/top_level.txt
 download_center/new_spider/__init__.py
 download_center/new_spider/downloader/__init__.py
 download_center/new_spider/downloader/config.py
-download_center/new_spider/downloader/downloader.py
-download_center/new_spider/downloader/html_capture.py
-download_center/new_spider/downloader/html_downloader.py
 download_center/new_spider/downloader/html_local_downloader.py
-download_center/new_spider/downloader/html_render.py
 download_center/new_spider/spider/__init__.py
 download_center/new_spider/spider/basespider.py
 download_center/new_spider/spider/spider.py
 download_center/new_spider/util/__init__.py
 download_center/new_spider/util/ua_mobile_list.txt
 download_center/new_spider/util/ua_pc_list.txt
 download_center/new_spider/util/ua_spider_list.txt
```

### Comparing `download-center-5.3.7/setup.py` & `download-center-5.3.9/setup.py`

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
-VERSION = '5.3.7'
+VERSION = '5.3.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo',
     'oss2',
     'redis',
     'DBUtils',
```

