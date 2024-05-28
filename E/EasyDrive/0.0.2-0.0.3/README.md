# Comparing `tmp/easydrive-0.0.2.tar.gz` & `tmp/easydrive-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydrive-0.0.2.tar", last modified: Tue May 28 01:11:51 2024, max compression
+gzip compressed data, was "easydrive-0.0.3.tar", last modified: Tue May 28 01:37:03 2024, max compression
```

## Comparing `easydrive-0.0.2.tar` & `easydrive-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:11:51.192786 easydrive-0.0.2/
--rw-rw-rw-   0        0        0      516 2024-05-28 01:11:51.191783 easydrive-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.2/README.md
--rw-rw-rw-   0        0        0      462 2024-05-28 01:10:12.000000 easydrive-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 01:11:51.192786 easydrive-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 01:11:51.176233 easydrive-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 01:11:51.183748 easydrive-0.0.2/src/EasyDrive/
--rw-rw-rw-   0        0        0     9076 2024-05-28 01:04:22.000000 easydrive-0.0.2/src/EasyDrive/Drive.py
--rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.2/src/EasyDrive/Exceptions.py
--rw-rw-rw-   0        0        0    11348 2024-05-28 00:37:45.000000 easydrive-0.0.2/src/EasyDrive/FileSystemTypes.py
--rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.2/src/EasyDrive/MIMETypes.py
--rw-rw-rw-   0        0        0       57 2024-05-28 01:07:17.000000 easydrive-0.0.2/src/EasyDrive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:11:51.190270 easydrive-0.0.2/src/EasyDrive.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-28 01:11:51.000000 easydrive-0.0.2/src/EasyDrive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-28 01:11:51.000000 easydrive-0.0.2/src/EasyDrive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:11:51.000000 easydrive-0.0.2/src/EasyDrive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-28 01:11:51.000000 easydrive-0.0.2/src/EasyDrive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 01:37:03.909837 easydrive-0.0.3/
+-rw-rw-rw-   0        0        0      516 2024-05-28 01:37:03.907727 easydrive-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.3/README.md
+-rw-rw-rw-   0        0        0      462 2024-05-28 01:19:55.000000 easydrive-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 01:37:03.909837 easydrive-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 01:37:03.866088 easydrive-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 01:37:03.883160 easydrive-0.0.3/src/EasyDrive/
+-rw-rw-rw-   0        0        0     9692 2024-05-28 01:36:51.000000 easydrive-0.0.3/src/EasyDrive/Drive.py
+-rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.3/src/EasyDrive/Exceptions.py
+-rw-rw-rw-   0        0        0    11349 2024-05-28 01:22:34.000000 easydrive-0.0.3/src/EasyDrive/FileSystemTypes.py
+-rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.3/src/EasyDrive/MIMETypes.py
+-rw-rw-rw-   0        0        0      142 2024-05-28 01:18:26.000000 easydrive-0.0.3/src/EasyDrive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:37:03.904226 easydrive-0.0.3/src/EasyDrive.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-28 01:37:03.000000 easydrive-0.0.3/src/EasyDrive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-28 01:37:03.000000 easydrive-0.0.3/src/EasyDrive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 01:37:03.000000 easydrive-0.0.3/src/EasyDrive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 01:37:03.000000 easydrive-0.0.3/src/EasyDrive.egg-info/top_level.txt
```

### Comparing `easydrive-0.0.2/PKG-INFO` & `easydrive-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDrive
-Version: 0.0.2
+Version: 0.0.3
 Summary: EasyGoogle Drive access
 Author-email: RanchMonster <ranchmonster06@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `easydrive-0.0.2/src/EasyDrive/Drive.py` & `easydrive-0.0.3/src/EasyDrive/Drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from os import PathLike
 import os.path
 from typing import Union
-from Exceptions import InvaildCredentials, DrivePathException
+from .Exceptions import InvaildCredentials, DrivePathException
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
-from FileSystemTypes import *
+from .FileSystemTypes import *
 from google.oauth2.credentials import Credentials
 
 def login(tokenFile: str = "token.json", credentialsFile: str = "credentials.json") -> Credentials:
     """
     Logs in to the Google API and returns credentials.
 
     Args:
@@ -50,18 +50,18 @@
     def __init__(self, creds) -> None:
         """
         Initializes a Google Drive instance.
 
         Args:
             creds: Credentials object for Google Drive API.
         """
-        self.service = build("drive", "v3", credentials=creds)
+        self.__service = build("drive", "v3", credentials=creds)
         # self.__currentDir = "/"
         
-        self.__root: RootFolder = RootFolder(self.service)
+        self.__root: RootFolder = RootFolder(self.__service)
         self.__currentFolder:Folder = self.__root
         self.__currentFolder = self.__root
     def cd(self, path: str) -> None:
         """
         Changes the current directory.
 
         Args:
@@ -185,15 +185,15 @@
 
         # Create the file
         file_metadata = {
             'name': filename,
             'parents': [folder.get_id()],
             'mimeType':type
         }
-        self.service.files().create(body=file_metadata, fields='id').execute()
+        self.__service.files().create(body=file_metadata, fields='id').execute()
         return folder.get_file_by_name(filename) # type: ignore
     def mkdir(self, path: str) -> None:
         """
         Creates a folder at the given path if one does not already exist.
 
         Args:
             path (str): The path where the folder should be created.
@@ -219,15 +219,29 @@
 
         # Create the folder
         folder_metadata = {
             'name': folder_name,
             'mimeType': 'application/vnd.google-apps.folder',
             'parents': [parent_folder.get_id()]
         }
-        self.service.files().create(body=folder_metadata, fields='id').execute()
+        self.__service.files().create(body=folder_metadata, fields='id').execute()
+    def rmdir(self, path: str) -> None:
+            
+        path = path.replace("\\", "/")
+        parts = path.split("/")
+        folder_name = parts.pop()
+
+        if parts:
+            parent_folder_path = "/".join(parts)
+            parent_folder = self.__transverse_path(parent_folder_path)
+        else:
+            parent_folder = self.__currentFolder if self.__currentFolder else self.__root
+        folder=parent_folder.get_folder_by_name(folder_name)
+        if not folder:raise DrivePathException(f"Folder '{folder_name}' does not exist at path '{path}'")
+        folder.delete()
     def getCurrentFolder(self)->str:
         """
         Gets the path to the current folder
         Returns:
             the path to the current folder
         """
         folders:list[Folder]=[self.__currentFolder]
```

### Comparing `easydrive-0.0.2/src/EasyDrive/FileSystemTypes.py` & `easydrive-0.0.3/src/EasyDrive/FileSystemTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 from tkinter import NO
 from typing import Union
 from googleapiclient.http import MediaIoBaseDownload, MediaFileUpload, MediaIoBaseUpload
 from googleapiclient.errors import HttpError
-from Exceptions import DrivePathException
+from .Exceptions import DrivePathException
 from googleapiclient.discovery import Resource
 class Folder:
     def __init__(self, folder_name:str, folder_id:str, service:Resource, parent:'Folder'):
         """
         Initialize a Folder instance.
 
         Args:
```

### Comparing `easydrive-0.0.2/src/EasyDrive/MIMETypes.py` & `easydrive-0.0.3/src/EasyDrive/MIMETypes.py`

 * *Files identical despite different names*

### Comparing `easydrive-0.0.2/src/EasyDrive.egg-info/PKG-INFO` & `easydrive-0.0.3/src/EasyDrive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDrive
-Version: 0.0.2
+Version: 0.0.3
 Summary: EasyGoogle Drive access
 Author-email: RanchMonster <ranchmonster06@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

