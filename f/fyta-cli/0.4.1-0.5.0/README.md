# Comparing `tmp/fyta_cli-0.4.1.tar.gz` & `tmp/fyta_cli-0.5.0.tar.gz`

## Comparing `fyta_cli-0.4.1.tar` & `fyta_cli-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/src/fyta_cli/__init__.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/src/fyta_cli/fyta_client.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/src/fyta_cli/fyta_connector.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/src/fyta_cli/fyta_exceptions.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/src/fyta_cli/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/src/fyta_cli/__init__.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/src/fyta_cli/fyta_client.py
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/src/fyta_cli/fyta_connector.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/src/fyta_cli/fyta_exceptions.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/src/fyta_cli/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.5.0/PKG-INFO
```

### Comparing `fyta_cli-0.4.1/.github/workflows/pylint.yml` & `fyta_cli-0.5.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.4.1/.github/workflows/python-publish.yml` & `fyta_cli-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.4.1/.github/workflows/ruff.yml` & `fyta_cli-0.5.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.4.1/src/fyta_cli/fyta_client.py` & `fyta_cli-0.5.0/src/fyta_cli/fyta_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,116 +4,134 @@
 
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime, timedelta
 import logging
 from typing import Any
+from zoneinfo import ZoneInfo
 
 from aiohttp import BasicAuth, ClientSession
 
 from .fyta_exceptions import (
     FytaConnectionError,
     FytaAuthentificationError,
     FytaPasswordError,
     FytaPlantError,
-    )
+)
 
-FYTA_AUTH_URL = 'https://web.fyta.de/api/auth/login'
-FYTA_PLANT_URL = 'https://web.fyta.de/api/user-plant'
+FYTA_AUTH_URL = "https://web.fyta.de/api/auth/login"
+FYTA_PLANT_URL = "https://web.fyta.de/api/user-plant"
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class Client():
+class Client:
     """Client class to access FYTA API."""
-    def __init__(self, email: str, password: str, access_token = "", expiration = None):
+
+    # pylint: disable=too-many-instance-attributes
+    # pylint: disable=too-many-arguments
+
+    def __init__(
+        self,
+        email: str,
+        password: str,
+        access_token: str,
+        expiration: datetime,
+        tz: ZoneInfo,
+    ):
+        """Initialization."""
 
         self.email = email
         self.password = password
         self.access_token = access_token
         self.expiration = expiration
+        self.timezone = tz
 
         self.session: ClientSession = ClientSession()
         self._close_session = True
 
         self.request_timeout = 10
 
     async def test_connection(self) -> bool:
         """Test the connection to FYTA-Server"""
 
         response = await self.session.post(FYTA_AUTH_URL)
-        r=await response.text()
+        r = await response.text()
 
         if r == '{"message": "Unsupported Media Type"}':
             return True
 
         return False
 
-
-    async def login(self) -> dict[str,str | datetime]:
+    async def login(self) -> dict[str, str | datetime]:
         """Handle a request to FYTA."""
 
-        if self.access_token != "" and self.expiration.timestamp() > datetime.now().timestamp():
+        if (
+            self.access_token != ""
+            and self.expiration.timestamp() > datetime.now().timestamp()
+        ):
             return {"access_token": self.access_token, "expiration": self.expiration}
 
         payload = {
-            'email': self.email,
-            'password': self.password,
+            "email": self.email,
+            "password": self.password,
         }
 
         try:
             async with asyncio.timeout(self.request_timeout):
                 response = await self.session.post(
                     url=FYTA_AUTH_URL,
                     auth=BasicAuth(self.email, self.password),
-                    json=payload
+                    json=payload,
                 )
 
         except asyncio.TimeoutError as exception:
             _LOGGER.exception("timeout error")
             msg = "Timeout occurred while connecting to Fyta-server"
             raise FytaConnectionError(msg) from exception
 
         json_response = await response.json()
 
