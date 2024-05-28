# Comparing `tmp/muffin_kafka-0.2.5.tar.gz` & `tmp/muffin_kafka-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_kafka-0.2.5.tar", max compression
+gzip compressed data, was "muffin_kafka-0.2.6.tar", max compression
```

## Comparing `muffin_kafka-0.2.5.tar` & `muffin_kafka-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1328 2024-03-27 09:35:41.980480 muffin_kafka-0.2.5/README.md
--rw-r--r--   0        0        0       74 2024-03-27 09:35:41.980480 muffin_kafka-0.2.5/muffin_kafka/__init__.py
--rw-r--r--   0        0        0     7795 2024-03-27 09:35:41.980480 muffin_kafka-0.2.5/muffin_kafka/plugin.py
--rw-r--r--   0        0        0        0 2024-03-27 09:35:41.980480 muffin_kafka-0.2.5/muffin_kafka/py.typed
--rw-r--r--   0        0        0     1798 2024-03-27 09:35:41.980480 muffin_kafka-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 muffin_kafka-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1328 2024-03-27 09:46:55.115080 muffin_kafka-0.2.6/README.md
+-rw-r--r--   0        0        0       74 2024-03-27 09:46:55.115080 muffin_kafka-0.2.6/muffin_kafka/__init__.py
+-rw-r--r--   0        0        0     7807 2024-03-27 09:46:55.115080 muffin_kafka-0.2.6/muffin_kafka/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:46:55.115080 muffin_kafka-0.2.6/muffin_kafka/py.typed
+-rw-r--r--   0        0        0     1798 2024-03-27 09:46:55.115080 muffin_kafka-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 muffin_kafka-0.2.6/PKG-INFO
```

### Comparing `muffin_kafka-0.2.5/README.md` & `muffin_kafka-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `muffin_kafka-0.2.5/muffin_kafka/plugin.py` & `muffin_kafka-0.2.6/muffin_kafka/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         for task in self.tasks:
             task.cancel()
 
         await gather(*self.tasks, return_exceptions=True)
 
         cfg = self.cfg
 
-        if cfg.produce and self.producer:
+        if cfg.produce and hasattr(self, "producer"):
             await self.producer.stop()
 
         if cfg.listen:
             await gather(*[consumer.stop() for consumer in self.consumers.values()])
 
     async def send(self, topic: str, value: Any, key=None, **params):
         """Send a message to Kafka."""
```

### Comparing `muffin_kafka-0.2.5/pyproject.toml` & `muffin_kafka-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-kafka"
-version = "0.2.5"
+version = "0.2.6"
 description = "Kafka Integration for Muffin framework"
 readme = "README.md"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 homepage = "https://github.com/klen/muffin-kafka"
 repository = "https://github.com/klen/muffin-kafka"
 keywords = ["kafka", "asyncio", "asgi", "muffin"]
```

### Comparing `muffin_kafka-0.2.5/PKG-INFO` & `muffin_kafka-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-kafka
-Version: 0.2.5
+Version: 0.2.6
 Summary: Kafka Integration for Muffin framework
 Home-page: https://github.com/klen/muffin-kafka
 License: MIT
 Keywords: kafka,asyncio,asgi,muffin
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.9,<4.0
```

