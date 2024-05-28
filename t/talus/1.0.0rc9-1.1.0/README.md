# Comparing `tmp/talus-1.0.0rc9.tar.gz` & `tmp/talus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc9.tar", last modified: Wed May 22 17:16:31 2024, max compression
+gzip compressed data, was "talus-1.1.0.tar", last modified: Tue May 28 21:03:23 2024, max compression
```

## Comparing `talus-1.0.0rc9.tar` & `talus-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 17:16:12.000000 talus-1.0.0rc9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 17:16:12.000000 talus-1.0.0rc9/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 17:16:12.000000 talus-1.0.0rc9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-22 17:16:12.000000 talus-1.0.0rc9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 17:16:31.005180 talus-1.0.0rc9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-22 17:16:12.000000 talus-1.0.0rc9/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-22 17:16:12.000000 talus-1.0.0rc9/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-22 17:16:12.000000 talus-1.0.0rc9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 17:16:31.005180 talus-1.0.0rc9/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-22 17:16:12.000000 talus-1.0.0rc9/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.009266 talus-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-28 21:03:10.000000 talus-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-28 21:03:10.000000 talus-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-28 21:03:10.000000 talus-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-28 21:03:10.000000 talus-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6242 2024-05-28 21:03:23.009266 talus-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5353 2024-05-28 21:03:10.000000 talus-1.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-05-28 21:03:10.000000 talus-1.1.0/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-05-28 21:03:10.000000 talus-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 21:03:23.009266 talus-1.1.0/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.005266 talus-1.1.0/talus/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-28 21:03:10.000000 talus-1.1.0/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-28 21:03:22.000000 talus-1.1.0/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-28 21:03:10.000000 talus-1.1.0/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-28 21:03:10.000000 talus-1.1.0/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.005266 talus-1.1.0/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2024-05-28 21:03:10.000000 talus-1.1.0/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-28 21:03:10.000000 talus-1.1.0/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.009266 talus-1.1.0/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.009266 talus-1.1.0/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-28 21:03:10.000000 talus-1.1.0/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 21:03:23.009266 talus-1.1.0/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6242 2024-05-28 21:03:22.000000 talus-1.1.0/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-28 21:03:23.000000 talus-1.1.0/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 21:03:22.000000 talus-1.1.0/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 21:03:22.000000 talus-1.1.0/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-28 21:03:22.000000 talus-1.1.0/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-28 21:03:22.000000 talus-1.1.0/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-28 21:03:10.000000 talus-1.1.0/tox.ini
```

### Comparing `talus-1.0.0rc9/.gitignore` & `talus-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/.pre-commit-config.yaml` & `talus-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/LICENSE` & `talus-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/PKG-INFO` & `talus-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc9
+Version: 1.1.0
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
-License: BSD 3-Clause
+License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pika>1.3
-Requires-Dist: tenacity>=8.0
+Requires-Dist: tenacity>=8.2
 Requires-Dist: pydantic>=2.0
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
@@ -47,83 +47,118 @@
    pip install talus
 
 Examples
 --------
 
 **Creating a consumer which listens on a queue, processes valid messages and publishes as part of processing**
 
+Uses default connection parameters and connection retryer expecting a rabbitmq server running in its default configuration.
+
 .. code:: python
 
-    from talus.consumer DurableConsumer
-    from talus.producer DurableProducer
-    from talus.models.retryer import ConnectionRetryerFactory
-    from talus.models.connection_parameters import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
-    from talus.models.processor import MessageProcessorBase
-    from talus.models.message import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
-    from talus.models.queue import Queue
-    from talus.models.exchange import Exchange
-    from talus.models.binding import Binding
+    from talus import DurableConsumer
+    from talus import DurableProducer
+    from talus import ConnectionRetryerFactory
+    from talus import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
+    from talus import MessageProcessorBase
+    from talus import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
+    from talus import Queue
+    from talus import Exchange
+    from talus import Binding
     from typing import Type
 
-    ############
-    # Consumer #
-    ############
+    ##########################
+    # Consumer Configurations#
+    ##########################
     # Configure messages that will be consumed
