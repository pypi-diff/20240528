# Comparing `tmp/cabinet-2024.5.27.1.tar.gz` & `tmp/cabinet-2024.5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.5.27.1.tar", last modified: Tue May 28 06:14:59 2024, max compression
+gzip compressed data, was "cabinet-2024.5.7.1.tar", last modified: Wed May  8 04:43:54 2024, max compression
```

## Comparing `cabinet-2024.5.27.1.tar` & `cabinet-2024.5.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.5.27.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7972 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7620 2024-05-28 06:14:30.000000 cabinet-2024.5.27.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.5.27.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.5.27.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.5.27.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    39712 2024-05-28 06:13:13.000000 cabinet-2024.5.27.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.5.27.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.5.27.1/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6528 2024-05-28 06:14:30.000000 cabinet-2024.5.27.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-28 06:14:59.075825 cabinet-2024.5.27.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7972 2024-05-28 06:14:59.000000 cabinet-2024.5.27.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-05-28 06:14:59.000000 cabinet-2024.5.27.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-28 06:14:59.000000 cabinet-2024.5.27.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-05-28 06:14:59.000000 cabinet-2024.5.27.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-05-28 06:14:59.000000 cabinet-2024.5.27.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.5.7.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38351 2024-05-08 04:41:54.000000 cabinet-2024.5.7.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.5.7.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.5.7.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.5.7.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.5.27.1/LICENSE` & `cabinet-2024.5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.5.27.1/PKG-INFO` & `cabinet-2024.5.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.5.27.1
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -126,15 +126,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

### Comparing `cabinet-2024.5.27.1/README.md` & `cabinet-2024.5.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

