# Comparing `tmp/pyscanasdk-1.0.7.tar.gz` & `tmp/pyscanasdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscanasdk-1.0.7.tar", last modified: Thu Oct 12 03:28:53 2023, max compression
+gzip compressed data, was "pyscanasdk-1.0.9.tar", last modified: Tue May 28 07:36:58 2024, max compression
```

## Comparing `pyscanasdk-1.0.7.tar` & `pyscanasdk-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-10-12 03:28:53.988888 pyscanasdk-1.0.7/
--rw-rw-rw-   0        0        0      167 2023-10-12 03:28:53.987898 pyscanasdk-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-12 03:28:53.976791 pyscanasdk-1.0.7/pyscanasdk/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:14:48.000000 pyscanasdk-1.0.7/pyscanasdk/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-10-11 09:14:48.000000 pyscanasdk-1.0.7/pyscanasdk/moderation.py
--rw-rw-rw-   0        0        0     7304 2023-10-12 03:21:39.000000 pyscanasdk-1.0.7/pyscanasdk/v3.py
-drwxrwxrwx   0        0        0        0 2023-10-12 03:28:53.987898 pyscanasdk-1.0.7/pyscanasdk.egg-info/
--rw-rw-rw-   0        0        0      167 2023-10-12 03:28:53.000000 pyscanasdk-1.0.7/pyscanasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-10-12 03:28:53.000000 pyscanasdk-1.0.7/pyscanasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-12 03:28:53.000000 pyscanasdk-1.0.7/pyscanasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-10-12 03:28:53.000000 pyscanasdk-1.0.7/pyscanasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-12 03:28:53.000000 pyscanasdk-1.0.7/pyscanasdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-12 03:28:53.988888 pyscanasdk-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-10-12 03:28:01.000000 pyscanasdk-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:36:58.873746 pyscanasdk-1.0.9/
+-rw-rw-rw-   0        0        0      173 2024-05-28 07:36:58.872744 pyscanasdk-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 07:36:58.857753 pyscanasdk-1.0.9/pyscanasdk/
+-rw-rw-rw-   0        0        0        0 2024-05-28 02:47:45.000000 pyscanasdk-1.0.9/pyscanasdk/__init__.py
+-rw-rw-rw-   0        0        0     2096 2024-05-28 02:47:45.000000 pyscanasdk-1.0.9/pyscanasdk/moderation.py
+-rw-rw-rw-   0        0        0     8523 2024-05-28 02:47:45.000000 pyscanasdk-1.0.9/pyscanasdk/v3.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:36:58.871753 pyscanasdk-1.0.9/pyscanasdk.egg-info/
+-rw-rw-rw-   0        0        0      173 2024-05-28 07:36:58.000000 pyscanasdk-1.0.9/pyscanasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-28 07:36:58.000000 pyscanasdk-1.0.9/pyscanasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:36:58.000000 pyscanasdk-1.0.9/pyscanasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 07:36:58.000000 pyscanasdk-1.0.9/pyscanasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-28 07:36:58.000000 pyscanasdk-1.0.9/pyscanasdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:36:58.873746 pyscanasdk-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      409 2024-05-28 07:36:32.000000 pyscanasdk-1.0.9/setup.py
```

### Comparing `pyscanasdk-1.0.7/pyscanasdk/moderation.py` & `pyscanasdk-1.0.9/pyscanasdk/moderation.py`

 * *Files identical despite different names*

### Comparing `pyscanasdk-1.0.7/pyscanasdk/v3.py` & `pyscanasdk-1.0.9/pyscanasdk/v3.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import time
 from urllib.parse import urlparse, parse_qsl, parse_qs
 
 
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#creating-the-package-files
 class ModerateClient(object):
     def __init__(self, app_id, secret_key, text_business_id='', img_business_id='', audio_business_id='',
-                 video_business_id='', doc_business_id=''):
+                 video_business_id='', doc_business_id='', url_business_id=''):
         """
         :param app_id: 获取来的appid
         :param secret_key: 获取到的和appid对应的secret_key
         :param text_business_id: 文本审核的业务id
         :return:
         """
         self.app_id = app_id
         self.secret_key = secret_key
         self.text_business_id = text_business_id
         self.img_business_id = img_business_id
         self.audio_business_id = audio_business_id
         self.video_business_id = video_business_id
         self.doc_business_id = doc_business_id
