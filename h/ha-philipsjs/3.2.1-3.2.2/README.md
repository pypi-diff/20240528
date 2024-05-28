# Comparing `tmp/ha-philipsjs-3.2.1.tar.gz` & `tmp/ha-philipsjs-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-philipsjs-3.2.1.tar", last modified: Tue May 21 21:33:07 2024, max compression
+gzip compressed data, was "ha-philipsjs-3.2.2.tar", last modified: Tue May 28 19:41:37 2024, max compression
```

## Comparing `ha-philipsjs-3.2.1.tar` & `ha-philipsjs-3.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.744592 ha-philipsjs-3.2.1/
--rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.2.1/LICENSE
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-21 21:33:07.744665 ha-philipsjs-3.2.1/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)     1479 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.1/README.md
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.742789 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-21 21:33:07.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)      522 2024-05-21 21:33:07.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/SOURCES.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2024-05-21 21:33:07.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/dependency_links.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/not-zip-safe
--rw-r--r--   0 joakim     (501) staff       (20)      123 2024-05-21 21:33:07.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/requires.txt
--rw-r--r--   0 joakim     (501) staff       (20)       12 2024-05-21 21:33:07.000000 ha-philipsjs-3.2.1/ha_philipsjs.egg-info/top_level.txt
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.743301 ha-philipsjs-3.2.1/haphilipsjs/
--rw-r--r--   0 joakim     (501) staff       (20)    51918 2024-05-21 21:30:19.000000 ha-philipsjs-3.2.1/haphilipsjs/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)    12169 2023-10-25 16:41:37.000000 ha-philipsjs-3.2.1/haphilipsjs/__main__.py
--rw-r--r--   0 joakim     (501) staff       (20)     7379 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.1/haphilipsjs/auth.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.743641 ha-philipsjs-3.2.1/haphilipsjs/data/
--rw-r--r--   0 joakim     (501) staff       (20)       20 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.1/haphilipsjs/data/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     6598 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.1/haphilipsjs/data/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)   428744 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.1/haphilipsjs/data/v6.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.744145 ha-philipsjs-3.2.1/haphilipsjs/dummy/
--rw-r--r--   0 joakim     (501) staff       (20)       18 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.1/haphilipsjs/dummy/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     1588 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.1/haphilipsjs/dummy/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.1/haphilipsjs/typing.py
--rw-r--r--   0 joakim     (501) staff       (20)      132 2024-05-21 21:33:07.744936 ha-philipsjs-3.2.1/setup.cfg
--rw-r--r--   0 joakim     (501) staff       (20)     1550 2024-05-21 21:33:00.000000 ha-philipsjs-3.2.1/setup.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-21 21:33:07.744480 ha-philipsjs-3.2.1/tests/
--rw-r--r--   0 joakim     (501) staff       (20)      392 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.1/tests/test_auth.py
--rw-r--r--   0 joakim     (501) staff       (20)    10142 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.1/tests/test_v1.py
--rw-r--r--   0 joakim     (501) staff       (20)    21781 2024-05-21 21:29:47.000000 ha-philipsjs-3.2.1/tests/test_v6.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.163080 ha-philipsjs-3.2.2/
+-rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.2.2/LICENSE
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-28 19:41:37.163166 ha-philipsjs-3.2.2/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)     1479 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.2/README.md
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.161238 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2024-05-28 19:41:37.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)      522 2024-05-28 19:41:37.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/SOURCES.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2024-05-28 19:41:37.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/dependency_links.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/not-zip-safe
+-rw-r--r--   0 joakim     (501) staff       (20)      123 2024-05-28 19:41:37.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/requires.txt
+-rw-r--r--   0 joakim     (501) staff       (20)       12 2024-05-28 19:41:37.000000 ha-philipsjs-3.2.2/ha_philipsjs.egg-info/top_level.txt
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.161737 ha-philipsjs-3.2.2/haphilipsjs/
+-rw-r--r--   0 joakim     (501) staff       (20)    51989 2024-05-28 19:41:28.000000 ha-philipsjs-3.2.2/haphilipsjs/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)    12169 2024-05-28 19:41:28.000000 ha-philipsjs-3.2.2/haphilipsjs/__main__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     7379 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.2/haphilipsjs/auth.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.162079 ha-philipsjs-3.2.2/haphilipsjs/data/
+-rw-r--r--   0 joakim     (501) staff       (20)       20 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.2/haphilipsjs/data/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     6598 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.2/haphilipsjs/data/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)   428744 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.2/haphilipsjs/data/v6.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.162612 ha-philipsjs-3.2.2/haphilipsjs/dummy/
+-rw-r--r--   0 joakim     (501) staff       (20)       18 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.2/haphilipsjs/dummy/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     1588 2023-10-24 10:31:13.000000 ha-philipsjs-3.2.2/haphilipsjs/dummy/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.2/haphilipsjs/typing.py
+-rw-r--r--   0 joakim     (501) staff       (20)      132 2024-05-28 19:41:37.163468 ha-philipsjs-3.2.2/setup.cfg
+-rw-r--r--   0 joakim     (501) staff       (20)     1550 2024-05-28 19:41:28.000000 ha-philipsjs-3.2.2/setup.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2024-05-28 19:41:37.162956 ha-philipsjs-3.2.2/tests/
+-rw-r--r--   0 joakim     (501) staff       (20)      392 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.2/tests/test_auth.py
+-rw-r--r--   0 joakim     (501) staff       (20)    10142 2023-10-24 10:31:39.000000 ha-philipsjs-3.2.2/tests/test_v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)    22068 2024-05-28 19:41:28.000000 ha-philipsjs-3.2.2/tests/test_v6.py
```

### Comparing `ha-philipsjs-3.2.1/LICENSE` & `ha-philipsjs-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/PKG-INFO` & `ha-philipsjs-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.2.1
+Version: 3.2.2
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.2
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.2.1/README.md` & `ha-philipsjs-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/ha_philipsjs.egg-info/PKG-INFO` & `ha-philipsjs-3.2.2/ha_philipsjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.2.1
+Version: 3.2.2
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.2.2
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.2.1/ha_philipsjs.egg-info/SOURCES.txt` & `ha-philipsjs-3.2.2/ha_philipsjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/__init__.py` & `ha-philipsjs-3.2.2/haphilipsjs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import httpx
 import logging
 import json
 import itertools
 from urllib.parse import quote
 from secrets import token_bytes, token_hex
 from base64 import b64decode, b64encode