### Comparing `cabinet-2024.5.27.1/setup.cfg` & `cabinet-2024.5.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.05.27.1
+version = 2024.05.07.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.5.27.1/src/cabinet/cabinet.py` & `cabinet-2024.5.7.1/src/cabinet/cabinet.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,28 @@
     ```
 """
 import inspect
 import os
 import ast
 import sys
 import json
+import time
 import logging
 import getpass
 import pathlib
 import argparse
 import subprocess
 import importlib.metadata
 from html import escape
-from datetime import date, datetime, timedelta, timezone
+from datetime import date, datetime
 from typing import Any, Type, Optional, TypeVar
 import pymongo.errors
 from prompt_toolkit import print_formatted_text, HTML
-from pymongo.errors import PyMongoError, OperationFailure, ConnectionFailure
 from pymongo.mongo_client import MongoClient
 from pymongo.server_api import ServerApi
-from pymongo.database import Database
 from bson import json_util, ObjectId
 from . import helpers
 from .constants import (
     NEW_SETUP_MSG_INTRO,
     NEW_SETUP_MSG_MONGODB_INSTRUCTIONS,
     CONFIG_MONGODB_USERNAME,
     CONFIG_MONGODB_PASSWORD,
@@ -59,22 +58,21 @@
 
     mongodb_username: str = ''
     mongodb_password: str = ''
     mongodb_cluster_name: str = ''
     mongodb_db_name: str = ''
     mongodb_uri = ""
     client: MongoClient | None = None
-    database: Database
+    database = None
     new_setup: bool = False
     path_config_dir = str(pathlib.Path(
         __file__).resolve().parent)
     path_config_file = f"{path_config_dir}/cabinet_config.json"
     path_cabinet: str = ''
     path_log: str = ''
-    cached_data: dict = {}
 
     def _get_config(self, key=None):
         """
         Retrieves the value associated with the specified key from the configuration file.
 
         Args:
             key (str): The key to retrieve the corresponding value.
@@ -263,18 +261,15 @@
         self.new_setup = False
 
         try:
             self.uri = (f"mongodb+srv://{self.mongodb_username}:{self.mongodb_password}"
                         f"@{self.mongodb_cluster_name}.1jxchnk.mongodb.net/"
                         f"{self.mongodb_db_name}?retryWrites=true&w=majority")
             self.client = MongoClient(self.uri, server_api=ServerApi('1'))
-            self.database = self.client[self.mongodb_db_name]
-            if self.database is None:
-                self.log("Database cannot be initialized", level="error")
-                return None
+            self.database = self.client.cabinet
         except pymongo.errors.InvalidURI as error:
             print(ERROR_CONFIG_FILE_INVALID)
             print(error._message)
             sys.exit(-1)
         except pymongo.errors.ServerSelectionTimeoutError as error:
             print(ERROR_MONGODB_TIMEOUT)
             print(error)
@@ -349,52 +344,38 @@
                 subprocess.run(['open', self.path_config_file], check=True)
             elif sys.platform.startswith('linux'):
                 # Linux
                 subprocess.run(['xdg-open', self.path_config_file], check=True)
             else:
                 print(f"Please edit ${self.path_config_file} to configure.")
 
-    def update_cache(self, path: str | None = None, force: bool = False) -> str | None:
+    def update_cache(self, path: str | None = None) -> str | None:
         """
         Writes all MongoDB data to a cache file for faster reads in most situations.
         Creates the cache file if it does not exist.
         
         Args:
             - path (str): full path, including filename, of cache.json
-            - force (bool): update cache regardless of how  old cache file is.
-                - overridden to 'true' if caller function is `put`.
         """
 
-        force_update: bool =  force or inspect.stack()[1].function == 'put'
-
         if path is None:
             path = f"{self.path_config_dir}/cache.json"
 
-        # Check if cache file exists and is less than 1 hour old
-        if not force_update and os.path.exists(path):
-            file_mod_time = datetime.fromtimestamp(os.path.getmtime(path))
-            if datetime.now() - file_mod_time < timedelta(hours=1):
-                with open(path, "r", encoding="utf-8") as cache_file:
-                    self.cached_data = json.load(cache_file)
-                return None
-
         collection_data = self.database.cabinet.find()
         json_data = json.dumps(list(collection_data), indent=4, default=json_util.default)
 
         try:
             # Ensure the directory exists and write the JSON data to cache
             os.makedirs(os.path.dirname(path), exist_ok=True)
             with open(path, "w", encoding="utf-8") as temp_file:
                 temp_file.write(json_data)
         except OSError as e:
             self.log(f"Error updating cache: {e}", level="error")
             return None
 
-        self.cached_data = json.loads(json_data)
-
         return json_data
 
     def edit_db(self):
         """
         Opens the data in self.database.cabinet within a JSON file in Vim.
         When the file is closed, it replaces the data in this collection in MongoDB.
         """
@@ -424,16 +405,14 @@
 
             self.database.cabinet.drop()  # Drop the existing collection
             self.database.cabinet.insert_many(
                 modified_data)  # Insert the modified data
 
             print("Data in the collection has been updated.")
 
-            self.update_cache()
-
         except FileNotFoundError:
             print("Error: Cache file not found.")
         except subprocess.CalledProcessError:
             print("Error: Failed to open the file in Vim.")
         except json.JSONDecodeError:
             self.log("Failed to parse the modified JSON data.", level="error")
             self.log("Refreshing cache with original data.", level="info")
@@ -572,18 +551,14 @@
                 json_structure[item] = cache
                 cache = json_structure
             except TypeError as error:
                 print(error)
 
         existing_data = self.database.cabinet.find_one({}, {"_id": 0})
 
-        if not existing_data:
-            self.log("Could not fetch MongoDB data after update", level="error")
-            return None
-
         # Merge the new data with the existing data
         update = {"$set": {}}
 
         if len(attribute) > 2:
             update["$set"][attribute[0]] = self.merge_nested_data(existing_data.get(
                 attribute[0], {}), json_structure[attribute[0]])
         else:
@@ -592,102 +567,108 @@
         result = self.database.cabinet.update_many(custom_filter, update)
 
         if is_print:
             print(f"Modified {result.modified_count} item(s)")
             print(
                 f"{' -> '.join(attribute[:-1])} set to {value}\n")
 
-        self.update_cache()
-
         return value
 
     T = TypeVar('T', bound=Any)  # Generic type variable for return_type
     def get(self, *attributes, warn_missing: bool = False, is_print: bool = False,
             no_cache: bool = False, return_type: Optional[Type[T]] = None) -> Optional[T]:
         """
-        Returns a property or properties from MongoDB based on the input attributes,
-        using a cache file to improve performance.
+            Returns a property or properties from MongoDB based on the input attributes,
+            using a cache file to improve performance.
 
-        Args:
-            *attributes (str): A sequence of strings representing nested attributes.
-            warn_missing (bool, optional): Whether to warn if an attribute is missing.
-            is_print (bool, optional): Whether to print the return value.
-            no_cache (bool, optional): Whether to force a fresh MongoDB call.
-            return_type (Type[T], optional): The expected return type of the result.
-                Defaults to object, which includes any type.
+            Args:
+                *attributes (str): A sequence of strings representing nested attributes.
+                warn_missing (bool, optional): Whether to warn if an attribute is missing.
+                is_print (bool, optional): Whether to print the return value.
+                no_cache (bool, optional): Whether to force a fresh MongoDB call.
+                return_type (Type[T], optional): The expected return type of the result.
+                    Defaults to object, which includes any type.
+
+            Returns:
+                The value of the attribute if it exists in the cache or MongoDB,
+                cast to return_type, otherwise None.
 
-        Returns:
-            The value of the attribute if it exists in the cache or MongoDB,
-            cast to return_type, otherwise None.
-
-        Usage:
-            get('person', 'tyler', 'salary')  # Returns the value of person -> tyler -> salary
-        """
+            Usage:
+                get('person', 'tyler', 'salary')  # Returns the value of person -> tyler -> salary
+            """
 
+        path_cache_file = f"{self.path_config_dir}/cache.json"
         cache_update_needed = no_cache
 
-        # Check if cache data is available and not expired
-        if not no_cache and hasattr(self, 'cached_data') and 'expiresAt' in self.cached_data:
-            expires_at = datetime.fromisoformat(self.cached_data['expiresAt'])
-            cache_update_needed = datetime.now(timezone.utc) >= expires_at
+        # Check if cache file exists and is less than 1 hour old
+        if os.path.exists(path_cache_file):
+            last_modified = os.path.getmtime(path_cache_file)
+            if (time.time() - last_modified) / 3600 > 1:
+                cache_update_needed = True
+        else:
+            cache_update_needed = True
 
-        if cache_update_needed or not self.cached_data:
+        if cache_update_needed:
             self.update_cache()
 
+        # Read from cache
+        try:
+            with open(path_cache_file, "r", encoding="utf-8") as file:
+                cached_data = json.load(file)
+        except FileNotFoundError:
+            self.log(f"Cache file not found at {path_cache_file}", level="warn")
+            return None
+        except json.decoder.JSONDecodeError:
+            self.log(f"Could not read Cabinet cache at {path_cache_file}. Clearing.", level="warn")
+            try:
+                os.remove(path_cache_file)
+                print(f"File removed successfully: {path_cache_file}")
+                print("Please retry your last command.")
+                sys.exit(0)
+            except PermissionError:
+                self.log(f"Permission denied: Unable to delete the file at {path_cache_file}",
+                         level="error")
+            return None
+
         # Process the cached data
-        for document in self.cached_data:
+        for document in cached_data:
             result = document
             for attribute in attributes:
                 if isinstance(result, dict) and attribute in result:
                     result = result[attribute]
                 else:
                     if warn_missing:
                         self.log(f"Attribute '{attribute}' is missing", level="warn")
                     return None
 
             if isinstance(result, str):
                 result = helpers.resolve_path(result)
 
             if is_print:
-                if isinstance(result, dict):
-                    print(json.dumps(result, indent=4))
-                else:
-                    print(result)
+                print(result)
 
             # Handle return_type if specified
             if return_type is not None:
                 try:
                     return return_type(result)
                 except (ValueError, TypeError) as e:
                     self.log(f"Error casting result to {return_type}: {str(e)}", level="error")
                     return None
             else:
-                # return as-is if no specific return_type is needed
-                return result  # type: ignore
+                return result  # Return as is if no specific return_type is needed
 
         if warn_missing:
-            self.log(f"'{attributes}' not found in cache or MongoDB", level="warn")
+            self.log("No document found in cache or MongoDB", level="warn")
         return None
 
-    def remove(self, *attribute: str, is_print: bool = False):
+    def remove(self, *attribute, is_print: bool = False):
         """
-        Removes a property from the data in the MongoDB collection.
-
-        Args:
-            attribute: A variable length argument list representing \
-                the nested structure of the attribute to remove.
-            is_print (bool): Whether to print the result of the removal operation.
-
-        Example:
-            To remove the nested attribute `a.b.c`, call remove('a', 'b', 'c').
+        Removes a property from the data
         """
 
-        if not attribute or len(attribute) < 1:
-            raise ValueError("At least one attribute must be provided")
-
         custom_filter = {}
 
         cache = attribute[-1]
         json_structure = {}
         for item in reversed(attribute[:-1]):
             try:
                 json_structure = {}
@@ -698,29 +679,15 @@
 
         if len(attribute) > 1:
             update = {"$unset": {attribute[0]: json_structure[attribute[0]]}}
         else:
             json_structure[attribute[0]] = 1
             update = {"$unset": json_structure}
 
-        try:
-            result = self.database.cabinet.update_many(custom_filter, update)
-        except ConnectionFailure as e:
-            print(f"Connection failure: {e}")
-            return
-        except OperationFailure as e:
-            print(f"Operation failure: {e}")
-            return
-        except PyMongoError as e:
-            print(f"General PyMongo error: {e}")
-            return
-        # pylint: disable=W0703
-        except Exception as e:
-            print(f"Unexpected error: {e}")
-            return
+        result = self.database.cabinet.update_many(custom_filter, update)
 
         if is_print:
             print(f"Modified {result.modified_count} item(s)")
             print(f"{' -> '.join(attribute)} removed\n")
 
     def log(self, message: str = '', log_name: str | None = None, level: str | None = None,
             log_folder_path: str | None = None, is_quiet: bool = False) -> None:
```