-    class ObjectMessageBody(MessageBodyBase):
+    class ConsumeMessageBody(MessageBodyBase):
         objectName: str
         bucket: str
 
     class ConsumeMessage(ConsumeMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody
+        message_body_cls: Type[ConsumeMessageBody] = ConsumeMessageBody
 
     # Configure the queue the messages should be consumed from
     inbound_queue = Queue(name="inbound.q")
 
-    # Configure a message processor to handle the consumed messages
-    class MessageProcessor(MessageProcessorBase):
-        def process_message(self, message: ConsumeMessage):
-            print(f"Received message: {message}")
-            outbound_message = PublishMessage(
-                body=ObjectMessageBody(objectName=message.body.objectName, bucket="newBucket"),
-            )  # change the bucket name for some reason
-            self.producer.publish(outbound_message)
-
 
-    ############
-    # Producer #
-    ############
+    ###########################
+    # Producer Configurations #
+    ###########################
     # Configure messages that will be produced
+    class ProducerMessageBody(MessageBodyBase):
+        key: str
+        code: str
+
     class PublishMessage(PublishMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody # using the same schema for simplicity
+        message_body_cls: Type[ProducerMessageBody] = ProducerMessageBody
         default_routing_key: str = "outbound.message.m"
 
-    # Configure the queue the messages should be routed to
+    # Configure the queues the message should be routed to
     outbound_queue_one = Queue(name="outbound.one.q")
     outbound_queue_two = Queue(name="outbound.two.q")
 
 
-    # Configure the exchange and queue bindings for publishing
+    # Configure the exchange and queue bindings for publishing (Publish Message -> Outbound Queues)
     publish_exchange = Exchange(name="outbound.exchange") # Direct exchange by default
     bindings = [Binding(queue=outbound_queue_one, message=PublishMessage),
                 Binding(queue=outbound_queue_two, message=PublishMessage)] # publishing PublishMessage will route to both queues.
 
+
+    ############################
+    # Processor Configurations #
+    ############################
+
+    # Configure a message processor to handle the consumed messages
+    class MessageProcessor(MessageProcessorBase):
+        def process_message(self, message: ConsumeMessage):
+            print(message)
+            outbound_message = PublishMessage(
+                body=ProducerMessageBody(
+                    key=message.body.objectName,
+                    code="newBucket",
+                    conversationId=message.body.conversationId,
+                )
+            )  # crosswalk the values from the consumed message to the produced message
+            self.producer.publish(outbound_message)
+            print(outbound_message)
+
+
     # Actually Connect and run the consumer
     def main():
+        """Starts a listener which will consume messages from the inbound queue and publish messages to the outbound queues."""
         with DurableProducer(
             queue_bindings=bindings,
             publish_exchange=publish_exchange,
             connection_parameters=ProducerConnectionParameterFactory(),
             connection_retryer=ConnectionRetryerFactory(),
         ) as producer:
             with DurableConsumer(
                 consume_queue=inbound_queue,
                 connection_parameters=ConsumerConnectionParameterFactory(),
                 connection_retryer=ConnectionRetryerFactory(),
             ) as consumer:
-                message_processor = MessageProcessor(producer=producer)
+                message_processor = MessageProcessor(message_cls=ConsumeMessage, producer=producer)
                 consumer.listen(message_processor)
 
+
     if __name__ == "__main__":
+        # First message to consume
+        class InitialMessage(PublishMessageBase):
+            message_body_cls: Type[
+                ConsumeMessageBody] = ConsumeMessageBody
+            default_routing_key: str = "inbound.message.m"
+
+        initial_message_bindings = [Binding(queue=inbound_queue, message=InitialMessage)]
+
+        with DurableProducer(
+                queue_bindings=initial_message_bindings,
+                publish_exchange=publish_exchange,
+                connection_parameters=ProducerConnectionParameterFactory(),
+                connection_retryer=ConnectionRetryerFactory(),
+        ) as producer:
+            producer.publish(InitialMessage(body={"objectName": "object", "bucket": "bucket"}))
+        # Consume the message and process it
         main()
 
 .. |codecov| image:: https://codecov.io/bb/dkistdc/interservice-bus-adapter/branch/master/graph/badge.svg
    :target: https://codecov.io/bb/dkistdc/interservice-bus-adapter
```

### Comparing `talus-1.0.0rc9/README.rst` & `talus-1.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -24,83 +24,118 @@
    pip install talus
 
 Examples
 --------
 
 **Creating a consumer which listens on a queue, processes valid messages and publishes as part of processing**
 
+Uses default connection parameters and connection retryer expecting a rabbitmq server running in its default configuration.
+
 .. code:: python
 
-    from talus.consumer DurableConsumer
-    from talus.producer DurableProducer
-    from talus.models.retryer import ConnectionRetryerFactory
-    from talus.models.connection_parameters import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
-    from talus.models.processor import MessageProcessorBase
-    from talus.models.message import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
-    from talus.models.queue import Queue
-    from talus.models.exchange import Exchange
-    from talus.models.binding import Binding
+    from talus import DurableConsumer
+    from talus import DurableProducer
+    from talus import ConnectionRetryerFactory
+    from talus import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
+    from talus import MessageProcessorBase
+    from talus import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
+    from talus import Queue
+    from talus import Exchange
+    from talus import Binding
     from typing import Type
 
-    ############
-    # Consumer #
-    ############
+    ##########################
+    # Consumer Configurations#
+    ##########################
     # Configure messages that will be consumed
-    class ObjectMessageBody(MessageBodyBase):
+    class ConsumeMessageBody(MessageBodyBase):
         objectName: str
         bucket: str
 
     class ConsumeMessage(ConsumeMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody
+        message_body_cls: Type[ConsumeMessageBody] = ConsumeMessageBody
 
     # Configure the queue the messages should be consumed from
     inbound_queue = Queue(name="inbound.q")
 
-    # Configure a message processor to handle the consumed messages
-    class MessageProcessor(MessageProcessorBase):
-        def process_message(self, message: ConsumeMessage):
-            print(f"Received message: {message}")
-            outbound_message = PublishMessage(
-                body=ObjectMessageBody(objectName=message.body.objectName, bucket="newBucket"),
-            )  # change the bucket name for some reason
-            self.producer.publish(outbound_message)
-
 
-    ############
-    # Producer #
-    ############
+    ###########################
+    # Producer Configurations #
+    ###########################
     # Configure messages that will be produced
+    class ProducerMessageBody(MessageBodyBase):
+        key: str
+        code: str
+
     class PublishMessage(PublishMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody # using the same schema for simplicity
+        message_body_cls: Type[ProducerMessageBody] = ProducerMessageBody
         default_routing_key: str = "outbound.message.m"
 
-    # Configure the queue the messages should be routed to
+    # Configure the queues the message should be routed to
     outbound_queue_one = Queue(name="outbound.one.q")
     outbound_queue_two = Queue(name="outbound.two.q")
 
 
-    # Configure the exchange and queue bindings for publishing
+    # Configure the exchange and queue bindings for publishing (Publish Message -> Outbound Queues)
     publish_exchange = Exchange(name="outbound.exchange") # Direct exchange by default
     bindings = [Binding(queue=outbound_queue_one, message=PublishMessage),
                 Binding(queue=outbound_queue_two, message=PublishMessage)] # publishing PublishMessage will route to both queues.
 
+
+    ############################
+    # Processor Configurations #
+    ############################
+
+    # Configure a message processor to handle the consumed messages
+    class MessageProcessor(MessageProcessorBase):
+        def process_message(self, message: ConsumeMessage):
+            print(message)
+            outbound_message = PublishMessage(
+                body=ProducerMessageBody(
+                    key=message.body.objectName,
+                    code="newBucket",
+                    conversationId=message.body.conversationId,
+                )
+            )  # crosswalk the values from the consumed message to the produced message
+            self.producer.publish(outbound_message)
+            print(outbound_message)
+
+
     # Actually Connect and run the consumer
     def main():
+        """Starts a listener which will consume messages from the inbound queue and publish messages to the outbound queues."""
         with DurableProducer(
             queue_bindings=bindings,
             publish_exchange=publish_exchange,
             connection_parameters=ProducerConnectionParameterFactory(),
             connection_retryer=ConnectionRetryerFactory(),
         ) as producer:
             with DurableConsumer(
                 consume_queue=inbound_queue,
                 connection_parameters=ConsumerConnectionParameterFactory(),
                 connection_retryer=ConnectionRetryerFactory(),
             ) as consumer:
-                message_processor = MessageProcessor(producer=producer)
+                message_processor = MessageProcessor(message_cls=ConsumeMessage, producer=producer)
                 consumer.listen(message_processor)
 
+
     if __name__ == "__main__":
+        # First message to consume
+        class InitialMessage(PublishMessageBase):
+            message_body_cls: Type[
+                ConsumeMessageBody] = ConsumeMessageBody
+            default_routing_key: str = "inbound.message.m"
+
+        initial_message_bindings = [Binding(queue=inbound_queue, message=InitialMessage)]
+
+        with DurableProducer(
+                queue_bindings=initial_message_bindings,
+                publish_exchange=publish_exchange,
+                connection_parameters=ProducerConnectionParameterFactory(),
+                connection_retryer=ConnectionRetryerFactory(),
+        ) as producer:
+            producer.publish(InitialMessage(body={"objectName": "object", "bucket": "bucket"}))
+        # Consume the message and process it
         main()
 
 .. |codecov| image:: https://codecov.io/bb/dkistdc/interservice-bus-adapter/branch/master/graph/badge.svg
    :target: https://codecov.io/bb/dkistdc/interservice-bus-adapter
```

### Comparing `talus-1.0.0rc9/bitbucket-pipelines.yml` & `talus-1.1.0/bitbucket-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -44,14 +44,17 @@
           - pip install .
           - pip freeze | grep -v @ > requirements.txt
           - cat requirements.txt
           - echo $SNYK_VERSION
           - curl -L -o snyk https://github.com/snyk/snyk/releases/download/$SNYK_VERSION/snyk-linux
           - chmod 755 snyk
           - ./snyk -d auth $SNYK_TOKEN
+          - echo $SNYK_IGNORE
+          - for id in $SNYK_IGNORE; do echo Ignoring $id; ./snyk ignore $id; done
+          - cat .snyk || echo "No .snyk found. Probably because there was nothing to ignore."
           - echo $SNYK_CLI_COMMAND
           - $SNYK_CLI_COMMAND
     - step: &publish
         caches:
           - pip
         name: Publish
         script:
```

### Comparing `talus-1.0.0rc9/pyproject.toml` & `talus-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
 ]
-license = { text = "BSD 3-Clause" }
+license = { text = "MIT" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
 
 dependencies = [
     "pika>1.3",
-    "tenacity>=8.0",
+    "tenacity>=8.2",
     "pydantic>=2.0",
 ]
 dynamic = ["version"]
 
 # tox is not required to run the tests, but simplifies IDE integration
 # Pygments is solely to support README.rst rendering
 [project.optional-dependencies]
```

### Comparing `talus-1.0.0rc9/talus/base.py` & `talus-1.1.0/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/consumer.py` & `talus-1.1.0/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/binding.py` & `talus-1.1.0/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/connection_parameters.py` & `talus-1.1.0/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/exchange.py` & `talus-1.1.0/talus/models/exchange.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/message.py` & `talus-1.1.0/talus/models/message.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/processor.py` & `talus-1.1.0/talus/models/processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/models/retryer.py` & `talus-1.1.0/talus/models/retryer.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,57 +12,62 @@
 from pika.exceptions import ConnectionWrongStateError
 from pika.exceptions import InvalidChannelNumber
 from pika.exceptions import NoFreeChannels
 from pika.exceptions import StreamLostError
 from pika.exceptions import UnexpectedFrameError
 from pydantic import BaseModel
 from tenacity import after_log
+from tenacity import before_log
 from tenacity import retry_if_exception_type
 from tenacity import Retrying
 from tenacity import stop_after_attempt
-from tenacity import wait_exponential
-from tenacity import wait_random
+from tenacity import stop_never
+from tenacity import wait_exponential_jitter
 
 logger = logging.getLogger(__name__)
 
 
 class RetryerFactory(BaseModel):
     """
     Translator for the retry configuration to a tenacity.Retrying object.
 
     >>> from talus.models.retryer import RetryerFactory
     >>> factory = RetryerFactory()
     >>> retryer = factory()
     """
 
-    delay_min: int = 1
-    delay_max: int = 300
-    jitter_min: int = 1
-    jitter_max: int = 10
+    delay_min: float = 1.0
+    delay_max: float = 300.0
+    backoff: float = 2.0
+    jitter_min: float = 0
+    jitter_max: float = 10.0
     attempts: int = -1  # -1 means retry forever
     exceptions: type[Exception] | tuple[type[Exception], ...] = type(
         Exception
     )  # retry any exception
 
     def __call__(self) -> Retrying:
         """
         Returns a tenacity.Retrying object based on the configuration.
         """
-        wait = wait_exponential(
-            multiplier=self.delay_min,
-            min=self.delay_min,
+        wait = wait_exponential_jitter(
+            initial=self.delay_min,
             max=self.delay_max,
-        ) + wait_random(self.jitter_min, self.jitter_max)
-        stop = None
+            exp_base=self.backoff,
+            jitter=self.jitter_max,
+        )
+
+        stop = stop_never
         if self.attempts > -1:
             stop = stop_after_attempt(self.attempts)
         return Retrying(
             retry=retry_if_exception_type(self.exceptions),
             wait=wait,
             stop=stop,
+            before=before_log(logger=logger, log_level=logging.INFO),
             after=after_log(logger=logger, log_level=logging.INFO),
         )
 
 
 DEFAULT_CONNECTION_EXCEPTIONS = (
     ConnectionOpenAborted,
     StreamLostError,
```

### Comparing `talus-1.0.0rc9/talus/producer.py` & `talus-1.1.0/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/conftest.py` & `talus-1.1.0/talus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/models/test_binding.py` & `talus-1.1.0/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/models/test_message.py` & `talus-1.1.0/talus/tests/models/test_message.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/models/test_processor.py` & `talus-1.1.0/talus/tests/models/test_processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/models/test_queue.py` & `talus-1.1.0/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/models/test_retryer.py` & `talus-1.1.0/talus/tests/models/test_retryer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     """
     # given
     factory = RetryerFactory()
     # when
     retryer = factory()
     # then
     assert isinstance(retryer, Retrying)
-    assert retryer.stop is None
 
 
 def test_retryer_with_attempts():
     """
     :given: A retryer factory with attempts > 1
     :when: The factory is called
     :then: A Retryer object is returned with a stop_after_attempt object
```

### Comparing `talus-1.0.0rc9/talus/tests/test_base.py` & `talus-1.1.0/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/test_consumer.py` & `talus-1.1.0/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus/tests/test_producer.py` & `talus-1.1.0/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/talus.egg-info/PKG-INFO` & `talus-1.1.0/talus.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc9
+Version: 1.1.0
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
-License: BSD 3-Clause
+License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pika>1.3
-Requires-Dist: tenacity>=8.0
+Requires-Dist: tenacity>=8.2
 Requires-Dist: pydantic>=2.0
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
@@ -47,83 +47,118 @@
    pip install talus
 
 Examples
 --------
 
 **Creating a consumer which listens on a queue, processes valid messages and publishes as part of processing**
 
+Uses default connection parameters and connection retryer expecting a rabbitmq server running in its default configuration.
+
 .. code:: python
 
-    from talus.consumer DurableConsumer
-    from talus.producer DurableProducer
-    from talus.models.retryer import ConnectionRetryerFactory
-    from talus.models.connection_parameters import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
-    from talus.models.processor import MessageProcessorBase
-    from talus.models.message import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
-    from talus.models.queue import Queue
-    from talus.models.exchange import Exchange
-    from talus.models.binding import Binding
+    from talus import DurableConsumer
+    from talus import DurableProducer
+    from talus import ConnectionRetryerFactory
+    from talus import ConsumerConnectionParameterFactory, ProducerConnectionParameterFactory
+    from talus import MessageProcessorBase
+    from talus import ConsumeMessageBase, PublishMessageBase, MessageBodyBase
+    from talus import Queue
+    from talus import Exchange
+    from talus import Binding
     from typing import Type
 
-    ############
-    # Consumer #
-    ############
+    ##########################
+    # Consumer Configurations#
+    ##########################
     # Configure messages that will be consumed
-    class ObjectMessageBody(MessageBodyBase):
+    class ConsumeMessageBody(MessageBodyBase):
         objectName: str
         bucket: str
 
     class ConsumeMessage(ConsumeMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody
+        message_body_cls: Type[ConsumeMessageBody] = ConsumeMessageBody
 
     # Configure the queue the messages should be consumed from
     inbound_queue = Queue(name="inbound.q")
 
-    # Configure a message processor to handle the consumed messages
-    class MessageProcessor(MessageProcessorBase):
-        def process_message(self, message: ConsumeMessage):
-            print(f"Received message: {message}")
-            outbound_message = PublishMessage(
-                body=ObjectMessageBody(objectName=message.body.objectName, bucket="newBucket"),
-            )  # change the bucket name for some reason
-            self.producer.publish(outbound_message)
-
 
-    ############
-    # Producer #
-    ############
+    ###########################
+    # Producer Configurations #
+    ###########################
     # Configure messages that will be produced
+    class ProducerMessageBody(MessageBodyBase):
+        key: str
+        code: str
+
     class PublishMessage(PublishMessageBase):
-        message_body_cls: Type[ObjectMessageBody] = ObjectMessageBody # using the same schema for simplicity
+        message_body_cls: Type[ProducerMessageBody] = ProducerMessageBody
         default_routing_key: str = "outbound.message.m"
 
-    # Configure the queue the messages should be routed to
+    # Configure the queues the message should be routed to
     outbound_queue_one = Queue(name="outbound.one.q")
     outbound_queue_two = Queue(name="outbound.two.q")
 
 
-    # Configure the exchange and queue bindings for publishing
+    # Configure the exchange and queue bindings for publishing (Publish Message -> Outbound Queues)
     publish_exchange = Exchange(name="outbound.exchange") # Direct exchange by default
     bindings = [Binding(queue=outbound_queue_one, message=PublishMessage),
                 Binding(queue=outbound_queue_two, message=PublishMessage)] # publishing PublishMessage will route to both queues.
 
+
+    ############################
+    # Processor Configurations #
+    ############################
+
+    # Configure a message processor to handle the consumed messages
+    class MessageProcessor(MessageProcessorBase):
+        def process_message(self, message: ConsumeMessage):
+            print(message)
+            outbound_message = PublishMessage(
+                body=ProducerMessageBody(
+                    key=message.body.objectName,
+                    code="newBucket",
+                    conversationId=message.body.conversationId,
+                )
+            )  # crosswalk the values from the consumed message to the produced message
+            self.producer.publish(outbound_message)
+            print(outbound_message)
+
+
     # Actually Connect and run the consumer
     def main():
+        """Starts a listener which will consume messages from the inbound queue and publish messages to the outbound queues."""
         with DurableProducer(
             queue_bindings=bindings,
             publish_exchange=publish_exchange,
             connection_parameters=ProducerConnectionParameterFactory(),
             connection_retryer=ConnectionRetryerFactory(),
         ) as producer:
             with DurableConsumer(
                 consume_queue=inbound_queue,
                 connection_parameters=ConsumerConnectionParameterFactory(),
                 connection_retryer=ConnectionRetryerFactory(),
             ) as consumer:
-                message_processor = MessageProcessor(producer=producer)
+                message_processor = MessageProcessor(message_cls=ConsumeMessage, producer=producer)
                 consumer.listen(message_processor)
 
+
     if __name__ == "__main__":
+        # First message to consume
+        class InitialMessage(PublishMessageBase):
+            message_body_cls: Type[
+                ConsumeMessageBody] = ConsumeMessageBody
+            default_routing_key: str = "inbound.message.m"
+
+        initial_message_bindings = [Binding(queue=inbound_queue, message=InitialMessage)]
+
+        with DurableProducer(
+                queue_bindings=initial_message_bindings,
+                publish_exchange=publish_exchange,
+                connection_parameters=ProducerConnectionParameterFactory(),
+                connection_retryer=ConnectionRetryerFactory(),
+        ) as producer:
+            producer.publish(InitialMessage(body={"objectName": "object", "bucket": "bucket"}))
+        # Consume the message and process it
         main()
 
 .. |codecov| image:: https://codecov.io/bb/dkistdc/interservice-bus-adapter/branch/master/graph/badge.svg
    :target: https://codecov.io/bb/dkistdc/interservice-bus-adapter
```

### Comparing `talus-1.0.0rc9/talus.egg-info/SOURCES.txt` & `talus-1.1.0/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc9/tox.ini` & `talus-1.1.0/tox.ini`

 * *Files identical despite different names*

