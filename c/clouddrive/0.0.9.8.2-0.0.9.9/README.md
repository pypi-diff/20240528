# Comparing `tmp/clouddrive-0.0.9.8.2.tar.gz` & `tmp/clouddrive-0.0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouddrive-0.0.9.8.2.tar", max compression
+gzip compressed data, was "clouddrive-0.0.9.9.tar", max compression
```

## Comparing `clouddrive-0.0.9.8.2.tar` & `clouddrive-0.0.9.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 clouddrive-0.0.9.8.2/LICENSE
--rw-r--r--   0        0        0    66762 2024-01-01 07:36:27.882881 clouddrive-0.0.9.8.2/clouddrive/__init__.py
--rw-r--r--   0        0        0     9270 2024-01-01 07:37:07.543207 clouddrive-0.0.9.8.2/clouddrive/__init_client.py
--rw-r--r--   0        0        0   106617 2024-01-01 07:37:18.049848 clouddrive-0.0.9.8.2/clouddrive/client.py
--rw-r--r--   0        0        0    30561 2024-01-01 07:03:40.644727 clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive.proto
--rw-r--r--   0        0        0    83973 2024-01-01 07:03:57.187695 clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_grpc.py
--rw-r--r--   0        0        0    55056 2024-01-01 07:03:57.187809 clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_pb2.py
--rw-r--r--   0        0        0   183404 2024-01-01 07:03:57.187914 clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_pb2_grpc.py
--rw-r--r--   0        0        0       87 2023-12-19 14:25:18.585337 clouddrive-0.0.9.8.2/clouddrive/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 clouddrive-0.0.9.8.2/clouddrive/util/_init_mimetypes.py
--rw-r--r--   0        0        0    13056 2023-12-14 09:14:41.064229 clouddrive-0.0.9.8.2/clouddrive/util/download.py
--rw-r--r--   0        0        0    12845 2023-12-29 08:12:54.747710 clouddrive-0.0.9.8.2/clouddrive/util/file.py
--rw-r--r--   0        0        0     7277 2023-12-30 05:04:08.462757 clouddrive-0.0.9.8.2/clouddrive/util/ignore.py
--rw-r--r--   0        0        0      678 2023-12-19 11:57:30.557217 clouddrive-0.0.9.8.2/clouddrive/util/iter.py
--rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 clouddrive-0.0.9.8.2/clouddrive/util/property.py
--rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 clouddrive-0.0.9.8.2/clouddrive/util/response.py
--rw-r--r--   0        0        0     5230 2023-12-19 14:03:21.120801 clouddrive-0.0.9.8.2/clouddrive/util/text.py
--rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 clouddrive-0.0.9.8.2/clouddrive/util/urlopen.py
--rw-r--r--   0        0        0     1425 2024-01-01 07:37:53.154543 clouddrive-0.0.9.8.2/pyproject.toml
--rw-r--r--   0        0        0    29267 2023-12-29 08:02:31.170732 clouddrive-0.0.9.8.2/readme.md
--rw-r--r--   0        0        0    30538 1970-01-01 00:00:00.000000 clouddrive-0.0.9.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 clouddrive-0.0.9.9/LICENSE
+-rw-r--r--   0        0        0     9215 2024-01-03 06:51:02.923994 clouddrive-0.0.9.9/clouddrive/__init_client.py
+-rw-r--r--   0        0        0   107339 2024-01-12 04:03:09.290313 clouddrive-0.0.9.9/clouddrive/client.py
+-rw-r--r--   0        0        0    30987 2024-01-12 04:02:43.856603 clouddrive-0.0.9.9/clouddrive/proto/CloudDrive.proto
+-rw-r--r--   0        0        0    83973 2024-01-12 04:03:22.264978 clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_grpc.py
+-rw-r--r--   0        0        0    55807 2024-01-12 04:03:22.265118 clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_pb2.py
+-rw-r--r--   0        0        0   183394 2024-01-12 04:03:22.265246 clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_pb2_grpc.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:18.585337 clouddrive-0.0.9.9/clouddrive/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 clouddrive-0.0.9.9/clouddrive/util/_init_mimetypes.py
+-rw-r--r--   0        0        0    13056 2023-12-14 09:14:41.064229 clouddrive-0.0.9.9/clouddrive/util/download.py
+-rw-r--r--   0        0        0    12845 2023-12-29 08:12:54.747710 clouddrive-0.0.9.9/clouddrive/util/file.py
+-rw-r--r--   0        0        0     7277 2023-12-30 05:04:08.462757 clouddrive-0.0.9.9/clouddrive/util/ignore.py
+-rw-r--r--   0        0        0      678 2023-12-19 11:57:30.557217 clouddrive-0.0.9.9/clouddrive/util/iter.py
+-rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 clouddrive-0.0.9.9/clouddrive/util/property.py
+-rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 clouddrive-0.0.9.9/clouddrive/util/response.py
+-rw-r--r--   0        0        0     5230 2023-12-19 14:03:21.120801 clouddrive-0.0.9.9/clouddrive/util/text.py
+-rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 clouddrive-0.0.9.9/clouddrive/util/urlopen.py
+-rw-r--r--   0        0        0     1423 2024-01-12 04:07:08.646584 clouddrive-0.0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    29267 2023-12-29 08:02:31.170732 clouddrive-0.0.9.9/readme.md
+-rw-r--r--   0        0        0    30536 1970-01-01 00:00:00.000000 clouddrive-0.0.9.9/PKG-INFO
```

### Comparing `clouddrive-0.0.9.8.2/LICENSE` & `clouddrive-0.0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/__init_client.py` & `clouddrive-0.0.9.9/clouddrive/__init_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -169,21 +169,19 @@
 file.write("""\
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["Client"]
 
-from asyncio import run
-from inspect import isawaitable
-from typing import Any, Iterator, Never
+from typing import Any, Iterator, Never, Optional
 
 from google.protobuf.empty_pb2 import Empty # type: ignore
-from grpc import insecure_channel # type: ignore
-from grpclib.client import Channel # type: ignore
+from grpc import insecure_channel, Channel # type: ignore
+from grpclib.client import Channel as AsyncChannel # type: ignore
 from yarl import URL
 
 import pathlib, sys
 PROTO_DIR = str(pathlib.Path(__file__).parent / "proto")
 if PROTO_DIR not in sys.path:
     sys.path.append(PROTO_DIR)
 
@@ -193,36 +191,36 @@
 
 
 class Client:
     "clouddrive client that encapsulates grpc APIs"
     origin: str
     username: str
     password: str
-    channel: Any
-    async_channel: Any
+    channel: Channel
+    async_channel: AsyncChannel
     stub: CloudDrive_pb2_grpc.CloudDriveFileSrvStub
     async_stub: CloudDrive_grpc.CloudDriveFileSrvStub
     download_baseurl: str
     metadata: list[tuple[str, str]]
 
     def __init__(
         self, 
         /, 
         origin: str = "http://localhost:19798", 
         username: str = "", 
         password: str = "", 
-        channel = None, 
-        async_channel = None, 
+        channel: Optional[Channel] = None, 
+        async_channel: Optional[AsyncChannel] = None, 
     ):
         origin = origin.rstrip("/")
         urlp = URL(origin)
         if channel is None:
             channel = insecure_channel(urlp.authority)
         if async_channel is None:
-            async_channel = Channel(urlp.host, urlp.port)
+            async_channel = AsyncChannel(urlp.host, urlp.port)
         self.__dict__.update(
             origin = origin, 
             download_baseurl = f"{origin}/static/http/{urlp.authority}/False/", 
             username = username, 
             password = password, 
             channel = channel, 
             async_channel = async_channel, 
@@ -252,21 +250,16 @@
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     def close(self, /):
         try:
             self.channel.close()
-        except:
-            pass
-        try:
-            clo = self.async_channel.close()
-            if isawaitable(clo):
-                run(clo)
-        except:
+            self.async_channel.close()
+        except AttributeError:
             pass
 
     def set_password(self, value: str, /):
         self.__dict__["password"] = value
         self.login()
 
     def login(
```

### Comparing `clouddrive-0.0.9.8.2/clouddrive/client.py` & `clouddrive-0.0.9.9/clouddrive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["Client"]
 
-from asyncio import run
-from inspect import isawaitable
-from typing import Any, Iterator, Never
+from typing import Any, Iterator, Never, Optional
 
 from google.protobuf.empty_pb2 import Empty # type: ignore
-from grpc import insecure_channel # type: ignore
-from grpclib.client import Channel # type: ignore
+from grpc import insecure_channel, Channel # type: ignore
+from grpclib.client import Channel as AsyncChannel # type: ignore
 from yarl import URL
 
 import pathlib, sys
 PROTO_DIR = str(pathlib.Path(__file__).parent / "proto")
 if PROTO_DIR not in sys.path:
     sys.path.append(PROTO_DIR)
 
@@ -24,36 +22,36 @@
 
 
 class Client:
     "clouddrive client that encapsulates grpc APIs"
     origin: str
     username: str
     password: str
-    channel: Any
-    async_channel: Any
+    channel: Channel
+    async_channel: AsyncChannel
     stub: CloudDrive_pb2_grpc.CloudDriveFileSrvStub
     async_stub: CloudDrive_grpc.CloudDriveFileSrvStub
     download_baseurl: str
     metadata: list[tuple[str, str]]
 
     def __init__(
         self, 
         /, 
         origin: str = "http://localhost:19798", 
         username: str = "", 
         password: str = "", 
-        channel = None, 
-        async_channel = None, 
+        channel: Optional[Channel] = None, 
+        async_channel: Optional[AsyncChannel] = None, 
     ):
         origin = origin.rstrip("/")
         urlp = URL(origin)
         if channel is None:
             channel = insecure_channel(urlp.authority)
         if async_channel is None:
-            async_channel = Channel(urlp.host, urlp.port)
+            async_channel = AsyncChannel(urlp.host, urlp.port)
         self.__dict__.update(
             origin = origin, 
             download_baseurl = f"{origin}/static/http/{urlp.authority}/False/", 
             username = username, 
             password = password, 
             channel = channel, 
             async_channel = async_channel, 
@@ -83,21 +81,16 @@
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     def close(self, /):
         try:
             self.channel.close()
-        except:
-            pass
-        try:
-            clo = self.async_channel.close()
-            if isawaitable(clo):
-                run(clo)
-        except:
+            self.async_channel.close()
+        except AttributeError:
             pass
 
     def set_password(self, value: str, /):
         self.__dict__["password"] = value
         self.login()
 
     def login(
@@ -355,14 +348,15 @@
             PikPakSha1 = 3;
           }
           map<uint32, string> fileHashes = 70;
         }
         message ListSubFileRequest {
           string path = 1;
           bool forceRefresh = 2;
+          optional bool checkExpires = 3;
         }
         message SubFilesReply { repeated CloudDriveFile subFiles = 1; }
         """
         return (self.async_stub if async_ else self.stub).GetSubFiles(arg, metadata=self.metadata)
 
     def GetSearchResults(self, arg: CloudDrive_pb2.SearchRequest, /, async_: bool = False) -> Iterator[CloudDrive_pb2.SubFilesReply]:
         """
@@ -2567,14 +2561,16 @@
           repeated FileBackupRule fileBackupRules = 3;
           FileReplaceRule fileReplaceRule = 4;
           FileDeleteRule fileDeleteRule = 5;
           bool isEnabled = 6;
           bool fileSystemWatchEnabled = 7;
           int64 walkingThroughIntervalSecs = 8; // 0 means never auto walking through
           bool forceWalkingThroughOnStart = 9;
+          repeated TimeSchedule timeSchedules = 10;
+          bool isTimeSchedulesEnabled = 11;
         }
         message BackupDestination {
           string destinationPath = 1;
           bool isEnabled = 2;
           optional google.protobuf.Timestamp lastFinishTime = 3;
         }
         message FileBackupRule {
@@ -2594,14 +2590,21 @@
           MoveToVersionHistory = 3;
         }
         enum FileReplaceRule {
           Skip = 0;
           Overwrite = 1;
           KeepHistoryVersion = 2;
         }
+        message TimeSchedule {
+          bool isEnabled = 1;
+          uint32 hour = 2;
+          uint32 minute = 3;
+          uint32 second = 4;
+          optional DaysOfWeek daysOfWeek = 5; //none means every day
+        }
         """
         return (self.async_stub if async_ else self.stub).BackupAdd(arg, metadata=self.metadata)
 
     def BackupRemove(self, arg: CloudDrive_pb2.StringValue, /, async_: bool = False) -> None:
         """
         remove a backup by it's source path
 
@@ -2635,14 +2638,16 @@
           repeated FileBackupRule fileBackupRules = 3;
           FileReplaceRule fileReplaceRule = 4;
           FileDeleteRule fileDeleteRule = 5;
           bool isEnabled = 6;
           bool fileSystemWatchEnabled = 7;
           int64 walkingThroughIntervalSecs = 8; // 0 means never auto walking through
           bool forceWalkingThroughOnStart = 9;
+          repeated TimeSchedule timeSchedules = 10;
+          bool isTimeSchedulesEnabled = 11;
         }
         message BackupDestination {
           string destinationPath = 1;
           bool isEnabled = 2;
           optional google.protobuf.Timestamp lastFinishTime = 3;
         }
         message FileBackupRule {
@@ -2662,14 +2667,21 @@
           MoveToVersionHistory = 3;
         }
         enum FileReplaceRule {
           Skip = 0;
           Overwrite = 1;
           KeepHistoryVersion = 2;
         }
+        message TimeSchedule {
+          bool isEnabled = 1;
+          uint32 hour = 2;
+          uint32 minute = 3;
+          uint32 second = 4;
+          optional DaysOfWeek daysOfWeek = 5; //none means every day
+        }
         """
         return (self.async_stub if async_ else self.stub).BackupUpdate(arg, metadata=self.metadata)
 
     def BackupAddDestination(self, arg: CloudDrive_pb2.BackupModifyRequest, /, async_: bool = False) -> None:
         """
         add destinations to a backup
 
@@ -2836,17 +2848,19 @@
           KeepHistoryVersion = 2;
         }
         """
         return (self.async_stub if async_ else self.stub).BackupSetFileSystemWatchEnabled(arg, metadata=self.metadata)
 
     def BackupUpdateStrategies(self, arg: CloudDrive_pb2.BackupModifyRequest, /, async_: bool = False) -> None:
         """
+        deprecated, use BackupUpdate instead
 
         ------------------- protobuf rpc definition --------------------
 
+        // deprecated, use BackupUpdate instead
         rpc BackupUpdateStrategies(BackupModifyRequest)
             returns (google.protobuf.Empty) {}
 
         ------------------- protobuf type definition -------------------
 
         message BackupDestination {
           string destinationPath = 1;
```

### Comparing `clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive.proto` & `clouddrive-0.0.9.9/clouddrive/proto/CloudDrive.proto`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 syntax = "proto3";
 
-package clouddrive;
-
-// 0.6.0
+package clouddrive;
 
 option csharp_namespace = "CloudDriveSrv.Protos";
+
+// 0.6.3
 
 import "google/protobuf/timestamp.proto";
 import "google/protobuf/empty.proto";
 
 service CloudDriveFileSrv {
   // public methods, no authorization is required
   // returns if clouddrive has logged in to cloudfs server and the user name
@@ -279,14 +279,15 @@
       returns (google.protobuf.Empty) {}
   // enable/disable a backup
   rpc BackupSetEnabled(BackupSetEnabledRequest)
       returns (google.protobuf.Empty) {}
   // enable/disable a backup's FileSystemWatch
   rpc BackupSetFileSystemWatchEnabled(BackupModifyRequest)
       returns (google.protobuf.Empty) {}
+  // deprecated, use BackupUpdate instead
   rpc BackupUpdateStrategies(BackupModifyRequest)
       returns (google.protobuf.Empty) {}
   rpc BackupRestartWalkingThrough(StringValue)
       returns (google.protobuf.Empty) {}
   rpc CanAddMoreBackups(google.protobuf.Empty)
       returns (FileOperationResult) {}
 }
@@ -309,14 +310,15 @@
 }
 message StringResult { string result = 1; }
 message UnmountArchiveResult { string result = 1; }
 
 message ListSubFileRequest {
   string path = 1;
   bool forceRefresh = 2;
+  optional bool checkExpires = 3;
 }
 message SearchRequest {
   string path = 1;
   string searchFor = 2;
   bool forceRefresh = 3;
   bool fuzzyMatch = 4;
 }
@@ -866,24 +868,36 @@
   MoveToVersionHistory = 3;
 }
 message BackupDestination {
   string destinationPath = 1;
   bool isEnabled = 2;
   optional google.protobuf.Timestamp lastFinishTime = 3;
 }
+message DaysOfWeek {
+  repeated uint32 daysOfWeek = 1; //Mon: 1, Tue: 2, ..., Sun: 0
+}
+message TimeSchedule {
+  bool isEnabled = 1;
+  uint32 hour = 2;
+  uint32 minute = 3;
+  uint32 second = 4;
+  optional DaysOfWeek daysOfWeek = 5; //none means every day
+}
 message Backup {
   string sourcePath = 1;
   repeated BackupDestination destinations = 2;
   repeated FileBackupRule fileBackupRules = 3;
   FileReplaceRule fileReplaceRule = 4;
   FileDeleteRule fileDeleteRule = 5;
   bool isEnabled = 6;
   bool fileSystemWatchEnabled = 7;
   int64 walkingThroughIntervalSecs = 8; // 0 means never auto walking through
   bool forceWalkingThroughOnStart = 9;
+  repeated TimeSchedule timeSchedules = 10;
+  bool isTimeSchedulesEnabled = 11;
 }
 message BackupStatus {
   enum Status {
     Idle = 0;
     WalkingThrough = 1;
     Error = 2;
     Disabled = 3;
```

### Comparing `clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_grpc.py` & `clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_grpc.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_pb2.py` & `clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x43loudDrive.proto\x12\nclouddrive\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"5\n\x0fGetTokenRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"p\n\x08JWTToken\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12.\n\nexpiration\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x1b\n\x0b\x46ileRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\" \n\x10MultiFileRequest\x12\x0c\n\x04path\x18\x01 \x03(\t\"U\n\x13\x46ileOperationResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\x12\x17\n\x0fresultFilePaths\x18\x03 \x03(\t\"\x1e\n\x0cStringResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"&\n\x14UnmountArchiveResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"8\n\x12ListSubFileRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x14\n\x0c\x66orceRefresh\x18\x02 \x01(\x08\"Z\n\rSearchRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tsearchFor\x18\x02 \x01(\t\x12\x14\n\x0c\x66orceRefresh\x18\x03 \x01(\x08\x12\x12\n\nfuzzyMatch\x18\x04 \x01(\x08\"7\n\x15\x41\x64\x64OfflineFileRequest\x12\x0c\n\x04urls\x18\x01 \x01(\t\x12\x10\n\x08toFolder\x18\x02 \x01(\t\"W\n\x14\x41\x64\x64SharedLinkRequest\x12\x15\n\rsharedLinkUrl\x18\x01 \x01(\t\x12\x16\n\x0esharedPassword\x18\x02 \x01(\t\x12\x10\n\x08toFolder\x18\x03 \x01(\t\"=\n\rSubFilesReply\x12,\n\x08subFiles\x18\x01 \x03(\x0b\x32\x1a.clouddrive.CloudDriveFile\"9\n\x15\x46indFileByPathRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"=\n\x13\x43reateFolderRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x12\n\nfolderName\x18\x02 \x01(\t\"x\n\x12\x43reateFolderResult\x12\x31\n\rfolderCreated\x18\x01 \x01(\x0b\x32\x1a.clouddrive.CloudDriveFile\x12/\n\x06result\x18\x02 \x01(\x0b\x32\x1f.clouddrive.FileOperationResult\"9\n\x11\x43reateFileRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x10\n\x08\x66ileName\x18\x02 \x01(\t\"&\n\x10\x43reateFileResult\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\"&\n\x10\x43loseFileRequest\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\"9\n\x0fMoveFileRequest\x12\x14\n\x0ctheFilePaths\x18\x01 \x03(\t\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\"k\n\x10WriteFileRequest\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\x12\x10\n\x08startPos\x18\x02 \x01(\x04\x12\x0e\n\x06length\x18\x03 \x01(\x04\x12\x0e\n\x06\x62uffer\x18\x04 \x01(\x0c\x12\x11\n\tcloseFile\x18\x05 \x01(\x08\"\'\n\x0fWriteFileResult\x12\x14\n\x0c\x62ytesWritten\x18\x01 \x01(\x04\"9\n\x11RenameFileRequest\x12\x13\n\x0btheFilePath\x18\x01 \x01(\t\x12\x0f\n\x07newName\x18\x02 \x01(\t\"H\n\x12RenameFilesRequest\x12\x32\n\x0brenameFiles\x18\x01 \x03(\x0b\x32\x1d.clouddrive.RenameFileRequest\"\xcc\x08\n\x0e\x43loudDriveFile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x66ullPathName\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x35\n\x08\x66ileType\x18\x05 \x01(\x0e\x32#.clouddrive.CloudDriveFile.FileType\x12.\n\ncreateTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\twriteTime\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\naccessTime\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x08\x43loudAPI\x18\t \x01(\x0b\x32\x14.clouddrive.CloudAPI\x12\x14\n\x0cthumbnailUrl\x18\n \x01(\t\x12\x12\n\npreviewUrl\x18\x0b \x01(\t\x12\x14\n\x0coriginalPath\x18\x0e \x01(\t\x12\x13\n\x0bisDirectory\x18\x1e \x01(\x08\x12\x0e\n\x06isRoot\x18\x1f \x01(\x08\x12\x13\n\x0bisCloudRoot\x18  \x01(\x08\x12\x18\n\x10isCloudDirectory\x18! \x01(\x08\x12\x13\n\x0bisCloudFile\x18\" \x01(\x08\x12\x16\n\x0eisSearchResult\x18# \x01(\x08\x12\x13\n\x0bisForbidden\x18$ \x01(\x08\x12\x0f\n\x07isLocal\x18% \x01(\x08\x12\x10\n\x08\x63\x61nMount\x18< \x01(\x08\x12\x12\n\ncanUnmount\x18= \x01(\x08\x12#\n\x1b\x63\x61nDirectAccessThumbnailURL\x18> \x01(\x08\x12\x11\n\tcanSearch\x18? \x01(\x08\x12\x1b\n\x13hasDetailProperties\x18@ \x01(\x08\x12:\n\x10\x64\x65tailProperties\x18\x41 \x01(\x0b\x32 .clouddrive.FileDetailProperties\x12\x1a\n\x12\x63\x61nOfflineDownload\x18\x42 \x01(\x08\x12\x17\n\x0f\x63\x61nAddShareLink\x18\x43 \x01(\x08\x12#\n\x16\x64irCacheTimeToLiveSecs\x18\x44 \x01(\x04H\x00\x88\x01\x01\x12\x1c\n\x14\x63\x61nDeletePermanently\x18\x45 \x01(\x08\x12>\n\nfileHashes\x18\x46 \x03(\x0b\x32*.clouddrive.CloudDriveFile.FileHashesEntry\x1a\x31\n\x0f\x46ileHashesEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\".\n\x08\x46ileType\x12\r\n\tDirectory\x10\x00\x12\x08\n\x04\x46ile\x10\x01\x12\t\n\x05Other\x10\x02\":\n\x08HashType\x12\x0b\n\x07Unknown\x10\x00\x12\x07\n\x03Md5\x10\x01\x12\x08\n\x04Sha1\x10\x02\x12\x0e\n\nPikPakSha1\x10\x03\x42\x19\n\x17_dirCacheTimeToLiveSecs\"E\n\tSpaceInfo\x12\x12\n\ntotalSpace\x18\x01 \x01(\x03\x12\x11\n\tusedSpace\x18\x02 \x01(\x03\x12\x11\n\tfreeSpace\x18\x03 \x01(\x03\"N\n\x08\x43loudAPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x10\n\x08nickName\x18\x03 \x01(\t\x12\x10\n\x08isLocked\x18\x04 \x01(\x08\"\x85\x01\n\x0f\x43loudMembership\x12\x10\n\x08identity\x18\x01 \x01(\t\x12\x33\n\nexpireTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12\x12\n\x05level\x18\x03 \x01(\tH\x01\x88\x01\x01\x42\r\n\x0b_expireTimeB\x08\n\x06_level\"D\n\x10\x43loudMemberships\x12\x30\n\x0bmemberships\x18\x01 \x03(\x0b\x32\x1b.clouddrive.CloudMembership\"\x94\x01\n\x14\x46ileDetailProperties\x12\x16\n\x0etotalFileCount\x18\x01 \x01(\x03\x12\x18\n\x10totalFolderCount\x18\x02 \x01(\x03\x12\x11\n\ttotalSize\x18\x03 \x01(\x03\x12\x0f\n\x07isFaved\x18\x04 \x01(\x08\x12\x10\n\x08isShared\x18\x05 \x01(\x08\x12\x14\n\x0coriginalPath\x18\x06 \x01(\t\"y\n\x0c\x46ileMetaData\x12\x38\n\x08metadata\x18\x01 \x03(\x0b\x32&.clouddrive.FileMetaData.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"9\n\x14\x43loudDriveSystemInfo\x12\x0f\n\x07IsLogin\x18\x01 \x01(\x08\x12\x10\n\x08UserName\x18\x02 \x01(\t\"N\n\x10UserLoginRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x16\n\x0esynDataToCloud\x18\x03 \x01(\x08\"9\n\x13UserRegisterRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11UserLogoutRequest\x12\x19\n\x11logoutFromCloudFS\x18\x01 \x01(\x08\"A\n\x15\x43hangePasswordRequest\x12\x13\n\x0boldPassword\x18\x01 \x01(\t\x12\x13\n\x0bnewPassword\x18\x02 \x01(\t\"\xb4\x01\n\x13\x41\x63\x63ountStatusResult\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x16\n\x0e\x65mailConfirmed\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x63\x63ountBalance\x18\x03 \x01(\x01\x12,\n\x0b\x61\x63\x63ountPlan\x18\x04 \x01(\x0b\x32\x17.clouddrive.AccountPlan\x12-\n\x0c\x61\x63\x63ountRoles\x18\x05 \x03(\x0b\x32\x17.clouddrive.AccountRole\"\x97\x01\n\x0b\x41\x63\x63ountPlan\x12\x10\n\x08planName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0f\x66ontAwesomeIcon\x18\x03 \x01(\t\x12\x1b\n\x13\x64urationDescription\x18\x04 \x01(\t\x12+\n\x07\x65ndTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"R\n\x0b\x41\x63\x63ountRole\x12\x10\n\x08roleName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x12\n\x05value\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_value\"c\n\x0bRuntimeInfo\x12\x13\n\x0bproductName\x18\x01 \x01(\t\x12\x16\n\x0eproductVersion\x18\x02 \x01(\t\x12\x17\n\x0f\x43loudAPIVersion\x18\x03 \x01(\t\x12\x0e\n\x06osInfo\x18\x04 \x01(\t\"\x83\x01\n\x07RunInfo\x12\x10\n\x08\x63puUsage\x18\x01 \x01(\x01\x12\x12\n\nmemUsageKB\x18\x02 \x01(\x04\x12\x0e\n\x06uptime\x18\x03 \x01(\x01\x12\x14\n\x0c\x66hTableCount\x18\x04 \x01(\x04\x12\x15\n\rdirCacheCount\x18\x05 \x01(\x04\x12\x15\n\rtempFileCount\x18\x06 \x01(\x04\"\xaa\x01\n\x0bMountOption\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12\x11\n\tsourceDir\x18\x02 \x01(\t\x12\x12\n\nlocalMount\x18\x03 \x01(\x08\x12\x10\n\x08readOnly\x18\x04 \x01(\x08\x12\x11\n\tautoMount\x18\x05 \x01(\x08\x12\x0b\n\x03uid\x18\x06 \x01(\r\x12\x0b\n\x03gid\x18\x07 \x01(\r\x12\x13\n\x0bpermissions\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\xc2\x01\n\nMountPoint\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12\x11\n\tsourceDir\x18\x02 \x01(\t\x12\x12\n\nlocalMount\x18\x03 \x01(\x08\x12\x10\n\x08readOnly\x18\x04 \x01(\x08\x12\x11\n\tautoMount\x18\x05 \x01(\x08\x12\x0b\n\x03uid\x18\x06 \x01(\r\x12\x0b\n\x03gid\x18\x07 \x01(\r\x12\x13\n\x0bpermissions\x18\x08 \x01(\t\x12\x11\n\tisMounted\x18\t \x01(\x08\x12\x12\n\nfailReason\x18\n \x01(\t\"\'\n\x11MountPointRequest\x12\x12\n\nMountPoint\x18\x01 \x01(\t\"C\n\x14GetMountPointsResult\x12+\n\x0bmountPoints\x18\x01 \x03(\x0b\x32\x16.clouddrive.MountPoint\"7\n\x10MountPointResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x12\n\nfailReason\x18\x02 \x01(\t\"^\n\x17UpdateMountPointRequest\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12/\n\x0enewMountOption\x18\x02 \x01(\x0b\x32\x17.clouddrive.MountOption\"<\n\x1fGetAvailableDriveLettersRequest\x12\x19\n\x11includeCloudDrive\x18\x01 \x01(\x08\"6\n\x1eGetAvailableDriveLettersResult\x12\x14\n\x0c\x64riveLetters\x18\x01 \x03(\t\"0\n\x15HasDriveLettersResult\x12\x17\n\x0fhasDriveLetters\x18\x01 \x01(\x08\"}\n\x17LocalGetSubFilesRequest\x12\x14\n\x0cparentFolder\x18\x01 \x01(\t\x12\x12\n\nfolderOnly\x18\x02 \x01(\x08\x12\x19\n\x11includeCloudDrive\x18\x03 \x01(\x08\x12\x1d\n\x15includeAvailableDrive\x18\x04 \x01(\x08\"*\n\x16LocalGetSubFilesResult\x12\x10\n\x08subFiles\x18\x01 \x03(\t\"(\n\x0bPushMessage\x12\x19\n\x11\x63louddriveVersion\x18\x01 \x01(\t\"\x85\x01\n\x16GetAllTasksCountResult\x12\x15\n\rdownloadCount\x18\x01 \x01(\r\x12\x13\n\x0buploadCount\x18\x02 \x01(\r\x12,\n\x0bpushMessage\x18\x03 \x01(\x0b\x32\x17.clouddrive.PushMessage\x12\x11\n\thasUpdate\x18\x04 \x01(\x08\"/\n\x1aGetDownloadFileCountResult\x12\x11\n\tfileCount\x18\x01 \x01(\r\"\x9b\x01\n\x10\x44ownloadFileInfo\x12\x10\n\x08\x66ilePath\x18\x01 \x01(\t\x12\x12\n\nfileLength\x18\x02 \x01(\x04\x12\x17\n\x0ftotalBufferUsed\x18\x03 \x01(\x04\x12\x1b\n\x13\x64ownloadThreadCount\x18\x04 \x01(\r\x12\x0f\n\x07process\x18\x05 \x03(\t\x12\x1a\n\x12\x64\x65tailDownloadInfo\x18\x06 \x01(\t\"n\n\x19GetDownloadFileListResult\x12\x1c\n\x14globalBytesPerSecond\x18\x01 \x01(\x01\x12\x33\n\rdownloadFiles\x18\x04 \x03(\x0b\x32\x1c.clouddrive.DownloadFileInfo\"-\n\x18GetUploadFileCountResult\x12\x11\n\tfileCount\x18\x01 \x01(\r\"|\n\x0eUploadFileInfo\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\x17\n\x0ftransferedBytes\x18\x04 \x01(\x04\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x06 \x01(\t\"d\n\x18GetUploadFileListRequest\x12\x0e\n\x06getAll\x18\x01 \x01(\x08\x12\x14\n\x0citemsPerPage\x18\x02 \x01(\r\x12\x12\n\npageNumber\x18\x03 \x01(\r\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"^\n\x17GetUploadFileListResult\x12\x12\n\ntotalCount\x18\x01 \x01(\r\x12/\n\x0buploadFiles\x18\x02 \x03(\x0b\x32\x1a.clouddrive.UploadFileInfo\"+\n\x1bMultpleUploadFileKeyRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\"=\n\x1dLogin115EditthiscookieRequest\x12\x1c\n\x14\x65\x64itThiscookieString\x18\x01 \x01(\t\"G\n\x15Login115QrCodeRequest\x12\x1b\n\x0eplatformString\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_platformString\"_\n\x1cLoginAliyundriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"O\n#LoginAliyundriveRefreshtokenRequest\x12\x14\n\x0crefreshToken\x18\x01 \x01(\t\x12\x12\n\nuseOpenAPI\x18\x02 \x01(\x08\"3\n\x1dLoginAliyundriveQRCodeRequest\x12\x12\n\nuseOpenAPI\x18\x01 \x01(\x08\"\\\n\x19LoginBaiduPanOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"\\\n\x19LoginOneDriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"_\n\x1cLoginGoogleDriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"f\n#LoginGoogleDriveRefreshTokenRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x15\n\rclient_secret\x18\x02 \x01(\t\x12\x15\n\rrefresh_token\x18\x03 \x01(\t\"K\n\x12LoginWebDavRequest\x12\x11\n\tserverUrl\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"7\n\x0e\x41PILoginResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"0\n\x15\x41\x64\x64LocalFolderRequest\x12\x17\n\x0flocalFolderPath\x18\x01 \x01(\t\"U\n\x15RemoveCloudAPIRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x17\n\x0fpermanentRemove\x18\x03 \x01(\x08\"?\n\x18GetCloudAPIConfigRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\"2\n\x0c\x43loudAPIList\x12\"\n\x04\x61pis\x18\x01 \x03(\x0b\x32\x14.clouddrive.CloudAPI\"\xc8\x01\n\x0e\x43loudAPIConfig\x12\x1a\n\x12maxDownloadThreads\x18\x01 \x01(\r\x12\x17\n\x0fminReadLengthKB\x18\x02 \x01(\x04\x12\x17\n\x0fmaxReadLengthKB\x18\x03 \x01(\x04\x12\x1b\n\x13\x64\x65\x66\x61ultReadLengthKB\x18\x04 \x01(\x04\x12\x1b\n\x13maxBufferPoolSizeMB\x18\x05 \x01(\x04\x12\x1b\n\x13maxQueriesPerSecond\x18\x06 \x01(\x01\x12\x11\n\tforceIpv4\x18\x07 \x01(\x08\"k\n\x18SetCloudAPIConfigRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.clouddrive.CloudAPIConfig\"!\n\x0e\x43ommandRequest\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"\x1f\n\rCommandResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"\x1c\n\x0bStringValue\x12\r\n\x05value\x18\x01 \x01(\t\"\\\n\x11QRCodeScanMessage\x12\x36\n\x0bmessageType\x18\x01 \x01(\x0e\x32!.clouddrive.QRCodeScanMessageType\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x1c\n\nStringList\x12\x0e\n\x06values\x18\x01 \x03(\t\"\x83\x05\n\x0eSystemSettings\x12#\n\x16\x64irCacheTimeToLiveSecs\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12maxPreProcessTasks\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0fmaxProcessTasks\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10tempFileLocation\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x1a\n\rsyncWithCloud\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12&\n\x19readDownloaderTimeoutSecs\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1c\n\x0fuploadDelaySecs\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12\x35\n\x10processBlackList\x18\x08 \x01(\x0b\x32\x16.clouddrive.StringListH\x07\x88\x01\x01\x12<\n\x17uploadIgnoredExtensions\x18\t \x01(\x0b\x32\x16.clouddrive.StringListH\x08\x88\x01\x01\x12\x35\n\rupdateChannel\x18\n \x01(\x0e\x32\x19.clouddrive.UpdateChannelH\t\x88\x01\x01\x42\x19\n\x17_dirCacheTimeToLiveSecsB\x15\n\x13_maxPreProcessTasksB\x12\n\x10_maxProcessTasksB\x13\n\x11_tempFileLocationB\x10\n\x0e_syncWithCloudB\x1c\n\x1a_readDownloaderTimeoutSecsB\x12\n\x10_uploadDelaySecsB\x13\n\x11_processBlackListB\x1a\n\x18_uploadIgnoredExtensionsB\x10\n\x0e_updateChannel\"d\n\x16SetDirCacheTimeRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\"\n\x15\x64irCachTimeToLiveSecs\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x18\n\x16_dirCachTimeToLiveSecs\"/\n\x1fGetEffectiveDirCacheTimeRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"-\n\x17GetOpenFileTableRequest\x12\x12\n\nincludeDir\x18\x01 \x01(\x08\":\n\x1eGetEffectiveDirCacheTimeResult\x12\x18\n\x10\x64irCacheTimeSecs\x18\x01 \x01(\x04\"J\n\x0cUpdateResult\x12\x11\n\thasUpdate\x18\x01 \x01(\x08\x12\x12\n\nnewVersion\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\xa6\x01\n\rOpenFileTable\x12\x43\n\ropenFileTable\x18\x01 \x03(\x0b\x32,.clouddrive.OpenFileTable.OpenFileTableEntry\x12\x1a\n\x12localOpenFileCount\x18\x02 \x01(\x04\x1a\x34\n\x12OpenFileTableEntry\x12\x0b\n\x03key\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"t\n\x0c\x44irCacheItem\x12.\n\ninsertTime\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0etimeToLiveSecs\x18\x02 \x01(\x04\x12\x1c\n\x14referencedSubfileLen\x18\x03 \x01(\x04\"\xa4\x01\n\rDirCacheTable\x12\x43\n\rdirCacheTable\x18\x01 \x03(\x0b\x32,.clouddrive.DirCacheTable.DirCacheTableEntry\x1aN\n\x12\x44irCacheTableEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.clouddrive.DirCacheItem:\x02\x38\x01\"1\n\rTempFileTable\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x11\n\ttempFiles\x18\x02 \x03(\t\"*\n\x13\x43onfirmEmailRequest\x12\x13\n\x0b\x63onfirmCode\x18\x01 \x01(\t\"-\n\x1cSendResetAccountEmailRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\"=\n\x13ResetAccountRequest\x12\x11\n\tresetCode\x18\x01 \x01(\t\x12\x13\n\x0bnewPassword\x18\x02 \x01(\t\"\x81\x02\n\x0e\x43loudDrivePlan\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05price\x18\x04 \x01(\x01\x12\x15\n\x08\x64uration\x18\x05 \x01(\x03H\x00\x88\x01\x01\x12\x1b\n\x13\x64urationDescription\x18\x06 \x01(\t\x12\x10\n\x08isActive\x18\x07 \x01(\x08\x12\x1c\n\x0f\x66ontAwesomeIcon\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1a\n\roriginalPrice\x18\t \x01(\x01H\x02\x88\x01\x01\x42\x0b\n\t_durationB\x12\n\x10_fontAwesomeIconB\x10\n\x0e_originalPrice\"E\n\x18GetCloudDrivePlansResult\x12)\n\x05plans\x18\x01 \x03(\x0b\x32\x1a.clouddrive.CloudDrivePlan\"I\n\x0fJoinPlanRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x17\n\ncouponCode\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_couponCode\"\xab\x01\n\x0bPaymentInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0f\n\x07plan_id\x18\x02 \x01(\t\x12\x43\n\x0epaymentMethods\x18\x03 \x03(\x0b\x32+.clouddrive.PaymentInfo.PaymentMethodsEntry\x1a\x35\n\x13PaymentMethodsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x0eJoinPlanResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0f\n\x07\x62\x61lance\x18\x02 \x01(\x01\x12\x10\n\x08planName\x18\x03 \x01(\t\x12\x17\n\x0fplanDescription\x18\x04 \x01(\t\x12\x33\n\nexpireTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12\x31\n\x0bpaymentInfo\x18\x06 \x01(\x0b\x32\x17.clouddrive.PaymentInfoH\x01\x88\x01\x01\x42\r\n\x0b_expireTimeB\x0e\n\x0c_paymentInfo\"\x99\x01\n\tPromotion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tcloudName\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x15\n\x08subTitle\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\r\n\x05rules\x18\x05 \x01(\t\x12\x13\n\x06notice\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x0b\n\x03url\x18\x07 \x01(\tB\x0b\n\t_subTitleB\t\n\x07_notice\"@\n\x13GetPromotionsResult\x12)\n\npromotions\x18\x01 \x03(\x0b\x32\x15.clouddrive.Promotion\"-\n\rOfflineStatus\x12\r\n\x05quota\x18\x01 \x01(\r\x12\r\n\x05total\x18\x02 \x01(\r\"\xcf\x01\n\x0bOfflineFile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x04\x12\x0b\n\x03url\x18\x03 \x01(\t\x12-\n\x06status\x18\x04 \x01(\x0e\x32\x1d.clouddrive.OfflineFileStatus\x12\x10\n\x08infoHash\x18\x05 \x01(\t\x12\x0e\n\x06\x66ileId\x18\x06 \x01(\t\x12\x10\n\x08\x61\x64\x64_time\x18\x07 \x01(\x04\x12\x10\n\x08parentId\x18\x08 \x01(\t\x12\x13\n\x0bpercendDone\x18\t \x01(\x01\x12\r\n\x05peers\x18\n \x01(\x04\"T\n\x19OfflineFileListAllRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x16\n\x0e\x63loudAccountId\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\"\xc1\x01\n\x18OfflineFileListAllResult\x12\x0e\n\x06pageNo\x18\x01 \x01(\r\x12\x14\n\x0cpageRowCount\x18\x02 \x01(\r\x12\x11\n\tpageCount\x18\x03 \x01(\r\x12\x12\n\ntotalCount\x18\x04 \x01(\r\x12)\n\x06status\x18\x05 \x01(\x0b\x32\x19.clouddrive.OfflineStatus\x12-\n\x0cofflineFiles\x18\x06 \x03(\x0b\x32\x17.clouddrive.OfflineFile\"q\n\x15OfflineFileListResult\x12-\n\x0cofflineFiles\x18\x01 \x03(\x0b\x32\x17.clouddrive.OfflineFile\x12)\n\x06status\x18\x02 \x01(\x0b\x32\x19.clouddrive.OfflineStatus\"D\n\x17\x42indCloudAccountRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x16\n\x0e\x63loudAccountId\x18\x02 \x01(\t\"N\n\x16TransferBalanceRequest\x12\x12\n\ntoUserName\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x10\n\x08password\x18\x03 \x01(\t\"U\n\x1a\x43hangeUserNameEmailRequest\x12\x13\n\x0bnewUserName\x18\x01 \x01(\t\x12\x10\n\x08newEmail\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"\xbb\x02\n\nBalanceLog\x12\x16\n\x0e\x62\x61lance_before\x18\x01 \x01(\x01\x12\x15\n\rbalance_after\x18\x02 \x01(\x01\x12\x16\n\x0e\x62\x61lance_change\x18\x03 \x01(\x01\x12\x41\n\toperation\x18\x04 \x01(\x0e\x32..clouddrive.BalanceLog.BalancceChangeOperation\x12\x18\n\x10operation_source\x18\x05 \x01(\t\x12\x14\n\x0coperation_id\x18\x06 \x01(\t\x12\x32\n\x0eoperation_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"?\n\x17\x42\x61lancceChangeOperation\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07\x44\x65posit\x10\x01\x12\n\n\x06Refund\x10\x02\"8\n\x10\x42\x61lanceLogResult\x12$\n\x04logs\x18\x01 \x03(\x0b\x32\x16.clouddrive.BalanceLog\"<\n\x16\x43heckFinalPriceRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x12\n\ncouponCode\x18\x02 \x01(\t\"\xab\x01\n\x15\x43heckFinalPriceResult\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x11\n\tplanPrice\x18\x02 \x01(\x01\x12\x13\n\x0buserBalance\x18\x03 \x01(\x01\x12\x1c\n\x14\x63ouponDiscountAmount\x18\x04 \x01(\x01\x12\x18\n\x0b\x63ouponError\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nfinalPrice\x18\x06 \x01(\x01\x42\x0e\n\x0c_couponError\"V\n\x19\x43heckActivationCodeResult\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x10\n\x08planName\x18\x02 \x01(\t\x12\x17\n\x0fplanDescription\x18\x03 \x01(\t\"<\n\x16\x43heckCouponCodeRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x12\n\ncouponCode\x18\x02 \x01(\t\"u\n\x10\x43ouponCodeResult\x12\x12\n\ncouponCode\x18\x01 \x01(\t\x12\x19\n\x11\x63ouponDescription\x18\x02 \x01(\t\x12\x14\n\x0cisPercentage\x18\x03 \x01(\x08\x12\x1c\n\x14\x63ouponDiscountAmount\x18\x04 \x01(\x01\"\x8f\x01\n\x0e\x46ileBackupRule\x12\x14\n\nextensions\x18\x01 \x01(\tH\x00\x12\x13\n\tfileNames\x18\x02 \x01(\tH\x00\x12\x0f\n\x05regex\x18\x03 \x01(\tH\x00\x12\x11\n\x07minSize\x18\x04 \x01(\x04H\x00\x12\x11\n\tisEnabled\x18\x64 \x01(\x08\x12\x13\n\x0bisBlackList\x18\x65 \x01(\x08\x42\x06\n\x04rule\"\x8b\x01\n\x11\x42\x61\x63kupDestination\x12\x17\n\x0f\x64\x65stinationPath\x18\x01 \x01(\t\x12\x11\n\tisEnabled\x18\x02 \x01(\x08\x12\x37\n\x0elastFinishTime\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x42\x11\n\x0f_lastFinishTime\"\xeb\x02\n\x06\x42\x61\x63kup\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x33\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x1d.clouddrive.BackupDestination\x12\x33\n\x0f\x66ileBackupRules\x18\x03 \x03(\x0b\x32\x1a.clouddrive.FileBackupRule\x12\x34\n\x0f\x66ileReplaceRule\x18\x04 \x01(\x0e\x32\x1b.clouddrive.FileReplaceRule\x12\x32\n\x0e\x66ileDeleteRule\x18\x05 \x01(\x0e\x32\x1a.clouddrive.FileDeleteRule\x12\x11\n\tisEnabled\x18\x06 \x01(\x08\x12\x1e\n\x16\x66ileSystemWatchEnabled\x18\x07 \x01(\x08\x12\"\n\x1awalkingThroughIntervalSecs\x18\x08 \x01(\x03\x12\"\n\x1a\x66orceWalkingThroughOnStart\x18\t \x01(\x08\"\xf3\x02\n\x0c\x42\x61\x63kupStatus\x12\"\n\x06\x62\x61\x63kup\x18\x01 \x01(\x0b\x32\x12.clouddrive.Backup\x12/\n\x06status\x18\x02 \x01(\x0e\x32\x1f.clouddrive.BackupStatus.Status\x12\x15\n\rstatusMessage\x18\x03 \x01(\t\x12?\n\rwatcherStatus\x18\x04 \x01(\x0e\x32(.clouddrive.BackupStatus.FileWatchStatus\x12\x1c\n\x14watcherStatusMessage\x18\x05 \x01(\t\"?\n\x06Status\x12\x08\n\x04Idle\x10\x00\x12\x12\n\x0eWalkingThrough\x10\x01\x12\t\n\x05\x45rror\x10\x02\x12\x0c\n\x08\x44isabled\x10\x03\"W\n\x0f\x46ileWatchStatus\x12\x0f\n\x0bWatcherIdle\x10\x00\x12\x0c\n\x08Watching\x10\x01\x12\x10\n\x0cWatcherError\x10\x02\x12\x13\n\x0fWatcherDisabled\x10\x03\"7\n\nBackupList\x12)\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32\x18.clouddrive.BackupStatus\"\xb6\x03\n\x13\x42\x61\x63kupModifyRequest\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x33\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x1d.clouddrive.BackupDestination\x12\x33\n\x0f\x66ileBackupRules\x18\x03 \x03(\x0b\x32\x1a.clouddrive.FileBackupRule\x12\x39\n\x0f\x66ileReplaceRule\x18\x04 \x01(\x0e\x32\x1b.clouddrive.FileReplaceRuleH\x00\x88\x01\x01\x12\x37\n\x0e\x66ileDeleteRule\x18\x05 \x01(\x0e\x32\x1a.clouddrive.FileDeleteRuleH\x01\x88\x01\x01\x12#\n\x16\x66ileSystemWatchEnabled\x18\x06 \x01(\x08H\x02\x88\x01\x01\x12\'\n\x1awalkingThroughIntervalSecs\x18\x07 \x01(\x03H\x03\x88\x01\x01\x42\x12\n\x10_fileReplaceRuleB\x11\n\x0f_fileDeleteRuleB\x19\n\x17_fileSystemWatchEnabledB\x1d\n\x1b_walkingThroughIntervalSecs\"@\n\x17\x42\x61\x63kupSetEnabledRequest\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x11\n\tisEnabled\x18\x02 \x01(\x08*h\n\x15QRCodeScanMessageType\x12\x0e\n\nSHOW_IMAGE\x10\x00\x12\x16\n\x12SHOW_IMAGE_CONTENT\x10\x01\x12\x11\n\rCHANGE_STATUS\x10\x02\x12\t\n\x05\x43LOSE\x10\x03\x12\t\n\x05\x45RROR\x10\x04*&\n\rUpdateChannel\x12\x0b\n\x07Release\x10\x00\x12\x08\n\x04\x42\x65ta\x10\x01*|\n\x11OfflineFileStatus\x12\x10\n\x0cOFFLINE_INIT\x10\x00\x12\x17\n\x13OFFLINE_DOWNLOADING\x10\x01\x12\x14\n\x10OFFLINE_FINISHED\x10\x02\x12\x11\n\rOFFLINE_ERROR\x10\x03\x12\x13\n\x0fOFFLINE_UNKNOWN\x10\x04*B\n\x0f\x46ileReplaceRule\x12\x08\n\x04Skip\x10\x00\x12\r\n\tOverwrite\x10\x01\x12\x16\n\x12KeepHistoryVersion\x10\x02*M\n\x0e\x46ileDeleteRule\x12\n\n\x06\x44\x65lete\x10\x00\x12\x0b\n\x07Recycle\x10\x01\x12\x08\n\x04Keep\x10\x02\x12\x18\n\x14MoveToVersionHistory\x10\x03\x32\xd0H\n\x11\x43loudDriveFileSrv\x12K\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a .clouddrive.CloudDriveSystemInfo\"\x00\x12?\n\x08GetToken\x12\x1b.clouddrive.GetTokenRequest\x1a\x14.clouddrive.JWTToken\"\x00\x12H\n\x05Login\x12\x1c.clouddrive.UserLoginRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12N\n\x08Register\x12\x1f.clouddrive.UserRegisterRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12[\n\x15SendResetAccountEmail\x12(.clouddrive.SendResetAccountEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0cResetAccount\x12\x1f.clouddrive.ResetAccountRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\x10SendConfirmEmail\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0c\x43onfirmEmail\x12\x1f.clouddrive.ConfirmEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x10GetAccountStatus\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.AccountStatusResult\"\x00\x12L\n\x0bGetSubFiles\x12\x1e.clouddrive.ListSubFileRequest\x1a\x19.clouddrive.SubFilesReply\"\x00\x30\x01\x12L\n\x10GetSearchResults\x12\x19.clouddrive.SearchRequest\x1a\x19.clouddrive.SubFilesReply\"\x00\x30\x01\x12Q\n\x0e\x46indFileByPath\x12!.clouddrive.FindFileByPathRequest\x1a\x1a.clouddrive.CloudDriveFile\"\x00\x12Q\n\x0c\x43reateFolder\x12\x1f.clouddrive.CreateFolderRequest\x1a\x1e.clouddrive.CreateFolderResult\"\x00\x12N\n\nRenameFile\x12\x1d.clouddrive.RenameFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12P\n\x0bRenameFiles\x12\x1e.clouddrive.RenameFilesRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12J\n\x08MoveFile\x12\x1b.clouddrive.MoveFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12H\n\nDeleteFile\x12\x17.clouddrive.FileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12S\n\x15\x44\x65leteFilePermanently\x12\x17.clouddrive.FileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12N\n\x0b\x44\x65leteFiles\x12\x1c.clouddrive.MultiFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12Y\n\x16\x44\x65leteFilesPermanently\x12\x1c.clouddrive.MultiFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12W\n\x0f\x41\x64\x64OfflineFiles\x12!.clouddrive.AddOfflineFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12V\n\x16ListOfflineFilesByPath\x12\x17.clouddrive.FileRequest\x1a!.clouddrive.OfflineFileListResult\"\x00\x12\x64\n\x13ListAllOfflineFiles\x12%.clouddrive.OfflineFileListAllRequest\x1a$.clouddrive.OfflineFileListAllResult\"\x00\x12V\n\x17GetFileDetailProperties\x12\x17.clouddrive.FileRequest\x1a .clouddrive.FileDetailProperties\"\x00\x12@\n\x0cGetSpaceInfo\x12\x17.clouddrive.FileRequest\x1a\x15.clouddrive.SpaceInfo\"\x00\x12N\n\x13GetCloudMemberships\x12\x17.clouddrive.FileRequest\x1a\x1c.clouddrive.CloudMemberships\"\x00\x12\x43\n\x0eGetRuntimeInfo\x12\x16.google.protobuf.Empty\x1a\x17.clouddrive.RuntimeInfo\"\x00\x12?\n\x0eGetRunningInfo\x12\x16.google.protobuf.Empty\x1a\x13.clouddrive.RunInfo\"\x00\x12J\n\x06Logout\x12\x1d.clouddrive.UserLogoutRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12R\n\x15\x43\x61nAddMoreMountPoints\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12L\n\x0eGetMountPoints\x12\x16.google.protobuf.Empty\x1a .clouddrive.GetMountPointsResult\"\x00\x12H\n\rAddMountPoint\x12\x17.clouddrive.MountOption\x1a\x1c.clouddrive.MountPointResult\"\x00\x12Q\n\x10RemoveMountPoint\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12\x46\n\x05Mount\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12H\n\x07Unmount\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12W\n\x10UpdateMountPoint\x12#.clouddrive.UpdateMountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12`\n\x18GetAvailableDriveLetters\x12\x16.google.protobuf.Empty\x1a*.clouddrive.GetAvailableDriveLettersResult\"\x00\x12N\n\x0fHasDriveLetters\x12\x16.google.protobuf.Empty\x1a!.clouddrive.HasDriveLettersResult\"\x00\x12_\n\x10LocalGetSubFiles\x12#.clouddrive.LocalGetSubFilesRequest\x1a\".clouddrive.LocalGetSubFilesResult\"\x00\x30\x01\x12P\n\x10GetAllTasksCount\x12\x16.google.protobuf.Empty\x1a\".clouddrive.GetAllTasksCountResult\"\x00\x12X\n\x14GetDownloadFileCount\x12\x16.google.protobuf.Empty\x1a&.clouddrive.GetDownloadFileCountResult\"\x00\x12V\n\x13GetDownloadFileList\x12\x16.google.protobuf.Empty\x1a%.clouddrive.GetDownloadFileListResult\"\x00\x12T\n\x12GetUploadFileCount\x12\x16.google.protobuf.Empty\x1a$.clouddrive.GetUploadFileCountResult\"\x00\x12`\n\x11GetUploadFileList\x12$.clouddrive.GetUploadFileListRequest\x1a#.clouddrive.GetUploadFileListResult\"\x00\x12H\n\x14\x43\x61ncelAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x11\x43\x61ncelUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\x13PauseAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x10PauseUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x14ResumeAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x11ResumeUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x13\x43\x61nAddMoreCloudApis\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12\x64\n\x19\x41PILogin115Editthiscookie\x12).clouddrive.Login115EditthiscookieRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12Y\n\x11\x41PILogin115QRCode\x12!.clouddrive.Login115QrCodeRequest\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12\x62\n\x18\x41PILoginAliyundriveOAuth\x12(.clouddrive.LoginAliyundriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12p\n\x1f\x41PILoginAliyundriveRefreshtoken\x12/.clouddrive.LoginAliyundriveRefreshtokenRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12i\n\x19\x41PILoginAliyunDriveQRCode\x12).clouddrive.LoginAliyundriveQRCodeRequest\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12\\\n\x15\x41PILoginBaiduPanOAuth\x12%.clouddrive.LoginBaiduPanOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12\\\n\x15\x41PILoginOneDriveOAuth\x12%.clouddrive.LoginOneDriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12\x62\n\x18\x41piLoginGoogleDriveOAuth\x12(.clouddrive.LoginGoogleDriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12p\n\x1f\x41piLoginGoogleDriveRefreshToken\x12/.clouddrive.LoginGoogleDriveRefreshTokenRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12N\n\x11\x41PILogin189QRCode\x12\x16.google.protobuf.Empty\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12L\n\x0e\x41PILoginPikPak\x12\x1c.clouddrive.UserLoginRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12N\n\x0e\x41PILoginWebDav\x12\x1e.clouddrive.LoginWebDavRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12T\n\x11\x41PIAddLocalFolder\x12!.clouddrive.AddLocalFolderRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12V\n\x0eRemoveCloudAPI\x12!.clouddrive.RemoveCloudAPIRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12\x45\n\x0fGetAllCloudApis\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.CloudAPIList\"\x00\x12W\n\x11GetCloudAPIConfig\x12$.clouddrive.GetCloudAPIConfigRequest\x1a\x1a.clouddrive.CloudAPIConfig\"\x00\x12S\n\x11SetCloudAPIConfig\x12$.clouddrive.SetCloudAPIConfigRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x11GetSystemSettings\x12\x16.google.protobuf.Empty\x1a\x1a.clouddrive.SystemSettings\"\x00\x12I\n\x11SetSystemSettings\x12\x1a.clouddrive.SystemSettings\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x13SetDirCacheTimeSecs\x12\".clouddrive.SetDirCacheTimeRequest\x1a\x16.google.protobuf.Empty\"\x00\x12y\n\x1cGetEffectiveDirCacheTimeSecs\x12+.clouddrive.GetEffectiveDirCacheTimeRequest\x1a*.clouddrive.GetEffectiveDirCacheTimeResult\"\x00\x12T\n\x10GetOpenFileTable\x12#.clouddrive.GetOpenFileTableRequest\x1a\x19.clouddrive.OpenFileTable\"\x00\x12G\n\x10GetDirCacheTable\x12\x16.google.protobuf.Empty\x1a\x19.clouddrive.DirCacheTable\"\x00\x12L\n\x17GetReferencedEntryPaths\x12\x17.clouddrive.FileRequest\x1a\x16.clouddrive.StringList\"\x00\x12G\n\x10GetTempFileTable\x12\x16.google.protobuf.Empty\x1a\x19.clouddrive.TempFileTable\"\x00\x12P\n\x0ePushTaskChange\x12\x16.google.protobuf.Empty\x1a\".clouddrive.GetAllTasksCountResult\"\x00\x30\x01\x12L\n\x16GetCloudDrive1UserData\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.StringResult\"\x00\x12\x42\n\x0eRestartService\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0fShutdownService\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\tHasUpdate\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.UpdateResult\"\x00\x12\x41\n\x0b\x43heckUpdate\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.UpdateResult\"\x00\x12\x42\n\x0e\x44ownloadUpdate\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x0cUpdateSystem\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x42\n\x0bGetMetaData\x12\x17.clouddrive.FileRequest\x1a\x18.clouddrive.FileMetaData\"\x00\x12\x46\n\x0fGetOriginalPath\x12\x17.clouddrive.FileRequest\x1a\x18.clouddrive.StringResult\"\x00\x12V\n\x0e\x43hangePassword\x12!.clouddrive.ChangePasswordRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12K\n\nCreateFile\x12\x1d.clouddrive.CreateFileRequest\x1a\x1c.clouddrive.CreateFileResult\"\x00\x12L\n\tCloseFile\x12\x1c.clouddrive.CloseFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12R\n\x11WriteToFileStream\x12\x1c.clouddrive.WriteFileRequest\x1a\x1b.clouddrive.WriteFileResult\"\x00(\x01\x12J\n\x0bWriteToFile\x12\x1c.clouddrive.WriteFileRequest\x1a\x1b.clouddrive.WriteFileResult\"\x00\x12J\n\rGetPromotions\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.GetPromotionsResult\"\x00\x12I\n\x15UpdatePromotionResult\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x12GetCloudDrivePlans\x12\x16.google.protobuf.Empty\x1a$.clouddrive.GetCloudDrivePlansResult\"\x00\x12\x45\n\x08JoinPlan\x12\x1b.clouddrive.JoinPlanRequest\x1a\x1a.clouddrive.JoinPlanResult\"\x00\x12Q\n\x10\x42indCloudAccount\x12#.clouddrive.BindCloudAccountRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x0fTransferBalance\x12\".clouddrive.TransferBalanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x0b\x43hangeEmail\x12&.clouddrive.ChangeUserNameEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\rGetBalanceLog\x12\x16.google.protobuf.Empty\x1a\x1c.clouddrive.BalanceLogResult\"\x00\x12W\n\x13\x43heckActivationCode\x12\x17.clouddrive.StringValue\x1a%.clouddrive.CheckActivationCodeResult\"\x00\x12\x45\n\x0c\x41\x63tivatePlan\x12\x17.clouddrive.StringValue\x1a\x1a.clouddrive.JoinPlanResult\"\x00\x12U\n\x0f\x43heckCouponCode\x12\".clouddrive.CheckCouponCodeRequest\x1a\x1c.clouddrive.CouponCodeResult\"\x00\x12\x44\n\x0fGetReferralCode\x12\x16.google.protobuf.Empty\x1a\x17.clouddrive.StringValue\"\x00\x12@\n\x0c\x42\x61\x63kupGetAll\x12\x16.google.protobuf.Empty\x1a\x16.clouddrive.BackupList\"\x00\x12\x39\n\tBackupAdd\x12\x12.clouddrive.Backup\x1a\x16.google.protobuf.Empty\"\x00\x12\x41\n\x0c\x42\x61\x63kupRemove\x12\x17.clouddrive.StringValue\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x0c\x42\x61\x63kupUpdate\x12\x12.clouddrive.Backup\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14\x42\x61\x63kupAddDestination\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x17\x42\x61\x63kupRemoveDestination\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x10\x42\x61\x63kupSetEnabled\x12#.clouddrive.BackupSetEnabledRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1f\x42\x61\x63kupSetFileSystemWatchEnabled\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x16\x42\x61\x63kupUpdateStrategies\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x1b\x42\x61\x63kupRestartWalkingThrough\x12\x17.clouddrive.StringValue\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\x11\x43\x61nAddMoreBackups\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x42\x17\xaa\x02\x14\x43loudDriveSrv.Protosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x43loudDrive.proto\x12\nclouddrive\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"5\n\x0fGetTokenRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"p\n\x08JWTToken\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12.\n\nexpiration\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x1b\n\x0b\x46ileRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\" \n\x10MultiFileRequest\x12\x0c\n\x04path\x18\x01 \x03(\t\"U\n\x13\x46ileOperationResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\x12\x17\n\x0fresultFilePaths\x18\x03 \x03(\t\"\x1e\n\x0cStringResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"&\n\x14UnmountArchiveResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"d\n\x12ListSubFileRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x14\n\x0c\x66orceRefresh\x18\x02 \x01(\x08\x12\x19\n\x0c\x63heckExpires\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x0f\n\r_checkExpires\"Z\n\rSearchRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tsearchFor\x18\x02 \x01(\t\x12\x14\n\x0c\x66orceRefresh\x18\x03 \x01(\x08\x12\x12\n\nfuzzyMatch\x18\x04 \x01(\x08\"7\n\x15\x41\x64\x64OfflineFileRequest\x12\x0c\n\x04urls\x18\x01 \x01(\t\x12\x10\n\x08toFolder\x18\x02 \x01(\t\"W\n\x14\x41\x64\x64SharedLinkRequest\x12\x15\n\rsharedLinkUrl\x18\x01 \x01(\t\x12\x16\n\x0esharedPassword\x18\x02 \x01(\t\x12\x10\n\x08toFolder\x18\x03 \x01(\t\"=\n\rSubFilesReply\x12,\n\x08subFiles\x18\x01 \x03(\x0b\x32\x1a.clouddrive.CloudDriveFile\"9\n\x15\x46indFileByPathRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"=\n\x13\x43reateFolderRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x12\n\nfolderName\x18\x02 \x01(\t\"x\n\x12\x43reateFolderResult\x12\x31\n\rfolderCreated\x18\x01 \x01(\x0b\x32\x1a.clouddrive.CloudDriveFile\x12/\n\x06result\x18\x02 \x01(\x0b\x32\x1f.clouddrive.FileOperationResult\"9\n\x11\x43reateFileRequest\x12\x12\n\nparentPath\x18\x01 \x01(\t\x12\x10\n\x08\x66ileName\x18\x02 \x01(\t\"&\n\x10\x43reateFileResult\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\"&\n\x10\x43loseFileRequest\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\"9\n\x0fMoveFileRequest\x12\x14\n\x0ctheFilePaths\x18\x01 \x03(\t\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\"k\n\x10WriteFileRequest\x12\x12\n\nfileHandle\x18\x01 \x01(\x04\x12\x10\n\x08startPos\x18\x02 \x01(\x04\x12\x0e\n\x06length\x18\x03 \x01(\x04\x12\x0e\n\x06\x62uffer\x18\x04 \x01(\x0c\x12\x11\n\tcloseFile\x18\x05 \x01(\x08\"\'\n\x0fWriteFileResult\x12\x14\n\x0c\x62ytesWritten\x18\x01 \x01(\x04\"9\n\x11RenameFileRequest\x12\x13\n\x0btheFilePath\x18\x01 \x01(\t\x12\x0f\n\x07newName\x18\x02 \x01(\t\"H\n\x12RenameFilesRequest\x12\x32\n\x0brenameFiles\x18\x01 \x03(\x0b\x32\x1d.clouddrive.RenameFileRequest\"\xcc\x08\n\x0e\x43loudDriveFile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x66ullPathName\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x35\n\x08\x66ileType\x18\x05 \x01(\x0e\x32#.clouddrive.CloudDriveFile.FileType\x12.\n\ncreateTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\twriteTime\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\naccessTime\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x08\x43loudAPI\x18\t \x01(\x0b\x32\x14.clouddrive.CloudAPI\x12\x14\n\x0cthumbnailUrl\x18\n \x01(\t\x12\x12\n\npreviewUrl\x18\x0b \x01(\t\x12\x14\n\x0coriginalPath\x18\x0e \x01(\t\x12\x13\n\x0bisDirectory\x18\x1e \x01(\x08\x12\x0e\n\x06isRoot\x18\x1f \x01(\x08\x12\x13\n\x0bisCloudRoot\x18  \x01(\x08\x12\x18\n\x10isCloudDirectory\x18! \x01(\x08\x12\x13\n\x0bisCloudFile\x18\" \x01(\x08\x12\x16\n\x0eisSearchResult\x18# \x01(\x08\x12\x13\n\x0bisForbidden\x18$ \x01(\x08\x12\x0f\n\x07isLocal\x18% \x01(\x08\x12\x10\n\x08\x63\x61nMount\x18< \x01(\x08\x12\x12\n\ncanUnmount\x18= \x01(\x08\x12#\n\x1b\x63\x61nDirectAccessThumbnailURL\x18> \x01(\x08\x12\x11\n\tcanSearch\x18? \x01(\x08\x12\x1b\n\x13hasDetailProperties\x18@ \x01(\x08\x12:\n\x10\x64\x65tailProperties\x18\x41 \x01(\x0b\x32 .clouddrive.FileDetailProperties\x12\x1a\n\x12\x63\x61nOfflineDownload\x18\x42 \x01(\x08\x12\x17\n\x0f\x63\x61nAddShareLink\x18\x43 \x01(\x08\x12#\n\x16\x64irCacheTimeToLiveSecs\x18\x44 \x01(\x04H\x00\x88\x01\x01\x12\x1c\n\x14\x63\x61nDeletePermanently\x18\x45 \x01(\x08\x12>\n\nfileHashes\x18\x46 \x03(\x0b\x32*.clouddrive.CloudDriveFile.FileHashesEntry\x1a\x31\n\x0f\x46ileHashesEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\".\n\x08\x46ileType\x12\r\n\tDirectory\x10\x00\x12\x08\n\x04\x46ile\x10\x01\x12\t\n\x05Other\x10\x02\":\n\x08HashType\x12\x0b\n\x07Unknown\x10\x00\x12\x07\n\x03Md5\x10\x01\x12\x08\n\x04Sha1\x10\x02\x12\x0e\n\nPikPakSha1\x10\x03\x42\x19\n\x17_dirCacheTimeToLiveSecs\"E\n\tSpaceInfo\x12\x12\n\ntotalSpace\x18\x01 \x01(\x03\x12\x11\n\tusedSpace\x18\x02 \x01(\x03\x12\x11\n\tfreeSpace\x18\x03 \x01(\x03\"N\n\x08\x43loudAPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x10\n\x08nickName\x18\x03 \x01(\t\x12\x10\n\x08isLocked\x18\x04 \x01(\x08\"\x85\x01\n\x0f\x43loudMembership\x12\x10\n\x08identity\x18\x01 \x01(\t\x12\x33\n\nexpireTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12\x12\n\x05level\x18\x03 \x01(\tH\x01\x88\x01\x01\x42\r\n\x0b_expireTimeB\x08\n\x06_level\"D\n\x10\x43loudMemberships\x12\x30\n\x0bmemberships\x18\x01 \x03(\x0b\x32\x1b.clouddrive.CloudMembership\"\x94\x01\n\x14\x46ileDetailProperties\x12\x16\n\x0etotalFileCount\x18\x01 \x01(\x03\x12\x18\n\x10totalFolderCount\x18\x02 \x01(\x03\x12\x11\n\ttotalSize\x18\x03 \x01(\x03\x12\x0f\n\x07isFaved\x18\x04 \x01(\x08\x12\x10\n\x08isShared\x18\x05 \x01(\x08\x12\x14\n\x0coriginalPath\x18\x06 \x01(\t\"y\n\x0c\x46ileMetaData\x12\x38\n\x08metadata\x18\x01 \x03(\x0b\x32&.clouddrive.FileMetaData.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"9\n\x14\x43loudDriveSystemInfo\x12\x0f\n\x07IsLogin\x18\x01 \x01(\x08\x12\x10\n\x08UserName\x18\x02 \x01(\t\"N\n\x10UserLoginRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x16\n\x0esynDataToCloud\x18\x03 \x01(\x08\"9\n\x13UserRegisterRequest\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11UserLogoutRequest\x12\x19\n\x11logoutFromCloudFS\x18\x01 \x01(\x08\"A\n\x15\x43hangePasswordRequest\x12\x13\n\x0boldPassword\x18\x01 \x01(\t\x12\x13\n\x0bnewPassword\x18\x02 \x01(\t\"\xb4\x01\n\x13\x41\x63\x63ountStatusResult\x12\x10\n\x08userName\x18\x01 \x01(\t\x12\x16\n\x0e\x65mailConfirmed\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x63\x63ountBalance\x18\x03 \x01(\x01\x12,\n\x0b\x61\x63\x63ountPlan\x18\x04 \x01(\x0b\x32\x17.clouddrive.AccountPlan\x12-\n\x0c\x61\x63\x63ountRoles\x18\x05 \x03(\x0b\x32\x17.clouddrive.AccountRole\"\x97\x01\n\x0b\x41\x63\x63ountPlan\x12\x10\n\x08planName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0f\x66ontAwesomeIcon\x18\x03 \x01(\t\x12\x1b\n\x13\x64urationDescription\x18\x04 \x01(\t\x12+\n\x07\x65ndTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"R\n\x0b\x41\x63\x63ountRole\x12\x10\n\x08roleName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x12\n\x05value\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_value\"c\n\x0bRuntimeInfo\x12\x13\n\x0bproductName\x18\x01 \x01(\t\x12\x16\n\x0eproductVersion\x18\x02 \x01(\t\x12\x17\n\x0f\x43loudAPIVersion\x18\x03 \x01(\t\x12\x0e\n\x06osInfo\x18\x04 \x01(\t\"\x83\x01\n\x07RunInfo\x12\x10\n\x08\x63puUsage\x18\x01 \x01(\x01\x12\x12\n\nmemUsageKB\x18\x02 \x01(\x04\x12\x0e\n\x06uptime\x18\x03 \x01(\x01\x12\x14\n\x0c\x66hTableCount\x18\x04 \x01(\x04\x12\x15\n\rdirCacheCount\x18\x05 \x01(\x04\x12\x15\n\rtempFileCount\x18\x06 \x01(\x04\"\xaa\x01\n\x0bMountOption\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12\x11\n\tsourceDir\x18\x02 \x01(\t\x12\x12\n\nlocalMount\x18\x03 \x01(\x08\x12\x10\n\x08readOnly\x18\x04 \x01(\x08\x12\x11\n\tautoMount\x18\x05 \x01(\x08\x12\x0b\n\x03uid\x18\x06 \x01(\r\x12\x0b\n\x03gid\x18\x07 \x01(\r\x12\x13\n\x0bpermissions\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\xc2\x01\n\nMountPoint\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12\x11\n\tsourceDir\x18\x02 \x01(\t\x12\x12\n\nlocalMount\x18\x03 \x01(\x08\x12\x10\n\x08readOnly\x18\x04 \x01(\x08\x12\x11\n\tautoMount\x18\x05 \x01(\x08\x12\x0b\n\x03uid\x18\x06 \x01(\r\x12\x0b\n\x03gid\x18\x07 \x01(\r\x12\x13\n\x0bpermissions\x18\x08 \x01(\t\x12\x11\n\tisMounted\x18\t \x01(\x08\x12\x12\n\nfailReason\x18\n \x01(\t\"\'\n\x11MountPointRequest\x12\x12\n\nMountPoint\x18\x01 \x01(\t\"C\n\x14GetMountPointsResult\x12+\n\x0bmountPoints\x18\x01 \x03(\x0b\x32\x16.clouddrive.MountPoint\"7\n\x10MountPointResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x12\n\nfailReason\x18\x02 \x01(\t\"^\n\x17UpdateMountPointRequest\x12\x12\n\nmountPoint\x18\x01 \x01(\t\x12/\n\x0enewMountOption\x18\x02 \x01(\x0b\x32\x17.clouddrive.MountOption\"<\n\x1fGetAvailableDriveLettersRequest\x12\x19\n\x11includeCloudDrive\x18\x01 \x01(\x08\"6\n\x1eGetAvailableDriveLettersResult\x12\x14\n\x0c\x64riveLetters\x18\x01 \x03(\t\"0\n\x15HasDriveLettersResult\x12\x17\n\x0fhasDriveLetters\x18\x01 \x01(\x08\"}\n\x17LocalGetSubFilesRequest\x12\x14\n\x0cparentFolder\x18\x01 \x01(\t\x12\x12\n\nfolderOnly\x18\x02 \x01(\x08\x12\x19\n\x11includeCloudDrive\x18\x03 \x01(\x08\x12\x1d\n\x15includeAvailableDrive\x18\x04 \x01(\x08\"*\n\x16LocalGetSubFilesResult\x12\x10\n\x08subFiles\x18\x01 \x03(\t\"(\n\x0bPushMessage\x12\x19\n\x11\x63louddriveVersion\x18\x01 \x01(\t\"\x85\x01\n\x16GetAllTasksCountResult\x12\x15\n\rdownloadCount\x18\x01 \x01(\r\x12\x13\n\x0buploadCount\x18\x02 \x01(\r\x12,\n\x0bpushMessage\x18\x03 \x01(\x0b\x32\x17.clouddrive.PushMessage\x12\x11\n\thasUpdate\x18\x04 \x01(\x08\"/\n\x1aGetDownloadFileCountResult\x12\x11\n\tfileCount\x18\x01 \x01(\r\"\x9b\x01\n\x10\x44ownloadFileInfo\x12\x10\n\x08\x66ilePath\x18\x01 \x01(\t\x12\x12\n\nfileLength\x18\x02 \x01(\x04\x12\x17\n\x0ftotalBufferUsed\x18\x03 \x01(\x04\x12\x1b\n\x13\x64ownloadThreadCount\x18\x04 \x01(\r\x12\x0f\n\x07process\x18\x05 \x03(\t\x12\x1a\n\x12\x64\x65tailDownloadInfo\x18\x06 \x01(\t\"n\n\x19GetDownloadFileListResult\x12\x1c\n\x14globalBytesPerSecond\x18\x01 \x01(\x01\x12\x33\n\rdownloadFiles\x18\x04 \x03(\x0b\x32\x1c.clouddrive.DownloadFileInfo\"-\n\x18GetUploadFileCountResult\x12\x11\n\tfileCount\x18\x01 \x01(\r\"|\n\x0eUploadFileInfo\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\x17\n\x0ftransferedBytes\x18\x04 \x01(\x04\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x06 \x01(\t\"d\n\x18GetUploadFileListRequest\x12\x0e\n\x06getAll\x18\x01 \x01(\x08\x12\x14\n\x0citemsPerPage\x18\x02 \x01(\r\x12\x12\n\npageNumber\x18\x03 \x01(\r\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"^\n\x17GetUploadFileListResult\x12\x12\n\ntotalCount\x18\x01 \x01(\r\x12/\n\x0buploadFiles\x18\x02 \x03(\x0b\x32\x1a.clouddrive.UploadFileInfo\"+\n\x1bMultpleUploadFileKeyRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\"=\n\x1dLogin115EditthiscookieRequest\x12\x1c\n\x14\x65\x64itThiscookieString\x18\x01 \x01(\t\"G\n\x15Login115QrCodeRequest\x12\x1b\n\x0eplatformString\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_platformString\"_\n\x1cLoginAliyundriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"O\n#LoginAliyundriveRefreshtokenRequest\x12\x14\n\x0crefreshToken\x18\x01 \x01(\t\x12\x12\n\nuseOpenAPI\x18\x02 \x01(\x08\"3\n\x1dLoginAliyundriveQRCodeRequest\x12\x12\n\nuseOpenAPI\x18\x01 \x01(\x08\"\\\n\x19LoginBaiduPanOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"\\\n\x19LoginOneDriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"_\n\x1cLoginGoogleDriveOAuthRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x04\"f\n#LoginGoogleDriveRefreshTokenRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x15\n\rclient_secret\x18\x02 \x01(\t\x12\x15\n\rrefresh_token\x18\x03 \x01(\t\"K\n\x12LoginWebDavRequest\x12\x11\n\tserverUrl\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"7\n\x0e\x41PILoginResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"0\n\x15\x41\x64\x64LocalFolderRequest\x12\x17\n\x0flocalFolderPath\x18\x01 \x01(\t\"U\n\x15RemoveCloudAPIRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12\x17\n\x0fpermanentRemove\x18\x03 \x01(\x08\"?\n\x18GetCloudAPIConfigRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\"2\n\x0c\x43loudAPIList\x12\"\n\x04\x61pis\x18\x01 \x03(\x0b\x32\x14.clouddrive.CloudAPI\"\xc8\x01\n\x0e\x43loudAPIConfig\x12\x1a\n\x12maxDownloadThreads\x18\x01 \x01(\r\x12\x17\n\x0fminReadLengthKB\x18\x02 \x01(\x04\x12\x17\n\x0fmaxReadLengthKB\x18\x03 \x01(\x04\x12\x1b\n\x13\x64\x65\x66\x61ultReadLengthKB\x18\x04 \x01(\x04\x12\x1b\n\x13maxBufferPoolSizeMB\x18\x05 \x01(\x04\x12\x1b\n\x13maxQueriesPerSecond\x18\x06 \x01(\x01\x12\x11\n\tforceIpv4\x18\x07 \x01(\x08\"k\n\x18SetCloudAPIConfigRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x10\n\x08userName\x18\x02 \x01(\t\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.clouddrive.CloudAPIConfig\"!\n\x0e\x43ommandRequest\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"\x1f\n\rCommandResult\x12\x0e\n\x06result\x18\x01 \x01(\t\"\x1c\n\x0bStringValue\x12\r\n\x05value\x18\x01 \x01(\t\"\\\n\x11QRCodeScanMessage\x12\x36\n\x0bmessageType\x18\x01 \x01(\x0e\x32!.clouddrive.QRCodeScanMessageType\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x1c\n\nStringList\x12\x0e\n\x06values\x18\x01 \x03(\t\"\x83\x05\n\x0eSystemSettings\x12#\n\x16\x64irCacheTimeToLiveSecs\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12maxPreProcessTasks\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0fmaxProcessTasks\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10tempFileLocation\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x1a\n\rsyncWithCloud\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12&\n\x19readDownloaderTimeoutSecs\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1c\n\x0fuploadDelaySecs\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12\x35\n\x10processBlackList\x18\x08 \x01(\x0b\x32\x16.clouddrive.StringListH\x07\x88\x01\x01\x12<\n\x17uploadIgnoredExtensions\x18\t \x01(\x0b\x32\x16.clouddrive.StringListH\x08\x88\x01\x01\x12\x35\n\rupdateChannel\x18\n \x01(\x0e\x32\x19.clouddrive.UpdateChannelH\t\x88\x01\x01\x42\x19\n\x17_dirCacheTimeToLiveSecsB\x15\n\x13_maxPreProcessTasksB\x12\n\x10_maxProcessTasksB\x13\n\x11_tempFileLocationB\x10\n\x0e_syncWithCloudB\x1c\n\x1a_readDownloaderTimeoutSecsB\x12\n\x10_uploadDelaySecsB\x13\n\x11_processBlackListB\x1a\n\x18_uploadIgnoredExtensionsB\x10\n\x0e_updateChannel\"d\n\x16SetDirCacheTimeRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\"\n\x15\x64irCachTimeToLiveSecs\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x18\n\x16_dirCachTimeToLiveSecs\"/\n\x1fGetEffectiveDirCacheTimeRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"-\n\x17GetOpenFileTableRequest\x12\x12\n\nincludeDir\x18\x01 \x01(\x08\":\n\x1eGetEffectiveDirCacheTimeResult\x12\x18\n\x10\x64irCacheTimeSecs\x18\x01 \x01(\x04\"J\n\x0cUpdateResult\x12\x11\n\thasUpdate\x18\x01 \x01(\x08\x12\x12\n\nnewVersion\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\xa6\x01\n\rOpenFileTable\x12\x43\n\ropenFileTable\x18\x01 \x03(\x0b\x32,.clouddrive.OpenFileTable.OpenFileTableEntry\x12\x1a\n\x12localOpenFileCount\x18\x02 \x01(\x04\x1a\x34\n\x12OpenFileTableEntry\x12\x0b\n\x03key\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"t\n\x0c\x44irCacheItem\x12.\n\ninsertTime\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0etimeToLiveSecs\x18\x02 \x01(\x04\x12\x1c\n\x14referencedSubfileLen\x18\x03 \x01(\x04\"\xa4\x01\n\rDirCacheTable\x12\x43\n\rdirCacheTable\x18\x01 \x03(\x0b\x32,.clouddrive.DirCacheTable.DirCacheTableEntry\x1aN\n\x12\x44irCacheTableEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.clouddrive.DirCacheItem:\x02\x38\x01\"1\n\rTempFileTable\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x11\n\ttempFiles\x18\x02 \x03(\t\"*\n\x13\x43onfirmEmailRequest\x12\x13\n\x0b\x63onfirmCode\x18\x01 \x01(\t\"-\n\x1cSendResetAccountEmailRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\"=\n\x13ResetAccountRequest\x12\x11\n\tresetCode\x18\x01 \x01(\t\x12\x13\n\x0bnewPassword\x18\x02 \x01(\t\"\x81\x02\n\x0e\x43loudDrivePlan\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05price\x18\x04 \x01(\x01\x12\x15\n\x08\x64uration\x18\x05 \x01(\x03H\x00\x88\x01\x01\x12\x1b\n\x13\x64urationDescription\x18\x06 \x01(\t\x12\x10\n\x08isActive\x18\x07 \x01(\x08\x12\x1c\n\x0f\x66ontAwesomeIcon\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1a\n\roriginalPrice\x18\t \x01(\x01H\x02\x88\x01\x01\x42\x0b\n\t_durationB\x12\n\x10_fontAwesomeIconB\x10\n\x0e_originalPrice\"E\n\x18GetCloudDrivePlansResult\x12)\n\x05plans\x18\x01 \x03(\x0b\x32\x1a.clouddrive.CloudDrivePlan\"I\n\x0fJoinPlanRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x17\n\ncouponCode\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_couponCode\"\xab\x01\n\x0bPaymentInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0f\n\x07plan_id\x18\x02 \x01(\t\x12\x43\n\x0epaymentMethods\x18\x03 \x03(\x0b\x32+.clouddrive.PaymentInfo.PaymentMethodsEntry\x1a\x35\n\x13PaymentMethodsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x0eJoinPlanResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0f\n\x07\x62\x61lance\x18\x02 \x01(\x01\x12\x10\n\x08planName\x18\x03 \x01(\t\x12\x17\n\x0fplanDescription\x18\x04 \x01(\t\x12\x33\n\nexpireTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12\x31\n\x0bpaymentInfo\x18\x06 \x01(\x0b\x32\x17.clouddrive.PaymentInfoH\x01\x88\x01\x01\x42\r\n\x0b_expireTimeB\x0e\n\x0c_paymentInfo\"\x99\x01\n\tPromotion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tcloudName\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x15\n\x08subTitle\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\r\n\x05rules\x18\x05 \x01(\t\x12\x13\n\x06notice\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x0b\n\x03url\x18\x07 \x01(\tB\x0b\n\t_subTitleB\t\n\x07_notice\"@\n\x13GetPromotionsResult\x12)\n\npromotions\x18\x01 \x03(\x0b\x32\x15.clouddrive.Promotion\"-\n\rOfflineStatus\x12\r\n\x05quota\x18\x01 \x01(\r\x12\r\n\x05total\x18\x02 \x01(\r\"\xcf\x01\n\x0bOfflineFile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x04\x12\x0b\n\x03url\x18\x03 \x01(\t\x12-\n\x06status\x18\x04 \x01(\x0e\x32\x1d.clouddrive.OfflineFileStatus\x12\x10\n\x08infoHash\x18\x05 \x01(\t\x12\x0e\n\x06\x66ileId\x18\x06 \x01(\t\x12\x10\n\x08\x61\x64\x64_time\x18\x07 \x01(\x04\x12\x10\n\x08parentId\x18\x08 \x01(\t\x12\x13\n\x0bpercendDone\x18\t \x01(\x01\x12\r\n\x05peers\x18\n \x01(\x04\"T\n\x19OfflineFileListAllRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x16\n\x0e\x63loudAccountId\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\"\xc1\x01\n\x18OfflineFileListAllResult\x12\x0e\n\x06pageNo\x18\x01 \x01(\r\x12\x14\n\x0cpageRowCount\x18\x02 \x01(\r\x12\x11\n\tpageCount\x18\x03 \x01(\r\x12\x12\n\ntotalCount\x18\x04 \x01(\r\x12)\n\x06status\x18\x05 \x01(\x0b\x32\x19.clouddrive.OfflineStatus\x12-\n\x0cofflineFiles\x18\x06 \x03(\x0b\x32\x17.clouddrive.OfflineFile\"q\n\x15OfflineFileListResult\x12-\n\x0cofflineFiles\x18\x01 \x03(\x0b\x32\x17.clouddrive.OfflineFile\x12)\n\x06status\x18\x02 \x01(\x0b\x32\x19.clouddrive.OfflineStatus\"D\n\x17\x42indCloudAccountRequest\x12\x11\n\tcloudName\x18\x01 \x01(\t\x12\x16\n\x0e\x63loudAccountId\x18\x02 \x01(\t\"N\n\x16TransferBalanceRequest\x12\x12\n\ntoUserName\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x10\n\x08password\x18\x03 \x01(\t\"U\n\x1a\x43hangeUserNameEmailRequest\x12\x13\n\x0bnewUserName\x18\x01 \x01(\t\x12\x10\n\x08newEmail\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"\xbb\x02\n\nBalanceLog\x12\x16\n\x0e\x62\x61lance_before\x18\x01 \x01(\x01\x12\x15\n\rbalance_after\x18\x02 \x01(\x01\x12\x16\n\x0e\x62\x61lance_change\x18\x03 \x01(\x01\x12\x41\n\toperation\x18\x04 \x01(\x0e\x32..clouddrive.BalanceLog.BalancceChangeOperation\x12\x18\n\x10operation_source\x18\x05 \x01(\t\x12\x14\n\x0coperation_id\x18\x06 \x01(\t\x12\x32\n\x0eoperation_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"?\n\x17\x42\x61lancceChangeOperation\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07\x44\x65posit\x10\x01\x12\n\n\x06Refund\x10\x02\"8\n\x10\x42\x61lanceLogResult\x12$\n\x04logs\x18\x01 \x03(\x0b\x32\x16.clouddrive.BalanceLog\"<\n\x16\x43heckFinalPriceRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x12\n\ncouponCode\x18\x02 \x01(\t\"\xab\x01\n\x15\x43heckFinalPriceResult\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x11\n\tplanPrice\x18\x02 \x01(\x01\x12\x13\n\x0buserBalance\x18\x03 \x01(\x01\x12\x1c\n\x14\x63ouponDiscountAmount\x18\x04 \x01(\x01\x12\x18\n\x0b\x63ouponError\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nfinalPrice\x18\x06 \x01(\x01\x42\x0e\n\x0c_couponError\"V\n\x19\x43heckActivationCodeResult\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x10\n\x08planName\x18\x02 \x01(\t\x12\x17\n\x0fplanDescription\x18\x03 \x01(\t\"<\n\x16\x43heckCouponCodeRequest\x12\x0e\n\x06planId\x18\x01 \x01(\t\x12\x12\n\ncouponCode\x18\x02 \x01(\t\"u\n\x10\x43ouponCodeResult\x12\x12\n\ncouponCode\x18\x01 \x01(\t\x12\x19\n\x11\x63ouponDescription\x18\x02 \x01(\t\x12\x14\n\x0cisPercentage\x18\x03 \x01(\x08\x12\x1c\n\x14\x63ouponDiscountAmount\x18\x04 \x01(\x01\"\x8f\x01\n\x0e\x46ileBackupRule\x12\x14\n\nextensions\x18\x01 \x01(\tH\x00\x12\x13\n\tfileNames\x18\x02 \x01(\tH\x00\x12\x0f\n\x05regex\x18\x03 \x01(\tH\x00\x12\x11\n\x07minSize\x18\x04 \x01(\x04H\x00\x12\x11\n\tisEnabled\x18\x64 \x01(\x08\x12\x13\n\x0bisBlackList\x18\x65 \x01(\x08\x42\x06\n\x04rule\"\x8b\x01\n\x11\x42\x61\x63kupDestination\x12\x17\n\x0f\x64\x65stinationPath\x18\x01 \x01(\t\x12\x11\n\tisEnabled\x18\x02 \x01(\x08\x12\x37\n\x0elastFinishTime\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x42\x11\n\x0f_lastFinishTime\" \n\nDaysOfWeek\x12\x12\n\ndaysOfWeek\x18\x01 \x03(\r\"\x8f\x01\n\x0cTimeSchedule\x12\x11\n\tisEnabled\x18\x01 \x01(\x08\x12\x0c\n\x04hour\x18\x02 \x01(\r\x12\x0e\n\x06minute\x18\x03 \x01(\r\x12\x0e\n\x06second\x18\x04 \x01(\r\x12/\n\ndaysOfWeek\x18\x05 \x01(\x0b\x32\x16.clouddrive.DaysOfWeekH\x00\x88\x01\x01\x42\r\n\x0b_daysOfWeek\"\xbc\x03\n\x06\x42\x61\x63kup\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x33\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x1d.clouddrive.BackupDestination\x12\x33\n\x0f\x66ileBackupRules\x18\x03 \x03(\x0b\x32\x1a.clouddrive.FileBackupRule\x12\x34\n\x0f\x66ileReplaceRule\x18\x04 \x01(\x0e\x32\x1b.clouddrive.FileReplaceRule\x12\x32\n\x0e\x66ileDeleteRule\x18\x05 \x01(\x0e\x32\x1a.clouddrive.FileDeleteRule\x12\x11\n\tisEnabled\x18\x06 \x01(\x08\x12\x1e\n\x16\x66ileSystemWatchEnabled\x18\x07 \x01(\x08\x12\"\n\x1awalkingThroughIntervalSecs\x18\x08 \x01(\x03\x12\"\n\x1a\x66orceWalkingThroughOnStart\x18\t \x01(\x08\x12/\n\rtimeSchedules\x18\n \x03(\x0b\x32\x18.clouddrive.TimeSchedule\x12\x1e\n\x16isTimeSchedulesEnabled\x18\x0b \x01(\x08\"\xf3\x02\n\x0c\x42\x61\x63kupStatus\x12\"\n\x06\x62\x61\x63kup\x18\x01 \x01(\x0b\x32\x12.clouddrive.Backup\x12/\n\x06status\x18\x02 \x01(\x0e\x32\x1f.clouddrive.BackupStatus.Status\x12\x15\n\rstatusMessage\x18\x03 \x01(\t\x12?\n\rwatcherStatus\x18\x04 \x01(\x0e\x32(.clouddrive.BackupStatus.FileWatchStatus\x12\x1c\n\x14watcherStatusMessage\x18\x05 \x01(\t\"?\n\x06Status\x12\x08\n\x04Idle\x10\x00\x12\x12\n\x0eWalkingThrough\x10\x01\x12\t\n\x05\x45rror\x10\x02\x12\x0c\n\x08\x44isabled\x10\x03\"W\n\x0f\x46ileWatchStatus\x12\x0f\n\x0bWatcherIdle\x10\x00\x12\x0c\n\x08Watching\x10\x01\x12\x10\n\x0cWatcherError\x10\x02\x12\x13\n\x0fWatcherDisabled\x10\x03\"7\n\nBackupList\x12)\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32\x18.clouddrive.BackupStatus\"\xb6\x03\n\x13\x42\x61\x63kupModifyRequest\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x33\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x1d.clouddrive.BackupDestination\x12\x33\n\x0f\x66ileBackupRules\x18\x03 \x03(\x0b\x32\x1a.clouddrive.FileBackupRule\x12\x39\n\x0f\x66ileReplaceRule\x18\x04 \x01(\x0e\x32\x1b.clouddrive.FileReplaceRuleH\x00\x88\x01\x01\x12\x37\n\x0e\x66ileDeleteRule\x18\x05 \x01(\x0e\x32\x1a.clouddrive.FileDeleteRuleH\x01\x88\x01\x01\x12#\n\x16\x66ileSystemWatchEnabled\x18\x06 \x01(\x08H\x02\x88\x01\x01\x12\'\n\x1awalkingThroughIntervalSecs\x18\x07 \x01(\x03H\x03\x88\x01\x01\x42\x12\n\x10_fileReplaceRuleB\x11\n\x0f_fileDeleteRuleB\x19\n\x17_fileSystemWatchEnabledB\x1d\n\x1b_walkingThroughIntervalSecs\"@\n\x17\x42\x61\x63kupSetEnabledRequest\x12\x12\n\nsourcePath\x18\x01 \x01(\t\x12\x11\n\tisEnabled\x18\x02 \x01(\x08*h\n\x15QRCodeScanMessageType\x12\x0e\n\nSHOW_IMAGE\x10\x00\x12\x16\n\x12SHOW_IMAGE_CONTENT\x10\x01\x12\x11\n\rCHANGE_STATUS\x10\x02\x12\t\n\x05\x43LOSE\x10\x03\x12\t\n\x05\x45RROR\x10\x04*&\n\rUpdateChannel\x12\x0b\n\x07Release\x10\x00\x12\x08\n\x04\x42\x65ta\x10\x01*|\n\x11OfflineFileStatus\x12\x10\n\x0cOFFLINE_INIT\x10\x00\x12\x17\n\x13OFFLINE_DOWNLOADING\x10\x01\x12\x14\n\x10OFFLINE_FINISHED\x10\x02\x12\x11\n\rOFFLINE_ERROR\x10\x03\x12\x13\n\x0fOFFLINE_UNKNOWN\x10\x04*B\n\x0f\x46ileReplaceRule\x12\x08\n\x04Skip\x10\x00\x12\r\n\tOverwrite\x10\x01\x12\x16\n\x12KeepHistoryVersion\x10\x02*M\n\x0e\x46ileDeleteRule\x12\n\n\x06\x44\x65lete\x10\x00\x12\x0b\n\x07Recycle\x10\x01\x12\x08\n\x04Keep\x10\x02\x12\x18\n\x14MoveToVersionHistory\x10\x03\x32\xd0H\n\x11\x43loudDriveFileSrv\x12K\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a .clouddrive.CloudDriveSystemInfo\"\x00\x12?\n\x08GetToken\x12\x1b.clouddrive.GetTokenRequest\x1a\x14.clouddrive.JWTToken\"\x00\x12H\n\x05Login\x12\x1c.clouddrive.UserLoginRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12N\n\x08Register\x12\x1f.clouddrive.UserRegisterRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12[\n\x15SendResetAccountEmail\x12(.clouddrive.SendResetAccountEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0cResetAccount\x12\x1f.clouddrive.ResetAccountRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\x10SendConfirmEmail\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0c\x43onfirmEmail\x12\x1f.clouddrive.ConfirmEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x10GetAccountStatus\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.AccountStatusResult\"\x00\x12L\n\x0bGetSubFiles\x12\x1e.clouddrive.ListSubFileRequest\x1a\x19.clouddrive.SubFilesReply\"\x00\x30\x01\x12L\n\x10GetSearchResults\x12\x19.clouddrive.SearchRequest\x1a\x19.clouddrive.SubFilesReply\"\x00\x30\x01\x12Q\n\x0e\x46indFileByPath\x12!.clouddrive.FindFileByPathRequest\x1a\x1a.clouddrive.CloudDriveFile\"\x00\x12Q\n\x0c\x43reateFolder\x12\x1f.clouddrive.CreateFolderRequest\x1a\x1e.clouddrive.CreateFolderResult\"\x00\x12N\n\nRenameFile\x12\x1d.clouddrive.RenameFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12P\n\x0bRenameFiles\x12\x1e.clouddrive.RenameFilesRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12J\n\x08MoveFile\x12\x1b.clouddrive.MoveFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12H\n\nDeleteFile\x12\x17.clouddrive.FileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12S\n\x15\x44\x65leteFilePermanently\x12\x17.clouddrive.FileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12N\n\x0b\x44\x65leteFiles\x12\x1c.clouddrive.MultiFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12Y\n\x16\x44\x65leteFilesPermanently\x12\x1c.clouddrive.MultiFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12W\n\x0f\x41\x64\x64OfflineFiles\x12!.clouddrive.AddOfflineFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12V\n\x16ListOfflineFilesByPath\x12\x17.clouddrive.FileRequest\x1a!.clouddrive.OfflineFileListResult\"\x00\x12\x64\n\x13ListAllOfflineFiles\x12%.clouddrive.OfflineFileListAllRequest\x1a$.clouddrive.OfflineFileListAllResult\"\x00\x12V\n\x17GetFileDetailProperties\x12\x17.clouddrive.FileRequest\x1a .clouddrive.FileDetailProperties\"\x00\x12@\n\x0cGetSpaceInfo\x12\x17.clouddrive.FileRequest\x1a\x15.clouddrive.SpaceInfo\"\x00\x12N\n\x13GetCloudMemberships\x12\x17.clouddrive.FileRequest\x1a\x1c.clouddrive.CloudMemberships\"\x00\x12\x43\n\x0eGetRuntimeInfo\x12\x16.google.protobuf.Empty\x1a\x17.clouddrive.RuntimeInfo\"\x00\x12?\n\x0eGetRunningInfo\x12\x16.google.protobuf.Empty\x1a\x13.clouddrive.RunInfo\"\x00\x12J\n\x06Logout\x12\x1d.clouddrive.UserLogoutRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12R\n\x15\x43\x61nAddMoreMountPoints\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12L\n\x0eGetMountPoints\x12\x16.google.protobuf.Empty\x1a .clouddrive.GetMountPointsResult\"\x00\x12H\n\rAddMountPoint\x12\x17.clouddrive.MountOption\x1a\x1c.clouddrive.MountPointResult\"\x00\x12Q\n\x10RemoveMountPoint\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12\x46\n\x05Mount\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12H\n\x07Unmount\x12\x1d.clouddrive.MountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12W\n\x10UpdateMountPoint\x12#.clouddrive.UpdateMountPointRequest\x1a\x1c.clouddrive.MountPointResult\"\x00\x12`\n\x18GetAvailableDriveLetters\x12\x16.google.protobuf.Empty\x1a*.clouddrive.GetAvailableDriveLettersResult\"\x00\x12N\n\x0fHasDriveLetters\x12\x16.google.protobuf.Empty\x1a!.clouddrive.HasDriveLettersResult\"\x00\x12_\n\x10LocalGetSubFiles\x12#.clouddrive.LocalGetSubFilesRequest\x1a\".clouddrive.LocalGetSubFilesResult\"\x00\x30\x01\x12P\n\x10GetAllTasksCount\x12\x16.google.protobuf.Empty\x1a\".clouddrive.GetAllTasksCountResult\"\x00\x12X\n\x14GetDownloadFileCount\x12\x16.google.protobuf.Empty\x1a&.clouddrive.GetDownloadFileCountResult\"\x00\x12V\n\x13GetDownloadFileList\x12\x16.google.protobuf.Empty\x1a%.clouddrive.GetDownloadFileListResult\"\x00\x12T\n\x12GetUploadFileCount\x12\x16.google.protobuf.Empty\x1a$.clouddrive.GetUploadFileCountResult\"\x00\x12`\n\x11GetUploadFileList\x12$.clouddrive.GetUploadFileListRequest\x1a#.clouddrive.GetUploadFileListResult\"\x00\x12H\n\x14\x43\x61ncelAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x11\x43\x61ncelUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\x13PauseAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x10PauseUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x14ResumeAllUploadFiles\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x11ResumeUploadFiles\x12\'.clouddrive.MultpleUploadFileKeyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x13\x43\x61nAddMoreCloudApis\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12\x64\n\x19\x41PILogin115Editthiscookie\x12).clouddrive.Login115EditthiscookieRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12Y\n\x11\x41PILogin115QRCode\x12!.clouddrive.Login115QrCodeRequest\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12\x62\n\x18\x41PILoginAliyundriveOAuth\x12(.clouddrive.LoginAliyundriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12p\n\x1f\x41PILoginAliyundriveRefreshtoken\x12/.clouddrive.LoginAliyundriveRefreshtokenRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12i\n\x19\x41PILoginAliyunDriveQRCode\x12).clouddrive.LoginAliyundriveQRCodeRequest\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12\\\n\x15\x41PILoginBaiduPanOAuth\x12%.clouddrive.LoginBaiduPanOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12\\\n\x15\x41PILoginOneDriveOAuth\x12%.clouddrive.LoginOneDriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12\x62\n\x18\x41piLoginGoogleDriveOAuth\x12(.clouddrive.LoginGoogleDriveOAuthRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12p\n\x1f\x41piLoginGoogleDriveRefreshToken\x12/.clouddrive.LoginGoogleDriveRefreshTokenRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12N\n\x11\x41PILogin189QRCode\x12\x16.google.protobuf.Empty\x1a\x1d.clouddrive.QRCodeScanMessage\"\x00\x30\x01\x12L\n\x0e\x41PILoginPikPak\x12\x1c.clouddrive.UserLoginRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12N\n\x0e\x41PILoginWebDav\x12\x1e.clouddrive.LoginWebDavRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12T\n\x11\x41PIAddLocalFolder\x12!.clouddrive.AddLocalFolderRequest\x1a\x1a.clouddrive.APILoginResult\"\x00\x12V\n\x0eRemoveCloudAPI\x12!.clouddrive.RemoveCloudAPIRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12\x45\n\x0fGetAllCloudApis\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.CloudAPIList\"\x00\x12W\n\x11GetCloudAPIConfig\x12$.clouddrive.GetCloudAPIConfigRequest\x1a\x1a.clouddrive.CloudAPIConfig\"\x00\x12S\n\x11SetCloudAPIConfig\x12$.clouddrive.SetCloudAPIConfigRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x11GetSystemSettings\x12\x16.google.protobuf.Empty\x1a\x1a.clouddrive.SystemSettings\"\x00\x12I\n\x11SetSystemSettings\x12\x1a.clouddrive.SystemSettings\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x13SetDirCacheTimeSecs\x12\".clouddrive.SetDirCacheTimeRequest\x1a\x16.google.protobuf.Empty\"\x00\x12y\n\x1cGetEffectiveDirCacheTimeSecs\x12+.clouddrive.GetEffectiveDirCacheTimeRequest\x1a*.clouddrive.GetEffectiveDirCacheTimeResult\"\x00\x12T\n\x10GetOpenFileTable\x12#.clouddrive.GetOpenFileTableRequest\x1a\x19.clouddrive.OpenFileTable\"\x00\x12G\n\x10GetDirCacheTable\x12\x16.google.protobuf.Empty\x1a\x19.clouddrive.DirCacheTable\"\x00\x12L\n\x17GetReferencedEntryPaths\x12\x17.clouddrive.FileRequest\x1a\x16.clouddrive.StringList\"\x00\x12G\n\x10GetTempFileTable\x12\x16.google.protobuf.Empty\x1a\x19.clouddrive.TempFileTable\"\x00\x12P\n\x0ePushTaskChange\x12\x16.google.protobuf.Empty\x1a\".clouddrive.GetAllTasksCountResult\"\x00\x30\x01\x12L\n\x16GetCloudDrive1UserData\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.StringResult\"\x00\x12\x42\n\x0eRestartService\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0fShutdownService\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\tHasUpdate\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.UpdateResult\"\x00\x12\x41\n\x0b\x43heckUpdate\x12\x16.google.protobuf.Empty\x1a\x18.clouddrive.UpdateResult\"\x00\x12\x42\n\x0e\x44ownloadUpdate\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x0cUpdateSystem\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x42\n\x0bGetMetaData\x12\x17.clouddrive.FileRequest\x1a\x18.clouddrive.FileMetaData\"\x00\x12\x46\n\x0fGetOriginalPath\x12\x17.clouddrive.FileRequest\x1a\x18.clouddrive.StringResult\"\x00\x12V\n\x0e\x43hangePassword\x12!.clouddrive.ChangePasswordRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12K\n\nCreateFile\x12\x1d.clouddrive.CreateFileRequest\x1a\x1c.clouddrive.CreateFileResult\"\x00\x12L\n\tCloseFile\x12\x1c.clouddrive.CloseFileRequest\x1a\x1f.clouddrive.FileOperationResult\"\x00\x12R\n\x11WriteToFileStream\x12\x1c.clouddrive.WriteFileRequest\x1a\x1b.clouddrive.WriteFileResult\"\x00(\x01\x12J\n\x0bWriteToFile\x12\x1c.clouddrive.WriteFileRequest\x1a\x1b.clouddrive.WriteFileResult\"\x00\x12J\n\rGetPromotions\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.GetPromotionsResult\"\x00\x12I\n\x15UpdatePromotionResult\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x12GetCloudDrivePlans\x12\x16.google.protobuf.Empty\x1a$.clouddrive.GetCloudDrivePlansResult\"\x00\x12\x45\n\x08JoinPlan\x12\x1b.clouddrive.JoinPlanRequest\x1a\x1a.clouddrive.JoinPlanResult\"\x00\x12Q\n\x10\x42indCloudAccount\x12#.clouddrive.BindCloudAccountRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x0fTransferBalance\x12\".clouddrive.TransferBalanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x0b\x43hangeEmail\x12&.clouddrive.ChangeUserNameEmailRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\rGetBalanceLog\x12\x16.google.protobuf.Empty\x1a\x1c.clouddrive.BalanceLogResult\"\x00\x12W\n\x13\x43heckActivationCode\x12\x17.clouddrive.StringValue\x1a%.clouddrive.CheckActivationCodeResult\"\x00\x12\x45\n\x0c\x41\x63tivatePlan\x12\x17.clouddrive.StringValue\x1a\x1a.clouddrive.JoinPlanResult\"\x00\x12U\n\x0f\x43heckCouponCode\x12\".clouddrive.CheckCouponCodeRequest\x1a\x1c.clouddrive.CouponCodeResult\"\x00\x12\x44\n\x0fGetReferralCode\x12\x16.google.protobuf.Empty\x1a\x17.clouddrive.StringValue\"\x00\x12@\n\x0c\x42\x61\x63kupGetAll\x12\x16.google.protobuf.Empty\x1a\x16.clouddrive.BackupList\"\x00\x12\x39\n\tBackupAdd\x12\x12.clouddrive.Backup\x1a\x16.google.protobuf.Empty\"\x00\x12\x41\n\x0c\x42\x61\x63kupRemove\x12\x17.clouddrive.StringValue\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x0c\x42\x61\x63kupUpdate\x12\x12.clouddrive.Backup\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14\x42\x61\x63kupAddDestination\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x17\x42\x61\x63kupRemoveDestination\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x10\x42\x61\x63kupSetEnabled\x12#.clouddrive.BackupSetEnabledRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1f\x42\x61\x63kupSetFileSystemWatchEnabled\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x16\x42\x61\x63kupUpdateStrategies\x12\x1f.clouddrive.BackupModifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x1b\x42\x61\x63kupRestartWalkingThrough\x12\x17.clouddrive.StringValue\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\x11\x43\x61nAddMoreBackups\x12\x16.google.protobuf.Empty\x1a\x1f.clouddrive.FileOperationResult\"\x00\x42\x17\xaa\x02\x14\x43loudDriveSrv.Protosb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'CloudDrive_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -30,24 +30,24 @@
   _FILEMETADATA_METADATAENTRY._serialized_options = b'8\001'
   _OPENFILETABLE_OPENFILETABLEENTRY._options = None
   _OPENFILETABLE_OPENFILETABLEENTRY._serialized_options = b'8\001'
   _DIRCACHETABLE_DIRCACHETABLEENTRY._options = None
   _DIRCACHETABLE_DIRCACHETABLEENTRY._serialized_options = b'8\001'
   _PAYMENTINFO_PAYMENTMETHODSENTRY._options = None
   _PAYMENTINFO_PAYMENTMETHODSENTRY._serialized_options = b'8\001'
-  _globals['_QRCODESCANMESSAGETYPE']._serialized_start=13871
-  _globals['_QRCODESCANMESSAGETYPE']._serialized_end=13975
-  _globals['_UPDATECHANNEL']._serialized_start=13977
-  _globals['_UPDATECHANNEL']._serialized_end=14015
-  _globals['_OFFLINEFILESTATUS']._serialized_start=14017
-  _globals['_OFFLINEFILESTATUS']._serialized_end=14141
-  _globals['_FILEREPLACERULE']._serialized_start=14143
-  _globals['_FILEREPLACERULE']._serialized_end=14209
-  _globals['_FILEDELETERULE']._serialized_start=14211
-  _globals['_FILEDELETERULE']._serialized_end=14288
+  _globals['_QRCODESCANMESSAGETYPE']._serialized_start=14176
+  _globals['_QRCODESCANMESSAGETYPE']._serialized_end=14280
+  _globals['_UPDATECHANNEL']._serialized_start=14282
+  _globals['_UPDATECHANNEL']._serialized_end=14320
+  _globals['_OFFLINEFILESTATUS']._serialized_start=14322
+  _globals['_OFFLINEFILESTATUS']._serialized_end=14446
+  _globals['_FILEREPLACERULE']._serialized_start=14448
+  _globals['_FILEREPLACERULE']._serialized_end=14514
+  _globals['_FILEDELETERULE']._serialized_start=14516
+  _globals['_FILEDELETERULE']._serialized_end=14593
   _globals['_GETTOKENREQUEST']._serialized_start=94
   _globals['_GETTOKENREQUEST']._serialized_end=147
   _globals['_JWTTOKEN']._serialized_start=149
   _globals['_JWTTOKEN']._serialized_end=261
   _globals['_FILEREQUEST']._serialized_start=263
   _globals['_FILEREQUEST']._serialized_end=290
   _globals['_MULTIFILEREQUEST']._serialized_start=292
@@ -55,265 +55,269 @@
   _globals['_FILEOPERATIONRESULT']._serialized_start=326
   _globals['_FILEOPERATIONRESULT']._serialized_end=411
   _globals['_STRINGRESULT']._serialized_start=413
   _globals['_STRINGRESULT']._serialized_end=443
   _globals['_UNMOUNTARCHIVERESULT']._serialized_start=445
   _globals['_UNMOUNTARCHIVERESULT']._serialized_end=483
   _globals['_LISTSUBFILEREQUEST']._serialized_start=485
-  _globals['_LISTSUBFILEREQUEST']._serialized_end=541
-  _globals['_SEARCHREQUEST']._serialized_start=543
-  _globals['_SEARCHREQUEST']._serialized_end=633
-  _globals['_ADDOFFLINEFILEREQUEST']._serialized_start=635
-  _globals['_ADDOFFLINEFILEREQUEST']._serialized_end=690
-  _globals['_ADDSHAREDLINKREQUEST']._serialized_start=692
-  _globals['_ADDSHAREDLINKREQUEST']._serialized_end=779
-  _globals['_SUBFILESREPLY']._serialized_start=781
-  _globals['_SUBFILESREPLY']._serialized_end=842
-  _globals['_FINDFILEBYPATHREQUEST']._serialized_start=844
-  _globals['_FINDFILEBYPATHREQUEST']._serialized_end=901
-  _globals['_CREATEFOLDERREQUEST']._serialized_start=903
-  _globals['_CREATEFOLDERREQUEST']._serialized_end=964
-  _globals['_CREATEFOLDERRESULT']._serialized_start=966
-  _globals['_CREATEFOLDERRESULT']._serialized_end=1086
-  _globals['_CREATEFILEREQUEST']._serialized_start=1088
-  _globals['_CREATEFILEREQUEST']._serialized_end=1145
-  _globals['_CREATEFILERESULT']._serialized_start=1147
-  _globals['_CREATEFILERESULT']._serialized_end=1185
-  _globals['_CLOSEFILEREQUEST']._serialized_start=1187
-  _globals['_CLOSEFILEREQUEST']._serialized_end=1225
-  _globals['_MOVEFILEREQUEST']._serialized_start=1227
-  _globals['_MOVEFILEREQUEST']._serialized_end=1284
-  _globals['_WRITEFILEREQUEST']._serialized_start=1286
-  _globals['_WRITEFILEREQUEST']._serialized_end=1393
-  _globals['_WRITEFILERESULT']._serialized_start=1395
-  _globals['_WRITEFILERESULT']._serialized_end=1434
-  _globals['_RENAMEFILEREQUEST']._serialized_start=1436
-  _globals['_RENAMEFILEREQUEST']._serialized_end=1493
-  _globals['_RENAMEFILESREQUEST']._serialized_start=1495
-  _globals['_RENAMEFILESREQUEST']._serialized_end=1567
-  _globals['_CLOUDDRIVEFILE']._serialized_start=1570
-  _globals['_CLOUDDRIVEFILE']._serialized_end=2670
-  _globals['_CLOUDDRIVEFILE_FILEHASHESENTRY']._serialized_start=2486
-  _globals['_CLOUDDRIVEFILE_FILEHASHESENTRY']._serialized_end=2535
-  _globals['_CLOUDDRIVEFILE_FILETYPE']._serialized_start=2537
-  _globals['_CLOUDDRIVEFILE_FILETYPE']._serialized_end=2583
-  _globals['_CLOUDDRIVEFILE_HASHTYPE']._serialized_start=2585
-  _globals['_CLOUDDRIVEFILE_HASHTYPE']._serialized_end=2643
-  _globals['_SPACEINFO']._serialized_start=2672
-  _globals['_SPACEINFO']._serialized_end=2741
-  _globals['_CLOUDAPI']._serialized_start=2743
-  _globals['_CLOUDAPI']._serialized_end=2821
-  _globals['_CLOUDMEMBERSHIP']._serialized_start=2824
-  _globals['_CLOUDMEMBERSHIP']._serialized_end=2957
-  _globals['_CLOUDMEMBERSHIPS']._serialized_start=2959
-  _globals['_CLOUDMEMBERSHIPS']._serialized_end=3027
-  _globals['_FILEDETAILPROPERTIES']._serialized_start=3030
-  _globals['_FILEDETAILPROPERTIES']._serialized_end=3178
-  _globals['_FILEMETADATA']._serialized_start=3180
-  _globals['_FILEMETADATA']._serialized_end=3301
-  _globals['_FILEMETADATA_METADATAENTRY']._serialized_start=3254
-  _globals['_FILEMETADATA_METADATAENTRY']._serialized_end=3301
-  _globals['_CLOUDDRIVESYSTEMINFO']._serialized_start=3303
-  _globals['_CLOUDDRIVESYSTEMINFO']._serialized_end=3360
-  _globals['_USERLOGINREQUEST']._serialized_start=3362
-  _globals['_USERLOGINREQUEST']._serialized_end=3440
-  _globals['_USERREGISTERREQUEST']._serialized_start=3442
-  _globals['_USERREGISTERREQUEST']._serialized_end=3499
-  _globals['_USERLOGOUTREQUEST']._serialized_start=3501
-  _globals['_USERLOGOUTREQUEST']._serialized_end=3547
-  _globals['_CHANGEPASSWORDREQUEST']._serialized_start=3549
-  _globals['_CHANGEPASSWORDREQUEST']._serialized_end=3614
-  _globals['_ACCOUNTSTATUSRESULT']._serialized_start=3617
-  _globals['_ACCOUNTSTATUSRESULT']._serialized_end=3797
-  _globals['_ACCOUNTPLAN']._serialized_start=3800
-  _globals['_ACCOUNTPLAN']._serialized_end=3951
-  _globals['_ACCOUNTROLE']._serialized_start=3953
-  _globals['_ACCOUNTROLE']._serialized_end=4035
-  _globals['_RUNTIMEINFO']._serialized_start=4037
-  _globals['_RUNTIMEINFO']._serialized_end=4136
-  _globals['_RUNINFO']._serialized_start=4139
-  _globals['_RUNINFO']._serialized_end=4270
-  _globals['_MOUNTOPTION']._serialized_start=4273
-  _globals['_MOUNTOPTION']._serialized_end=4443
-  _globals['_MOUNTPOINT']._serialized_start=4446
-  _globals['_MOUNTPOINT']._serialized_end=4640
-  _globals['_MOUNTPOINTREQUEST']._serialized_start=4642
-  _globals['_MOUNTPOINTREQUEST']._serialized_end=4681
-  _globals['_GETMOUNTPOINTSRESULT']._serialized_start=4683
-  _globals['_GETMOUNTPOINTSRESULT']._serialized_end=4750
-  _globals['_MOUNTPOINTRESULT']._serialized_start=4752
-  _globals['_MOUNTPOINTRESULT']._serialized_end=4807
-  _globals['_UPDATEMOUNTPOINTREQUEST']._serialized_start=4809
-  _globals['_UPDATEMOUNTPOINTREQUEST']._serialized_end=4903
-  _globals['_GETAVAILABLEDRIVELETTERSREQUEST']._serialized_start=4905
-  _globals['_GETAVAILABLEDRIVELETTERSREQUEST']._serialized_end=4965
-  _globals['_GETAVAILABLEDRIVELETTERSRESULT']._serialized_start=4967
-  _globals['_GETAVAILABLEDRIVELETTERSRESULT']._serialized_end=5021
-  _globals['_HASDRIVELETTERSRESULT']._serialized_start=5023
-  _globals['_HASDRIVELETTERSRESULT']._serialized_end=5071
-  _globals['_LOCALGETSUBFILESREQUEST']._serialized_start=5073
-  _globals['_LOCALGETSUBFILESREQUEST']._serialized_end=5198
-  _globals['_LOCALGETSUBFILESRESULT']._serialized_start=5200
-  _globals['_LOCALGETSUBFILESRESULT']._serialized_end=5242
-  _globals['_PUSHMESSAGE']._serialized_start=5244
-  _globals['_PUSHMESSAGE']._serialized_end=5284
-  _globals['_GETALLTASKSCOUNTRESULT']._serialized_start=5287
-  _globals['_GETALLTASKSCOUNTRESULT']._serialized_end=5420
-  _globals['_GETDOWNLOADFILECOUNTRESULT']._serialized_start=5422
-  _globals['_GETDOWNLOADFILECOUNTRESULT']._serialized_end=5469
-  _globals['_DOWNLOADFILEINFO']._serialized_start=5472
-  _globals['_DOWNLOADFILEINFO']._serialized_end=5627
-  _globals['_GETDOWNLOADFILELISTRESULT']._serialized_start=5629
-  _globals['_GETDOWNLOADFILELISTRESULT']._serialized_end=5739
-  _globals['_GETUPLOADFILECOUNTRESULT']._serialized_start=5741
-  _globals['_GETUPLOADFILECOUNTRESULT']._serialized_end=5786
-  _globals['_UPLOADFILEINFO']._serialized_start=5788
-  _globals['_UPLOADFILEINFO']._serialized_end=5912
-  _globals['_GETUPLOADFILELISTREQUEST']._serialized_start=5914
-  _globals['_GETUPLOADFILELISTREQUEST']._serialized_end=6014
-  _globals['_GETUPLOADFILELISTRESULT']._serialized_start=6016
-  _globals['_GETUPLOADFILELISTRESULT']._serialized_end=6110
-  _globals['_MULTPLEUPLOADFILEKEYREQUEST']._serialized_start=6112
-  _globals['_MULTPLEUPLOADFILEKEYREQUEST']._serialized_end=6155
-  _globals['_LOGIN115EDITTHISCOOKIEREQUEST']._serialized_start=6157
-  _globals['_LOGIN115EDITTHISCOOKIEREQUEST']._serialized_end=6218
-  _globals['_LOGIN115QRCODEREQUEST']._serialized_start=6220
-  _globals['_LOGIN115QRCODEREQUEST']._serialized_end=6291
-  _globals['_LOGINALIYUNDRIVEOAUTHREQUEST']._serialized_start=6293
-  _globals['_LOGINALIYUNDRIVEOAUTHREQUEST']._serialized_end=6388
-  _globals['_LOGINALIYUNDRIVEREFRESHTOKENREQUEST']._serialized_start=6390
-  _globals['_LOGINALIYUNDRIVEREFRESHTOKENREQUEST']._serialized_end=6469
-  _globals['_LOGINALIYUNDRIVEQRCODEREQUEST']._serialized_start=6471
-  _globals['_LOGINALIYUNDRIVEQRCODEREQUEST']._serialized_end=6522
-  _globals['_LOGINBAIDUPANOAUTHREQUEST']._serialized_start=6524
-  _globals['_LOGINBAIDUPANOAUTHREQUEST']._serialized_end=6616
-  _globals['_LOGINONEDRIVEOAUTHREQUEST']._serialized_start=6618
-  _globals['_LOGINONEDRIVEOAUTHREQUEST']._serialized_end=6710
-  _globals['_LOGINGOOGLEDRIVEOAUTHREQUEST']._serialized_start=6712
-  _globals['_LOGINGOOGLEDRIVEOAUTHREQUEST']._serialized_end=6807
-  _globals['_LOGINGOOGLEDRIVEREFRESHTOKENREQUEST']._serialized_start=6809
-  _globals['_LOGINGOOGLEDRIVEREFRESHTOKENREQUEST']._serialized_end=6911
-  _globals['_LOGINWEBDAVREQUEST']._serialized_start=6913
-  _globals['_LOGINWEBDAVREQUEST']._serialized_end=6988
-  _globals['_APILOGINRESULT']._serialized_start=6990
-  _globals['_APILOGINRESULT']._serialized_end=7045
-  _globals['_ADDLOCALFOLDERREQUEST']._serialized_start=7047
-  _globals['_ADDLOCALFOLDERREQUEST']._serialized_end=7095
-  _globals['_REMOVECLOUDAPIREQUEST']._serialized_start=7097
-  _globals['_REMOVECLOUDAPIREQUEST']._serialized_end=7182
-  _globals['_GETCLOUDAPICONFIGREQUEST']._serialized_start=7184
-  _globals['_GETCLOUDAPICONFIGREQUEST']._serialized_end=7247
-  _globals['_CLOUDAPILIST']._serialized_start=7249
-  _globals['_CLOUDAPILIST']._serialized_end=7299
-  _globals['_CLOUDAPICONFIG']._serialized_start=7302
-  _globals['_CLOUDAPICONFIG']._serialized_end=7502
-  _globals['_SETCLOUDAPICONFIGREQUEST']._serialized_start=7504
-  _globals['_SETCLOUDAPICONFIGREQUEST']._serialized_end=7611
-  _globals['_COMMANDREQUEST']._serialized_start=7613
-  _globals['_COMMANDREQUEST']._serialized_end=7646
-  _globals['_COMMANDRESULT']._serialized_start=7648
-  _globals['_COMMANDRESULT']._serialized_end=7679
-  _globals['_STRINGVALUE']._serialized_start=7681
-  _globals['_STRINGVALUE']._serialized_end=7709
-  _globals['_QRCODESCANMESSAGE']._serialized_start=7711
-  _globals['_QRCODESCANMESSAGE']._serialized_end=7803
-  _globals['_STRINGLIST']._serialized_start=7805
-  _globals['_STRINGLIST']._serialized_end=7833
-  _globals['_SYSTEMSETTINGS']._serialized_start=7836
-  _globals['_SYSTEMSETTINGS']._serialized_end=8479
-  _globals['_SETDIRCACHETIMEREQUEST']._serialized_start=8481
-  _globals['_SETDIRCACHETIMEREQUEST']._serialized_end=8581
-  _globals['_GETEFFECTIVEDIRCACHETIMEREQUEST']._serialized_start=8583
-  _globals['_GETEFFECTIVEDIRCACHETIMEREQUEST']._serialized_end=8630
-  _globals['_GETOPENFILETABLEREQUEST']._serialized_start=8632
-  _globals['_GETOPENFILETABLEREQUEST']._serialized_end=8677
-  _globals['_GETEFFECTIVEDIRCACHETIMERESULT']._serialized_start=8679
-  _globals['_GETEFFECTIVEDIRCACHETIMERESULT']._serialized_end=8737
-  _globals['_UPDATERESULT']._serialized_start=8739
-  _globals['_UPDATERESULT']._serialized_end=8813
-  _globals['_OPENFILETABLE']._serialized_start=8816
-  _globals['_OPENFILETABLE']._serialized_end=8982
-  _globals['_OPENFILETABLE_OPENFILETABLEENTRY']._serialized_start=8930
-  _globals['_OPENFILETABLE_OPENFILETABLEENTRY']._serialized_end=8982
-  _globals['_DIRCACHEITEM']._serialized_start=8984
-  _globals['_DIRCACHEITEM']._serialized_end=9100
-  _globals['_DIRCACHETABLE']._serialized_start=9103
-  _globals['_DIRCACHETABLE']._serialized_end=9267
-  _globals['_DIRCACHETABLE_DIRCACHETABLEENTRY']._serialized_start=9189
-  _globals['_DIRCACHETABLE_DIRCACHETABLEENTRY']._serialized_end=9267
-  _globals['_TEMPFILETABLE']._serialized_start=9269
-  _globals['_TEMPFILETABLE']._serialized_end=9318
-  _globals['_CONFIRMEMAILREQUEST']._serialized_start=9320
-  _globals['_CONFIRMEMAILREQUEST']._serialized_end=9362
-  _globals['_SENDRESETACCOUNTEMAILREQUEST']._serialized_start=9364
-  _globals['_SENDRESETACCOUNTEMAILREQUEST']._serialized_end=9409
-  _globals['_RESETACCOUNTREQUEST']._serialized_start=9411
-  _globals['_RESETACCOUNTREQUEST']._serialized_end=9472
-  _globals['_CLOUDDRIVEPLAN']._serialized_start=9475
-  _globals['_CLOUDDRIVEPLAN']._serialized_end=9732
-  _globals['_GETCLOUDDRIVEPLANSRESULT']._serialized_start=9734
-  _globals['_GETCLOUDDRIVEPLANSRESULT']._serialized_end=9803
-  _globals['_JOINPLANREQUEST']._serialized_start=9805
-  _globals['_JOINPLANREQUEST']._serialized_end=9878
-  _globals['_PAYMENTINFO']._serialized_start=9881
-  _globals['_PAYMENTINFO']._serialized_end=10052
-  _globals['_PAYMENTINFO_PAYMENTMETHODSENTRY']._serialized_start=9999
-  _globals['_PAYMENTINFO_PAYMENTMETHODSENTRY']._serialized_end=10052
-  _globals['_JOINPLANRESULT']._serialized_start=10055
-  _globals['_JOINPLANRESULT']._serialized_end=10283
-  _globals['_PROMOTION']._serialized_start=10286
-  _globals['_PROMOTION']._serialized_end=10439
-  _globals['_GETPROMOTIONSRESULT']._serialized_start=10441
-  _globals['_GETPROMOTIONSRESULT']._serialized_end=10505
-  _globals['_OFFLINESTATUS']._serialized_start=10507
-  _globals['_OFFLINESTATUS']._serialized_end=10552
-  _globals['_OFFLINEFILE']._serialized_start=10555
-  _globals['_OFFLINEFILE']._serialized_end=10762
-  _globals['_OFFLINEFILELISTALLREQUEST']._serialized_start=10764
-  _globals['_OFFLINEFILELISTALLREQUEST']._serialized_end=10848
-  _globals['_OFFLINEFILELISTALLRESULT']._serialized_start=10851
-  _globals['_OFFLINEFILELISTALLRESULT']._serialized_end=11044
-  _globals['_OFFLINEFILELISTRESULT']._serialized_start=11046
-  _globals['_OFFLINEFILELISTRESULT']._serialized_end=11159
-  _globals['_BINDCLOUDACCOUNTREQUEST']._serialized_start=11161
-  _globals['_BINDCLOUDACCOUNTREQUEST']._serialized_end=11229
-  _globals['_TRANSFERBALANCEREQUEST']._serialized_start=11231
-  _globals['_TRANSFERBALANCEREQUEST']._serialized_end=11309
-  _globals['_CHANGEUSERNAMEEMAILREQUEST']._serialized_start=11311
-  _globals['_CHANGEUSERNAMEEMAILREQUEST']._serialized_end=11396
-  _globals['_BALANCELOG']._serialized_start=11399
-  _globals['_BALANCELOG']._serialized_end=11714
-  _globals['_BALANCELOG_BALANCCECHANGEOPERATION']._serialized_start=11651
-  _globals['_BALANCELOG_BALANCCECHANGEOPERATION']._serialized_end=11714
-  _globals['_BALANCELOGRESULT']._serialized_start=11716
-  _globals['_BALANCELOGRESULT']._serialized_end=11772
-  _globals['_CHECKFINALPRICEREQUEST']._serialized_start=11774
-  _globals['_CHECKFINALPRICEREQUEST']._serialized_end=11834
-  _globals['_CHECKFINALPRICERESULT']._serialized_start=11837
-  _globals['_CHECKFINALPRICERESULT']._serialized_end=12008
-  _globals['_CHECKACTIVATIONCODERESULT']._serialized_start=12010
-  _globals['_CHECKACTIVATIONCODERESULT']._serialized_end=12096
-  _globals['_CHECKCOUPONCODEREQUEST']._serialized_start=12098
-  _globals['_CHECKCOUPONCODEREQUEST']._serialized_end=12158
-  _globals['_COUPONCODERESULT']._serialized_start=12160
-  _globals['_COUPONCODERESULT']._serialized_end=12277
-  _globals['_FILEBACKUPRULE']._serialized_start=12280
-  _globals['_FILEBACKUPRULE']._serialized_end=12423
-  _globals['_BACKUPDESTINATION']._serialized_start=12426
-  _globals['_BACKUPDESTINATION']._serialized_end=12565
-  _globals['_BACKUP']._serialized_start=12568
-  _globals['_BACKUP']._serialized_end=12931
-  _globals['_BACKUPSTATUS']._serialized_start=12934
-  _globals['_BACKUPSTATUS']._serialized_end=13305
-  _globals['_BACKUPSTATUS_STATUS']._serialized_start=13153
-  _globals['_BACKUPSTATUS_STATUS']._serialized_end=13216
-  _globals['_BACKUPSTATUS_FILEWATCHSTATUS']._serialized_start=13218
-  _globals['_BACKUPSTATUS_FILEWATCHSTATUS']._serialized_end=13305
-  _globals['_BACKUPLIST']._serialized_start=13307
-  _globals['_BACKUPLIST']._serialized_end=13362
-  _globals['_BACKUPMODIFYREQUEST']._serialized_start=13365
-  _globals['_BACKUPMODIFYREQUEST']._serialized_end=13803
-  _globals['_BACKUPSETENABLEDREQUEST']._serialized_start=13805
-  _globals['_BACKUPSETENABLEDREQUEST']._serialized_end=13869
-  _globals['_CLOUDDRIVEFILESRV']._serialized_start=14291
-  _globals['_CLOUDDRIVEFILESRV']._serialized_end=23587
+  _globals['_LISTSUBFILEREQUEST']._serialized_end=585
+  _globals['_SEARCHREQUEST']._serialized_start=587
+  _globals['_SEARCHREQUEST']._serialized_end=677
+  _globals['_ADDOFFLINEFILEREQUEST']._serialized_start=679
+  _globals['_ADDOFFLINEFILEREQUEST']._serialized_end=734
+  _globals['_ADDSHAREDLINKREQUEST']._serialized_start=736
+  _globals['_ADDSHAREDLINKREQUEST']._serialized_end=823
+  _globals['_SUBFILESREPLY']._serialized_start=825
+  _globals['_SUBFILESREPLY']._serialized_end=886
+  _globals['_FINDFILEBYPATHREQUEST']._serialized_start=888
+  _globals['_FINDFILEBYPATHREQUEST']._serialized_end=945
+  _globals['_CREATEFOLDERREQUEST']._serialized_start=947
+  _globals['_CREATEFOLDERREQUEST']._serialized_end=1008
+  _globals['_CREATEFOLDERRESULT']._serialized_start=1010
+  _globals['_CREATEFOLDERRESULT']._serialized_end=1130
+  _globals['_CREATEFILEREQUEST']._serialized_start=1132
+  _globals['_CREATEFILEREQUEST']._serialized_end=1189
+  _globals['_CREATEFILERESULT']._serialized_start=1191
+  _globals['_CREATEFILERESULT']._serialized_end=1229
+  _globals['_CLOSEFILEREQUEST']._serialized_start=1231
+  _globals['_CLOSEFILEREQUEST']._serialized_end=1269
+  _globals['_MOVEFILEREQUEST']._serialized_start=1271
+  _globals['_MOVEFILEREQUEST']._serialized_end=1328
+  _globals['_WRITEFILEREQUEST']._serialized_start=1330
+  _globals['_WRITEFILEREQUEST']._serialized_end=1437
+  _globals['_WRITEFILERESULT']._serialized_start=1439
+  _globals['_WRITEFILERESULT']._serialized_end=1478
+  _globals['_RENAMEFILEREQUEST']._serialized_start=1480
+  _globals['_RENAMEFILEREQUEST']._serialized_end=1537
+  _globals['_RENAMEFILESREQUEST']._serialized_start=1539
+  _globals['_RENAMEFILESREQUEST']._serialized_end=1611
+  _globals['_CLOUDDRIVEFILE']._serialized_start=1614
+  _globals['_CLOUDDRIVEFILE']._serialized_end=2714
+  _globals['_CLOUDDRIVEFILE_FILEHASHESENTRY']._serialized_start=2530
+  _globals['_CLOUDDRIVEFILE_FILEHASHESENTRY']._serialized_end=2579
+  _globals['_CLOUDDRIVEFILE_FILETYPE']._serialized_start=2581
+  _globals['_CLOUDDRIVEFILE_FILETYPE']._serialized_end=2627
+  _globals['_CLOUDDRIVEFILE_HASHTYPE']._serialized_start=2629
+  _globals['_CLOUDDRIVEFILE_HASHTYPE']._serialized_end=2687
+  _globals['_SPACEINFO']._serialized_start=2716
+  _globals['_SPACEINFO']._serialized_end=2785
+  _globals['_CLOUDAPI']._serialized_start=2787
+  _globals['_CLOUDAPI']._serialized_end=2865
+  _globals['_CLOUDMEMBERSHIP']._serialized_start=2868
+  _globals['_CLOUDMEMBERSHIP']._serialized_end=3001
+  _globals['_CLOUDMEMBERSHIPS']._serialized_start=3003
+  _globals['_CLOUDMEMBERSHIPS']._serialized_end=3071
+  _globals['_FILEDETAILPROPERTIES']._serialized_start=3074
+  _globals['_FILEDETAILPROPERTIES']._serialized_end=3222
+  _globals['_FILEMETADATA']._serialized_start=3224
+  _globals['_FILEMETADATA']._serialized_end=3345
+  _globals['_FILEMETADATA_METADATAENTRY']._serialized_start=3298
+  _globals['_FILEMETADATA_METADATAENTRY']._serialized_end=3345
+  _globals['_CLOUDDRIVESYSTEMINFO']._serialized_start=3347
+  _globals['_CLOUDDRIVESYSTEMINFO']._serialized_end=3404
+  _globals['_USERLOGINREQUEST']._serialized_start=3406
+  _globals['_USERLOGINREQUEST']._serialized_end=3484
+  _globals['_USERREGISTERREQUEST']._serialized_start=3486
+  _globals['_USERREGISTERREQUEST']._serialized_end=3543
+  _globals['_USERLOGOUTREQUEST']._serialized_start=3545
+  _globals['_USERLOGOUTREQUEST']._serialized_end=3591
+  _globals['_CHANGEPASSWORDREQUEST']._serialized_start=3593
+  _globals['_CHANGEPASSWORDREQUEST']._serialized_end=3658
+  _globals['_ACCOUNTSTATUSRESULT']._serialized_start=3661
+  _globals['_ACCOUNTSTATUSRESULT']._serialized_end=3841
+  _globals['_ACCOUNTPLAN']._serialized_start=3844
+  _globals['_ACCOUNTPLAN']._serialized_end=3995
+  _globals['_ACCOUNTROLE']._serialized_start=3997
+  _globals['_ACCOUNTROLE']._serialized_end=4079
+  _globals['_RUNTIMEINFO']._serialized_start=4081
+  _globals['_RUNTIMEINFO']._serialized_end=4180
+  _globals['_RUNINFO']._serialized_start=4183
+  _globals['_RUNINFO']._serialized_end=4314
+  _globals['_MOUNTOPTION']._serialized_start=4317
+  _globals['_MOUNTOPTION']._serialized_end=4487
+  _globals['_MOUNTPOINT']._serialized_start=4490
+  _globals['_MOUNTPOINT']._serialized_end=4684
+  _globals['_MOUNTPOINTREQUEST']._serialized_start=4686
+  _globals['_MOUNTPOINTREQUEST']._serialized_end=4725
+  _globals['_GETMOUNTPOINTSRESULT']._serialized_start=4727
+  _globals['_GETMOUNTPOINTSRESULT']._serialized_end=4794
+  _globals['_MOUNTPOINTRESULT']._serialized_start=4796
+  _globals['_MOUNTPOINTRESULT']._serialized_end=4851
+  _globals['_UPDATEMOUNTPOINTREQUEST']._serialized_start=4853
+  _globals['_UPDATEMOUNTPOINTREQUEST']._serialized_end=4947
+  _globals['_GETAVAILABLEDRIVELETTERSREQUEST']._serialized_start=4949
+  _globals['_GETAVAILABLEDRIVELETTERSREQUEST']._serialized_end=5009
+  _globals['_GETAVAILABLEDRIVELETTERSRESULT']._serialized_start=5011
+  _globals['_GETAVAILABLEDRIVELETTERSRESULT']._serialized_end=5065
+  _globals['_HASDRIVELETTERSRESULT']._serialized_start=5067
+  _globals['_HASDRIVELETTERSRESULT']._serialized_end=5115
+  _globals['_LOCALGETSUBFILESREQUEST']._serialized_start=5117
+  _globals['_LOCALGETSUBFILESREQUEST']._serialized_end=5242
+  _globals['_LOCALGETSUBFILESRESULT']._serialized_start=5244
+  _globals['_LOCALGETSUBFILESRESULT']._serialized_end=5286
+  _globals['_PUSHMESSAGE']._serialized_start=5288
+  _globals['_PUSHMESSAGE']._serialized_end=5328
+  _globals['_GETALLTASKSCOUNTRESULT']._serialized_start=5331
+  _globals['_GETALLTASKSCOUNTRESULT']._serialized_end=5464
+  _globals['_GETDOWNLOADFILECOUNTRESULT']._serialized_start=5466
+  _globals['_GETDOWNLOADFILECOUNTRESULT']._serialized_end=5513
+  _globals['_DOWNLOADFILEINFO']._serialized_start=5516
+  _globals['_DOWNLOADFILEINFO']._serialized_end=5671
+  _globals['_GETDOWNLOADFILELISTRESULT']._serialized_start=5673
+  _globals['_GETDOWNLOADFILELISTRESULT']._serialized_end=5783
+  _globals['_GETUPLOADFILECOUNTRESULT']._serialized_start=5785
+  _globals['_GETUPLOADFILECOUNTRESULT']._serialized_end=5830
+  _globals['_UPLOADFILEINFO']._serialized_start=5832
+  _globals['_UPLOADFILEINFO']._serialized_end=5956
+  _globals['_GETUPLOADFILELISTREQUEST']._serialized_start=5958
+  _globals['_GETUPLOADFILELISTREQUEST']._serialized_end=6058
+  _globals['_GETUPLOADFILELISTRESULT']._serialized_start=6060
+  _globals['_GETUPLOADFILELISTRESULT']._serialized_end=6154
+  _globals['_MULTPLEUPLOADFILEKEYREQUEST']._serialized_start=6156
+  _globals['_MULTPLEUPLOADFILEKEYREQUEST']._serialized_end=6199
+  _globals['_LOGIN115EDITTHISCOOKIEREQUEST']._serialized_start=6201
+  _globals['_LOGIN115EDITTHISCOOKIEREQUEST']._serialized_end=6262
+  _globals['_LOGIN115QRCODEREQUEST']._serialized_start=6264
+  _globals['_LOGIN115QRCODEREQUEST']._serialized_end=6335
+  _globals['_LOGINALIYUNDRIVEOAUTHREQUEST']._serialized_start=6337
+  _globals['_LOGINALIYUNDRIVEOAUTHREQUEST']._serialized_end=6432
+  _globals['_LOGINALIYUNDRIVEREFRESHTOKENREQUEST']._serialized_start=6434
+  _globals['_LOGINALIYUNDRIVEREFRESHTOKENREQUEST']._serialized_end=6513
+  _globals['_LOGINALIYUNDRIVEQRCODEREQUEST']._serialized_start=6515
+  _globals['_LOGINALIYUNDRIVEQRCODEREQUEST']._serialized_end=6566
+  _globals['_LOGINBAIDUPANOAUTHREQUEST']._serialized_start=6568
+  _globals['_LOGINBAIDUPANOAUTHREQUEST']._serialized_end=6660
+  _globals['_LOGINONEDRIVEOAUTHREQUEST']._serialized_start=6662
+  _globals['_LOGINONEDRIVEOAUTHREQUEST']._serialized_end=6754
+  _globals['_LOGINGOOGLEDRIVEOAUTHREQUEST']._serialized_start=6756
+  _globals['_LOGINGOOGLEDRIVEOAUTHREQUEST']._serialized_end=6851
+  _globals['_LOGINGOOGLEDRIVEREFRESHTOKENREQUEST']._serialized_start=6853
+  _globals['_LOGINGOOGLEDRIVEREFRESHTOKENREQUEST']._serialized_end=6955
+  _globals['_LOGINWEBDAVREQUEST']._serialized_start=6957
+  _globals['_LOGINWEBDAVREQUEST']._serialized_end=7032
+  _globals['_APILOGINRESULT']._serialized_start=7034
+  _globals['_APILOGINRESULT']._serialized_end=7089
+  _globals['_ADDLOCALFOLDERREQUEST']._serialized_start=7091
+  _globals['_ADDLOCALFOLDERREQUEST']._serialized_end=7139
+  _globals['_REMOVECLOUDAPIREQUEST']._serialized_start=7141
+  _globals['_REMOVECLOUDAPIREQUEST']._serialized_end=7226
+  _globals['_GETCLOUDAPICONFIGREQUEST']._serialized_start=7228
+  _globals['_GETCLOUDAPICONFIGREQUEST']._serialized_end=7291
+  _globals['_CLOUDAPILIST']._serialized_start=7293
+  _globals['_CLOUDAPILIST']._serialized_end=7343
+  _globals['_CLOUDAPICONFIG']._serialized_start=7346
+  _globals['_CLOUDAPICONFIG']._serialized_end=7546
+  _globals['_SETCLOUDAPICONFIGREQUEST']._serialized_start=7548
+  _globals['_SETCLOUDAPICONFIGREQUEST']._serialized_end=7655
+  _globals['_COMMANDREQUEST']._serialized_start=7657
+  _globals['_COMMANDREQUEST']._serialized_end=7690
+  _globals['_COMMANDRESULT']._serialized_start=7692
+  _globals['_COMMANDRESULT']._serialized_end=7723
+  _globals['_STRINGVALUE']._serialized_start=7725
+  _globals['_STRINGVALUE']._serialized_end=7753
+  _globals['_QRCODESCANMESSAGE']._serialized_start=7755
+  _globals['_QRCODESCANMESSAGE']._serialized_end=7847
+  _globals['_STRINGLIST']._serialized_start=7849
+  _globals['_STRINGLIST']._serialized_end=7877
+  _globals['_SYSTEMSETTINGS']._serialized_start=7880
+  _globals['_SYSTEMSETTINGS']._serialized_end=8523
+  _globals['_SETDIRCACHETIMEREQUEST']._serialized_start=8525
+  _globals['_SETDIRCACHETIMEREQUEST']._serialized_end=8625
+  _globals['_GETEFFECTIVEDIRCACHETIMEREQUEST']._serialized_start=8627
+  _globals['_GETEFFECTIVEDIRCACHETIMEREQUEST']._serialized_end=8674
+  _globals['_GETOPENFILETABLEREQUEST']._serialized_start=8676
+  _globals['_GETOPENFILETABLEREQUEST']._serialized_end=8721
+  _globals['_GETEFFECTIVEDIRCACHETIMERESULT']._serialized_start=8723
+  _globals['_GETEFFECTIVEDIRCACHETIMERESULT']._serialized_end=8781
+  _globals['_UPDATERESULT']._serialized_start=8783
+  _globals['_UPDATERESULT']._serialized_end=8857
+  _globals['_OPENFILETABLE']._serialized_start=8860
+  _globals['_OPENFILETABLE']._serialized_end=9026
+  _globals['_OPENFILETABLE_OPENFILETABLEENTRY']._serialized_start=8974
+  _globals['_OPENFILETABLE_OPENFILETABLEENTRY']._serialized_end=9026
+  _globals['_DIRCACHEITEM']._serialized_start=9028
+  _globals['_DIRCACHEITEM']._serialized_end=9144
+  _globals['_DIRCACHETABLE']._serialized_start=9147
+  _globals['_DIRCACHETABLE']._serialized_end=9311
+  _globals['_DIRCACHETABLE_DIRCACHETABLEENTRY']._serialized_start=9233
+  _globals['_DIRCACHETABLE_DIRCACHETABLEENTRY']._serialized_end=9311
+  _globals['_TEMPFILETABLE']._serialized_start=9313
+  _globals['_TEMPFILETABLE']._serialized_end=9362
+  _globals['_CONFIRMEMAILREQUEST']._serialized_start=9364
+  _globals['_CONFIRMEMAILREQUEST']._serialized_end=9406
+  _globals['_SENDRESETACCOUNTEMAILREQUEST']._serialized_start=9408
+  _globals['_SENDRESETACCOUNTEMAILREQUEST']._serialized_end=9453
+  _globals['_RESETACCOUNTREQUEST']._serialized_start=9455
+  _globals['_RESETACCOUNTREQUEST']._serialized_end=9516
+  _globals['_CLOUDDRIVEPLAN']._serialized_start=9519
+  _globals['_CLOUDDRIVEPLAN']._serialized_end=9776
+  _globals['_GETCLOUDDRIVEPLANSRESULT']._serialized_start=9778
+  _globals['_GETCLOUDDRIVEPLANSRESULT']._serialized_end=9847
+  _globals['_JOINPLANREQUEST']._serialized_start=9849
+  _globals['_JOINPLANREQUEST']._serialized_end=9922
+  _globals['_PAYMENTINFO']._serialized_start=9925
+  _globals['_PAYMENTINFO']._serialized_end=10096
+  _globals['_PAYMENTINFO_PAYMENTMETHODSENTRY']._serialized_start=10043
+  _globals['_PAYMENTINFO_PAYMENTMETHODSENTRY']._serialized_end=10096
+  _globals['_JOINPLANRESULT']._serialized_start=10099
+  _globals['_JOINPLANRESULT']._serialized_end=10327
+  _globals['_PROMOTION']._serialized_start=10330
+  _globals['_PROMOTION']._serialized_end=10483
+  _globals['_GETPROMOTIONSRESULT']._serialized_start=10485
+  _globals['_GETPROMOTIONSRESULT']._serialized_end=10549
+  _globals['_OFFLINESTATUS']._serialized_start=10551
+  _globals['_OFFLINESTATUS']._serialized_end=10596
+  _globals['_OFFLINEFILE']._serialized_start=10599
+  _globals['_OFFLINEFILE']._serialized_end=10806
+  _globals['_OFFLINEFILELISTALLREQUEST']._serialized_start=10808
+  _globals['_OFFLINEFILELISTALLREQUEST']._serialized_end=10892
+  _globals['_OFFLINEFILELISTALLRESULT']._serialized_start=10895
+  _globals['_OFFLINEFILELISTALLRESULT']._serialized_end=11088
+  _globals['_OFFLINEFILELISTRESULT']._serialized_start=11090
+  _globals['_OFFLINEFILELISTRESULT']._serialized_end=11203
+  _globals['_BINDCLOUDACCOUNTREQUEST']._serialized_start=11205
+  _globals['_BINDCLOUDACCOUNTREQUEST']._serialized_end=11273
+  _globals['_TRANSFERBALANCEREQUEST']._serialized_start=11275
+  _globals['_TRANSFERBALANCEREQUEST']._serialized_end=11353
+  _globals['_CHANGEUSERNAMEEMAILREQUEST']._serialized_start=11355
+  _globals['_CHANGEUSERNAMEEMAILREQUEST']._serialized_end=11440
+  _globals['_BALANCELOG']._serialized_start=11443
+  _globals['_BALANCELOG']._serialized_end=11758
+  _globals['_BALANCELOG_BALANCCECHANGEOPERATION']._serialized_start=11695
+  _globals['_BALANCELOG_BALANCCECHANGEOPERATION']._serialized_end=11758
+  _globals['_BALANCELOGRESULT']._serialized_start=11760
+  _globals['_BALANCELOGRESULT']._serialized_end=11816
+  _globals['_CHECKFINALPRICEREQUEST']._serialized_start=11818
+  _globals['_CHECKFINALPRICEREQUEST']._serialized_end=11878
+  _globals['_CHECKFINALPRICERESULT']._serialized_start=11881
+  _globals['_CHECKFINALPRICERESULT']._serialized_end=12052
+  _globals['_CHECKACTIVATIONCODERESULT']._serialized_start=12054
+  _globals['_CHECKACTIVATIONCODERESULT']._serialized_end=12140
+  _globals['_CHECKCOUPONCODEREQUEST']._serialized_start=12142
+  _globals['_CHECKCOUPONCODEREQUEST']._serialized_end=12202
+  _globals['_COUPONCODERESULT']._serialized_start=12204
+  _globals['_COUPONCODERESULT']._serialized_end=12321
+  _globals['_FILEBACKUPRULE']._serialized_start=12324
+  _globals['_FILEBACKUPRULE']._serialized_end=12467
+  _globals['_BACKUPDESTINATION']._serialized_start=12470
+  _globals['_BACKUPDESTINATION']._serialized_end=12609
+  _globals['_DAYSOFWEEK']._serialized_start=12611
+  _globals['_DAYSOFWEEK']._serialized_end=12643
+  _globals['_TIMESCHEDULE']._serialized_start=12646
+  _globals['_TIMESCHEDULE']._serialized_end=12789
+  _globals['_BACKUP']._serialized_start=12792
+  _globals['_BACKUP']._serialized_end=13236
+  _globals['_BACKUPSTATUS']._serialized_start=13239
+  _globals['_BACKUPSTATUS']._serialized_end=13610
+  _globals['_BACKUPSTATUS_STATUS']._serialized_start=13458
+  _globals['_BACKUPSTATUS_STATUS']._serialized_end=13521
+  _globals['_BACKUPSTATUS_FILEWATCHSTATUS']._serialized_start=13523
+  _globals['_BACKUPSTATUS_FILEWATCHSTATUS']._serialized_end=13610
+  _globals['_BACKUPLIST']._serialized_start=13612
+  _globals['_BACKUPLIST']._serialized_end=13667
+  _globals['_BACKUPMODIFYREQUEST']._serialized_start=13670
+  _globals['_BACKUPMODIFYREQUEST']._serialized_end=14108
+  _globals['_BACKUPSETENABLEDREQUEST']._serialized_start=14110
+  _globals['_BACKUPSETENABLEDREQUEST']._serialized_end=14174
+  _globals['_CLOUDDRIVEFILESRV']._serialized_start=14596
+  _globals['_CLOUDDRIVEFILESRV']._serialized_end=23892
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clouddrive-0.0.9.8.2/clouddrive/proto/CloudDrive_pb2_grpc.py` & `clouddrive-0.0.9.9/clouddrive/proto/CloudDrive_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1371,15 +1371,16 @@
         """enable/disable a backup's FileSystemWatch
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BackupUpdateStrategies(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """deprecated, use BackupUpdate instead
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BackupRestartWalkingThrough(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
```

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/_init_mimetypes.py` & `clouddrive-0.0.9.9/clouddrive/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/download.py` & `clouddrive-0.0.9.9/clouddrive/util/download.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/file.py` & `clouddrive-0.0.9.9/clouddrive/util/file.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/ignore.py` & `clouddrive-0.0.9.9/clouddrive/util/ignore.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/iter.py` & `clouddrive-0.0.9.9/clouddrive/util/iter.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/property.py` & `clouddrive-0.0.9.9/clouddrive/util/property.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/response.py` & `clouddrive-0.0.9.9/clouddrive/util/response.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/text.py` & `clouddrive-0.0.9.9/clouddrive/util/text.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/clouddrive/util/urlopen.py` & `clouddrive-0.0.9.9/clouddrive/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/pyproject.toml` & `clouddrive-0.0.9.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clouddrive"
-version = "0.0.9.8.2"
+version = "0.0.9.9"
 description = "Python wrapper for CloudDrive."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-clouddrive-web-api"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-clouddrive-web-api"
 keywords = ["nas", "clouddrive"]
```

### Comparing `clouddrive-0.0.9.8.2/readme.md` & `clouddrive-0.0.9.9/readme.md`

 * *Files identical despite different names*

### Comparing `clouddrive-0.0.9.8.2/PKG-INFO` & `clouddrive-0.0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clouddrive
-Version: 0.0.9.8.2
+Version: 0.0.9.9
 Summary: Python wrapper for CloudDrive.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-clouddrive-web-api
 License: MIT
 Keywords: nas,clouddrive
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

