# Comparing `tmp/openobd-0.14.0.tar.gz` & `tmp/openobd-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-0.14.0.tar", last modified: Wed May 22 15:13:19 2024, max compression
+gzip compressed data, was "openobd-0.15.0.tar", last modified: Tue May 28 13:15:33 2024, max compression
```

## Comparing `openobd-0.14.0.tar` & `openobd-0.15.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:19.574339 openobd-0.14.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-22 15:13:16.000000 openobd-0.14.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-22 15:13:19.574339 openobd-0.14.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2024-05-22 15:13:16.000000 openobd-0.14.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1773 2024-05-22 15:13:16.000000 openobd-0.14.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 15:13:19.574339 openobd-0.14.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:19.571339 openobd-0.14.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:19.572339 openobd-0.14.0/src/openobd/
--rw-r--r--   0 root         (0) root         (0)     1947 2024-05-22 15:13:16.000000 openobd-0.14.0/src/openobd/__init__.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-22 15:13:16.000000 openobd-0.14.0/src/openobd/_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     9289 2024-05-22 15:13:16.000000 openobd-0.14.0/src/openobd/openobd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:19.574339 openobd-0.14.0/src/openobd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-22 15:13:19.000000 openobd-0.14.0/src/openobd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-22 15:13:19.000000 openobd-0.14.0/src/openobd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 15:13:19.000000 openobd-0.14.0/src/openobd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-22 15:13:19.000000 openobd-0.14.0/src/openobd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-22 15:13:19.000000 openobd-0.14.0/src/openobd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:15:33.706030 openobd-0.15.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-28 13:15:30.000000 openobd-0.15.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-28 13:15:33.705030 openobd-0.15.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-28 13:15:30.000000 openobd-0.15.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-05-28 13:15:30.000000 openobd-0.15.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 13:15:33.706030 openobd-0.15.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:15:33.702030 openobd-0.15.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:15:33.703030 openobd-0.15.0/src/openobd/
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-28 13:15:30.000000 openobd-0.15.0/src/openobd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 13:15:30.000000 openobd-0.15.0/src/openobd/_metadata.py
+-rwxr-xr-x   0 root         (0) root         (0)     9987 2024-05-28 13:15:30.000000 openobd-0.15.0/src/openobd/openobd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:15:33.705030 openobd-0.15.0/src/openobd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-28 13:15:33.000000 openobd-0.15.0/src/openobd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-28 13:15:33.000000 openobd-0.15.0/src/openobd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 13:15:33.000000 openobd-0.15.0/src/openobd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-28 13:15:33.000000 openobd-0.15.0/src/openobd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 13:15:33.000000 openobd-0.15.0/src/openobd.egg-info/top_level.txt
```

### Comparing `openobd-0.14.0/LICENSE` & `openobd-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-0.14.0/PKG-INFO` & `openobd-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd
-Version: 0.14.0
+Version: 0.15.0
 Summary: Jifeline Networks OpenOBD Python Client Library
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,15 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openobd-protocol==0.13.0
+Requires-Dist: openobd-protocol==0.14.0
 Requires-Dist: openobd-utils==0.13.0
 
 OpenOBD Client by Jifeline Networks for Python 3
 
 Release notes:
 
  - 0.0.30 : First openobd package that uses openobd-protocol
```

### Comparing `openobd-0.14.0/pyproject.toml` & `openobd-0.15.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openobd"
 description = "Jifeline Networks OpenOBD Python Client Library"
 requires-python = ">=3.11"
 dependencies = [
-    "openobd-protocol==0.13.0",
+    "openobd-protocol==0.14.0",
     "openobd-utils==0.13.0"
 ]
 
 license = {file = "LICENSE"}
 dynamic = ["version"]
 readme = "README.md"
```

### Comparing `openobd-0.14.0/src/openobd/__init__.py` & `openobd-0.15.0/src/openobd/__init__.py`

 * *Files identical despite different names*

### Comparing `openobd-0.14.0/src/openobd/openobd.py` & `openobd-0.15.0/src/openobd/openobd.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from openobd_protocol import BasicResponse_pb2 as grpcBasicResponse
 from openobd_protocol.SessionController import Session_pb2 as grpcSession
 from openobd_protocol.SessionController import SessionServices_pb2_grpc as grpcSessionControllerService
 from openobd_protocol.CAN import Isotp_pb2 as grpcIsotp
 from openobd_protocol.CAN import CanServices_pb2_grpc as grpcCanService
 from openobd_protocol.UserInterface import UserInterface_pb2 as grpcUserInterface
 from openobd_protocol.UserInterface import UserInterfaceServices_pb2_grpc as grpcUserInterfaceService
+from openobd_protocol.ConnectionMonitor import ConnectionInformation_pb2 as grpcConnectionInformation
+from openobd_protocol.ConnectionMonitor import ConnectionMonitorServices_pb2_grpc as grpcConnectionMonitorService
 
 
 from typing import Iterator
 
 
 def _is_valid_response(response, response_object):
     try:
@@ -60,14 +62,15 @@
         self.grpc_host = self.session_info.grpc_endpoint
         self.grpc_port = grpc_port
         self._connect()
 
         self.rds = grpcService.RemoteDiagnosticServicesStub(self.channel)
         self.can = grpcCanService.CanServicesStub(self.channel)
         self.ui = grpcUserInterfaceService.UserInterfaceServicesStub(self.channel)
+        self.connector_monitor = grpcConnectionMonitorService.ConnectionMonitorServicesStub(self.channel)
 
     def id(self):
         return self.session_info.id
 
     def _metadata(self):
         metadata = []
         metadata.append(("authorization", "Bearer {}".format(self.session_info.authentication_token)))
@@ -102,14 +105,21 @@
         """
         Client function to control various components of the user interface
         :param user_interface_messages: An iterator containing the user interface message to be controlled
         :return: User interface component with output or answers depending upon the control fields sent
         """
         return self.ui.control(user_interface_messages, metadata=self._metadata())
 
+    def get_connector_information(self) -> grpcConnectionInformation.ConnectorInformation:
+        """
+        Client function to retrieve connector information at the give instant
+        :return: gRPC Connector Information object
+        """
+        return self.connector_monitor.getConnectorInformation(request=grpcBasicResponse.EmptyMessage(), metadata=self._metadata())
+
 
 class OpenOBD(object):
     """
     Client for gRPC functionality
     """
     session_controller = None
 
@@ -226,10 +236,10 @@
 
     def get_session_list(self) -> grpcSession.SessionInfoList:
         """
         Manager function to request a list of active sessions
         :return: List of sessions
         """
 
-        return self.session_controller.getSessionList(request=grpcBasicResponse.EmptyRequest(), metadata=self._metadata())
+        return self.session_controller.getSessionList(request=grpcBasicResponse.EmptyMessage(), metadata=self._metadata())
```

### Comparing `openobd-0.14.0/src/openobd.egg-info/PKG-INFO` & `openobd-0.15.0/src/openobd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd
-Version: 0.14.0
+Version: 0.15.0
 Summary: Jifeline Networks OpenOBD Python Client Library
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,15 +31,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openobd-protocol==0.13.0
+Requires-Dist: openobd-protocol==0.14.0
 Requires-Dist: openobd-utils==0.13.0
 
 OpenOBD Client by Jifeline Networks for Python 3
 
 Release notes:
 
  - 0.0.30 : First openobd package that uses openobd-protocol
```

