# Comparing `tmp/yc_aws_wrapper-0.0.1.tar.gz` & `tmp/yc_aws_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yc_aws_wrapper-0.0.1.tar", last modified: Wed May 22 14:53:22 2024, max compression
+gzip compressed data, was "yc_aws_wrapper-0.0.2.tar", last modified: Tue May 28 07:50:49 2024, max compression
```

## Comparing `yc_aws_wrapper-0.0.1.tar` & `yc_aws_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.649551 yc_aws_wrapper-0.0.1/
--rw-r--r--   0 macuser    (502) staff       (20)     1226 2023-08-25 10:40:36.000000 yc_aws_wrapper-0.0.1/COPYRIGHT
--rw-r--r--   0 macuser    (502) staff       (20)    35149 2024-05-20 12:22:26.000000 yc_aws_wrapper-0.0.1/LICENSE
--rw-r--r--   0 macuser    (502) staff       (20)       52 2024-05-20 12:46:04.000000 yc_aws_wrapper-0.0.1/MANIFEST.in
--rw-r--r--   0 macuser    (502) staff       (20)     2118 2024-05-22 14:53:22.649328 yc_aws_wrapper-0.0.1/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)      780 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/README.md
--rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-22 14:53:22.649587 yc_aws_wrapper-0.0.1/setup.cfg
--rw-r--r--   0 macuser    (502) staff       (20)     3713 2024-05-22 14:52:38.000000 yc_aws_wrapper-0.0.1/setup.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.646514 yc_aws_wrapper-0.0.1/tests/
--rw-r--r--   0 macuser    (502) staff       (20)     1842 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/tests/test_s3.py
--rw-r--r--   0 macuser    (502) staff       (20)     1907 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/tests/test_sqs.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.647147 yc_aws_wrapper-0.0.1/yc_aws_wrapper/
--rw-r--r--   0 macuser    (502) staff       (20)     1966 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/__about__.py
--rw-r--r--   0 macuser    (502) staff       (20)     1703 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/__init__.py
--rw-r--r--   0 macuser    (502) staff       (20)     2230 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/base.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648294 yc_aws_wrapper-0.0.1/yc_aws_wrapper/kinesis/
--rw-r--r--   0 macuser    (502) staff       (20)      600 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/kinesis/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648536 yc_aws_wrapper-0.0.1/yc_aws_wrapper/s3/
--rw-r--r--   0 macuser    (502) staff       (20)     1306 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/s3/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648776 yc_aws_wrapper-0.0.1/yc_aws_wrapper/sqs/
--rw-r--r--   0 macuser    (502) staff       (20)     2578 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/sqs/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.649065 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/
--rw-r--r--   0 macuser    (502) staff       (20)     2118 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)      483 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-22 13:53:56.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 macuser    (502) staff       (20)       31 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/requires.txt
--rw-r--r--   0 macuser    (502) staff       (20)       15 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.028074 yc_aws_wrapper-0.0.2/
+-rw-r--r--   0 macuser    (502) staff       (20)     1226 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/COPYRIGHT
+-rw-r--r--   0 macuser    (502) staff       (20)    35149 2024-05-20 12:22:26.000000 yc_aws_wrapper-0.0.2/LICENSE
+-rw-r--r--   0 macuser    (502) staff       (20)       52 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/MANIFEST.in
+-rw-r--r--   0 macuser    (502) staff       (20)     3204 2024-05-28 07:50:49.027840 yc_aws_wrapper-0.0.2/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)     1865 2024-05-27 15:43:12.000000 yc_aws_wrapper-0.0.2/README.md
+-rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-28 07:50:49.028113 yc_aws_wrapper-0.0.2/setup.cfg
+-rw-r--r--   0 macuser    (502) staff       (20)     3713 2024-05-22 15:24:55.000000 yc_aws_wrapper-0.0.2/setup.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.025238 yc_aws_wrapper-0.0.2/tests/
+-rw-r--r--   0 macuser    (502) staff       (20)     2375 2024-05-28 07:47:49.000000 yc_aws_wrapper-0.0.2/tests/test_s3.py
+-rw-r--r--   0 macuser    (502) staff       (20)     2379 2024-05-28 07:47:10.000000 yc_aws_wrapper-0.0.2/tests/test_sqs.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.025871 yc_aws_wrapper-0.0.2/yc_aws_wrapper/
+-rw-r--r--   0 macuser    (502) staff       (20)     1966 2024-05-28 07:50:27.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/__about__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     1703 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/__init__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     4001 2024-05-28 07:43:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/base.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.026820 yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/
+-rw-r--r--   0 macuser    (502) staff       (20)      600 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027063 yc_aws_wrapper-0.0.2/yc_aws_wrapper/s3/
+-rw-r--r--   0 macuser    (502) staff       (20)     1696 2024-05-27 15:02:06.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/s3/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027273 yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/
+-rw-r--r--   0 macuser    (502) staff       (20)     3108 2024-05-27 14:45:14.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027559 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/
+-rw-r--r--   0 macuser    (502) staff       (20)     3204 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)      483 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 07:50:48.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 macuser    (502) staff       (20)       31 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/requires.txt
+-rw-r--r--   0 macuser    (502) staff       (20)       15 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/top_level.txt
```

### Comparing `yc_aws_wrapper-0.0.1/COPYRIGHT` & `yc_aws_wrapper-0.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.1/LICENSE` & `yc_aws_wrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.1/setup.py` & `yc_aws_wrapper-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.1/tests/test_s3.py` & `yc_aws_wrapper-0.0.2/tests/test_s3.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import unittest
 
 from yc_aws_wrapper.s3 import S3
 
 
 def order(number):
     def decorator(func):