-        if json_response == {"statusCode":404,"error":"Not Found"}:
+        if json_response == {"statusCode": 404, "error": "Not Found"}:
             _LOGGER.exception("Authentication failed")
             raise FytaAuthentificationError
         if json_response == {
-            "statusCode":401,
-            "error":"Unauthorized",
-            "errors":[{"message":"Could not authenticate user"}]
+            "statusCode": 401,
+            "error": "Unauthorized",
+            "errors": [{"message": "Could not authenticate user"}],
         }:
             raise FytaPasswordError
 
         self.access_token = json_response["access_token"]
-        #self.refresh_token = json_response["refresh_token"]
-        self.expiration = datetime.now() + timedelta(seconds=int(json_response["expires_in"]))
+        # self.refresh_token = json_response["refresh_token"]
+        self.expiration = datetime.now(self.timezone) + timedelta(
+            seconds=int(json_response["expires_in"])
+        )
 
         return {"access_token": self.access_token, "expiration": self.expiration}
 
-    async def get_plants(self) -> dict[int,str]:
+    async def get_plants(self) -> dict[int, str]:
         """Get a list of all available plants from FYTA"""
 
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
         if self.expiration.timestamp() > datetime.now().timestamp():
-            await self.login() #get new access token, if current token expired
+            await self.login()  # get new access token, if current token expired
 
         header = {
             "Authorization": f"Bearer {self.access_token}",
             "Content-Type": "application/json",
         }
 
         try:
             async with asyncio.timeout(self.request_timeout):
-                response = await self.session.get(url=FYTA_PLANT_URL, headers = header)
+                response = await self.session.get(url=FYTA_PLANT_URL, headers=header)
         except asyncio.TimeoutError as exception:
             msg = "Timeout occurred while connecting to Fyta-server"
             raise FytaConnectionError(msg) from exception
 
         content_type = response.headers.get("Content-Type", "")
 
         if content_type.count("text/html") > 0:
@@ -124,55 +142,81 @@
                 {"Content-Type": content_type, "response": text},
             )
 
         json_response = await response.json()
 
         plant_list: dict = json_response["plants"]
 
-        plants: dict[int,str] = {}
+        plants: dict[int, str] = {}
         for plant in plant_list:
             plants |= {int(plant["id"]): plant["nickname"]}
 
         return plants
 
-    async def get_plant_data(self, plant_id: int) -> dict[str,Any]:
+    async def get_plant_data(self, plant_id: int) -> dict[str, Any]:
         """Get information about a specific plant"""
 
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
         if self.expiration.timestamp() > datetime.now().timestamp():
-            await self.login() #get new access token, if current token expired
+            await self.login()  # get new access token, if current token expired
 
         header = {
             "Authorization": f"Bearer {self.access_token}",
             "Content-Type": "application/json",
         }
 
         url = f"{FYTA_PLANT_URL}/{plant_id}"
 
         try:
             async with asyncio.timeout(self.request_timeout):
-                response = await self.session.get(url=url, headers = header)
+                response = await self.session.get(url=url, headers=header)
+        except asyncio.TimeoutError as exception:
+            msg = "Timeout occurred while connecting to Fyta-server"
+            raise FytaConnectionError(msg) from exception
+
+        content_type = response.headers.get("Content-Type", "")
+
+        if content_type.count("text/html") > 0:
+            text = await response.text()
+            msg = f"Error occurred while fetching plant data for plant {plant_id}"
+            raise FytaPlantError(
+                msg,
+                {"Content-Type": content_type, "response": text},
+            )
+
+        plant = await response.json()
+
+        #fetch DLI information from measurements
+        url = f"{FYTA_PLANT_URL}/measurements/{plant_id}"
+        body = "{'search': {'timeline': 'day'}}"
+
+        try:
+            async with asyncio.timeout(self.request_timeout):
+                response = await self.session.post(url=url, headers=header, data=body)
         except asyncio.TimeoutError as exception:
             msg = "Timeout occurred while connecting to Fyta-server"
             raise FytaConnectionError(msg) from exception
 
         content_type = response.headers.get("Content-Type", "")
 
         if content_type.count("text/html") > 0:
             text = await response.text()
             msg = f"Error occurred while fetching plant data for plant {plant_id}"
             raise FytaPlantError(
                 msg,
                 {"Content-Type": content_type, "response": text},
             )
 
