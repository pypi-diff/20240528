# Comparing `tmp/autogencap_rajan_jedi-0.0.8.tar.gz` & `tmp/autogencap_rajan_jedi-0.0.9.tar.gz`

## Comparing `autogencap_rajan_jedi-0.0.8.tar` & `autogencap_rajan_jedi-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Actor.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ActorConnector.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Broker.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Config.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/Constants.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/DebugLog.py
--rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/DirectorySvc.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/LocalActorNetwork.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/requirements.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/setup.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/utility.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AG2CAP.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AGActor.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AutoGenConnector.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAP2AG.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChat.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChatManager.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPPair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/agent.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen.proto
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.pyi
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP.proto
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/proto-instructions.txt
--rwxr-xr-x   0        0        0 11783121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/protoc.exe
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/autogencap/proto/test.seqdiag
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/README.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/Actor.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ActorConnector.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/Broker.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ComponentEnsemble.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/Config.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/Constants.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/DebugLog.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/DirectorySvc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/requirements.txt
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/setup.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/utility.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/AG2CAP.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/AGActor.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/AutoGenConnector.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAP2AG.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAPGroupChat.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAPGroupChatManager.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAPPair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/agent.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen.proto
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen_pb2.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen_pb2.pyi
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP.proto
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP_pb2.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP_pb2.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/proto-instructions.txt
+-rwxr-xr-x   0        0        0 11783121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/protoc.exe
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/autogencap/proto/test.seqdiag
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/README.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.9/PKG-INFO
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/Actor.py` & `autogencap_rajan_jedi-0.0.9/autogencap/Actor.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 class Actor:
     def __init__(self, agent_name: str, description: str):
         self.actor_name: str = agent_name
         self.agent_description: str = description
         self.run = False
         self._start_event = threading.Event()
 
-    def connect_network(self, network):
+    def on_connect(self, network):
         Debug(self.actor_name, f"is connecting to {network}")
         Debug(self.actor_name, "connected")
 
-    def _process_txt_msg(self, msg: str, msg_type: str, topic: str, sender: str) -> bool:
+    def on_txt_msg(self, msg: str, msg_type: str, receiver: str, sender: str) -> bool:
         Info(self.actor_name, f"InBox: {msg}")
         return True
 
-    def _process_bin_msg(self, msg: bytes, msg_type: str, topic: str, sender: str) -> bool:
-        Info(self.actor_name, f"Msg: topic=[{topic}], msg_type=[{msg_type}]")
+    def on_bin_msg(self, msg: bytes, msg_type: str, receiver: str, sender: str) -> bool:
+        Info(self.actor_name, f"Msg: receiver=[{receiver}], msg_type=[{msg_type}]")
         return True
 
     def _recv_thread(self):
         try:
             Debug(self.actor_name, "recv thread started")
             self._socket: zmq.Socket = self._context.socket(zmq.SUB)
             self._socket.setsockopt(zmq.RCVTIMEO, 500)
@@ -47,20 +47,20 @@
                     continue  # No message received, continue to next iteration
                 except Exception as e:
                     Error(self.actor_name, f"recv thread encountered an error: {e}")
                     traceback.print_exc()
                     continue
                 if msg_type == "text":
                     msg = msg.decode("utf-8")  # Convert bytes to string
-                    if not self._process_txt_msg(msg, msg_type, topic, sender_topic):
+                    if not self.on_txt_msg(msg, msg_type, topic, sender_topic):
                         msg = "quit"
                     if msg.lower() == "quit":
                         break
                 else:
-                    if not self._process_bin_msg(msg, msg_type, topic, sender_topic):
+                    if not self.on_bin_msg(msg, msg_type, topic, sender_topic):
                         break
         except Exception as e:
             Debug(self.actor_name, f"recv thread encountered an error: {e}")
             traceback.print_exc()
         finally:
             self.run = False
             # In case there was an exception at startup signal
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ActorConnector.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ActorConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     def send_txt_msg(self, msg):
         self._sender.send_txt_msg(msg)
 
     def send_bin_msg(self, msg_type: str, msg):
         self._sender.send_bin_msg(msg_type, msg)
 
