# Comparing `tmp/slurpit_sdk-0.9.23.tar.gz` & `tmp/slurpit_sdk-0.9.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_sdk-0.9.23.tar", max compression
+gzip compressed data, was "slurpit_sdk-0.9.32.tar", max compression
```

## Comparing `slurpit_sdk-0.9.23.tar` & `slurpit_sdk-0.9.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-05-21 13:11:58.110837 slurpit_sdk-0.9.23/LICENSE
--rw-r--r--   0        0        0     1710 2024-05-21 17:21:43.856014 slurpit_sdk-0.9.23/README.md
--rw-r--r--   0        0        0      297 2024-05-21 17:21:43.856014 slurpit_sdk-0.9.23/pyproject.toml
--rw-r--r--   0        0        0       57 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/api.py
--rw-r--r--   0        0        0        0 2024-05-21 17:22:03.612142 slurpit_sdk-0.9.23/src/slurpit/apis/__init__.py
--rw-r--r--   0        0        0     7758 2024-05-21 13:57:31.144522 slurpit_sdk-0.9.23/src/slurpit/apis/baseapi.py
--rw-r--r--   0        0        0    11278 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/deviceapi.py
--rw-r--r--   0        0        0     4077 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/planningapi.py
--rw-r--r--   0        0        0     1182 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/platformapi.py
--rw-r--r--   0        0        0     7962 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/scannerapi.py
--rw-r--r--   0        0        0    14842 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/scraperapi.py
--rw-r--r--   0        0        0     8168 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/templateapi.py
--rw-r--r--   0        0        0     4847 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/userapi.py
--rw-r--r--   0        0        0     4441 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/apis/vaultapi.py
--rw-r--r--   0        0        0        0 2024-05-21 17:22:03.616142 slurpit_sdk-0.9.23/src/slurpit/models/__init__.py
--rw-r--r--   0        0        0       27 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/basemodel.py
--rw-r--r--   0        0        0     2606 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/device.py
--rw-r--r--   0        0        0     1301 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/planning.py
--rw-r--r--   0        0        0      396 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/platform.py
--rw-r--r--   0        0        0     2017 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/scanner.py
--rw-r--r--   0        0        0     1932 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/template.py
--rw-r--r--   0        0        0     2107 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/user.py
--rw-r--r--   0        0        0     2738 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.23/src/slurpit/models/vault.py
--rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.23/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-21 13:11:58.110837 slurpit_sdk-0.9.32/LICENSE
+-rw-r--r--   0        0        0     1710 2024-05-28 08:14:23.504730 slurpit_sdk-0.9.32/README.md
+-rw-r--r--   0        0        0      297 2024-05-28 08:28:20.669911 slurpit_sdk-0.9.32/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/__init__.py
+-rw-r--r--   0        0        0     2643 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/api.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:34:49.520606 slurpit_sdk-0.9.32/src/slurpit/apis/__init__.py
+-rw-r--r--   0        0        0     7759 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/baseapi.py
+-rw-r--r--   0        0        0    12580 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/deviceapi.py
+-rw-r--r--   0        0        0     4077 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/planningapi.py
+-rw-r--r--   0        0        0     1182 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/platformapi.py
+-rw-r--r--   0        0        0     7962 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/scannerapi.py
+-rw-r--r--   0        0        0    14842 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/scraperapi.py
+-rw-r--r--   0        0        0     8168 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/templateapi.py
+-rw-r--r--   0        0        0     4847 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/userapi.py
+-rw-r--r--   0        0        0     4441 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/apis/vaultapi.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:34:49.532606 slurpit_sdk-0.9.32/src/slurpit/models/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/basemodel.py
+-rw-r--r--   0        0        0     2606 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/device.py
+-rw-r--r--   0        0        0     1301 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/planning.py
+-rw-r--r--   0        0        0      396 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/platform.py
+-rw-r--r--   0        0        0     2017 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/scanner.py
+-rw-r--r--   0        0        0     1932 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/template.py
+-rw-r--r--   0        0        0     2107 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/user.py
+-rw-r--r--   0        0        0     2738 2024-05-28 08:14:23.508730 slurpit_sdk-0.9.32/src/slurpit/models/vault.py
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.32/PKG-INFO
```

### Comparing `slurpit_sdk-0.9.23/LICENSE` & `slurpit_sdk-0.9.32/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/README.md` & `slurpit_sdk-0.9.32/README.md`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/api.py` & `slurpit_sdk-0.9.32/src/slurpit/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,17 +21,29 @@
             token (str): The API key used for authenticating requests.
             users (UserAPI): An instance of UserAPI initialized with the base URL and API key.
             vault (VaultAPI): An instance of VaultAPI initialized with the base URL and API key.
             platform (PlatformAPI): An instance of PlatformAPI initialized with the base URL and API key.
         """
         base_url = "{}/api".format(url if url[-1] != "/" else url[:-1])  # Format the base URL to ensure it ends with '/api'
         self.base_url = base_url  # Set the formatted base URL
-        self.token = api_key  # Store the API key
+        self.api_key = api_key  # Store the API key
         self.users = UserAPI(base_url, api_key)  # Initialize the UserAPI with the base URL and API key
         self.vault = VaultAPI(base_url, api_key)  # Initialize the VaultAPI with the base URL and API key
         self.platform = PlatformAPI(base_url, api_key)  # Initialize the PlatformAPI with the base URL and API key
         self.device = DeviceAPI(base_url, api_key)
         self.planning = PlanningAPI(base_url, api_key)
         self.scanner = ScannerAPI(base_url, api_key)
         self.scraper = ScraperAPI(base_url, api_key)
         self.templates = TemplateAPI(base_url, api_key)
+
+    def get_all(self):
+        if not self.base_url or not self.api_key:
+            raise Exception("Please confirm the host url or api key.")
+        
+        users = self.users.get_users()
+        vaults = self.vault.get_vaults()
+        plannings = self.planning.get_plannings()
+        templates = self.templates.get_templates()
+        scanners = self.scanner.get
+        devices = self.device.get_devices()
+
```

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/baseapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/baseapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             error_message = e.response.json().get('messages', {}).get('error', 'No error message provided')
             print(f"HTTP Error: {e}")
             print(f"Error Message: {error_message}")
             raise
         except requests.exceptions.RequestException as e:
             print(f"Request Error: {e}")
             raise