-        plant: dict[str,Any] = await response.json()
+        measurements = await response.json()
+
+        if measurements["dli_light"] != []:
+            plant["plant"] |= {"dli_light": measurements["dli_light"][0]["dli_light"]}
 
         return plant
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
```

### Comparing `fyta_cli-0.4.1/src/fyta_cli/fyta_connector.py` & `fyta_cli-0.5.0/src/fyta_cli/fyta_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, UTC
 from typing import Any
 from zoneinfo import ZoneInfo
 
 from .fyta_client import Client
 from .utils import safe_get
 
-#status = 0 if user_plant deleted, 1 for user_plant in green, 2 for yellow, 3 for red
+# status = 0 if user_plant deleted, 1 for user_plant in green, 2 for yellow, 3 for red
 PLANT_STATUS = {
     0: "deleted",
     1: "doing_great",
     2: "need_attention",
     3: "no_sensor",
 }
 
@@ -28,44 +28,47 @@
 class FytaConnector:
     """Connector class to access FYTA API."""
 
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-many-arguments
 
     def __init__(
-            self,
-            email: str,
-            password: str,
-            access_token: str = "",
-            expiration: datetime | None = None,
-            tz: str = "",
+        self,
+        email: str,
+        password: str,
+        access_token: str = "",
+        expiration: datetime | None = None,
+        tz: str = "",
     ) -> None:
         """Initialize connector class."""
-        self.email: str = email
-        self.password: str = password
-        self.client = Client(email, password, access_token, expiration)
+
+        timezone: ZoneInfo = UTC if tz == "" else ZoneInfo(tz)
+        ex: datetime = (
+            datetime.now(timezone)
+            if expiration is None
+            else expiration.astimezone(timezone)
+        )
         self.online: bool = False
         self.plant_list: dict[int, str] = {}
         self.plants: dict[int, dict[str, Any]] = {}
-        self.access_token: str = access_token
-        self.expiration: datetime | None = expiration
-        self.timezone: ZoneInfo = UTC if tz == "" else ZoneInfo(tz)
+
+        self.client = Client(email, password, access_token, ex, timezone)
 
     async def test_connection(self) -> bool:
         """Test if connection to FYTA API works."""
 
         return await self.client.test_connection()
 
     async def login(self) -> dict[str, str | datetime]:
         """Login with credentials to get access token."""
 
         login = await self.client.login()
-        self.access_token = login["access_token"]
-        self.expiration = login["expiration"]
-        self.online = True
+
+        if login != {}:
+            self.online = True
 
         return login
 
     async def update_plant_list(self) -> dict[int, str]:
         """Get list of all available plants."""
 
         self.plant_list = await self.client.get_plants()
@@ -98,50 +101,102 @@
         if ("plant" not in p) or (p["plant"]["sensor"] is None):
             current_plant |= {"sensor_available": False}
         else:
             plant_data: dict = p["plant"]
             current_plant |= {"online": True}
             current_plant |= {"sensor_available": True}
             current_plant |= {
-                "battery_status:": safe_get(plant_data, "sensor.is_battery_low", bool)}
+                "battery_status:": safe_get(plant_data, "sensor.is_battery_low", bool)
+            }
             current_plant |= {"sw_version": safe_get(plant_data, "sensor.version", str)}
             current_plant |= {"plant_id": safe_get(plant_data, "plant_id", int)}
             current_plant |= {"name": safe_get(plant_data, "nickname", str)}
-            current_plant |= {"scientific_name": safe_get(plant_data, "scientific_name", str)}
+            current_plant |= {
+                "scientific_name": safe_get(plant_data, "scientific_name", str)
+            }
             current_plant |= {"status": safe_get(plant_data, "status", int)}