### Comparing `cabinet-2024.5.27.1/src/cabinet/constants.py` & `cabinet-2024.5.7.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.5.27.1/src/cabinet/mail.py` & `cabinet-2024.5.7.1/src/cabinet/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 Does not support Gmail.
 
 A throwaway email is highly recommended.
 """
 
 import smtplib
 from urllib.parse import unquote
-import subprocess
-import socket
-import shlex
-import pwd
 import sys
+import pwd
 import os
+import subprocess
+import shlex
 from typing import List
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 import cabinet
 
 class Mail:
     """
@@ -53,29 +52,29 @@
         Args:
         - subject (str): The subject of the email.
         - body (str): The body of the email.
         - signature (str): The signature to include at the end of the email.
         - to_addr (List): A list of email addresses to send the email to.
         - from_name (str, optional): The name to appear in the "From" field of the email.
             Reads from cabinet -> email -> from_name if unset.
-            If this is unset, defaults to machine's hostname or `Cabinet`
+            If this is unset, defaults to os.getenv("HOSTNAME") or `Cabinet`
         - logging_enabled (bool, optional): Whether to log the email send event.
             Defaults to True.
         - is_quiet: Whether to suppress log output.
             Defaults to False.
 
         Raises:
         - smtplib.SMTPAuthenticationError: If the SMTP server rejects the login credentials.
 
         Gmail will almost certainly not work.
         """
 
-        hostname = socket.gethostname()
+        hostname = os.getenv("HOSTNAME")
         if hostname:
-            hostname = hostname.capitalize().replace(".local", "")
+            hostname = hostname.capitalize()
 
         cab_from_name = self.cab.get("email", "from_name") or hostname or "Cabinet"
 
         # send IP if reminder came directly from outside of server
         client_name = os.getenv('SSH_CONNECTION')
 
         if client_name:
```

### Comparing `cabinet-2024.5.27.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.5.27.1
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -126,15 +126,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

