# Comparing `tmp/autoutils_log-0.2.0.tar.gz` & `tmp/autoutils_log-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils_log-0.2.0.tar", max compression
+gzip compressed data, was "autoutils_log-0.3.0.tar", max compression
```

## Comparing `autoutils_log-0.2.0.tar` & `autoutils_log-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.2.0/LICENSE
--rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.2.0/README.md
--rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.2.0/autoutils_log/__init__.py
--rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.2.0/autoutils_log/base.py
--rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.2.0/autoutils_log/colorful_stream_handler.py
--rw-r--r--   0        0        0     1804 2024-05-27 21:03:17.926701 autoutils_log-0.2.0/autoutils_log/kafka_handler.py
--rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.2.0/autoutils_log/logstash_handler.py
--rw-r--r--   0        0        0      740 2024-05-27 21:03:18.958720 autoutils_log-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 autoutils_log-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.3.0/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.3.0/README.md
+-rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.3.0/autoutils_log/__init__.py
+-rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.3.0/autoutils_log/base.py
+-rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.3.0/autoutils_log/colorful_stream_handler.py
+-rw-r--r--   0        0        0     1773 2024-05-28 10:31:18.901528 autoutils_log-0.3.0/autoutils_log/kafka_handler.py
+-rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.3.0/autoutils_log/logstash_handler.py
+-rw-r--r--   0        0        0      740 2024-05-28 10:31:20.514557 autoutils_log-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 autoutils_log-0.3.0/PKG-INFO
```

### Comparing `autoutils_log-0.2.0/LICENSE` & `autoutils_log-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.2.0/autoutils_log/base.py` & `autoutils_log-0.3.0/autoutils_log/base.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.2.0/autoutils_log/colorful_stream_handler.py` & `autoutils_log-0.3.0/autoutils_log/colorful_stream_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.2.0/autoutils_log/kafka_handler.py` & `autoutils_log-0.3.0/autoutils_log/kafka_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,39 +5,41 @@
 
 import pytz
 from confluent_kafka import Producer
 
 from .base import BaseLogHandler
 
 
+def delivery_report(err, msg):
+    pass
+
+
 class KafkaHandler(BaseLogHandler):
     """
         A handler class which send data to logstash.
     """
 
     def __init__(self, log_server: str, topic: str, app_name: str = None, host_name: str = None,
-                 extra_data: dict = None, timeout: int = 2,
+                 extra_data: dict = None,
                  timezone: str = "Asia/Tehran"):
         super().__init__(app_name=app_name, host_name=host_name, extra_data=extra_data)
         self.log_server = log_server
         self.timezone = timezone
         self.topic = topic
-        self.timeout = timeout
         self.producer = Producer({'bootstrap.servers': self.log_server}) if self.log_server else None
 
     def _get_send_data(self, record: logging.LogRecord):
         send_data = super()._get_send_data(record=record)
         send_data["time"] = self.get_now_time_for_elastic()
         return send_data
 
     def send(self, send_data: dict):
         if self.producer is None:
             return
-        self.producer.produce(self.topic, json.dumps(send_data).encode("utf-8"))
-        self.producer.flush(timeout=self.timeout)
+        self.producer.produce(self.topic, json.dumps(send_data).encode("utf-8"), callback=delivery_report)
 
     def emit(self, record: logging.LogRecord) -> None:
         if not self.log_server or not self.topic:
             return
         try:
             send_data = self._get_send_data(record=record)
             self.send(send_data=send_data)
```

### Comparing `autoutils_log-0.2.0/autoutils_log/logstash_handler.py` & `autoutils_log-0.3.0/autoutils_log/logstash_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.2.0/pyproject.toml` & `autoutils_log-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils-log"
-version = "0.2.0"
+version = "0.3.0"
 description = "Some Good Function For Log"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils-log"
 repository = "https://github.com/rezazeiny/autoutils-log"
 keywords = ["autoutils_log"]
```

### Comparing `autoutils_log-0.2.0/PKG-INFO` & `autoutils_log-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoutils-log
-Version: 0.2.0
+Version: 0.3.0
 Summary: Some Good Function For Log
 Home-page: https://github.com/rezazeiny/autoutils-log
 License: MIT
 Keywords: autoutils_log
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.12,<4.0
```