-    def binary_request(self, msg_type: str, msg, num_attempts=5):
+    def send_recv_msg(self, msg_type: str, msg, num_attempts=5):
         original_timeout: int = 0
         if num_attempts == -1:
             original_timeout = self._resp_socket.getsockopt(zmq.RCVTIMEO)
             self._resp_socket.setsockopt(zmq.RCVTIMEO, 1000)
 
         try:
             self._sender.send_bin_request_msg(msg_type, msg, self._resp_topic)
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/Broker.py` & `autogencap_rajan_jedi-0.0.9/autogencap/Broker.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/DebugLog.py` & `autogencap_rajan_jedi-0.0.9/autogencap/DebugLog.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/DirectorySvc.py` & `autogencap_rajan_jedi-0.0.9/autogencap/DirectorySvc.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,33 +31,33 @@
 
 class DirectoryActor(Actor):
     def __init__(self, topic: str, name: str):
         super().__init__(topic, name)
         self._registered_actors = {}
         self._network_prefix = ""
 
-    def _process_bin_msg(self, msg: bytes, msg_type: str, topic: str, sender: str) -> bool:
+    def on_bin_msg(self, msg: bytes, msg_type: str, topic: str, sender: str) -> bool:
         if msg_type == ActorRegistration.__name__:
-            self._actor_registration_msg_handler(topic, msg_type, msg, sender)
+            self._on_actor_registration_msg(topic, msg_type, msg, sender)
         elif msg_type == ActorLookup.__name__:
-            self._actor_lookup_msg_handler(topic, msg_type, msg, sender)
+            self._on_actor_lookup_msg(topic, msg_type, msg, sender)
         elif msg_type == Ping.__name__:
-            self._ping_msg_handler(topic, msg_type, msg, sender)
+            self._on_ping_msg(topic, msg_type, msg, sender)
         else:
             Error("DirectorySvc", f"Unknown message type: {msg_type}")
         return True
 