+from functools import wraps
+
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.padding import PKCS7
 from cryptography.hazmat.primitives.hashes import SHA1
 from cryptography.hazmat.primitives.hmac import HMAC
 
 from .typing import (
@@ -196,14 +198,35 @@
         super().__init__(f"Non json data received: {data}")
         self.data = data
 
 
 T = TypeVar("T")
 
 
+def handle_httpx_exceptions(f):
+    """Wrap up httpx exceptions in our wanted variants."""
+    @wraps(f)
+    async def wrapper(*args, **kwds):
+        try:
+            try:
+                return await f(*args, **kwds)
+            except httpx.RemoteProtocolError as err:
+                LOG.warning("%r. We retry once, could be a reused session that was closed", err)
+                return await f(*args, **kwds)
+
+        except (httpx.ConnectTimeout, httpx.ConnectError) as err:
+            raise ConnectionFailure(err) from err
+        except (httpx.ProtocolError, httpx.ReadError) as err:
+            raise ProtocolFailure(err) from err
+        except httpx.HTTPError as err:
+            raise GeneralFailure(err) from err
+
+    return wrapper
+
+
 class PhilipsTV(object):
 
     channels: ChannelsType
     """All available channels, with ccid as key."""
 
     def __init__(
         self,
@@ -565,46 +588,40 @@
         if protocol == "https":
             port = HTTPS_PORT
         else:
             port = HTTP_PORT
 
         return f"{protocol}://{self._host}:{port}/{self.api_version}/{path}"
 
+    @handle_httpx_exceptions
     async def getReq(self, path, protocol = None) -> Optional[Dict]:
-        try:
-            resp = await self.session.get(self._url(path, protocol = protocol))
-            if resp.status_code == 401:
-                raise AutenticationFailure("Authenticaion failed to device")
+        resp = await self.session.get(self._url(path, protocol = protocol))
 
-            if resp.status_code != 200:
-                LOG.debug("Get failed: %s -> %d %s", path, resp.status_code, resp.text)
-                return None
+        if resp.status_code == 401:
+            raise AutenticationFailure("Authenticaion failed to device")
 
-            LOG.debug("Get succeded: %s -> %s", path, resp.text)
-            return decode_xtv_response(resp)
-        except (httpx.ConnectTimeout, httpx.ConnectError) as err:
-            raise ConnectionFailure(err) from err
-        except httpx.HTTPError as err:
-            raise GeneralFailure(err) from err
+        if resp.status_code != 200:
+            LOG.debug("Get failed: %s -> %d %s", path, resp.status_code, resp.text)
+            return None
 
+        LOG.debug("Get succeded: %s -> %s", path, resp.text)
+        return decode_xtv_response(resp)
+  
+    @handle_httpx_exceptions
     async def _getBinary(self, path: str) -> Tuple[Optional[bytes], Optional[str]]:
 
-        try:
-            resp = await self.session.get(self._url(path))
-            if resp.status_code == 401:
-                raise AutenticationFailure("Authenticaion failed to device")
-
-            if resp.status_code != 200:
-                return None, None
-            return resp.content, resp.headers.get("content-type")
-        except (httpx.ConnectTimeout, httpx.ConnectError) as err:
-            raise ConnectionFailure(err) from err
-        except httpx.HTTPError as err:
-            raise GeneralFailure(err) from err
+        resp = await self.session.get(self._url(path))
+        if resp.status_code == 401:
+            raise AutenticationFailure("Authenticaion failed to device")
+
+        if resp.status_code != 200:
+            return None, None
+        return resp.content, resp.headers.get("content-type")
 
+    @handle_httpx_exceptions
     async def postReq(self, path: str, data: Any, timeout=None, protocol=None) -> Optional[Dict]:
         try:
             resp = await self.session.post(self._url(path, protocol), json=data, timeout=timeout)
             if resp.status_code == 401:
                 raise AutenticationFailure("Authenticaion failed to device")
 
             if resp.status_code == 200:
@@ -612,20 +629,14 @@
                 return decode_xtv_response(resp)
 
             LOG.warning("Post failed: %s -> %s", data, resp.text)
             return None
         except httpx.ReadTimeout:
             LOG.debug("Read time out on postReq", exc_info=True)
             return None
-        except (httpx.ConnectTimeout, httpx.ConnectError) as err:
-            raise ConnectionFailure(err) from err
-        except (httpx.ProtocolError, httpx.ReadError) as err:
-            raise ProtocolFailure(err) from err
-        except httpx.HTTPError as err:
-            raise GeneralFailure(err) from err
 
     async def pairRequest(
         self,
         app_id: str,
         app_name: str,
         device_name: str,
         device_os: str,
```

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/__main__.py` & `ha-philipsjs-3.2.2/haphilipsjs/__main__.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/auth.py` & `ha-philipsjs-3.2.2/haphilipsjs/auth.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/data/v1.py` & `ha-philipsjs-3.2.2/haphilipsjs/data/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/data/v6.py` & `ha-philipsjs-3.2.2/haphilipsjs/data/v6.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/dummy/v1.py` & `ha-philipsjs-3.2.2/haphilipsjs/dummy/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/haphilipsjs/typing.py` & `ha-philipsjs-3.2.2/haphilipsjs/typing.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/setup.py` & `ha-philipsjs-3.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 PACKAGE_NAME = 'ha-philipsjs'
 HERE = os.path.abspath(os.path.dirname(__file__))
-VERSION = '3.2.1'
+VERSION = '3.2.2'
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*', 'dist', 'ccu', 'build'])
 
 REQUIRES = [
     "cryptography",
     "httpx>=0.22.0",
 ]
```

### Comparing `ha-philipsjs-3.2.1/tests/test_v1.py` & `ha-philipsjs-3.2.2/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.2.1/tests/test_v6.py` & `ha-philipsjs-3.2.2/tests/test_v6.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,23 @@
 async def test_send_key_off(client_mock, param: Param):
     respx.post(f"{param.base}/input/key").mock(side_effect=httpx.ConnectTimeout)
 
     with pytest.raises(haphilipsjs.ConnectionFailure):
         await client_mock.sendKey("Standby")
 
 
+async def test_send_key_retry(client_mock, param: Param):
+    route = respx.post(f"{param.base}/input/key").mock(side_effect=httpx.RemoteProtocolError)
+
+    with pytest.raises(haphilipsjs.ProtocolFailure):
+        await client_mock.sendKey("Standby")
+
+    assert route.call_count == 2
+
+
 async def test_ambilight_mode(client_mock, param):
     await client_mock.getSystem()
 
     respx.post(f"{param.base}/ambilight/mode").respond(json={})
     await client_mock.setAmbilightMode("internal")
 
     if client_mock.quirk_ambilight_mode_ignored:
```