-        setattr(func, 'order', number)
+        setattr(func, "order", number)
         return func
 
     return decorator
 
 
 class TestS3(unittest.TestCase):
-    bucket = os.getenv("S3_BUCKET")
+    bucket = os.getenv("S3_BUCKET_FOO")
     s3 = S3("s3")
     data = {"Name": "Test", "Service": "S3", "package": "yc-aws-wrapper"}
     file_name = os.path.join("test", "wrapper", "aws", "yc.json")
     file = bytes(json.dumps(data, indent=4).encode("utf8"))
 
     @classmethod
     def sortTestMethodsUsing(cls, pre, then):
@@ -32,30 +32,45 @@
             self.assertTrue(True)
 
     @order(2)
     def test_put(self):
         if self.file is not None:
             hasher = hashlib.md5()
             hasher.update(self.file)
-            response = self.s3.put(key=self.file_name, bucket=self.bucket, body=self.file, acl="private")
+            response = self.s3.foo.put(key=self.file_name, body=self.file, acl="private")
             self.assertEqual(hasher.hexdigest(), str(response.get("ETag", None)).strip("\""))
         else:
             self.assertTrue(False)
 
     @order(3)
     def test_get(self):
-        response = self.s3.get(key=self.file_name, bucket=self.bucket)
+        response = self.s3.foo.get(key=self.file_name)
         if response is not None:
             hasher = hashlib.md5()
             hasher.update(self.file)
             download = response["Body"]
             self.assertEqual(hasher.hexdigest(), str(response.get("ETag", None)).strip("\""))
         else:
             self.assertIsNotNone(response)
 
     @order(4)
     def test_deserialize(self):
         data = self.s3.deserialize(self.s3.buffer(self.data))
         self.assertTrue(isinstance(data, dict))
 
+    @order(5)
+    def test_load_all_clients(self):
+        os.environ.setdefault("S3_BUCKET_FOO2", os.getenv("S3_BUCKET_FOO"))
+        os.environ.setdefault("S3_BUCKET_FOO3", os.getenv("S3_BUCKET_FOO"))
+        if "foo2" not in self.s3 and "foo3" not in self.s3:
+            self.s3.load_all_clients()
+        else:
+            self.assertTrue(False)
+        self.assertTrue("foo2" in self.s3 and "foo3" in self.s3)
+
+    @classmethod
+    def tearDownClass(cls) -> None:
+        os.environ.pop("S3_BUCKET_FOO2", "")
+        os.environ.pop("S3_BUCKET_FOO3", "")
+
 
 unittest.TestLoader.sortTestMethodsUsing = TestS3.sortTestMethodsUsing
```

### Comparing `yc_aws_wrapper-0.0.1/yc_aws_wrapper/__about__.py` & `yc_aws_wrapper-0.0.2/yc_aws_wrapper/__about__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,12 @@
     "__license__",
     "__copyright__"
 ]
 
 __title__ = "yc-aws-wrapper"
 __summary__ = "yc-aws-wrapper."
 __uri__ = "https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "MCode GmbH"
 __email__ = "python-yandex-cloud-sdk-wrapper@mcode.cc"
 __license__ = "GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007"
 __copyright__ = "2021 %s" % __author__