-            current_plant |= {"plant_thumb_path": safe_get(plant_data, "plant_thumb_path", str)}
-            current_plant |= {"plant_origin_path": safe_get(plant_data, "plant_origin_path", str)}
             current_plant |= {
-                "temperature_status": safe_get(plant_data, "measurements.temperature.status", int)}
+                "plant_thumb_path": safe_get(plant_data, "plant_thumb_path", str)
+            }
             current_plant |= {
-                "light_status": safe_get(plant_data, "measurements.light.status", int)}
+                "plant_origin_path": safe_get(plant_data, "plant_origin_path", str)
+            }
             current_plant |= {
-                "moisture_status": safe_get(plant_data, "measurements.moisture.status", int)}
+                "temperature_status": safe_get(
+                    plant_data, "measurements.temperature.status", int
+                )
+            }
             current_plant |= {
-                "salinity_status": safe_get(plant_data, "measurements.salinity.status", int)}
-            current_plant |= {"ph": safe_get(plant_data, "measurements.ph.values.current", float)}
+                "light_status": safe_get(plant_data, "measurements.light.status", int)
+            }
+            current_plant |= {
+                "moisture_status": safe_get(
+                    plant_data, "measurements.moisture.status", int
+                )
+            }
+            current_plant |= {
+                "salinity_status": safe_get(
+                    plant_data, "measurements.salinity.status", int
+                )
+            }
+            current_plant |= {
+                "ph": safe_get(plant_data, "measurements.ph.values.current", float)
+            }
             current_plant |= {
                 "temperature": safe_get(
-                    plant_data, "measurements.temperature.values.current", float)}
+                    plant_data, "measurements.temperature.values.current", float
+                )
+            }
             current_plant |= {
-                "light": safe_get(plant_data, "measurements.light.values.current", float)}
+                "light": safe_get(
+                    plant_data, "measurements.light.values.current", float
+                )
+            }
+            current_plant |= {"light_dli": safe_get(plant_data, "dli_light", float)}
             current_plant |= {
-                "moisture": safe_get(plant_data, "measurements.moisture.values.current", float)}
+                "moisture": safe_get(
+                    plant_data, "measurements.moisture.values.current", float
+                )
+            }
             current_plant |= {
-                "salinity": safe_get(plant_data, "measurements.salinity.values.current", float)}
-            current_plant |= {"battery_level": safe_get(plant_data, "measurements.battery", float)}
+                "salinity": safe_get(
+                    plant_data, "measurements.salinity.values.current", float
+                )
+            }
+            current_plant |= {
+                "battery_level": safe_get(plant_data, "measurements.battery", float)
+            }
             current_plant |= {
                 "last_updated": safe_get(
-                    plant_data, "sensor.received_data_at", datetime, self.timezone)
+                    plant_data,
+                    "sensor.received_data_at",
+                    datetime,
+                    self.client.timezone,
+                )
             }
 
         return current_plant
 
     @property
-    def fyta_id(self) -> str:
-        """ID for FYTA object."""
-        return self.email
+    def access_token(self) -> str:
+        """Access token for FYTA API."""
+        return self.client.access_token
 
     @property
     def data(self) -> dict:
         """ID for FYTA object."""
         return self.plants
+
+    @property
+    def email(self) -> str:
+        """Email of FYTA account."""
+        return self.client.email
+
+    @property
+    def expiration(self) -> datetime:
+        """Expiration of access token."""
+        return self.client.expiration
+
+    @property
+    def fyta_id(self) -> str:
+        """ID for FYTA object."""
+        return self.email
```

### Comparing `fyta_cli-0.4.1/src/fyta_cli/utils.py` & `fyta_cli-0.5.0/src/fyta_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.4.1/LICENSE` & `fyta_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.4.1/pyproject.toml` & `fyta_cli-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fyta_cli"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the FYTA API"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `fyta_cli-0.4.1/PKG-INFO` & `fyta_cli-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fyta_cli
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python library to access the FYTA API
 Project-URL: Repository, https://github.com/dontinelli/fyta_cli.git
 Project-URL: Issues, https://github.com/dontinelli/fyta_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/fyta_cli/blob/master/CHANGELOG.md
 Project-URL: FYTA homepage, https://fyta.de/
 Project-URL: API Documentation, https://fyta-io.notion.site/FYTA-Public-API-d2f4c30306f74504924c9a40402a3afd
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