+
     
     def post(self, url, data, **kwargs):
         """
         Sends a POST request with JSON data to the specified URL.
 
         Args:
             url (str): The URL to send the POST request to.
```

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/deviceapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/deviceapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             list[Device] | bytes | pd.DataFrame: A list of Device instances, CSV data as bytes if export_csv is True, 
                                                 or a pandas DataFrame if export_df is True.
         """
         url = f"{self.base_url}/devices"
         params = {'offset': offset, 'limit': limit}
         try:
             response = self.get(url, params=params)
+
             if response:
                 devices_data = response.json()
                 if export_csv:
                     return self.json_to_csv_bytes(devices_data)
                 elif export_df:
                     return pd.DataFrame(devices_data)
                 else:
@@ -259,14 +260,45 @@
             if response:
                 snapshot_data = response.json()
                 return snapshot_data
         except Exception as e:
             print(f"Unexpected error: {e}")
             raise
 
+
+    def get_all_snapshots(self, export_csv: bool = False, export_df: bool = False):
+        """
+        Retrieve latest data for all devices, and optionally exports the data to a CSV format or pandas DataFrame.
+
+        Args:
+            export_csv (bool): If True, returns the snapshot data in CSV format as bytes.
+                            If False, returns a list of snapshot data dictionaries.
+            export_df (bool): If True, returns the snapshot data as a pandas DataFrame.
+
+        Returns:
+            list[dict] | bytes | pd.DataFrame: A list of snapshot data dictionaries, CSV data as bytes if export_csv is True,
+                                            or a pandas DataFrame if export_df is True.
+        """
+        snapshots = []
+        devices = self.get_devices()
+        if devices:
+            for device in devices:
+                try:
+                    data = self.get_snapshots(device.hostname)
+                    snapshots.extend(data)
+                except Exception as e:
+                    print(f"Error retrieving snapshots for device {device.hostname}: {e}")
+
+        if export_csv:
+            return self.json_to_csv_bytes(snapshots)
+        elif export_df:
+            return pd.DataFrame(snapshots)
+        else:
+            return snapshots
+        
     def test_ssh(self, ssh_info: dict):
         """
         Tests SSH connectivity using the provided SSH information.
 
         Args:
             ssh_info (dict): A dictionary containing the SSH credentials and details.
```

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/planningapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/planningapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/platformapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/platformapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/scannerapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/scannerapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/scraperapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/scraperapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/templateapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/templateapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/userapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/userapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/apis/vaultapi.py` & `slurpit_sdk-0.9.32/src/slurpit/apis/vaultapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/device.py` & `slurpit_sdk-0.9.32/src/slurpit/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/planning.py` & `slurpit_sdk-0.9.32/src/slurpit/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/scanner.py` & `slurpit_sdk-0.9.32/src/slurpit/models/scanner.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/template.py` & `slurpit_sdk-0.9.32/src/slurpit/models/template.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/user.py` & `slurpit_sdk-0.9.32/src/slurpit/models/user.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/src/slurpit/models/vault.py` & `slurpit_sdk-0.9.32/src/slurpit/models/vault.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.23/PKG-INFO` & `slurpit_sdk-0.9.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_sdk
-Version: 0.9.23
+Version: 0.9.32
 Summary: A robust Python SDK for slurpit
 Author: Slurp'it
 Author-email: info@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