-    def _ping_msg_handler(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
+    def _on_ping_msg(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
         Info("DirectorySvc", f"Ping received: {sender_topic}")
         pong = Pong()
         serialized_msg = pong.SerializeToString()
         sender_connection = ActorSender(self._context, sender_topic)
         sender_connection.send_bin_msg(Pong.__name__, serialized_msg)
 
-    def _actor_registration_msg_handler(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
+    def _on_actor_registration_msg(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
         actor_reg = ActorRegistration()
         actor_reg.ParseFromString(msg)
         Info("DirectorySvc", f"Actor registration: {actor_reg.actor_info.name}")
         name = actor_reg.actor_info.name
         # TODO (Future DirectorySv PR) network_id should be namespace prefixed to support multiple networks
         actor_reg.actor_info.name + self._network_prefix
         err = ErrorMsg()
@@ -67,15 +67,15 @@
         else:
             self._registered_actors[name] = actor_reg.actor_info
 
         sender_connection = ActorSender(self._context, sender_topic)
         serialized_msg = err.SerializeToString()
         sender_connection.send_bin_msg(ErrorMsg.__name__, serialized_msg)
 
-    def _actor_lookup_msg_handler(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
+    def _on_actor_lookup_msg(self, topic: str, msg_type: str, msg: bytes, sender_topic: str):
         actor_lookup = ActorLookup()
         actor_lookup.ParseFromString(msg)
         Debug("DirectorySvc", f"Actor lookup: {actor_lookup.actor_info.name}")
         actor_lookup_resp = ActorLookupResponse()
         actor_lookup_resp.found = False
         try:
             pattern = re.compile(actor_lookup.actor_info.name)
@@ -107,15 +107,15 @@
         self._directory_connector: ActorConnector = None
         self._directory_actor: DirectoryActor = None
 
     def _no_other_directory(self) -> bool:
         Debug("DirectorySvc", "Pinging existing DirectorySvc")
         ping = Ping()
         serialized_msg = ping.SerializeToString()
-        _, _, resp = self._directory_connector.binary_request(Ping.__name__, serialized_msg, num_attempts=1)
+        _, _, resp = self._directory_connector.send_recv_msg(Ping.__name__, serialized_msg, num_attempts=1)
         if resp is None:
             return True
         return False
 
     def start(self):
         Debug("DirectorySvc", "Starting.")
         self._directory_connector = ActorConnector(self._context, Directory_Svc_Topic)
@@ -134,26 +134,26 @@
 
     def register_actor(self, actor_info: ActorInfo):
         # Send a message to the directory service
         # to register the actor
         actor_reg = ActorRegistration()
         actor_reg.actor_info.CopyFrom(actor_info)
         serialized_msg = actor_reg.SerializeToString()
-        _, _, resp = self._directory_connector.binary_request(ActorRegistration.__name__, serialized_msg)
+        _, _, resp = self._directory_connector.send_recv_msg(ActorRegistration.__name__, serialized_msg)
         report_error_msg(resp, "DirectorySvc")
 
     def register_actor_by_name(self, actor_name: str):
         actor_info = ActorInfo(name=actor_name)
         self.register_actor(actor_info)
 
     def _lookup_actors_by_name(self, name_regex: str):
         actor_info = ActorInfo(name=name_regex)
         actor_lookup = ActorLookup(actor_info=actor_info)
         serialized_msg = actor_lookup.SerializeToString()
-        _, _, resp = self._directory_connector.binary_request(ActorLookup.__name__, serialized_msg)
+        _, _, resp = self._directory_connector.send_recv_msg(ActorLookup.__name__, serialized_msg)
         actor_lookup_resp = ActorLookupResponse()
         actor_lookup_resp.ParseFromString(resp)
         return actor_lookup_resp
 
     def lookup_actor_by_name(self, actor_name: str) -> ActorInfo:
         actor_lookup_resp = self._lookup_actors_by_name(actor_name)
         if actor_lookup_resp.found:
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/LocalActorNetwork.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ComponentEnsemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .DebugLog import Debug, Warn
 from .DirectorySvc import DirectorySvc
 from .proto.CAP_pb2 import ActorInfo, ActorInfoCollection
 
 # TODO: remove time import
 
 
-class LocalActorNetwork:
+class ComponentEnsemble:
     def __init__(self, name: str = "Local Actor Network", start_broker: bool = True):
         self.local_actors = {}
         self.name: str = name
         self._context: zmq.Context = zmq.Context()
         self._start_broker: bool = start_broker
         self._broker: Broker = None
         self._directory_svc: DirectorySvc = None
@@ -45,40 +45,40 @@
         self.local_actors[actor.actor_name] = actor
         actor.start(self._context)
         Debug("Local_Actor_Network", f"{actor.actor_name} registered in the network.")
 
     def connect(self):
         self._init_runtime()
         for actor in self.local_actors.values():
-            actor.connect_network(self)
+            actor.on_connect(self)
 
     def disconnect(self):
         for actor in self.local_actors.values():
             actor.disconnect_network(self)
         if self._directory_svc:
             self._directory_svc.stop()
         if self._broker:
             self._broker.stop()
 
-    def actor_connector_by_topic(self, topic: str) -> ActorConnector:
+    def find_by_topic(self, topic: str) -> ActorConnector:
         return ActorConnector(self._context, topic)
 
-    def lookup_actor(self, name: str) -> ActorConnector:
+    def find_by_name(self, name: str) -> ActorConnector:
         actor_info: ActorInfo = self._directory_svc.lookup_actor_by_name(name)
         if actor_info is None:
             Warn("Local_Actor_Network", f"{name}, not found in the network.")
             return None
         Debug("Local_Actor_Network", f"[{name}] found in the network.")
-        return self.actor_connector_by_topic(name)
+        return self.find_by_topic(name)
 
-    def lookup_termination(self) -> ActorConnector:
+    def find_termination(self) -> ActorConnector:
         termination_topic: str = Termination_Topic
-        return self.actor_connector_by_topic(termination_topic)
+        return self.find_by_topic(termination_topic)
 
-    def lookup_actor_info(self, name_regex) -> List[ActorInfo]:
+    def find_by_name_regex(self, name_regex) -> List[ActorInfo]:
         actor_info: ActorInfoCollection = self._directory_svc.lookup_actor_info_by_name(name_regex)
         if actor_info is None:
             Warn("Local_Actor_Network", f"{name_regex}, not found in the network.")
             return None
         Debug("Local_Actor_Network", f"[{name_regex}] found in the network.")
         actor_list = []
         for actor in actor_info.info_coll:
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/test.py` & `autogencap_rajan_jedi-0.0.9/autogencap/test.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AG2CAP.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/AG2CAP.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import time
 from typing import Callable, Dict, List, Optional, Union
 
 from autogen import Agent, ConversableAgent
 
-from ..LocalActorNetwork import LocalActorNetwork
+from ..ComponentEnsemble import ComponentEnsemble
 from .AutoGenConnector import AutoGenConnector
 
 
 class AG2CAP(ConversableAgent):
     """
     A conversable agent proxy that sends messages to CAN when called
     """
 
     def __init__(
         self,
-        network: LocalActorNetwork,
+        ensemble: ComponentEnsemble,
         agent_name: str,
         agent_description: Optional[str] = None,
     ):
         super().__init__(name=agent_name, description=agent_description, llm_config=False)
         self._agent_connector: AutoGenConnector = None
-        self._network: LocalActorNetwork = network
+        self._ensemble: ComponentEnsemble = ensemble
         self._recv_called = False
 
     def reset_receive_called(self):
         self._recv_called = False
 
     def was_receive_called(self):
         return self._recv_called
@@ -34,16 +34,16 @@
         Set the name of the agent.
         Why? because we need it to look like different agents
         """
         self._name = name
 
     def _check_connection(self):
         if self._agent_connector is None:
-            self._agent_connector = AutoGenConnector(self._network.lookup_actor(self.name))
-            self._terminate_connector = AutoGenConnector(self._network.lookup_termination())
+            self._agent_connector = AutoGenConnector(self._ensemble.find_by_name(self.name))
+            self._terminate_connector = AutoGenConnector(self._ensemble.find_termination())
 
     def receive(
         self,
         message: Union[Dict, str],
         sender: Agent,
         request_reply: Optional[bool] = None,
         silent: Optional[bool] = False,
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/AutoGenConnector.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/AutoGenConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Send a GenReplyReq message to CAP and receive the response.
         """
         msg = GenReplyReq()
         serialized_msg = msg.SerializeToString()
         # Setting retry to -1 to keep trying until a response is received
         # This normal AutoGen behavior but does not handle the case when an AutoGen agent
         # is not running. In that case, the connector will keep trying indefinitely.
-        _, _, resp = self._can_channel.binary_request(type(msg).__name__, serialized_msg, num_attempts=-1)
+        _, _, resp = self._can_channel.send_recv_msg(type(msg).__name__, serialized_msg, num_attempts=-1)
         gen_reply_resp = GenReplyResp()
         gen_reply_resp.ParseFromString(resp)
         return gen_reply_resp.data
 
     def send_receive_req(
         self,
         message: Union[Dict, str],
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAP2AG.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAP2AG.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from enum import Enum
 from typing import Optional
 
 from autogen import ConversableAgent
 
 from ..DebugLog import Debug, Error, Info, Warn, shorten
-from ..LocalActorNetwork import LocalActorNetwork
+from ..ComponentEnsemble import ComponentEnsemble
 from ..proto.Autogen_pb2 import GenReplyReq, GenReplyResp, PrepChat, ReceiveReq, Terminate
 from .AG2CAP import AG2CAP
 from .AGActor import AGActor
 
 
 class CAP2AG(AGActor):
     """
@@ -23,34 +23,34 @@
         self._the_ag_agent: ConversableAgent = ag_agent
         self._ag2can_other_agent: AG2CAP = None
         self._other_agent_name: str = the_other_name
         self._init_chat: bool = init_chat
         self.STATE = self.States.INIT
         self._can2ag_name: str = self.actor_name + ".can2ag"
         self._self_recursive: bool = self_recursive
-        self._network: LocalActorNetwork = None
+        self._ensemble: ComponentEnsemble = None
         self._connectors = {}
 
-    def connect_network(self, network: LocalActorNetwork):
+    def on_connect(self, ensemble: ComponentEnsemble):
         """
         Connect to the AutoGen system.
         """
-        self._network = network
-        self._ag2can_other_agent = AG2CAP(self._network, self._other_agent_name)
-        Debug(self._can2ag_name, "connected to {network}")
+        self._ensemble = ensemble
+        self._ag2can_other_agent = AG2CAP(self._ensemble, self._other_agent_name)
+        Debug(self._can2ag_name, "connected to {ensemble}")
 
-    def disconnect_network(self, network: LocalActorNetwork):
+    def disconnect_network(self, ensemble: ComponentEnsemble):
         """
         Disconnect from the AutoGen system.
         """
-        super().disconnect_network(network)
+        super().disconnect_network(ensemble)
         #        self._the_other.close()
         Debug(self.actor_name, "disconnected")
 
-    def _process_txt_msg(self, msg: str, msg_type: str, topic: str, sender: str):
+    def on_txt_msg(self, msg: str, msg_type: str, topic: str, sender: str):
         """
         Process a text message received from the AutoGen system.
         """
         Info(self._can2ag_name, f"proc_txt_msg: [{topic}], [{msg_type}], {shorten(msg)}")
         if self.STATE == self.States.INIT:
             self.STATE = self.States.CONVERSING
             if self._init_chat:
@@ -79,15 +79,15 @@
                 value = json.loads(json_value)
                 data[key] = value
         else:
             data = receive_params.data
         self._the_ag_agent.receive(data, self._ag2can_other_agent, request_reply, silent)
         self._ag2can_other_agent.set_name(save_name)
 
-    def receive_msgproc(self, msg: bytes):
+    def on_receive_msg(self, msg: bytes):
         """
         Process a ReceiveReq message received from the AutoGen system.
         """
         receive_params = ReceiveReq()
         receive_params.ParseFromString(msg)
 
         self._ag2can_other_agent.reset_receive_called()
@@ -113,19 +113,19 @@
     def get_actor_connector(self, topic: str):
         """
         Get the actor connector for the given topic.
         """
         if topic in self._connectors:
             return self._connectors[topic]
         else:
-            connector = self._network.actor_connector_by_topic(topic)
+            connector = self._ensemble.find_by_topic(topic)
             self._connectors[topic] = connector
             return connector
 
-    def generate_reply_msgproc(self, msg: GenReplyReq, sender_topic: str):
+    def on_generate_reply_msg(self, msg: GenReplyReq, sender_topic: str):
         """
         Process a GenReplyReq message received from the AutoGen system and generate a reply.
         """
         generate_reply_params = GenReplyReq()
         generate_reply_params.ParseFromString(msg)
         reply = self._the_ag_agent.generate_reply(sender=self._ag2can_other_agent)
         connector = self.get_actor_connector(sender_topic)
@@ -133,30 +133,30 @@
         reply_msg = GenReplyResp()
         if reply:
             reply_msg.data = reply.encode("utf8")
         serialized_msg = reply_msg.SerializeToString()
         connector.send_bin_msg(type(reply_msg).__name__, serialized_msg)
         return True
 
-    def prepchat_msgproc(self, msg, sender_topic):
+    def on_prepchat_msg(self, msg, sender_topic):
         prep_chat = PrepChat()
         prep_chat.ParseFromString(msg)
         self._the_ag_agent._prepare_chat(self._ag2can_other_agent, prep_chat.clear_history, prep_chat.prepare_recipient)
         return True
 
-    def _process_bin_msg(self, msg: bytes, msg_type: str, topic: str, sender: str):
+    def on_bin_msg(self, msg: bytes, msg_type: str, topic: str, sender: str):
         """
         Process a binary message received from the AutoGen system.
         """
         Info(self._can2ag_name, f"proc_bin_msg: topic=[{topic}], msg_type=[{msg_type}]")
         if msg_type == ReceiveReq.__name__:
-            return self.receive_msgproc(msg)
+            return self.on_receive_msg(msg)
         elif msg_type == GenReplyReq.__name__:
-            return self.generate_reply_msgproc(msg, sender)
+            return self.on_generate_reply_msg(msg, sender)
         elif msg_type == PrepChat.__name__:
-            return self.prepchat_msgproc(msg, sender)
+            return self.on_prepchat_msg(msg, sender)
         elif msg_type == Terminate.__name__:
             Warn(self._can2ag_name, f"TERMINATE received: topic=[{topic}], msg_type=[{msg_type}]")
             return False
         else:
             Error(self._can2ag_name, f"Unhandled message type: topic=[{topic}], msg_type=[{msg_type}]")
         return True
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPGroupChat.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAPGroupChat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import List
 
 from autogen import Agent, AssistantAgent, GroupChat
 from autogencap.ag_adapter.AG2CAP import AG2CAP
 from autogencap.ag_adapter.CAP2AG import CAP2AG
-from autogencap.LocalActorNetwork import LocalActorNetwork
+from autogencap.ComponentEnsemble import ComponentEnsemble
 
 
 class CAPGroupChat(GroupChat):
     def __init__(
         self,
         agents: List[AssistantAgent],
         messages: List[str],
         max_round: int,
         chat_initiator: str,
-        network: LocalActorNetwork,
+        ensemble: ComponentEnsemble,
     ):
         self.chat_initiator: str = chat_initiator
-        self._cap_network: LocalActorNetwork = network
+        self._cap_network: ComponentEnsemble = ensemble
         self._cap_proxies: List[CAP2AG] = []
         self._ag_proxies: List[AG2CAP] = []
         self._ag_agents: List[Agent] = agents
         self._init_cap_proxies()
         self._init_ag_proxies()
         super().__init__(agents=self._ag_proxies, messages=messages, max_round=max_round)
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/CAPPair.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/CAPPair.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,12 @@
             self_recursive=True,
         )
         self._network.register(self._first_adptr)
         self._network.register(self._second_adptr)
         self._network.connect()
 
         # Send a message to the user_proxy
-        agent_connection = self._network.lookup_actor(self._first_ag_agent.name)
+        agent_connection = self._network.find_by_name(self._first_ag_agent.name)
         agent_connection.send_txt_msg(message)
 
     def running(self):
         return self._first_adptr.run and self._second_adptr.run
```

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/ag_adapter/agent.py` & `autogencap_rajan_jedi-0.0.9/autogencap/ag_adapter/agent.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen.proto` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.py` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/Autogen_pb2.pyi` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/Autogen_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP.proto` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.py` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/CAP_pb2.pyi` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/CAP_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/autogencap/proto/protoc.exe` & `autogencap_rajan_jedi-0.0.9/autogencap/proto/protoc.exe`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/.gitignore` & `autogencap_rajan_jedi-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/README.md` & `autogencap_rajan_jedi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.8/pyproject.toml` & `autogencap_rajan_jedi-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autogencap_rajan.jedi"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Rajan Chari", email="rajan.jedi@gmail.com" },
 ]
 dependencies = [
     "pyzmq >= 25.1.2",
     "protobuf >= 4.25.3",
     "termcolor >= 2.4.0",
```

### Comparing `autogencap_rajan_jedi-0.0.8/PKG-INFO` & `autogencap_rajan_jedi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autogencap_rajan.jedi
-Version: 0.0.8
+Version: 0.0.9
 Summary: CAP w/ autogen bindings
 Project-URL: Homepage, https://github.com/microsoft/autogen
 Project-URL: Bug Tracker, https://github.com/microsoft/autogen/issues
 Author-email: Rajan Chari <rajan.jedi@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