+        self.url_business_id = url_business_id
 
     def text(self, content, ac=False, extra="", timeout=10):
         """
         文本审核的接口
         :param content: 待审核的文本内容
         :param ac: False同步/True异步
         :param timeout: 超时时间，单位秒
@@ -67,74 +68,104 @@
             "businessId": self.img_business_id,
             "images": content,
             "extra": extra
         }
         resp = requests.post(url=moderation_url, json=data, timeout=timeout)
         return resp.json()
 
-    def audio(self, content, extra="", timeout=10):
+    def audio(self, content, content_id, extra="", timeout=10):
         """
         图片审核的接口
         :param content: 待审核的音频
+        :param content_id: 内容id
         :param timeout: 超时时间，单位秒
         :param extra: 透传字段
         :return:
         """
         if not self.audio_business_id:
             return {"msg": "音频business_id不能为空!"}
         async_url = "https://newkmsapi.qixincha.com/kms-open/v3/audio/async"
         moderation_url = async_url
         data = {
             "appId": self.app_id,
             "secretKey": self.secret_key,
             "businessId": self.audio_business_id,
+            "contentId": content_id,
             "url": content,
             "extra": extra
         }
         resp = requests.post(url=moderation_url, json=data, timeout=timeout)
         return resp.json()
 
-    def video(self, content, extra="", timeout=10):
+    def video(self, content, content_id, extra="", timeout=10):
         """
         图片审核的接口
         :param content: 待审核的视频
+        :param content_id: 内容id
         :param timeout: 超时时间，单位秒
         :param extra: 透传字段
         :return:
         """
         if not self.video_business_id:
             return {"msg": "视频business_id不能为空!"}
         async_url = "https://newkmsapi.qixincha.com/kms-open/v3/video/async"
         moderation_url = async_url
         data = {
             "appId": self.app_id,
             "secretKey": self.secret_key,
             "businessId": self.video_business_id,
+            "contentId": content_id,
             "url": content,
             "extra": extra
         }
         resp = requests.post(url=moderation_url, json=data, timeout=timeout)
         return resp.json()
 
-    def doc(self, content, extra="", timeout=10):
+    def doc(self, content, content_id, extra="", timeout=10):
         """
         文档审核的接口
         :param content: 待审核的文档
+        :param content_id: 内容id
         :param timeout: 超时时间，单位秒
         :param extra: 透传字段
         :return:
         """
         if not self.doc_business_id:
             return {"msg": "文档business_id不能为空!"}
         async_url = "https://newkmsapi.qixincha.com/kms-open/v3/doc/async"
         moderation_url = async_url
         data = {
             "appId": self.app_id,
             "secretKey": self.secret_key,
             "businessId": self.doc_business_id,
+            "contentId": content_id,
+            "url": content,
+            "extra": extra
+        }
+        resp = requests.post(url=moderation_url, json=data, timeout=timeout)
+        return resp.json()
+
+    def url(self, content, content_id, extra="", timeout=10):
+        """
+        图片审核的接口
+        :param content_id: 内容id
+        :param content: 待审核的url
+        :param timeout: 超时时间，单位秒
+        :param extra: 透传字段
+        :return:
+        """
+        if not self.url_business_id:
+            return {"msg": "url_business_id不能为空!"}
+        async_url = "https://newkmsapi.qixincha.com/kms-open/v3/url/async"
+        moderation_url = async_url
+        data = {
+            "appId": self.app_id,
+            "secretKey": self.secret_key,
+            "businessId": self.url_business_id,
+            "contentId": content_id,
             "url": content,
             "extra": extra
         }
         resp = requests.post(url=moderation_url, json=data, timeout=timeout)
         return resp.json()
 
     def gen_signature(self, business_id, timestamp, nonce):
@@ -143,15 +174,16 @@
         timestamp 时间戳
         nonce 随机数 不要取0
         Returns: 参数签名md5值
         """
         if not any([business_id, timestamp, nonce]):
             print('businessId,timestamp,nonce不能为空！')
             return ''
-        params = {"nonce": nonce, "timestamp": timestamp, 'businessId': business_id}
+        params = {"nonce": nonce, "timestamp": timestamp,
+                  'businessId': business_id}
         buff = ""
         for k in sorted(params.keys()):
             buff += str(k) + str(params[k])
         buff += self.secret_key
         return hashlib.md5(buff.encode('utf8')).hexdigest()
 
     @staticmethod
```