```

### Comparing `yc_aws_wrapper-0.0.1/yc_aws_wrapper/__init__.py` & `yc_aws_wrapper-0.0.2/yc_aws_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.1/yc_aws_wrapper/kinesis/__init__.py` & `yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.1/yc_aws_wrapper/sqs/__init__.py` & `yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,75 @@
 import json
 from typing import Optional, Union
 
+import boto3
 from botocore.exceptions import ClientError
 
-from ..base import Service
+from ..base import DynamicClient, DynamicService
 
 
-class SQS(Service):
-    def get_url(self, queue: str) -> Optional[str]:
-        return self.client.get_queue_url(QueueName=queue).get("QueueUrl", None)
+class SQSClient(DynamicClient):
+    def __init__(self, client: boto3.client, path: str):
+        super().__init__(client, path)
+        self.queue = self.client.get_queue_url(QueueName=path).get("QueueUrl", None)
 
-    def send(self, queue: str, message: Union[dict, str], attributes: dict = None):
+    def send(self, message: Union[dict, str], attributes: dict = None) -> dict:
+        """
+        :param message: MessageBody
+        :param attributes: MessageAttribute
+        :return: response form send
+        """
         params = {
-            "QueueUrl": self.get_url(queue=queue),
+            "QueueUrl": self.queue,
             "MessageBody": json.dumps(message) if isinstance(message, dict) else message
         }
         if isinstance(attributes, dict):
             params["MessageAttribute"] = attributes
         return self.client.send_message(**params)
 
-    def receive(self, queue: str, visibility: int = 60, wait: int = 0,
-                max_number: int = 10,  additional: dict = None) -> list:
+    def receive(self, visibility: int = 60, wait: int = 20, max_number: int = 10, **kwargs) -> list:
         """
-        :param queue: Queue name
         :param visibility: The duration (in seconds) that the received messages are hidden from subsequent retrieve
             requests after being retrieved by a ReceiveMessage request.
         :param wait: The duration (in seconds) for which the call waits for a message to arrive in the queue before
             returning. If a message is available, the call returns sooner than WaitTimeSeconds. If no messages are
             available and the wait time expires, the call does not return a message list.
         :param max_number: The maximum number of messages to return. Amazon SQS never returns more messages than this
             value (however, fewer messages might be returned). Valid values: 1 to 10
-        :param additional: additional params from guide boto3 -> SQS.Client.receive_message
+        :param kwargs: additional params from guide boto3 -> SQS.Client.receive_message
         :return: list, dicts or empty
         """
-        if not isinstance(additional, dict):
-            additional = {}
+
         params = {
-            "QueueUrl": self.get_url(queue=queue),
+            "QueueUrl": self.queue,
             "VisibilityTimeout": visibility,
             "WaitTimeSeconds": wait,
             "MaxNumberOfMessages": max_number,
-            **additional
+            **kwargs
         }
         return self.client.receive_message(**params).get("Messages", [])
 
-    def delete_message(self, queue: str, receipt: str) -> bool:
+    def delete_message(self, receipt: str) -> bool:
         try:
-            self.client.delete_message(QueueUrl=self.get_url(queue), ReceiptHandle=receipt)
+            self.client.delete_message(QueueUrl=self.queue, ReceiptHandle=receipt)
             result = True
         except ClientError as e:
             try:
                 if e.response["Error"]["Code"] == "ReceiptHandleIsInvalid":
                     result = False
                 else:
                     raise e
             except Exception:
                 raise e
         return result
+
+
+class SQS(DynamicService):
+    def __init__(self, name: str = "sqs", prefix: str = "TUBE",
+                 client_class=SQSClient, auth: bool = True, config: dict = None):
+        super().__init__(name=name, prefix=prefix, client_class=client_class, auth=auth, config=config)
+
+    def get_url(self, queue: str) -> Optional[str]:
+        return self.client.get_queue_url(QueueName=queue).get("QueueUrl", None)
+
+    def __getattr__(self, item: str) -> SQSClient:
+        return super().__getattr__(item)
```

