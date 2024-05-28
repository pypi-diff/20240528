# Comparing `tmp/uat_breeze_connect-1.0.14rc38.tar.gz` & `tmp/uat_breeze_connect-1.0.14rc39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\uat_breeze_connect-1.0.14rc38.tar", last modified: Fri May 17 10:03:51 2024, max compression
+gzip compressed data, was "dist\uat_breeze_connect-1.0.14rc39.tar", last modified: Tue May 28 09:04:26 2024, max compression
```

## Comparing `uat_breeze_connect-1.0.14rc38.tar` & `uat_breeze_connect-1.0.14rc39.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.660234 uat_breeze_connect-1.0.14rc38/
--rw-rw-rw-   0        0        0     1100 2024-05-17 09:48:40.000000 uat_breeze_connect-1.0.14rc38/LICENSE
--rw-rw-rw-   0        0        0    20013 2024-05-17 10:03:51.659972 uat_breeze_connect-1.0.14rc38/PKG-INFO
--rw-rw-rw-   0        0        0    19478 2024-05-17 10:03:38.000000 uat_breeze_connect-1.0.14rc38/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.555112 uat_breeze_connect-1.0.14rc38/breeze_connect/
--rw-rw-rw-   0        0        0       55 2024-05-17 09:48:41.000000 uat_breeze_connect-1.0.14rc38/breeze_connect/__init__.py
--rw-rw-rw-   0        0        0    98442 2024-05-17 10:02:30.000000 uat_breeze_connect-1.0.14rc38/breeze_connect/breeze_connect.py
--rw-rw-rw-   0        0        0       42 2024-05-17 10:03:51.685066 uat_breeze_connect-1.0.14rc38/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-17 09:52:01.000000 uat_breeze_connect-1.0.14rc38/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.657841 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/
--rw-rw-rw-   0        0        0    20013 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 09:04:26.616498 uat_breeze_connect-1.0.14rc39/
+-rw-rw-rw-   0        0        0     1100 2024-05-28 08:58:50.000000 uat_breeze_connect-1.0.14rc39/LICENSE
+-rw-rw-rw-   0        0        0    19975 2024-05-28 09:04:26.616498 uat_breeze_connect-1.0.14rc39/PKG-INFO
+-rw-rw-rw-   0        0        0    19463 2024-05-28 09:03:35.000000 uat_breeze_connect-1.0.14rc39/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:04:26.506295 uat_breeze_connect-1.0.14rc39/breeze_connect/
+-rw-rw-rw-   0        0        0       55 2024-05-28 08:58:50.000000 uat_breeze_connect-1.0.14rc39/breeze_connect/__init__.py
+-rw-rw-rw-   0        0        0    98345 2024-05-28 09:02:31.000000 uat_breeze_connect-1.0.14rc39/breeze_connect/breeze_connect.py
+-rw-rw-rw-   0        0        0    11141 2024-05-27 17:08:37.000000 uat_breeze_connect-1.0.14rc39/breeze_connect/config.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:04:26.620829 uat_breeze_connect-1.0.14rc39/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-05-28 09:03:35.000000 uat_breeze_connect-1.0.14rc39/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:04:26.614314 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/
+-rw-rw-rw-   0        0        0    19975 2024-05-28 09:04:26.000000 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-28 09:04:26.000000 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:04:26.000000 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-28 09:04:26.000000 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-28 09:04:26.000000 uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/top_level.txt
```

### Comparing `uat_breeze_connect-1.0.14rc38/LICENSE` & `uat_breeze_connect-1.0.14rc39/LICENSE`

 * *Files identical despite different names*

### Comparing `uat_breeze_connect-1.0.14rc38/PKG-INFO` & `uat_breeze_connect-1.0.14rc39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc38
+Version: 1.0.14rc39
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-socketio[client]
 Requires-Dist: requests
-Requires-Dist: pandas
 
 # Index
 
 <div class="sticky" id="index">
 <ul>
  <li><a href="#Uat_Breeze">UAT_Breeze_Connect_SDK</a></li>
  <li><a href="#Setup_env">Setup Virtual Environment</a></li>
@@ -79,15 +78,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc38
+pip install uat-breeze-connect==1.0.14rc39
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -430,15 +429,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -448,30 +447,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc38 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc39 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
-[client] Requires-Dist: requests Requires-Dist: pandas # Index
+[client] Requires-Dist: requests # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
     * _S_e_t_u_p_ _V_i_r_t_u_a_l_ _E_n_v_i_r_o_n_m_e_n_t
     * _I_n_s_t_a_l_l_i_n_g_ _t_h_e_ _c_l_i_e_n_t
     * _W_e_b_s_o_c_k_e_t_ _U_s_a_g_e
     * _A_P_I_ _U_s_a_g_e
     * _g_e_t___c_u_s_t_o_m_e_r___d_e_t_a_i_l_s
     * _g_e_t___d_e_m_a_t___h_o_l_d_i_n_g_s
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc39 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -291,15 +291,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -309,29 +309,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

### Comparing `uat_breeze_connect-1.0.14rc38/README.md` & `uat_breeze_connect-1.0.14rc39/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc38
+pip install uat-breeze-connect==1.0.14rc39
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -413,15 +413,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -431,30 +431,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -34,15 +34,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc39 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -285,15 +285,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -303,29 +303,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

### Comparing `uat_breeze_connect-1.0.14rc38/breeze_connect/breeze_connect.py` & `uat_breeze_connect-1.0.14rc39/breeze_connect/breeze_connect.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,272 @@
 import socketio
 import json
 import requests
 import base64
 from datetime import datetime
 from hashlib import sha256
 import csv
-from urllib3.exceptions import InsecureRequestWarning
 from io import BytesIO
 from zipfile import ZipFile
 from urllib.request import urlopen
 import pandas as pd
-import logging
-import functools
 import os
-import time
+import sys
+import logging
+
+dirs = os.path.dirname(os.path.abspath(__file__))
+
+sys.path.insert(1,dirs)
+import config
+import socket
 
 
-CACHE_FILE = "response_cache.json"
-CACHE_EXPIRATION = 120  # Cache expiration time in seconds
-response_cache = {}
 
 requests.packages.urllib3.util.connection.HAS_IPV6 = False
-url = "https://directlink.icicidirect.com/NewSecurityMaster/SecurityMaster.zip"
-resp = urlopen(url)
-zipfile = ZipFile(BytesIO(resp.read()))
 
-logger = logging.getLogger("engineio.client")
+resp = urlopen(config.SECURITY_MASTER_URL)
+zipfile = ZipFile(BytesIO(resp.read()))
+api_endpoint = config.APIEndPoint
+resp_message = config.ResponseMessage
+except_message = config.ExceptionMessage
+req_type = config.APIRequestType
+logger = logging.getLogger('engineio.client')
 logger.propagate = False
 logger.setLevel(logging.CRITICAL)
 
 
 class SocketEventBreeze(socketio.ClientNamespace):
-
+    
     def __init__(self, namespace, breeze_instance):
         super().__init__(namespace)
         self.breeze = breeze_instance
-        self.hostname = "https://uatstreams.icicidirect.com"
         self.sio = socketio.Client()
-        # self.sio.on('disconnect', on_trigger)
         self.tokenlist = set()
+        self.ohlcstate = set()
+        self.authentication = True
 
-    def connect(self):
-        auth = {
-            "user": self.breeze.user_id,
-            "token": self.breeze.session_key,
-            "appkey": self.breeze.api_key,
-        }
-        self.sio.connect(
-            self.hostname,
-            headers={"User-Agent": "python-socketio[client]/socket"},
-            auth=auth,
-            transports="websocket",
-            wait_timeout=50,
-        )
+    def my_connect_error(self,error):
+        self.authentication = False
+
+    def connect(self,hostname,is_ohlc_stream = False,strategy_flag = False):
+        try:
+            auth = {"user": self.breeze.user_id, "token": self.breeze.session_key}
+            if is_ohlc_stream:
+                self.sio.connect(hostname,socketio_path='ohlcvstream' ,headers={"User-Agent": "python-socketio[client]/socket"},auth=auth,transports="websocket", wait_timeout=3)
+            else:
+                self.sio.connect(hostname, headers={"User-Agent": "python-socketio[client]/socket"},auth=auth,transports="websocket", wait_timeout=3)
+            self.sio.on("connect_error", self.my_connect_error)
+        except Exception as e:
+            if self.sio.connected:
+                pass
+            else:
+                if hostname == config.LIVE_OHLC_STREAM_URL:
+                    raise Exception(except_message.OHLC_SOCKET_CONNECTION_DISCONNECTED.value)
+                elif hostname == config.LIVE_STREAM_URL:
+                    raise Exception(except_message.LIVESTREAM_SOCKET_CONNECTION_DISCONNECTED.value)
+                else:
+                    raise Exception(except_message.ORDERNOTIFY_SOCKET_CONNECTION_DISCONNECTED.value)            
 
     def on_disconnect(self):
         self.sio.emit("disconnect", "transport close")
-
-    def on_trigger(self):
-        print("reconnection triggered")
-
+        
+    def notify(self):
+        self.sio.on('order', self.on_message)
+    
     def on_message(self, data):
-
         data = self.breeze.parse_data(data)
-        if "symbol" in data and data["symbol"] != None and len(data["symbol"]) > 0:
-            data.update(self.breeze.get_data_from_stock_token_value(data["symbol"]))
-        # print(self.breeze)
-        if self.breeze.on_ticks != None:
+        if 'symbol' in data and data['symbol'] != None and len(data['symbol'])>0:
+            data.update(self.breeze.get_data_from_stock_token_value(data['symbol']))
+        if(self.breeze.on_ticks!=None):
             self.breeze.on_ticks(data)
-        if self.breeze.on_ticks2 != None:
+        if(self.breeze.on_ticks2!=None):
             self.breeze.on_ticks2(data)
 
-    def rewatch(self):
-        # print("rewatch",self.values)
-        if len(self.tokenlist) > 0:
-            self.sio.emit("join", list(self.tokenlist))
-            self.sio.on("stock", self.on_message)
-
-    def notify(self):
-        self.sio.on("order", self.on_message)
+    def on_ohlc_stream(self,data):
+        data = self.breeze.parse_ohlc_data(data)
+        self.breeze.on_ticks(data)
+
+    def rewatchohlc(self):
+        if(len(self.ohlcstate) > 0):
+            for room,channel in self.ohlcstate:
+                self.sio.emit('join',room)
+                self.sio.on(channel, self.on_ohlc_stream)
+    
+    def watch_stream_data(self,data,channel):
+        try:
+            if self.sio.connected:
+                if((data,channel) not in self.ohlcstate):
+                    self.ohlcstate.add((data,channel))
+                self.sio.emit('join', data)
+                self.sio.on(channel, self.on_ohlc_stream)
+                self.sio.on('connect',self.rewatchohlc)
+            else:
+                raise Exception(except_message.OHLC_SOCKET_CONNECTION_DISCONNECTED.value)
+        except Exception as e:
+            raise Exception(except_message.OHLC_SOCKET_CONNECTION_DISCONNECTED.value)
 
-    def watch(self, data, isStrategy=False):
-        if isinstance(data, list):
-            for entry in data:
-                self.tokenlist.add(entry)
-        else:
-            self.tokenlist.add(data)
-        self.sio.emit("join", data)
-        self.sio.on("stock", self.on_message)
-        self.sio.on("disconnect", self.on_trigger)
-        self.sio.on("connect", self.rewatch)
+    def rewatch(self):
+        self.notify()
+        if(len(self.tokenlist) > 0):    
+            self.sio.emit('join', list(self.tokenlist))
+            self.sio.on('stock', self.on_message)
+
+    def watch(self, data):
+        try:
+            if self.sio.connected:
+                if isinstance(data, list):
+                    for entry in data:   
+                        self.tokenlist.add(entry)
+                else:
+                    self.tokenlist.add(data)
 
+                self.sio.emit('join', data)
+                self.sio.on('stock', self.on_message)
+                self.sio.on('connect',self.rewatch)
+            else:
+                raise Exception(except_message.LIVESTREAM_SOCKET_CONNECTION_DISCONNECTED.value)
+        except Exception as e:
+            raise Exception(except_message.LIVESTREAM_SOCKET_CONNECTION_DISCONNECTED.value)
+        
     def unwatch(self, data):
         if isinstance(data, list):
             for entry in data:
-                if entry in self.tokenlist:
+                if(entry in self.tokenlist):
                     self.tokenlist.discard(entry)
         else:
-            if data in self.tokenlist:
+            if(data in self.tokenlist):
                 self.tokenlist.discard(data)
 
-        self.sio.emit("leave", data)
-
-    # @sio.on('reconnect')
-
-    # print("I'm connected to the /chat namespace!")
+        if(len(self.ohlcstate) > 0): 
+            to_be_removed = set()
+            for room,channel in self.ohlcstate:
+                if(room == data):
+                    to_be_removed.add((room,channel))
+            
+            for room,channel in to_be_removed:
+                self.ohlcstate.discard((room,channel))
 
+        self.sio.emit("leave", data)
 
-class BreezeConnect:
+class BreezeConnect():
 
     def __init__(self, api_key):  # needed for hashing json data
         self.user_id = None
         self.api_key = api_key
         self.session_key = None
         self.secret_key = None
-
-        self.sio_handler = None
+        self.sio_rate_refresh_handler = None
+        self.sio_order_refresh_handler = None
+        self.sio_ohlcv_stream_handler = None
         self.api_handler = None
         self.on_ticks = None
-        self.on_ticks2 = None
+        self.on_ticks2 = None #for strategy algo, not to expose to users
         self.stock_script_dict_list = []
         self.token_script_dict_list = []
-        self.tux_to_user_value = {
-            "orderFlow": {"B": "Buy", "S": "Sell", "N": "NA"},
-            "limitMarketFlag": {"L": "Limit", "M": "Market", "S": "StopLoss"},
-            "orderType": {"T": "Day", "I": "IoC", "V": "VTC"},
-            "productType": {
-                "F": "Futures",
-                "O": "Options",
-                "P": "FuturePlus",
-                "U": "FuturePlus_sltp",
-                "I": "OptionPlus",
-                "C": "Cash",
-                "Y": "eATM",
-                "B": "BTST",
-                "M": "Margin",
-                "T": "MarginPlus",
-            },
-            "orderStatus": {
-                "A": "All",
-                "R": "Requested",
-                "Q": "Queued",
-                "O": "Ordered",
-                "P": "Partially Executed",
-                "E": "Executed",
-                "J": "Rejected",
-                "X": "Expired",
-                "B": "Partially Executed And Expired",
-                "D": "Partially Executed And Cancelled",
-                "F": "Freezed",
-                "C": "Cancelled",
-            },
-            "optionType": {"C": "Call", "P": "Put", "*": "Others"},
-        }
+        self.tux_to_user_value = config.TUX_TO_USER_MAP
+        self.orderconnect = 0
+
+    def socket_connection_response(self,message):
+        return {"message":message}
+
+    def subscribe_exception(self,message):
+        return Exception(message)
+
+    def _ws_connect(self,handler,order_flag=False,ohlcv_flag=False,strategy_flag = False): 
+        if order_flag or strategy_flag:
+            if not self.sio_order_refresh_handler:
+                self.sio_order_refresh_handler = SocketEventBreeze("/", self)
+            if(self.orderconnect == 0):
+                self.sio_order_refresh_handler.connect(config.LIVE_FEEDS_URL)
+                self.orderconnect+=1
+            else:
+                pass
+        elif ohlcv_flag:
+            if not self.sio_ohlcv_stream_handler:
+                self.sio_ohlcv_stream_handler = SocketEventBreeze("/", self)
+            self.sio_ohlcv_stream_handler.connect(config.LIVE_OHLC_STREAM_URL,is_ohlc_stream=True)           
+        else:
+            if not self.sio_rate_refresh_handler: 
+                self.sio_rate_refresh_handler = SocketEventBreeze("/", self)
+            self.sio_rate_refresh_handler.connect(config.LIVE_STREAM_URL)
+    
+    def ws_disconnect(self):   
+        response = []       
+        if not self.sio_rate_refresh_handler:
+            response.append(self.socket_connection_response(resp_message.RATE_REFRESH_NOT_CONNECTED.value))
+        else:
+            self.sio_rate_refresh_handler.on_disconnect()
+            self.sio_rate_refresh_handler = None
+            response.append(self.socket_connection_response(resp_message.RATE_REFRESH_DISCONNECTED.value))
+        
+        if not self.sio_ohlcv_stream_handler:
+            response.append(self.socket_connection_response(resp_message.OHLCV_STREAM_NOT_CONNECTED.value))
+        else:
+            self.sio_ohlcv_stream_handler.on_disconnect()
+            self.sio_ohlcv_stream_handler = None
+            response.append(self.socket_connection_response(resp_message.OHLCV_STREAM_DISCONNECTED.value))
+        
+        if not self.sio_order_refresh_handler:
+            response.append(self.socket_connection_response(resp_message.ORDER_REFRESH_NOT_CONNECTED.value))
+        else:
+            self.orderconnect = 0
+            self.sio_order_refresh_handler.on_disconnect()
+            self.sio_order_refresh_handler = None
+            response.append(self.socket_connection_response(resp_message.ORDER_REFRESH_DISCONNECTED.value))
+        return(response)
 
-    def ws_connect(self):
-        if not self.sio_handler:
-            self.sio_handler = SocketEventBreeze("/", self)
-            self.sio_handler.connect()
-
-    def ws_disconnect(self):
-        if not self.sio_handler:
-            self.sio_handler = SocketEventBreeze("/", self)
-        self.sio_handler.on_disconnect()
 
+    def ws_disconnect_ohlc(self):
+        if self.sio_rate_refresh_handler:
+            self.sio_rate_refresh_handler.on_disconnect()
+            self.sio_rate_refresh_handler = None
+        if not self.sio_ohlcv_stream_handler:
+            return self.socket_connection_response(resp_message.OHLCV_STREAM_NOT_CONNECTED.value)
+        else:
+            self.sio_ohlcv_stream_handler.on_disconnect()
+            self.sio_ohlcv_stream_handler = None
+            return self.socket_connection_response(resp_message.OHLCV_STREAM_DISCONNECTED.value)
+    
+    def ws_connect(self):
+        self._ws_connect(self.sio_rate_refresh_handler,False)
+        
     def get_data_from_stock_token_value(self, input_stock_token):
         try:
             output_data = {}
             stock_token = input_stock_token.split(".")
             exchange_type, stock_token = stock_token[0], stock_token[1].split("!")[1]
             exchange_code_list = {
                 "1": "BSE",
                 "4": "NSE",
                 "13": "NDX",
                 "6": "MCX",
             }
             exchange_code_name = exchange_code_list.get(exchange_type, False)
             if exchange_code_name == False:
-                raise Exception(
-                    "Stock-Token cannot be found due to wrong exchange-code."
-                )
+                self.subscribe_exception(except_message.WRONG_EXCHANGE_CODE_EXCEPTION.value)
             elif exchange_code_name.lower() == "bse":
                 stock_data = self.token_script_dict_list[0].get(stock_token, False)
                 if stock_data == False:
-                    raise Exception(
-                        "Stock-Data does not exist in exchange-code BSE for Stock-Token "
-                        + input_stock_token
-                        + "."
-                    )
+                    self.subscribe_exception(except_message.STOCK_NOT_EXIST_EXCEPTION.value.format("BSE",input_stock_token))
             elif exchange_code_name.lower() == "nse":
                 stock_data = self.token_script_dict_list[1].get(stock_token, False)
                 if stock_data == False:
                     stock_data = self.token_script_dict_list[4].get(stock_token, False)
-                    if stock_data == False:
-                        raise Exception(
-                            "Stock_Token does not exist in both exchange-code i.e. NSE or NFO for Stock-Token "
-                            + input_stock_token
-                            + "."
-                        )
+                    if stock_data == False:    
+                        self.subscribe_exception(except_message.STOCK_NOT_EXIST_EXCEPTION.value.format("i.e. NSE or NFO",input_stock_token))
                     else:
                         exchange_code_name = "NFO"
             elif exchange_code_name.lower() == "ndx":
                 stock_data = self.token_script_dict_list[2].get(stock_token, False)
                 if stock_data == False:
-                    raise Exception(
-                        "Stock-Data does not exist in exchange-code NDX for Stock-Token "
-                        + input_stock_token
-                        + "."
-                    )
+                    self.subscribe_exception(except_message.STOCK_NOT_EXIST_EXCEPTION.value.format("NDX",input_stock_token))
             elif exchange_code_name.lower() == "mcx":
                 stock_data = self.token_script_dict_list[3].get(stock_token, False)
                 if stock_data == False:
-                    raise Exception(
-                        "Stock-Data does not exist in exchange-code MCX for Stock-Token "
-                        + input_stock_token
-                        + "."
-                    )
+                    self.subscribe_exception(except_message.STOCK_NOT_EXIST_EXCEPTION.value.format("MCX",input_stock_token))
             output_data["stock_name"] = stock_data[1]
             if exchange_code_name.lower() not in ["nse", "bse"]:
                 product_type = stock_data[0].split("-")[0]
                 if product_type.lower() == "fut":
                     output_data["product_type"] = "Futures"
                 if product_type.lower() == "opt":
                     output_data["product_type"] = "Options"
@@ -234,430 +281,391 @@
                         output_data["right"] = "Put"
                     if right.upper() == "CE":
                         output_data["right"] = "Call"
             return output_data
         except Exception as e:
             return {}
 
-    def get_stock_token_value(
-        self,
-        exchange_code="",
-        stock_code="",
-        product_type="",
-        expiry_date="",
-        strike_price="",
-        right="",
-        get_exchange_quotes=True,
-        get_market_depth=True,
-    ):
+    def get_stock_token_value(self, exchange_code="", stock_code="", product_type="", expiry_date="", strike_price="", right="", get_exchange_quotes=True, get_market_depth=True):
         if get_exchange_quotes == False and get_market_depth == False:
-            raise Exception(
-                "Either getExchangeQuotes must be true or getMarketDepth must be true"
-            )
+            self.subscribe_exception(except_message.QUOTE_DEPTH_EXCEPTION.value)
         else:
             exchange_code_name = ""
             exchange_code_list = {
                 "BSE": "1.",
                 "NSE": "4.",
                 "NDX": "13.",
                 "MCX": "6.",
                 "NFO": "4.",
                 "BFO": "2.",
             }
             exchange_code_name = exchange_code_list.get(exchange_code, False)
             if exchange_code_name == False:
-                raise Exception(
-                    "Exchange Code allowed are 'BSE', 'NSE', 'NDX', 'MCX', 'NFO', 'BFO'."
-                )
+                self.subscribe_exception(except_message.EXCHANGE_CODE_EXCEPTION.value)
             elif stock_code == "":
-                raise Exception("Stock-Code cannot be empty.")
+                self.subscribe_exception(except_message.STOCK_CODE_EXCEPTION.value)
             else:
                 token_value = False
                 if exchange_code.lower() == "bse":
                     token_value = self.stock_script_dict_list[0].get(stock_code, False)
                 elif exchange_code.lower() == "nse":
                     token_value = self.stock_script_dict_list[1].get(stock_code, False)
                 else:
                     if expiry_date == "":
-                        raise Exception(
-                            "Expiry-Date cannot be empty for given Exchange-Code."
-                        )
+                        self.subscribe_exception(except_message.EXPIRY_DATE_EXCEPTION.value)
                     if product_type.lower() == "futures":
                         contract_detail_value = "FUT"
                     elif product_type.lower() == "options":
                         contract_detail_value = "OPT"
                     else:
-                        raise Exception(
-                            "Product-Type should either be Futures or Options for given Exchange-Code."
-                        )
-                    contract_detail_value = (
-                        contract_detail_value + "-" + stock_code + "-" + expiry_date
-                    )
+                        self.subscribe_exception(except_message.PRODUCT_TYPE_EXCEPTION.value)
+                    contract_detail_value = contract_detail_value + "-" + stock_code + "-" + expiry_date
                     if product_type.lower() == "options":
                         if strike_price == "":
-                            raise Exception(
-                                "Strike Price cannot be empty for Product-Type 'Options'."
-                            )
+                            self.subscribe_exception(except_message.STRIKE_PRICE_EXCEPTION.value)
                         else:
-                            contract_detail_value = (
-                                contract_detail_value + "-" + strike_price
-                            )
+                            contract_detail_value = contract_detail_value + "-" + strike_price
                         if right.lower() == "put":
                             contract_detail_value = contract_detail_value + "-" + "PE"
                         elif right.lower() == "call":
                             contract_detail_value = contract_detail_value + "-" + "CE"
                         else:
-                            raise Exception(
-                                "Rights should either be Put or Call for Product-Type 'Options'."
-                            )
+                            self.subscribe_exception(except_message.RIGHT_EXCEPTION.value)
                     if exchange_code.lower() == "ndx":
-                        token_value = self.stock_script_dict_list[2].get(
-                            contract_detail_value, False
-                        )
+                        token_value = self.stock_script_dict_list[2].get(contract_detail_value, False)
                     elif exchange_code.lower() == "mcx":
-                        token_value = self.stock_script_dict_list[3].get(
-                            contract_detail_value, False
-                        )
+                        token_value = self.stock_script_dict_list[3].get(contract_detail_value, False)
                     elif exchange_code.lower() == "nfo":
-                        token_value = self.stock_script_dict_list[4].get(
-                            contract_detail_value, False
-                        )
+                        token_value = self.stock_script_dict_list[4].get(contract_detail_value, False)
                     elif exchange_code.lower() == "bfo":
-                        token_value = self.stock_script_dict_list[5].get(
-                            contract_detail_value, False
-                        )
+                        token_value = self.stock_script_dict_list[5].get(contract_detail_value, False)
                 if token_value == False:
-                    raise Exception("Stock-Code not found.")
+                    self.subscribe_exception(except_message.STOCK_INVALID_EXCEPTION.value)
                 exchange_quotes_token_value = False
                 if get_exchange_quotes != False:
-                    exchange_quotes_token_value = (
-                        exchange_code_name + "1!" + token_value
-                    )
+                    exchange_quotes_token_value = exchange_code_name + "1!" + token_value
                 market_depth_token_value = False
                 if get_market_depth != False:
                     market_depth_token_value = exchange_code_name + "2!" + token_value
                 return exchange_quotes_token_value, market_depth_token_value
 
-    def subscribe_feeds(
-        self,
-        stock_token="",
-        exchange_code="",
-        stock_code="",
-        product_type="",
-        expiry_date="",
-        strike_price="",
-        right="",
-        get_exchange_quotes=True,
-        get_market_depth=True,
-        get_order_notification=False,
-        get_strategy=None,
-    ):
-        if self.sio_handler:
+    def subscribe_feeds(self, stock_token="", exchange_code="", stock_code="", product_type="", expiry_date="", strike_price="", right="", interval = "", get_exchange_quotes=True, get_market_depth=True, get_order_notification=False):
+        
+        if(self.sio_rate_refresh_handler and self.sio_rate_refresh_handler.authentication == False):
+            raise Exception(except_message.AUTHENICATION_EXCEPTION.value)
+        
+        if interval != "":
+            if interval not in config.INTERVAL_TYPES_STREAM_OHLC:
+                raise Exception(except_message.STREAM_OHLC_INTERVAL_ERROR.value)
+            else:
+                interval = config.channel_interval_map[interval]
+        if self.sio_rate_refresh_handler:
             return_object = {}
+            if self.sio_order_refresh_handler and stock_token in config.STRATEGY_SUBSCRIPTION:
+                self._ws_connect(self.sio_order_refresh_handler,strategy_flag=True)
+                self.sio_order_refresh_handler.watch(stock_token)
+                return_object = self.socket_connection_response(resp_message.STRATEGY_STREAM_SUBSCRIBED.value.format(stock_token))
+                return return_object
             if get_order_notification == True:
-                self.sio_handler.notify()
-                return_object = {
-                    "message": "Order Notification subscribed successfully"
-                }
+                self._ws_connect(self.sio_order_refresh_handler,order_flag=True)
+                self.sio_order_refresh_handler.notify()
+                return_object = self.socket_connection_response(resp_message.ORDER_NOTIFICATION_SUBSRIBED.value)
+                return return_object
             if stock_token != "":
-                if stock_token != "STRATEGY":
-                    self.sio_handler.watch(stock_token, False)
+                if interval!="":
+                    if self.sio_ohlcv_stream_handler is None:
+                        self._ws_connect(self.sio_ohlcv_stream_handler,ohlcv_flag=True)
+                    self.sio_ohlcv_stream_handler.watch_stream_data(stock_token,interval)
                 else:
-                    self.sio_handler.watch(stock_token, True)
-                return_object = {
-                    "message": "Stock " + stock_token + " subscribed successfully"
-                }
-
+                    self.sio_rate_refresh_handler.watch(stock_token)
+                return_object = self.socket_connection_response(resp_message.STOCK_SUBSCRIBE_MESSAGE.value.format(stock_token))
             elif get_order_notification == True and exchange_code == "":
                 return return_object
             else:
-                # self.sio_handler.reconnect()
-                exchange_quotes_token, market_depth_token = self.get_stock_token_value(
-                    exchange_code=exchange_code,
-                    stock_code=stock_code,
-                    product_type=product_type,
-                    expiry_date=expiry_date,
-                    strike_price=strike_price,
-                    right=right,
-                    get_exchange_quotes=get_exchange_quotes,
-                    get_market_depth=get_market_depth,
-                )
-                if exchange_quotes_token != False:
-                    self.sio_handler.watch(exchange_quotes_token)
-                if market_depth_token != False:
-                    self.sio_handler.watch(market_depth_token)
-                return_object = {
-                    "message": "Stock " + stock_code + " subscribed successfully"
-                }
+                exchange_quotes_token, market_depth_token = self.get_stock_token_value(exchange_code=exchange_code, stock_code=stock_code, product_type=product_type, expiry_date=expiry_date, strike_price=strike_price, right=right, get_exchange_quotes=get_exchange_quotes, get_market_depth=get_market_depth)
+                if interval!="":
+                    if self.sio_ohlcv_stream_handler is None:
+                        self._ws_connect(self.sio_ohlcv_stream_handler,ohlcv_flag=True)
+                    self.sio_ohlcv_stream_handler.watch_stream_data(exchange_quotes_token,interval)
+                else:
+                    if exchange_quotes_token != False:
+                        self.sio_rate_refresh_handler.watch(exchange_quotes_token)
+                    if market_depth_token != False:
+                        self.sio_rate_refresh_handler.watch(market_depth_token)
+                return_object =  self.socket_connection_response(resp_message.STOCK_SUBSCRIBE_MESSAGE.value.format(stock_code))
             return return_object
+        
+    def unsubscribe_feeds(self, stock_token="", exchange_code="", stock_code="", product_type="", expiry_date="", strike_price="", right="",interval = "",get_exchange_quotes=True, get_market_depth=True,get_order_notification=False):
+        if interval != "":
+            if interval not in config.INTERVAL_TYPES_STREAM_OHLC:
+                raise Exception(except_message.STREAM_OHLC_INTERVAL_ERROR.value)
+            else:
+                interval = config.channel_interval_map[interval]
+
+        if(get_order_notification == True):
+            if self.sio_order_refresh_handler:
+                self.sio_order_refresh_handler.on_disconnect()
+                self.sio_order_refresh_handler = None
+                self.orderconnect = 0
+                return self.socket_connection_response(resp_message.ORDER_REFRESH_DISCONNECTED.value)
+            else:
+                return self.socket_connection_response(resp_message.ORDER_REFRESH_NOT_CONNECTED.value)
+
+        if(stock_token in config.STRATEGY_SUBSCRIPTION):
+            if self.sio_order_refresh_handler:
+                self.sio_order_refresh_handler.unwatch(stock_token)
+                return self.socket_connection_response(resp_message.STRATEGY_STREAM_UNSUBSCRIBED.value.format(stock_token))
+            else:
+                return self.socket_connection_response(resp_message.STRATEGY_STREAM_NOT_CONNECTED.value)
 
-    def unsubscribe_feeds(
-        self,
-        stock_token="",
-        exchange_code="",
-        stock_code="",
-        product_type="",
-        expiry_date="",
-        strike_price="",
-        right="",
-        get_exchange_quotes=True,
-        get_market_depth=True,
-    ):
-        if self.sio_handler:
+        if self.sio_rate_refresh_handler:
             if stock_token != "":
-                self.sio_handler.unwatch(stock_token)
-                return {
-                    "message": "Stock " + stock_token + " unsubscribed successfully"
+                if interval != "":
+                    if self.sio_ohlcv_stream_handler is not None:
+                        self.sio_ohlcv_stream_handler.unwatch(stock_token)
+                else:
+                    self.sio_rate_refresh_handler.unwatch(stock_token)
+                return self.socket_connection_response(resp_message.STOCK_UNSUBSCRIBE_MESSAGE.value.format(stock_token))
+            else:
+                exchange_quotes_token, market_depth_token = self.get_stock_token_value(exchange_code=exchange_code, stock_code=stock_code, product_type=product_type, expiry_date=expiry_date, strike_price=strike_price, right=right, get_exchange_quotes=get_exchange_quotes, get_market_depth=get_market_depth)
+                if interval != "":
+                    if self.sio_ohlcv_stream_handler is not None:
+                        self.sio_ohlcv_stream_handler.unwatch(exchange_quotes_token)
+                else:
+                    if exchange_quotes_token != False:
+                        self.sio_rate_refresh_handler.unwatch(exchange_quotes_token)
+                    if market_depth_token != False:
+                        self.sio_rate_refresh_handler.unwatch(market_depth_token)
+                return self.socket_connection_response(resp_message.STOCK_UNSUBSCRIBE_MESSAGE.value.format(stock_code))
+
+    def parse_ohlc_data(self,data):
+        split_data = data.split(",")
+        if split_data[0] in ["NSE","BSE"]:
+            parsed_data = {
+                "interval":config.feed_interval_map[split_data[8]],
+                "exchange_code":split_data[0],
+                "stock_code":split_data[1],
+                "low":split_data[2],
+                "high":split_data[3],
+                "open":split_data[4],
+                "close":split_data[5],
+                "volume":split_data[6],
+                "datetime":split_data[7]
+            }
+        elif split_data[0] in ["NFO","NDX","MCX"]:
+            if len(split_data) == 13:
+                parsed_data = {
+                    "interval":config.feed_interval_map[split_data[12]],
+                    "exchange_code":split_data[0],
+                    "stock_code":split_data[1],
+                    "expiry_date":split_data[2],
+                    "strike_price":split_data[3],
+                    "right_type":split_data[4],
+                    "low":split_data[5],
+                    "high":split_data[6],
+                    "open":split_data[7],
+                    "close":split_data[8],
+                    "volume":split_data[9],
+                    "oi":split_data[10],
+                    "datetime":split_data[11]
                 }
             else:
-                exchange_quotes_token, market_depth_token = self.get_stock_token_value(
-                    exchange_code=exchange_code,
-                    stock_code=stock_code,
-                    product_type=product_type,
-                    expiry_date=expiry_date,
-                    strike_price=strike_price,
-                    right=right,
-                    get_exchange_quotes=get_exchange_quotes,
-                    get_market_depth=get_market_depth,
-                )
-                if exchange_quotes_token != False:
-                    self.sio_handler.unwatch(exchange_quotes_token)
-                if market_depth_token != False:
-                    self.sio_handler.unwatch(market_depth_token)
-                return {"message": "Stock " + stock_code + " unsubscribed successfully"}
+                parsed_data = {
+                    "interval":config.feed_interval_map[split_data[10]],
+                    "exchange_code":split_data[0],
+                    "stock_code":split_data[1],
+                    "expiry_date":split_data[2],
+                    "low":split_data[3],
+                    "high":split_data[4],
+                    "open":split_data[5],
+                    "close":split_data[6],
+                    "volume":split_data[7],
+                    "oi":split_data[8],
+                    "datetime":split_data[9]
+                }
+        return parsed_data
 
     def parse_market_depth(self, data, exchange):
         depth = []
         counter = 0
         for lis in data:
             counter += 1
             dict = {}
-            if exchange == "1":
-                dict["BestBuyRate-" + str(counter)] = lis[0]
-                dict["BestBuyQty-" + str(counter)] = lis[1]
-                dict["BestSellRate-" + str(counter)] = lis[2]
-                dict["BestSellQty-" + str(counter)] = lis[3]
+            if exchange == '1':
+                dict["BestBuyRate-"+str(counter)] = lis[0]
+                dict["BestBuyQty-"+str(counter)] = lis[1]
+                dict["BestSellRate-"+str(counter)] = lis[2]
+                dict["BestSellQty-"+str(counter)] = lis[3]
                 depth.append(dict)
             else:
-                dict["BestBuyRate-" + str(counter)] = lis[0]
-                dict["BestBuyQty-" + str(counter)] = lis[1]
-                dict["BuyNoOfOrders-" + str(counter)] = lis[2]
-                dict["BuyFlag-" + str(counter)] = lis[3]
-                dict["BestSellRate-" + str(counter)] = lis[4]
-                dict["BestSellQty-" + str(counter)] = lis[5]
-                dict["SellNoOfOrders-" + str(counter)] = lis[6]
-                dict["SellFlag-" + str(counter)] = lis[7]
+                dict["BestBuyRate-"+str(counter)] = lis[0]
+                dict["BestBuyQty-"+str(counter)] = lis[1]
+                dict["BuyNoOfOrders-"+str(counter)] = lis[2]
+                dict["BuyFlag-"+str(counter)] = lis[3]
+                dict["BestSellRate-"+str(counter)] = lis[4]
+                dict["BestSellQty-"+str(counter)] = lis[5]
+                dict["SellNoOfOrders-"+str(counter)] = lis[6]
+                dict["SellFlag-"+str(counter)] = lis[7]
                 depth.append(dict)
         return depth
 
-    def parse_data(self, data):
-        if (
-            data
-            and type(data) == list
-            and len(data) > 0
-            and type(data[0]) == str
-            and "!" not in data[0]
-            and len(data) == 10
-        ):
+    def parse_data(self, data):    
+        if data and type(data) == list and len(data) > 0 and type(data[0]) == str and "!" not in data[0] and len(data) == 19:
+            #if data and type(data) == list and len(data) > 0 and type(data[0]) == str and "!" not in data[0] and len(data) == 19:
             iclick_data = dict()
-            iclick_data["stock_name"] = data[0]
-            iclick_data["stock_description"] = data[1]
-            iclick_data["recommended_price_and_date"] = data[2]
-            iclick_data["target_price"] = data[3]
-            iclick_data["sltp_price"] = data[4]
-            iclick_data["part_profit_percentage"] = data[5]
-            iclick_data["profit_price"] = data[6]
-            iclick_data["exit_price"] = data[7]
-            iclick_data["recommended_update"] = data[8]
-            iclick_data["iclick_status"] = data[9]
-            return iclick_data
-        if (
-            data
-            and type(data) == list
-            and len(data) > 0
-            and type(data[0]) == str
-            and "!" not in data[0]
-            and len(data) == 28
-        ):
+            #iclick_data['sequence_number'] = data[0]
+            iclick_data['stock_name'] = data[0]
+            iclick_data['stock_code'] = data[1]
+            iclick_data['action_type'] = data[2]
+            iclick_data['expiry_date'] = data[3]
+            iclick_data['strike_price'] = data[4]
+            iclick_data['option_type'] = data[5]
+            iclick_data['stock_description'] = data[6]
+            iclick_data['recommended_price_and_date'] = data[7]
+            iclick_data['recommended_price_from'] = data[8]
+            iclick_data['recommended_price_to'] = data[9]
+            iclick_data['recommended_date'] = data[10]
+            iclick_data['target_price'] = data[11]
+            iclick_data['sltp_price'] = data[12]
+            iclick_data['part_profit_percentage'] = data[13]
+            iclick_data['profit_price'] = data[14]
+            iclick_data['exit_price'] = data[15]
+            iclick_data['recommended_update'] = data[16]
+            iclick_data['iclick_status'] = data[17]
+            iclick_data['subscription_type'] = data[18]
+            return(iclick_data)
+        if data and type(data) == list and len(data) > 0 and type(data[0]) == str and "!" not in data[0] and len(data) == 28:
             strategy_dict = dict()
-            strategy_dict["strategy_date"] = data[0]
-            strategy_dict["modification_date"] = data[1]
-            strategy_dict["portfolio_id"] = data[2]
-            strategy_dict["call_action"] = data[3]
-            strategy_dict["portfolio_name"] = data[4]
-            strategy_dict["exchange_code"] = data[5]
-            strategy_dict["product_type"] = data[6]
-            # strategy_dict['INDEX/STOCK'] = data[7]
-            strategy_dict["underlying"] = data[8]
-            strategy_dict["expiry_date"] = data[9]
-            # strategy_dict['OCR_EXER_TYP'] = data[10]
-            strategy_dict["option_type"] = data[11]
-            strategy_dict["strike_price"] = data[12]
-            strategy_dict["action"] = data[13]
-            strategy_dict["recommended_price_from"] = data[14]
-            strategy_dict["recommended_price_to"] = data[15]
-            strategy_dict["minimum_lot_quantity"] = data[16]
-            strategy_dict["last_traded_price"] = data[17]
-            strategy_dict["best_bid_price"] = data[18]
-            strategy_dict["best_offer_price"] = data[19]
-            strategy_dict["last_traded_quantity"] = data[20]
-            strategy_dict["target_price"] = data[21]
-            strategy_dict["expected_profit_per_lot"] = data[22]
-            strategy_dict["stop_loss_price"] = data[23]
-            strategy_dict["expected_loss_per_lot"] = data[24]
-            strategy_dict["total_margin"] = data[25]
-            strategy_dict["leg_no"] = data[26]
-            strategy_dict["status"] = data[27]
-            return strategy_dict
-        elif (
-            data
-            and type(data) == list
-            and len(data) > 0
-            and type(data[0]) == str
-            and "!" not in data[0]
-        ):
+            strategy_dict['strategy_date'] = data[0]
+            strategy_dict['modification_date'] = data[1]
+            strategy_dict['portfolio_id'] = data[2]
+            strategy_dict['call_action'] = data[3]
+            strategy_dict['portfolio_name'] = data[4]
+            strategy_dict['exchange_code'] = data[5]
+            strategy_dict['product_type'] = data[6]
+            #strategy_dict['INDEX/STOCK'] = data[7]
+            strategy_dict['underlying'] = data[8]
+            strategy_dict['expiry_date'] = data[9]
+            #strategy_dict['OCR_EXER_TYP'] = data[10]
+            strategy_dict['option_type'] = data[11]
+            strategy_dict['strike_price'] = data[12]
+            strategy_dict['action'] = data[13]
+            strategy_dict['recommended_price_from'] = data[14]
+            strategy_dict['recommended_price_to'] = data[15]
+            strategy_dict['minimum_lot_quantity'] = data[16]
+            strategy_dict['last_traded_price'] = data[17]
+            strategy_dict['best_bid_price'] = data[18]
+            strategy_dict['best_offer_price'] = data[19]
+            strategy_dict['last_traded_quantity'] = data[20]
+            strategy_dict['target_price'] = data[21]           
+            strategy_dict['expected_profit_per_lot'] = data[22]
+            strategy_dict['stop_loss_price'] = data[23]
+            strategy_dict['expected_loss_per_lot'] = data[24]
+            strategy_dict['total_margin'] = data[25]
+            strategy_dict['leg_no'] = data[26]
+            strategy_dict['status'] = data[27]
+            return(strategy_dict)
+        if data and type(data) == list and len(data) > 0 and type(data[0]) == str and "!" not in data[0]:
             order_dict = {}
-            order_dict["sourceNumber"] = data[0]  # Source Number
-            order_dict["group"] = data[1]  # Group
-            order_dict["userId"] = data[2]  # User_id
-            order_dict["key"] = data[3]  # Key
-            order_dict["messageLength"] = data[4]  # Message Length
-            order_dict["requestType"] = data[5]  # Request Type
-            order_dict["messageSequence"] = data[6]  # Message Sequence
-            order_dict["messageDate"] = data[7]  # Date
-            order_dict["messageTime"] = data[8]  # Time
-            order_dict["messageCategory"] = data[9]  # Message Category
-            order_dict["messagePriority"] = data[10]  # Priority
-            order_dict["messageType"] = data[11]  # Message Type
-            order_dict["orderMatchAccount"] = data[12]  # Order Match Account
-            order_dict["orderExchangeCode"] = data[13]  # Exchange Code
-            if data[11] == "4" or data[11] == "5":
-                order_dict["stockCode"] = data[14]  # Stock Code
-                order_dict["orderFlow"] = self.tux_to_user_value["orderFlow"].get(
-                    str(data[15]).upper(), str(data[15])
-                )  # Order Flow
-                order_dict["limitMarketFlag"] = self.tux_to_user_value[
-                    "limitMarketFlag"
-                ].get(
-                    str(data[16]).upper(), str(data[16])
-                )  # Limit Market Flag
-                order_dict["orderType"] = self.tux_to_user_value["orderType"].get(
-                    str(data[17]).upper(), str(data[17])
-                )  # OrderType
-                order_dict["orderLimitRate"] = data[18]  # Limit Rate
-                order_dict["productType"] = self.tux_to_user_value["productType"].get(
-                    str(data[19]).upper(), str(data[19])
-                )  # Product Type
-                order_dict["orderStatus"] = self.tux_to_user_value["orderStatus"].get(
-                    str(data[20]).upper(), str(data[20])
-                )  # Order Status
-                order_dict["orderDate"] = data[21]  # Order  Date
-                order_dict["orderTradeDate"] = data[22]  # Trade Date
-                order_dict["orderReference"] = data[23]  # Order Reference
-                order_dict["orderQuantity"] = data[24]  # Order Quantity
-                order_dict["openQuantity"] = data[25]  # Open Quantity
-                order_dict["orderExecutedQuantity"] = data[
-                    26
-                ]  # Order Executed Quantity
-                order_dict["cancelledQuantity"] = data[27]  # Cancelled Quantity
-                order_dict["expiredQuantity"] = data[28]  # Expired Quantity
-                order_dict["orderDisclosedQuantity"] = data[
-                    29
-                ]  # Order Disclosed Quantity
-                order_dict["orderStopLossTrigger"] = data[30]  # Order Stop Loss Triger
-                order_dict["orderSquareFlag"] = data[31]  # Order Square Flag
-                order_dict["orderAmountBlocked"] = data[32]  # Order Amount Blocked
-                order_dict["orderPipeId"] = data[33]  # Order PipeId
-                order_dict["channel"] = data[34]  # Channel
-                order_dict["exchangeSegmentCode"] = data[35]  # Exchange Segment Code
-                order_dict["exchangeSegmentSettlement"] = data[
-                    36
-                ]  # Exchange Segment Settlement
-                order_dict["segmentDescription"] = data[37]  # Segment Description
-                order_dict["marginSquareOffMode"] = data[38]  # Margin Square Off Mode
-                order_dict["orderValidDate"] = data[40]  # Order Valid Date
-                order_dict["orderMessageCharacter"] = data[
-                    41
-                ]  # Order Message Character
-                order_dict["averageExecutedRate"] = data[42]  # Average Exited Rate
-                order_dict["orderPriceImprovementFlag"] = data[43]  # Order Price Flag
-                order_dict["orderMBCFlag"] = data[44]  # Order MBC Flag
-                order_dict["orderLimitOffset"] = data[45]  # Order Limit Offset
-                order_dict["systemPartnerCode"] = data[46]  # System Partner Code
-            elif data[11] == "6" or data[11] == "7":
-                order_dict["stockCode"] = data[14]  # stockCode
-                order_dict["productType"] = self.tux_to_user_value["productType"].get(
-                    str(data[15]).upper(), str(data[15])
-                )  # Product Type
-                order_dict["optionType"] = self.tux_to_user_value["optionType"].get(
-                    str(data[16]).upper(), str(data[16])
-                )  # Option Type
-                order_dict["exerciseType"] = data[17]  # Exercise Type
-                order_dict["strikePrice"] = data[18]  # Strike Price
-                order_dict["expiryDate"] = data[19]  # Expiry Date
-                order_dict["orderValidDate"] = data[20]  # Order Valid Date
-                order_dict["orderFlow"] = self.tux_to_user_value["orderFlow"].get(
-                    str(data[21]).upper(), str(data[21])
-                )  # Order  Flow
-                order_dict["limitMarketFlag"] = self.tux_to_user_value[
-                    "limitMarketFlag"
-                ].get(
-                    str(data[22]).upper(), str(data[22])
-                )  # Limit Market Flag
-                order_dict["orderType"] = self.tux_to_user_value["orderType"].get(
-                    str(data[23]).upper(), str(data[23])
-                )  # Order Type
-                order_dict["limitRate"] = data[24]  # Limit Rate
-                order_dict["orderStatus"] = self.tux_to_user_value["orderStatus"].get(
-                    str(data[25]).upper(), str(data[25])
-                )  # Order Status
-                order_dict["orderReference"] = data[26]  # Order Reference
-                order_dict["orderTotalQuantity"] = data[27]  # Order Total Quantity
-                order_dict["executedQuantity"] = data[28]  # Executed Quantity
-                order_dict["cancelledQuantity"] = data[29]  # Cancelled Quantity
-                order_dict["expiredQuantity"] = data[30]  # Expired Quantity
-                order_dict["stopLossTrigger"] = data[31]  # Stop Loss Trigger
-                order_dict["specialFlag"] = data[32]  # Special Flag
-                order_dict["pipeId"] = data[33]  # PipeId
-                order_dict["channel"] = data[34]  # Channel
-                order_dict["modificationOrCancelFlag"] = data[
-                    35
-                ]  # Modification or Cancel Flag
-                order_dict["tradeDate"] = data[36]  # Trade Date
-                order_dict["acknowledgeNumber"] = data[37]  # Acknowledgement Number
-                order_dict["stopLossOrderReference"] = data[
-                    37
-                ]  # Stop Loss Order Reference
-                order_dict["totalAmountBlocked"] = data[38]  # Total Amount Blocked
-                order_dict["averageExecutedRate"] = data[39]  # Average Executed Rate
-                order_dict["cancelFlag"] = data[40]  # Cancel Flag
-                order_dict["squareOffMarket"] = data[41]  # SquareOff Market
-                order_dict["quickExitFlag"] = data[42]  # Quick Exit Flag
-                order_dict["stopValidTillDateFlag"] = data[
-                    43
-                ]  # Stop Valid till Date Flag
-                order_dict["priceImprovementFlag"] = data[44]  # Price Improvement Flag
-                order_dict["conversionImprovementFlag"] = data[
-                    45
-                ]  # Conversion Improvement Flag
-                order_dict["trailUpdateCondition"] = data[45]  # Trail Update Condition
-                order_dict["systemPartnerCode"] = data[46]  # System Partner Code
+            order_dict["sourceNumber"] = data[0]                            #Source Number
+            order_dict["group"] = data[1]                                   #Group
+            order_dict["userId"] = data[2]                                  #User_id
+            order_dict["key"] = data[3]                                     #Key
+            order_dict["messageLength"] = data[4]                           #Message Length
+            order_dict["requestType"] = data[5]                             #Request Type
+            order_dict["messageSequence"] = data[6]                         #Message Sequence
+            order_dict["messageDate"] = data[7]                             #Date
+            order_dict["messageTime"] = data[8]                             #Time
+            order_dict["messageCategory"] = data[9]                         #Message Category
+            order_dict["messagePriority"] = data[10]                        #Priority
+            order_dict["messageType"] = data[11]                            #Message Type
+            order_dict["orderMatchAccount"] = data[12]                      #Order Match Account
+            order_dict["orderExchangeCode"] = data[13]                      #Exchange Code
+            if data[11] == '4' or data[11] == '5':
+                order_dict["stockCode"] = data[14]                     #Stock Code
+                order_dict["orderFlow"] = self.tux_to_user_value['orderFlow'].get(str(data[15]).upper(),str(data[15]))                          # Order Flow
+                order_dict["limitMarketFlag"] = self.tux_to_user_value['limitMarketFlag'].get(str(data[16]).upper(),str(data[16]))                    #Limit Market Flag
+                order_dict["orderType"] = self.tux_to_user_value['orderType'].get(str(data[17]).upper(),str(data[17]))                          #OrderType
+                order_dict["orderLimitRate"] = data[18]                     #Limit Rate
+                order_dict["productType"] = self.tux_to_user_value['productType'].get(str(data[19]).upper(),str(data[19]))                        #Product Type
+                order_dict["orderStatus"] = self.tux_to_user_value['orderStatus'].get(str(data[20]).upper(),str(data[20]))                        # Order Status
+                order_dict["orderDate"] = data[21]                          #Order  Date
+                order_dict["orderTradeDate"] = data[22]                     #Trade Date
+                order_dict["orderReference"] = data[23]                     #Order Reference
+                order_dict["orderQuantity"] = data[24]                      #Order Quantity
+                order_dict["openQuantity"] = data[25]                       #Open Quantity
+                order_dict["orderExecutedQuantity"] = data[26]              #Order Executed Quantity
+                order_dict["cancelledQuantity"] = data[27]                  #Cancelled Quantity
+                order_dict["expiredQuantity"] = data[28]                    #Expired Quantity
+                order_dict["orderDisclosedQuantity"] = data[29]             # Order Disclosed Quantity
+                order_dict["orderStopLossTrigger"] = data[30]               #Order Stop Loss Triger
+                order_dict["orderSquareFlag"] = data[31]                    #Order Square Flag
+                order_dict["orderAmountBlocked"] = data[32]                 # Order Amount Blocked
+                order_dict["orderPipeId"] = data[33]                        #Order PipeId
+                order_dict["channel"] = data[34]                            #Channel
+                order_dict["exchangeSegmentCode"] = data[35]                #Exchange Segment Code
+                order_dict["exchangeSegmentSettlement"] = data[36]          #Exchange Segment Settlement 
+                order_dict["segmentDescription"] = data[37]                 #Segment Description
+                order_dict["marginSquareOffMode"] = data[38]                #Margin Square Off Mode
+                order_dict["orderValidDate"] = data[40]                     #Order Valid Date
+                order_dict["orderMessageCharacter"] = data[41]              #Order Message Character
+                order_dict["averageExecutedRate"] = data[42]                #Average Exited Rate
+                order_dict["orderPriceImprovementFlag"] = data[43]          #Order Price Flag
+                order_dict["orderMBCFlag"] = data[44]                       #Order MBC Flag
+                order_dict["orderLimitOffset"] = data[45]                   #Order Limit Offset
+                order_dict["systemPartnerCode"] = data[46]                  #System Partner Code
+            elif data[11] == '6' or data[11] == '7':
+                order_dict["stockCode"] = data[14]                         #stockCode
+                order_dict["productType"] =  self.tux_to_user_value['productType'].get(str(data[15]).upper(),str(data[15]))                        #Product Type
+                order_dict["optionType"] = self.tux_to_user_value['optionType'].get(str(data[16]).upper(),str(data[16]))                         #Option Type
+                order_dict["exerciseType"] = data[17]                       #Exercise Type
+                order_dict["strikePrice"] = data[18]                        #Strike Price
+                order_dict["expiryDate"] = data[19]                         #Expiry Date
+                order_dict["orderValidDate"] = data[20]                     #Order Valid Date
+                order_dict["orderFlow"] = self.tux_to_user_value['orderFlow'].get(str(data[21]).upper(),str(data[21]))                          #Order  Flow
+                order_dict["limitMarketFlag"] = self.tux_to_user_value['limitMarketFlag'].get(str(data[22]).upper(),str(data[22]))                    #Limit Market Flag
+                order_dict["orderType"] = self.tux_to_user_value['orderType'].get(str(data[23]).upper(),str(data[23]))                          #Order Type
+                order_dict["limitRate"] = data[24]                          #Limit Rate
+                order_dict["orderStatus"] = self.tux_to_user_value['orderStatus'].get(str(data[25]).upper(),str(data[25]))                        #Order Status
+                order_dict["orderReference"] = data[26]                     #Order Reference
+                order_dict["orderTotalQuantity"] = data[27]                 #Order Total Quantity
+                order_dict["executedQuantity"] = data[28]                   #Executed Quantity
+                order_dict["cancelledQuantity"] = data[29]                  #Cancelled Quantity
+                order_dict["expiredQuantity"] = data[30]                    #Expired Quantity
+                order_dict["stopLossTrigger"] = data[31]                    #Stop Loss Trigger
+                order_dict["specialFlag"] = data[32]                        #Special Flag
+                order_dict["pipeId"] = data[33]                             #PipeId
+                order_dict["channel"] = data[34]                            #Channel
+                order_dict["modificationOrCancelFlag"] = data[35]           #Modification or Cancel Flag
+                order_dict["tradeDate"] = data[36]                          #Trade Date
+                order_dict["acknowledgeNumber"] = data[37]                  #Acknowledgement Number
+                order_dict["stopLossOrderReference"] = data[37]             #Stop Loss Order Reference
+                order_dict["totalAmountBlocked"] = data[38]                 # Total Amount Blocked
+                order_dict["averageExecutedRate"] = data[39]                #Average Executed Rate
+                order_dict["cancelFlag"] = data[40]                         #Cancel Flag
+                order_dict["squareOffMarket"] = data[41]                    #SquareOff Market
+                order_dict["quickExitFlag"] = data[42]                      #Quick Exit Flag
+                order_dict["stopValidTillDateFlag"] = data[43]              #Stop Valid till Date Flag
+                order_dict["priceImprovementFlag"] = data[44]               #Price Improvement Flag
+                order_dict["conversionImprovementFlag"] = data[45]          #Conversion Improvement Flag
+                order_dict["trailUpdateCondition"] = data[45]               #Trail Update Condition
+                order_dict["systemPartnerCode"] = data[46]                  #System Partner Code
             return order_dict
-        exchange = str.split(data[0], "!")[0].split(".")[0]
-        data_type = str.split(data[0], "!")[0].split(".")[1]
-        if exchange == "6":
+        exchange = str.split(data[0], '!')[0].split('.')[0]
+        data_type = str.split(data[0], '!')[0].split('.')[1]
+        if exchange == '6':
             data_dict = {}
             data_dict["symbol"] = data[0]
             data_dict["AndiOPVolume"] = data[1]
             data_dict["Reserved"] = data[2]
             data_dict["IndexFlag"] = data[3]
             data_dict["ttq"] = data[4]
             data_dict["last"] = data[5]
             data_dict["ltq"] = data[6]
-            data_dict["ltt"] = datetime.fromtimestamp(data[7]).strftime("%c")
+            data_dict["ltt"] = datetime.fromtimestamp(data[7]).strftime('%c')
             data_dict["AvgTradedPrice"] = data[8]
             data_dict["TotalBuyQnt"] = data[9]
             data_dict["TotalSellQnt"] = data[10]
             data_dict["ReservedStr"] = data[11]
             data_dict["ClosePrice"] = data[12]
             data_dict["OpenPrice"] = data[13]
             data_dict["HighPrice"] = data[14]
@@ -666,180 +674,131 @@
             data_dict["CurrOpenInterest"] = data[17]
             data_dict["TotalTrades"] = data[18]
             data_dict["HightestPriceEver"] = data[19]
             data_dict["LowestPriceEver"] = data[20]
             data_dict["TotalTradedValue"] = data[21]
             marketDepthIndex = 0
             for i in range(22, len(data)):
-                data_dict["Quantity-" + str(marketDepthIndex)] = data[i][0]
-                data_dict["OrderPrice-" + str(marketDepthIndex)] = data[i][1]
-                data_dict["TotalOrders-" + str(marketDepthIndex)] = data[i][2]
-                data_dict["Reserved-" + str(marketDepthIndex)] = data[i][3]
-                data_dict["SellQuantity-" + str(marketDepthIndex)] = data[i][4]
-                data_dict["SellOrderPrice-" + str(marketDepthIndex)] = data[i][5]
-                data_dict["SellTotalOrders-" + str(marketDepthIndex)] = data[i][6]
-                data_dict["SellReserved-" + str(marketDepthIndex)] = data[i][7]
+                data_dict["Quantity-"+str(marketDepthIndex)] = data[i][0]
+                data_dict["OrderPrice-"+str(marketDepthIndex)] = data[i][1]
+                data_dict["TotalOrders-"+str(marketDepthIndex)] = data[i][2]
+                data_dict["Reserved-"+str(marketDepthIndex)] = data[i][3]
+                data_dict["SellQuantity-"+str(marketDepthIndex)] = data[i][4]
+                data_dict["SellOrderPrice-"+str(marketDepthIndex)] = data[i][5]
+                data_dict["SellTotalOrders-"+str(marketDepthIndex)] = data[i][6]
+                data_dict["SellReserved-"+str(marketDepthIndex)] = data[i][7]
                 marketDepthIndex += 1
-        elif data_type == "1":
+        elif data_type == '1':
             data_dict = {
                 "symbol": data[0],
                 "open": data[1],
                 "last": data[2],
                 "high": data[3],
                 "low": data[4],
                 "change": data[5],
                 "bPrice": data[6],
                 "bQty": data[7],
                 "sPrice": data[8],
                 "sQty": data[9],
                 "ltq": data[10],
                 "avgPrice": data[11],
-                "quotes": "Quotes Data",
+                "quotes": "Quotes Data"
             }
             # For NSE & BSE conversion
             if len(data) == 21:
                 data_dict["ttq"] = data[12]
                 data_dict["totalBuyQt"] = data[13]
                 data_dict["totalSellQ"] = data[14]
                 data_dict["ttv"] = data[15]
                 data_dict["trend"] = data[16]
                 data_dict["lowerCktLm"] = data[17]
                 data_dict["upperCktLm"] = data[18]
-                data_dict["ltt"] = datetime.fromtimestamp(data[19]).strftime("%c")
+                data_dict["ltt"] = datetime.fromtimestamp(
+                    data[19]).strftime('%c')
                 data_dict["close"] = data[20]
             # For FONSE & CDNSE conversion
             elif len(data) == 23:
                 data_dict["OI"] = data[12]
                 data_dict["CHNGOI"] = data[13]
                 data_dict["ttq"] = data[14]
                 data_dict["totalBuyQt"] = data[15]
                 data_dict["totalSellQ"] = data[16]
                 data_dict["ttv"] = data[17]
                 data_dict["trend"] = data[18]
                 data_dict["lowerCktLm"] = data[19]
                 data_dict["upperCktLm"] = data[20]
-                data_dict["ltt"] = datetime.fromtimestamp(data[21]).strftime("%c")
+                data_dict["ltt"] = datetime.fromtimestamp(
+                    data[21]).strftime('%c')
                 data_dict["close"] = data[22]
         else:
             data_dict = {
                 "symbol": data[0],
-                "time": datetime.fromtimestamp(data[1]).strftime("%c"),
+                "time": datetime.fromtimestamp(data[1]).strftime('%c'),
                 "depth": self.parse_market_depth(data[2], exchange),
-                "quotes": "Market Depth",
+                "quotes": "Market Depth"
             }
-        if exchange == "4" and len(data) == 21:
-            data_dict["exchange"] = "NSE Equity"
-        elif exchange == "1":
-            data_dict["exchange"] = "BSE"
-        elif exchange == "13":
-            data_dict["exchange"] = "NSE Currency"
-        elif exchange == "4" and len(data) == 23:
-            data_dict["exchange"] = "NSE Futures & Options"
-        elif exchange == "6":
-            data_dict["exchange"] = "Commodity"
+        if exchange == '4' and len(data) == 21:
+            data_dict['exchange'] = 'NSE Equity'
+        elif exchange == '1':
+            data_dict['exchange'] = 'BSE'
+        elif exchange == '13':
+            data_dict['exchange'] = 'NSE Currency'
+        elif exchange == '4' and len(data) == 23:
+            data_dict['exchange'] = 'NSE Futures & Options'
+        elif exchange == '6':
+            data_dict['exchange'] = 'Commodity'
         return data_dict
 
     def api_util(self):
         try:
-            headers = {"Content-Type": "application/json"}
-            body = {"SessionToken": self.session_key, "AppKey": self.api_key}
-            body = json.dumps(body, separators=(",", ":"))
-            url = "https://uatapi.icicidirect.com/iciciDirectWebApi_core/api/v1/customerdetails"
-            response = requests.get(url=url, data=body, headers=headers, verify=False)
-            if response.json()["Success"] != None:
-                base64_session_token = response.json()["Success"]["session_token"]
-                result = base64.b64decode(base64_session_token.encode("ascii")).decode(
-                    "ascii"
-                )
+            headers = {
+                "Content-Type": "application/json"
+            }
+            body = {
+                "SessionToken": self.session_key,
+                "AppKey": self.api_key
+            }
+            body = json.dumps(body, separators=(',', ':'))
+            url = config.API_URL + api_endpoint.CUST_DETAILS.value
+            response = requests.get(url=url, data=body, headers=headers)
+            json_data = response.json()
+            if 'Success' in json_data and json_data['Success'] is not None:
+                base64_session_token = json_data['Success']['session_token']
+                result = base64.b64decode(base64_session_token.encode('ascii')).decode('ascii')
                 self.user_id = result.split(":")[0]
                 self.session_key = result.split(":")[1]
+            elif 'Status' in json_data and 'Error' in json_data and json_data['Status'] != 200:
+                if json_data['Error'] == 'Invalid session.':
+                    raise Exception(except_message.SESSIONKEY_INCORRECT.value)
+                elif json_data['Error'] == 'Public Key does not exist.':
+                    raise Exception(except_message.APPKEY_INCORRECT.value)
+                elif json_data['Error'] == 'Resource not available.':
+                    raise Exception(except_message.SESSIONKEY_EXPIRED.value)
+                else:
+                    raise Exception(except_message.CUSTOMERDETAILS_API_EXCEPTION.value)
             else:
-                raise Exception(
-                    "Could not authenticate credentials. Please check token and keys"
-                )
-        except Exception as e:
-            raise Exception(
-                "Could not authenticate credentials. Please check token and keys"
-            )
-
-    def load_cache(self):
-        global response_cache
-        if os.path.exists(CACHE_FILE):
-            with open(CACHE_FILE, "r") as file:
-                try:
-                    response_cache = json.load(file)
-                except json.JSONDecodeError:
-                    response_cache = {}
-
-    def save_cache(self):
-        with open(CACHE_FILE, "w") as file:
-            json.dump(response_cache, file)
-
-    def cache_response(self, func):
-        @functools.wraps(func)
-        def wrapper(link, timeout=3):
-            cache_key = str((link, str(timeout)))
-            if cache_key in response_cache:
-
-                cached_response = response_cache[cache_key]
-                if time.time() - cached_response["timestamp"] <= CACHE_EXPIRATION:
-                    print("Using cached response for:", link)
-                    cached_response_data = cached_response["data"]
-                    response = requests.Response()
-                    response.status_code = cached_response_data["status_code"]
-                    response._content = base64.b64decode(
-                        cached_response_data["content"]
-                    )
-                    # response.url = link
-                    return response
-
-            try:
-                print("network call..")
-                # print(link,timeout)
-                response = func(link)
-                # print("response : ",response)
-                response.raise_for_status()
-                response_cache[cache_key] = {
-                    "timestamp": time.time(),
-                    "data": {
-                        "status_code": response.status_code,
-                        "content": base64.b64encode(response.content).decode("utf-8"),
-                    },
-                }
-                self.save_cache()
-                return response
-            except requests.exceptions.Timeout:
-                print(
-                    f"The request timed out for: {link} as the server failed to respond"
-                )
-            except requests.exceptions.RequestException as e:
-                print("An error occurred:", e)
-            except Exception as e:
-                print("An unexpected error occurred:", e)
-
-        return wrapper
-
-    def get_response(self, link, timeout=3):
-        start = time.time()
-        data = self.cache_response(requests.get)(link, timeout)
-        end = time.time()
-        print(f"execution time : {end - start}")
-        return data
+                raise Exception("Unexpected format in API response")
+        except json.decoder.JSONDecodeError:
+            # Handle JSON decoding error
+            raise Exception("Invalid JSON format in API response")
+        except KeyError as e:
+            # Handle missing key error
+            raise Exception(f"KeyError: {e} not found in API response")
+        except Exception as e:
+            # Handle other exceptions
+            raise Exception(f"Unexpected error: {str(e)}")
 
     def get_stock_script_list(self):
         try:
-            self.load_cache()
             self.stock_script_dict_list = [{}, {}, {}, {}, {}, {}]
             self.token_script_dict_list = [{}, {}, {}, {}, {}, {}]
-            link = "https://traderweb.icicidirect.com/Content/File/txtFile/ScripFile/StockScriptNew.csv"
-            response = self.get_response(link)
-            if response is not None:
-
-                # download = s.get("https://traderweb.icicidirect.com/Content/File/txtFile/ScripFile/StockScriptNew.csv")
-                cr = csv.reader(response.text.splitlines(), delimiter=",")
+            with requests.Session() as s:
+                download = s.get(config.STOCK_SCRIPT_CSV_URL)
+                decoded_content = download.content.decode('utf-8')
+                cr = csv.reader(decoded_content.splitlines(), delimiter=',')
                 my_list = list(cr)
                 for row in my_list:
                     if row[2] == "BSE":
                         self.stock_script_dict_list[0][row[3]] = row[5]
                         self.token_script_dict_list[0][row[5]] = [row[3], row[1]]
                     elif row[2] == "NSE":
                         self.stock_script_dict_list[1][row[3]] = row[5]
@@ -852,18 +811,16 @@
                         self.token_script_dict_list[3][row[5]] = [row[7], row[1]]
                     elif row[2] == "NFO":
                         self.stock_script_dict_list[4][row[7]] = row[5]
                         self.token_script_dict_list[4][row[5]] = [row[7], row[1]]
                     elif row[2] == "BFO":
                         self.stock_script_dict_list[5][row[7]] = row[5]
                         self.token_script_dict_list[5][row[5]] = [row[7], row[1]]
-
         except Exception as e:
-            print("error", e)
-            # pass
+            pass
 
     def generate_session(self, api_secret, session_token):
         self.session_key = session_token
         self.secret_key = api_secret
         self.api_util()
         self.get_stock_script_list()
         self.api_handler = ApificationBreeze(self)
@@ -880,653 +837,344 @@
         if self.api_handler:
             return self.api_handler.get_funds()
 
     def set_funds(self, transaction_type="", amount="", segment=""):
         if self.api_handler:
             return self.api_handler.set_funds(transaction_type, amount, segment)
 
-    def get_historical_data(
-        self,
-        interval="",
-        from_date="",
-        to_date="",
-        stock_code="",
-        exchange_code="",
-        product_type="",
-        expiry_date="",
-        right="",
-        strike_price="",
-    ):
-        if self.api_handler:
-            return self.api_handler.get_historical_data(
-                interval,
-                from_date,
-                to_date,
-                stock_code,
-                exchange_code,
-                product_type,
-                expiry_date,
-                right,
-                strike_price,
-            )
-
-    def add_margin(
-        self,
-        product_type="",
-        stock_code="",
-        exchange_code="",
-        settlement_id="",
-        add_amount="",
-        margin_amount="",
-        open_quantity="",
-        cover_quantity="",
-        category_index_per_stock="",
-        expiry_date="",
-        right="",
-        contract_tag="",
-        strike_price="",
-        segment_code="",
-    ):
-        if self.api_handler:
-            return self.api_handler.add_margin(
-                product_type,
-                stock_code,
-                exchange_code,
-                settlement_id,
-                add_amount,
-                margin_amount,
-                open_quantity,
-                cover_quantity,
-                category_index_per_stock,
-                expiry_date,
-                right,
-                contract_tag,
-                strike_price,
-                segment_code,
-            )
+    def get_historical_data(self, interval="", from_date="", to_date="", stock_code="", exchange_code="", product_type="", expiry_date="", right="", strike_price=""):
+        if self.api_handler:
+            return self.api_handler.get_historical_data(interval, from_date, to_date, stock_code, exchange_code, product_type, expiry_date, right, strike_price)
+
+    def get_historical_data_v2(self, interval="", from_date="", to_date="", stock_code="", exchange_code="", product_type="", expiry_date="", right="", strike_price=""):
+        if self.api_handler:
+            return self.api_handler.get_historical_data_v2(interval, from_date, to_date, stock_code, exchange_code, product_type, expiry_date, right, strike_price)
+
+    def add_margin(self, product_type="", stock_code="", exchange_code="", settlement_id="", add_amount="", margin_amount="", open_quantity="", cover_quantity="", category_index_per_stock="", expiry_date="", right="", contract_tag="", strike_price="", segment_code=""):
+        if self.api_handler:
+            return self.api_handler.add_margin(product_type, stock_code, exchange_code, settlement_id, add_amount, margin_amount, open_quantity, cover_quantity, category_index_per_stock, expiry_date, right, contract_tag, strike_price, segment_code)
 
     def get_margin(self, exchange_code=""):
         if self.api_handler:
             return self.api_handler.get_margin(exchange_code)
 
-    def place_order(
-        self,
-        stock_code="",
-        exchange_code="",
-        product="",
-        action="",
-        order_type="",
-        stoploss="",
-        quantity="",
-        price="",
-        validity="",
-        validity_date="",
-        disclosed_quantity="",
-        expiry_date="",
-        right="",
-        strike_price="",
-        user_remark="",
-        order_type_fresh="",
-        order_rate_fresh="",
-        lots="",
-    ):
-        if self.api_handler:
-            return self.api_handler.place_order(
-                stock_code=stock_code,
-                exchange_code=exchange_code,
-                product=product,
-                action=action,
-                order_type=order_type,
-                stoploss=stoploss,
-                quantity=quantity,
-                price=price,
-                validity=validity,
-                validity_date=validity_date,
-                disclosed_quantity=disclosed_quantity,
-                expiry_date=expiry_date,
-                right=right,
-                strike_price=strike_price,
-                user_remark=user_remark,
-                order_type_fresh=order_type_fresh,
-                order_rate_fresh=order_rate_fresh,
-                lots=lots,
-            )
+    def place_order(self, stock_code="", exchange_code="", product="", action="", order_type="", stoploss="", quantity="", price="", validity="", validity_date="", disclosed_quantity="", expiry_date="", right="", strike_price="", user_remark="",order_type_fresh="",order_rate_fresh="",settlement_id = "",order_segment_code = "",lots=""):
+        if self.api_handler:
+            return self.api_handler.place_order(stock_code=stock_code, exchange_code=exchange_code, product=product, action=action, order_type=order_type, stoploss=stoploss, quantity=quantity, price=price, validity=validity, validity_date=validity_date, disclosed_quantity=disclosed_quantity, expiry_date=expiry_date, right=right, strike_price=strike_price, user_remark=user_remark, order_type_fresh=order_type_fresh, order_rate_fresh=order_rate_fresh,settlement_id = settlement_id,order_segment_code = order_segment_code, lots=lots,)
 
     def get_order_detail(self, exchange_code="", order_id=""):
         if self.api_handler:
             return self.api_handler.get_order_detail(exchange_code, order_id)
 
     def get_order_list(self, exchange_code="", from_date="", to_date=""):
         if self.api_handler:
             return self.api_handler.get_order_list(exchange_code, from_date, to_date)
 
     def cancel_order(self, exchange_code="", order_id=""):
         if self.api_handler:
             return self.api_handler.cancel_order(exchange_code, order_id)
 
-    def modify_order(
-        self,
-        order_id="",
-        exchange_code="",
-        order_type="",
-        stoploss="",
-        quantity="",
-        price="",
-        validity="",
-        disclosed_quantity="",
-        validity_date="",
-    ):
-        if self.api_handler:
-            return self.api_handler.modify_order(
-                order_id,
-                exchange_code,
-                order_type,
-                stoploss,
-                quantity,
-                price,
-                validity,
-                disclosed_quantity,
-                validity_date,
-            )
-
-    def get_portfolio_holdings(
-        self,
-        exchange_code="",
-        from_date="",
-        to_date="",
-        stock_code="",
-        portfolio_type="",
-    ):
-        if self.api_handler:
-            return self.api_handler.get_portfolio_holdings(
-                exchange_code, from_date, to_date, stock_code, portfolio_type
-            )
+    def modify_order(self, order_id="", exchange_code="", order_type="", stoploss="", quantity="", price="", validity="", disclosed_quantity="", validity_date=""):
+        if self.api_handler:
+            return self.api_handler.modify_order(order_id, exchange_code, order_type, stoploss, quantity, price, validity, disclosed_quantity, validity_date)
+
+    def get_portfolio_holdings(self, exchange_code="", from_date="", to_date="", stock_code="", portfolio_type=""):
+        if self.api_handler:
+            return self.api_handler.get_portfolio_holdings(exchange_code, from_date, to_date, stock_code, portfolio_type)
 
     def get_portfolio_positions(self):
         if self.api_handler:
             return self.api_handler.get_portfolio_positions()
 
-    def get_quotes(
-        self,
-        stock_code="",
-        exchange_code="",
-        expiry_date="",
-        product_type="",
-        right="",
-        strike_price="",
-    ):
-        if self.api_handler:
-            return self.api_handler.get_quotes(
-                stock_code,
-                exchange_code,
-                expiry_date,
-                product_type,
-                right,
-                strike_price,
-            )
-
-    def get_option_chain_quotes(
-        self,
-        stock_code="",
-        exchange_code="",
-        expiry_date="",
-        product_type="",
-        right="",
-        strike_price="",
-    ):
-        if self.api_handler:
-            return self.api_handler.get_option_chain_quotes(
-                stock_code,
-                exchange_code,
-                expiry_date,
-                product_type,
-                right,
-                strike_price,
-            )
-
-    def square_off(
-        self,
-        source_flag="",
-        stock_code="",
-        exchange_code="",
-        quantity="",
-        price="",
-        action="",
-        order_type="",
-        validity="",
-        stoploss="",
-        disclosed_quantity="",
-        protection_percentage="",
-        settlement_id="",
-        margin_amount="",
-        open_quantity="",
-        cover_quantity="",
-        product_type="",
-        expiry_date="",
-        right="",
-        strike_price="",
-        validity_date="",
-        trade_password="",
-        alias_name="",
-        lots="",
-    ):
-        if self.api_handler:
-            return self.api_handler.square_off(
-                source_flag,
-                stock_code,
-                exchange_code,
-                quantity,
-                price,
-                action,
-                order_type,
-                validity,
-                stoploss,
-                disclosed_quantity,
-                protection_percentage,
-                settlement_id,
-                margin_amount,
-                open_quantity,
-                cover_quantity,
-                product_type,
-                expiry_date,
-                right,
-                strike_price,
-                validity_date,
-                trade_password,
-                alias_name,
-                lots,
-            )
-
-    def get_trade_list(
-        self,
-        from_date="",
-        to_date="",
-        exchange_code="",
-        product_type="",
-        action="",
-        stock_code="",
-    ):
-        if self.api_handler:
-            return self.api_handler.get_trade_list(
-                from_date, to_date, exchange_code, product_type, action, stock_code
-            )
+    def get_quotes(self, stock_code="", exchange_code="", expiry_date="", product_type="", right="", strike_price=""):
+        if self.api_handler:
+            return self.api_handler.get_quotes(stock_code, exchange_code, expiry_date, product_type, right, strike_price)
+
+    def get_option_chain_quotes(self, stock_code="", exchange_code="", expiry_date="", product_type="", right="", strike_price=""):
+        if(self.api_handler):
+            return self.api_handler.get_option_chain_quotes(stock_code, exchange_code, expiry_date, product_type, right, strike_price)
+
+    def square_off(self, source_flag="", stock_code="", exchange_code="", quantity="", price="", action="", order_type="", validity="", stoploss="", disclosed_quantity="", protection_percentage="", settlement_id="", margin_amount="", open_quantity="", cover_quantity="", product="", expiry_date="", right="", strike_price="", validity_date="", trade_password="", alias_name="", order_reference = "", position_exchange_code = "", lots="",):
+        if self.api_handler:
+            return self.api_handler.square_off(source_flag, stock_code, exchange_code, quantity, price, action, order_type, validity, stoploss, disclosed_quantity, protection_percentage, settlement_id, margin_amount, open_quantity, cover_quantity, product, expiry_date, right, strike_price, validity_date, trade_password, alias_name, order_reference, position_exchange_code, lots,)
+
+    def get_trade_list(self, from_date="", to_date="", exchange_code="", product_type="", action="", stock_code=""):
+        if self.api_handler:
+            return self.api_handler.get_trade_list(from_date, to_date, exchange_code, product_type, action, stock_code)
 
     def get_trade_detail(self, exchange_code="", order_id=""):
         if self.api_handler:
             return self.api_handler.get_trade_detail(exchange_code, order_id)
-
-    def get_names(self, exchange_code="", stock_code=""):
+    
+    def get_names(self, exchange_code="",stock_code=""):
         if self.api_handler:
             return self.api_handler.get_names(exchange_code, stock_code)
+    
+    def preview_order(self, stock_code="",exchange_code="",product="",order_type="",price="",action="",quantity="",expiry_date="",right="",strike_price="",specialflag="",stoploss="",order_rate_fresh=""):
+        if self.api_handler:
+            return self.api_handler.preview_order(stock_code, exchange_code, product, order_type, price, action, quantity, expiry_date, right, strike_price, specialflag, stoploss, order_rate_fresh)
+    
 
-    def preview_order(
-        self,
-        stock_code="",
-        exchange_code="",
-        product="",
-        order_type="",
-        price="",
-        action="",
-        quantity="",
-        expiry_date="",
-        right="",
-        strike_price="",
-        specialflag="",
-        stoploss="",
-        order_rate_fresh="",
-    ):
-        if self.api_handler:
-            return self.api_handler.preview_order(
-                stock_code,
-                exchange_code,
-                product,
-                order_type,
-                price,
-                action,
-                quantity,
-                expiry_date,
-                right,
-                strike_price,
-                specialflag,
-                stoploss,
-                order_rate_fresh,
-            )
-
+    def limit_calculator(self,strike_price,product_type,expiry_date,underlying,exchange_code,order_flow,stop_loss_trigger,option_type,source_flag,limit_rate,order_reference,available_quantity,market_type,fresh_order_limit):
+        if self.api_handler:
+            return self.api_handler.limit_calculator(strike_price,product_type,expiry_date,underlying,exchange_code,order_flow,stop_loss_trigger,option_type,source_flag,limit_rate,order_reference,available_quantity,market_type,fresh_order_limit)
 
-class ApificationBreeze:
+    def margin_calculator(self,lists,exchange_code):
+        if self.api_handler:
+            return self.api_handler.margin_calculator(lists,exchange_code)
+    
+    
+class ApificationBreeze():
 
     def __init__(self, breeze_instance):
         self.breeze = breeze_instance
-        self.hostname = "https://uatapi.icicidirect.com/iciciDirectWebApi_core/api/v1/"
+        self.hostname = config.API_URL
         self.base64_session_token = base64.b64encode(
-            (self.breeze.user_id + ":" + self.breeze.session_key).encode("ascii")
-        ).decode("ascii")
+            (self.breeze.user_id + ":" + self.breeze.session_key).encode('ascii')).decode('ascii')
+        
+    def error_exception(self,func_name,error):
+        message = "{0}() Error".format(func_name)
+        raise Exception(message).with_traceback(error.__traceback__)
+
+    def validation_error_response(self,message):
+        return {
+                    "Success": "", 
+                    "Status": 500, 
+                    "Error": message
+                }
 
     def generate_headers(self, body):
         try:
-            current_date = datetime.utcnow().isoformat()[:19] + ".000Z"
+            current_date = datetime.utcnow().isoformat()[:19] + '.000Z'
             checksum = sha256(
-                (current_date + body + self.breeze.secret_key).encode("utf-8")
-            ).hexdigest()
+                (current_date+body+self.breeze.secret_key).encode("utf-8")).hexdigest()
             headers = {
                 "Content-Type": "application/json",
-                "X-Checksum": "token " + checksum,
-                "X-Timestamp": current_date,
-                "X-AppKey": self.breeze.api_key,
-                "X-SessionToken": self.base64_session_token,
+                'X-Checksum': "token "+checksum,
+                'X-Timestamp': current_date,
+                'X-AppKey': self.breeze.api_key,
+                'X-SessionToken': self.base64_session_token,
+                'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_5_8) AppleWebKit/534.50.2 (KHTML, like Gecko) Version/5.0.6 Safari/533.22.3'
             }
             return headers
         except Exception as e:
-            print("generate_headers() Error - ", e)
+            self.error_exception(self.generate_headers.__name__,e)
 
     def make_request(self, method, endpoint, body, headers):
         try:
             url = self.hostname + endpoint
-            if method == "GET":
-                res = requests.get(url=url, data=body, headers=headers, verify=False)
+            if method == req_type.GET:
+                res = requests.get(url=url, data=body, headers=headers)
                 return res
-            elif method == "POST":
-                res = requests.post(url=url, data=body, headers=headers, verify=False)
+            elif method == req_type.POST:
+                res = requests.post(url=url, data=body, headers=headers)
                 return res
-            elif method == "PUT":
-                res = requests.put(url=url, data=body, headers=headers, verify=False)
+            elif method == req_type.PUT:
+                res = requests.put(url=url, data=body, headers=headers)
                 return res
-            elif method == "DELETE":
-                res = requests.delete(url=url, data=body, headers=headers, verify=False)
+            elif method == req_type.DELETE:
+                res = requests.delete(url=url, data=body, headers=headers)
                 return res
-            else:
-                print("Invalid Request Method - Must be GET, POST, PUT or DELETE")
         except Exception as e:
-            print("Error while trying to make request " + method + " " + url + " - ", e)
+            self.error_exception(except_message.API_REQUEST_EXCEPTION.value.format(method,url),e)
 
     def get_customer_details(self, api_session=""):
         try:
             if api_session == "" or api_session == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "api_session cannot be empty",
-                }
-                return response
-            headers = {"Content-Type": "application/json"}
+                return self.validation_error_response(resp_message.API_SESSION_ERROR.value)
+            headers = {
+                "Content-Type": "application/json"
+            }
             body = {
                 "SessionToken": api_session,
                 "AppKey": self.breeze.api_key,
             }
-            body = json.dumps(body, separators=(",", ":"))
-            response = self.make_request("GET", "customerdetails", body, headers)
+            body = json.dumps(body, separators=(',', ':'))
+            response = self.make_request(
+                req_type.GET, api_endpoint.CUST_DETAILS.value, body, headers)
             response = response.json()
-            if (
-                "Success" in response
-                and response["Success"] != None
-                and "session_token" in response["Success"]
-            ):
-                del response["Success"]["session_token"]
+            if 'Success' in response and response['Success'] != None and 'session_token' in response['Success']:
+                del response['Success']['session_token']
             return response
         except Exception as e:
-            print("get_customer_details() Error - ", e)
+            self.error_exception(self.get_customer_details.__name__,e)
 
     def get_demat_holdings(self):
         try:
             body = {}
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "dematholdings", body, headers)
+            response = self.make_request(req_type.GET,api_endpoint.DEMAT_HOLDING.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_demat_holdings() Error- ", e)
+            self.error_exception(self.get_demat_holdings.__name__,e)
 
     def get_funds(self):
         try:
             body = {}
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "funds", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.FUND.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_funds() Error - ", e)
+            self.error_exception(self.get_funds.__name__,e)
 
     def set_funds(self, transaction_type="", amount="", segment=""):
         try:
-            if (
-                transaction_type == ""
-                or transaction_type == None
-                or amount == ""
-                or amount == None
-                or segment == ""
-                or segment == None
-            ):
-                response = {"Success": "", "Status": 500, "Error": ""}
+            if transaction_type == "" or transaction_type == None or amount == "" or amount == None or segment == "" or segment == None:
                 if transaction_type == "" or transaction_type == None:
-                    response["Error"] = "Transaction-Type cannot be empty"
+                    return self.validation_error_response(resp_message.BLANK_TRANSACTION_TYPE.value)
                 elif amount == "" or amount == None:
-                    response["Error"] = "Amount cannot be empty"
+                    return self.validation_error_response(resp_message.BLANK_AMOUNT.value)
                 elif segment == "" or segment == None:
-                    response["Error"] = "Segment cannot be empty"
-                return response
-            elif transaction_type.lower() not in ["debit", "credit"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Transaction-Type should be either 'debit' or 'credit'",
-                }
-                return response
+                    return self.validation_error_response(resp_message.BLANK_SEGMENT.value)
+            elif transaction_type.lower() not in config.TRANSACTION_TYPES:
+                return self.validation_error_response(resp_message.TRANSACTION_TYPE_ERROR.value)
+            # elif not int(amount) > 0:
+            #     return self.validation_error_response(resp_message.ZERO_AMOUNT_ERROR.value)
             if amount.isdigit():  # Check if the input does not consist only of digits
                 if not int(amount) > 0:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Amount should be more than 0",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.ZERO_AMOUNT_ERROR.value)
             else:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Amount should only contain digits",
-                }
-                return response
+                return self.validation_error_response(resp_message.AMOUNT_DIGIT_ERROR.value)
 
             body = {
                 "transaction_type": transaction_type,
                 "amount": amount,
-                "segment": segment,
+                "segment": segment
             }
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("POST", "funds", body, headers)
+            response = self.make_request(req_type.POST, api_endpoint.FUND.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("set_funds() Error - ", e)
+            self.error_exception(self.set_funds.__name__,e)
 
-    def get_historical_data(
-        self,
-        interval="",
-        from_date="",
-        to_date="",
-        stock_code="",
-        exchange_code="",
-        product_type="",
-        expiry_date="",
-        right="",
-        strike_price="",
-    ):
+    def get_historical_data(self, interval="", from_date="", to_date="", stock_code="", exchange_code="", product_type="", expiry_date="", right="", strike_price=""):
         try:
             if interval == "" or interval == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Interval cannot be empty",
-                }
-                return response
-            elif interval.lower() not in ["1minute", "5minute", "30minute", "1day"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Interval should be either '1minute', '5minute', '30minute', or '1day'",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_INTERVAL.value)
+            elif interval.lower() not in config.INTERVAL_TYPES:
+                return self.validation_error_response(resp_message.INTERVAL_TYPE_ERROR.value)
             elif exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
-            elif exchange_code.lower() not in ["nse", "nfo", "ndx", "mcx"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code should be either 'nse', or 'nfo' or 'ndx' or 'mcx'",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif exchange_code.lower() not in config.EXCHANGE_CODES_HIST:
+                return self.validation_error_response(resp_message.EXCHANGE_CODE_ERROR.value)
             elif from_date == "" or from_date == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "From-Date cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_FROM_DATE.value)
             elif to_date == "" or to_date == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "To-Date cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_TO_DATE.value)
             elif stock_code == "" or stock_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Stock-Code cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
             elif exchange_code.lower() == "nfo":
                 if product_type == "" or product_type == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Product-type cannot be empty for Exchange-Code 'nfo'",
-                    }
-                    return response
-                elif product_type.lower() not in [
-                    "futures",
-                    "options",
-                    "futureplus",
-                    "optionplus",
-                ]:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Product-type should be either 'futures', 'options', 'futureplus', or 'optionplus' for Exchange-Code 'NFO'",
-                    }
-                    return response
-                elif product_type.lower() == "options" and (
-                    strike_price == "" or strike_price == None
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Strike-Price cannot be empty for Product-Type 'options'",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_PRODUCT_TYPE_NFO.value)
+                elif product_type.lower() not in config.PRODUCT_TYPES_HIST:
+                    return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR_NFO.value)
+                elif product_type.lower() == "options" and (strike_price == "" or strike_price == None):
+                    return self.validation_error_response(resp_message.BLANK_STRIKE_PRICE.value)
                 elif expiry_date == "" or expiry_date == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Expiry-Date cannot be empty for exchange-code 'nfo'",
-                    }
-                    return response
-            if interval == "1minute":
-                interval = "minute"
-            elif interval == "1day":
-                interval = "day"
+                    return self.validation_error_response(resp_message.BLANK_EXPIRY_DATE.value)
+
+            if interval == '1minute':
+                interval = 'minute'
+            elif interval == '1day':
+                interval = 'day'
             body = {
                 "interval": interval,
                 "from_date": from_date,
                 "to_date": to_date,
                 "stock_code": stock_code,
-                "exchange_code": exchange_code,
+                "exchange_code": exchange_code
             }
             if product_type != "" and product_type != None:
                 body["product_type"] = product_type
             if expiry_date != "" and expiry_date != None:
                 body["expiry_date"] = expiry_date
             if strike_price != "" and strike_price != None:
                 body["strike_price"] = strike_price
             if right != "" and right != None:
                 body["right"] = right
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "historicalcharts", body, headers)
+            response = self.make_request(
+                req_type.GET, api_endpoint.HIST_CHART.value, body, headers)
+            response = response.json()
+            return response
+        except Exception as e:
+            self.error_exception(self.get_historical_data.__name__,e)
+
+    def get_historical_data_v2(self, interval="", from_date="", to_date="", stock_code="", exchange_code="", product_type="", expiry_date="", right="", strike_price=""):
+        try:
+            if interval == "" or interval == None:
+                return self.validation_error_response(resp_message.BLANK_INTERVAL.value)
+            elif interval.lower() not in config.INTERVAL_TYPES_HIST_V2:
+                return self.validation_error_response(resp_message.INTERVAL_TYPE_ERROR_HIST_V2.value)
+            elif exchange_code == "" or exchange_code == None:
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif exchange_code.lower() not in config.EXCHANGE_CODES_HIST_V2:
+                return self.validation_error_response(resp_message.EXCHANGE_CODE_HIST_V2_ERROR.value)
+            elif from_date == "" or from_date == None:
+                return self.validation_error_response(resp_message.BLANK_FROM_DATE.value)
+            elif to_date == "" or to_date == None:
+                return self.validation_error_response(resp_message.BLANK_TO_DATE.value)
+            elif stock_code == "" or stock_code == None:
+                return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
+            elif exchange_code.lower() in config.FNO_EXCHANGE_TYPES:
+                if product_type == "" or product_type == None:
+                    return self.validation_error_response(resp_message.BLANK_PRODUCT_TYPE_HIST_V2.value)
+                elif product_type.lower() not in config.PRODUCT_TYPES_HIST_V2:
+                    return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR_HIST_V2.value)
+                elif product_type.lower() == "options" and (strike_price == "" or strike_price == None):
+                    return self.validation_error_response(resp_message.BLANK_STRIKE_PRICE.value)
+                elif expiry_date == "" or expiry_date == None:
+                    return self.validation_error_response(resp_message.BLANK_EXPIRY_DATE.value)
+
+            url_params = {
+                "interval": interval,
+                "from_date": from_date,
+                "to_date": to_date,
+                "stock_code": stock_code,
+                "exch_code": exchange_code
+            }
+            if product_type != "" and product_type != None:
+                url_params["product_type"] = product_type
+            if expiry_date != "" and expiry_date != None:
+                url_params["expiry_date"] = expiry_date
+            if strike_price != "" and strike_price != None:
+                url_params["strike_price"] = strike_price
+            if right != "" and right != None:
+                url_params["right"] = right
+            headers = {
+                "Content-Type": "application/json",
+                'X-SessionToken':self.base64_session_token,
+                'apikey':self.breeze.api_key
+            }
+            url = config.BREEZE_NEW_URL + api_endpoint.HIST_CHART.value
+            response = requests.get(url=url, params=url_params, headers=headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_historical_data() Error - ", e)
+            self.error_exception(self.get_historical_data_v2.__name__,e)
 
-    def add_margin(
-        self,
-        product_type="",
-        stock_code="",
-        exchange_code="",
-        settlement_id="",
-        add_amount="",
-        margin_amount="",
-        open_quantity="",
-        cover_quantity="",
-        category_index_per_stock="",
-        expiry_date="",
-        right="",
-        contract_tag="",
-        strike_price="",
-        segment_code="",
-    ):
+    def add_margin(self, product_type="", stock_code="", exchange_code="", settlement_id="", add_amount="", margin_amount="", open_quantity="", cover_quantity="", category_index_per_stock="", expiry_date="", right="", contract_tag="", strike_price="", segment_code=""):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
-            elif (
-                product_type != ""
-                and product_type != None
-                and product_type.lower()
-                not in [
-                    "futures",
-                    "options",
-                    "futureplus",
-                    "optionplus",
-                    "cash",
-                    "eatm",
-                    "margin",
-                ]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product-type should be either 'futures', 'options', 'futureplus', 'optionplus', 'cash', 'eatm', or 'margin'",
-                }
-                return response
-            elif (
-                right != ""
-                and right != None
-                and right.lower() not in ["call", "put", "others"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Right should be either 'call', 'put', or 'others'",
-                }
-                return response
-            body = {"exchange_code": exchange_code}
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif product_type != "" and product_type != None and product_type.lower() not in config.PRODUCT_TYPES:
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR.value)
+            elif right != "" and right != None and right.lower() not in config.RIGHT_TYPES:
+                return self.validation_error_response(resp_message.RIGHT_TYPE_ERROR.value)
+
+            body = {
+                "exchange_code": exchange_code
+            }
             if product_type != "" and product_type != None:
                 body["product_type"] = product_type
             if stock_code != "" and stock_code != None:
                 body["stock_code"] = stock_code
             if cover_quantity != "" and cover_quantity != None:
                 body["cover_quantity"] = cover_quantity
             if category_index_per_stock != "" and category_index_per_stock != None:
@@ -1545,380 +1193,190 @@
                 body["segment_code"] = segment_code
             if settlement_id != "" and settlement_id != None:
                 body["settlement_id"] = settlement_id
             if add_amount != "" and add_amount != None:
                 body["add_amount"] = add_amount
             if open_quantity != "" and open_quantity != None:
                 body["open_quantity"] = open_quantity
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("POST", "margin", body, headers)
+            response = self.make_request(req_type.POST, api_endpoint.MARGIN.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("add_margin() Error - ", e)
+            self.error_exception(self.add_margin.__name__,e)
 
     def get_margin(self, exchange_code=""):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
-            body = {"exchange_code": exchange_code}
-            body = json.dumps(body, separators=(",", ":"))
-            headers = self.generate_headers(body)
-            print("headers---------------------->", headers)
-            response = self.make_request("GET", "margin", body, headers)
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+
+            body = {
+                "exchange_code": exchange_code
+            }
+            body = json.dumps(body, separators=(',', ':'))
+            headers = self.generate_headers(body)
+            response = self.make_request(req_type.GET,  api_endpoint.MARGIN.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_margin() Error - ", e)
-
-    def place_order(
-        self,
-        stock_code="",
-        exchange_code="",
-        product="",
-        action="",
-        order_type="",
-        stoploss="",
-        quantity="",
-        price="",
-        validity="",
-        validity_date="",
-        disclosed_quantity="",
-        expiry_date="",
-        right="",
-        strike_price="",
-        user_remark="",
-        order_type_fresh="",
-        order_rate_fresh="",
-        lots="",
-    ):
-        try:
-            if (
-                stock_code == ""
-                or stock_code == None
-                or exchange_code == ""
-                or exchange_code == None
-                or product == ""
-                or product == None
-                or action == ""
-                or action == None
-                or order_type == ""
-                or order_type == None
-                or price == ""
-                or price == None
-                or action == ""
-                or action == None
-            ):
+            self.error_exception(self.get_margin.__name__,e)
+
+    def place_order(self, stock_code="", exchange_code="", product="", action="", order_type="", stoploss="", quantity="", price="", validity="", validity_date="", disclosed_quantity="", expiry_date="", right="", strike_price="", user_remark="",order_type_fresh="",order_rate_fresh="",settlement_id = "",order_segment_code = "",lots="",):
+        try:
+            if stock_code == "" or stock_code == None or exchange_code == "" or exchange_code == None or product == "" or product == None or action == "" or action == None or order_type == "" or order_type == None or price == "" or price == None or action == "" or action == None:
                 if stock_code == "" or stock_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Stock-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
                 elif exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 elif product == "" or product == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Product cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_PRODUCT_TYPE.value)
                 elif action == "" or action == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Action cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_ACTION.value)
                 elif order_type == "" or order_type == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Order-type cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_ORDER_TYPE.value)
+                # elif quantity == "" or quantity == None:
+                #     return self.validation_error_response(resp_message.BLANK_QUANTITY.value)
                 elif validity == "" or validity == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Validity cannot be empty",
-                    }
-                    return response
-            elif product.lower() not in [
-                "futures",
-                "options",
-                "futureplus",
-                "optionplus",
-                "cash",
-                "eatm",
-                "margin",
-            ]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product should be either 'futures', 'options', 'futureplus', 'optionplus', 'cash', 'eatm', or 'margin'",
-                }
-                return response
-            elif action.lower() not in ["buy", "sell"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Action should be either 'buy', or 'sell'",
-                }
-                return response
-            elif order_type.lower() not in ["limit", "market", "stoploss"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Order-type should be either 'limit', 'market', or 'stoploss'",
-                }
-                return response
-            elif validity.lower() not in ["day", "ioc", "vtc"]:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Validity should be either 'day', 'ioc', or 'vtc'",
-                }
-                return response
-            elif (
-                right != ""
-                and right != None
-                and right.lower() not in ["call", "put", "others"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Right should be either 'call', 'put', or 'others'",
-                }
-                return response
-            if exchange_code.lower() in ["mcx", "ndx"]:
+                    return self.validation_error_response(resp_message.BLANK_VALIDITY.value)
+            elif product.lower() not in config.PRODUCT_TYPES:
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR.value)
+            elif action.lower() not in config.ACTION_TYPES:
+                return self.validation_error_response(resp_message.ACTION_TYPE_ERROR.value)
+            elif order_type.lower() not in config.ORDER_TYPES:
+                return self.validation_error_response(resp_message.ORDER_TYPE_ERROR.value)
+            elif validity.lower() not in config.VALIDITY_TYPES:
+                return self.validation_error_response(resp_message.VALIDITY_TYPE_ERROR.value)
+            elif right != "" and right != None and right.lower() not in config.RIGHT_TYPES:
+                return self.validation_error_response(resp_message.RIGHT_TYPE_ERROR.value)
+            if exchange_code.lower() in ["mcx"]:
                 if lots == "" or lots == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Lots cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_LOTS.value)
+            elif exchange_code.lower() in ["ndx"]:
+                return self.validation_error_response(resp_message.CURRENCY_NOT_ALLOWED.value)
             else:
                 if quantity == "" or quantity == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Quantity cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_QUANTITY.value)
+
             body = {
                 "stock_code": stock_code,
-                "exchange_code": exchange_code,
+                "exchange_code": exchange_code.upper(),
                 "product": product,
                 "action": action,
                 "order_type": order_type,
                 "quantity": quantity,
                 "price": price,
                 "validity": validity,
-                "order_type_fresh": order_type_fresh,
-                "order_rate_fresh": order_rate_fresh,
-                "lots": lots,
+                "settlement_id" : settlement_id,
+                "order_segment_code" : order_segment_code,
+                "lots": lots, 
             }
+
             if stoploss != "" and stoploss != None:
                 body["stoploss"] = stoploss
             if validity_date != "" and validity_date != None:
                 body["validity_date"] = validity_date
             if disclosed_quantity != "" and disclosed_quantity != None:
                 body["disclosed_quantity"] = disclosed_quantity
             if expiry_date != "" and expiry_date != None:
                 body["expiry_date"] = expiry_date
             if right != "" and right != None:
                 body["right"] = right
             if strike_price != "" and strike_price != None:
                 body["strike_price"] = strike_price
             if user_remark != "" and user_remark != None:
                 body["user_remark"] = user_remark
-            body = json.dumps(body, separators=(",", ":"))
+            if(order_type_fresh != "" and order_type_fresh != None):
+                body['order_type_fresh'] = order_type_fresh
+            if(order_rate_fresh != "" and order_rate_fresh != None):
+                body['order_rate_fresh'] = order_rate_fresh
+
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("POST", "order", body, headers)
+            response = self.make_request(req_type.POST, api_endpoint.ORDER.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("place_order() Error - ", e)
+            self.error_exception(self.place_order.__name__,e)
 
     def get_order_detail(self, exchange_code, order_id):
         try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or order_id == ""
-                or order_id == None
-            ):
+            if exchange_code == "" or exchange_code == None or order_id == "" or order_id == None:
                 if exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 elif order_id == "" or order_id == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Order-Id cannot be empty",
-                    }
-                    return response
-            body = {"exchange_code": exchange_code, "order_id": order_id}
-            body = json.dumps(body, separators=(",", ":"))
+                    return self.validation_error_response(resp_message.BLANK_ORDER_ID.value)
+
+            body = {
+                "exchange_code": exchange_code,
+                "order_id": order_id
+            }
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "order", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.ORDER.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_order_detail() Error - ", e)
+            self.error_exception(self.get_order_detail.__name__,e)
 
     def get_order_list(self, exchange_code, from_date, to_date):
         try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or from_date == ""
-                or from_date == None
-                or to_date == ""
-                or to_date == None
-            ):
+            if exchange_code == "" or exchange_code == None or from_date == "" or from_date == None or to_date == "" or to_date == None:
                 if exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 elif from_date == "" or from_date == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "From-Date cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_FROM_DATE.value)
                 elif to_date == "" or to_date == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "To-Date cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_TO_DATE.value)
+
             body = {
                 "exchange_code": exchange_code,
                 "from_date": from_date,
-                "to_date": to_date,
+                "to_date": to_date
             }
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "order", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.ORDER.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_order_list() Error - ", e)
+            self.error_exception(self.get_order_list.__name__,e)
 
     def cancel_order(self, exchange_code, order_id):
         try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or order_id == ""
-                or order_id == None
-            ):
+            if exchange_code == "" or exchange_code == None or order_id == "" or order_id == None:
                 if exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 elif order_id == "" or order_id == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Order-Id cannot be empty",
-                    }
-                    return response
-            body = {"exchange_code": exchange_code, "order_id": order_id}
-            body = json.dumps(body, separators=(",", ":"))
-            headers = self.generate_headers(body)
-            response = self.make_request("DELETE", "order", body, headers)
+                    return self.validation_error_response(resp_message.BLANK_ORDER_ID.value)
+
+            body = {
+                "exchange_code": exchange_code,
+                "order_id": order_id
+            }
+            body = json.dumps(body, separators=(',', ':'))
+            headers = self.generate_headers(body)
+            response = self.make_request(req_type.DELETE, api_endpoint.ORDER.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("cancel_order() Error - ", e)
-
-    def modify_order(
-        self,
-        order_id,
-        exchange_code,
-        order_type,
-        stoploss,
-        quantity,
-        price,
-        validity,
-        disclosed_quantity,
-        validity_date,
-    ):
-        try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or order_id == ""
-                or order_id == None
-            ):
+            self.error_exception(self.cancel_order.__name__,e)
+
+    def modify_order(self, order_id, exchange_code, order_type, stoploss, quantity, price, validity, disclosed_quantity, validity_date):
+        try:
+            if exchange_code == "" or exchange_code == None or order_id == "" or order_id == None:
                 if exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 elif order_id == "" or order_id == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Order-Id cannot be empty",
-                    }
-                    return response
-            elif (
-                order_type != ""
-                and order_type != None
-                and order_type.lower() not in ["limit", "market", "stoploss"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Order-type should be either 'limit', 'market', or 'stoploss'",
-                }
-                return response
-            elif (
-                validity != ""
-                and validity != None
-                and validity.lower() not in ["day", "ioc", "vtc"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Validity should be either 'day', 'ioc', or 'vtc'",
-                }
-                return response
+                    return self.validation_error_response(resp_message.BLANK_ORDER_ID.value)
+            elif order_type != "" and order_type != None and order_type.lower() not in config.ORDER_TYPES:
+                return self.validation_error_response(resp_message.ORDER_TYPE_ERROR.value)
+            elif validity != "" and validity != None and validity.lower() not in config.VALIDITY_TYPES:
+                return self.validation_error_response(resp_message.VALIDITY_TYPE_ERROR.value)
+
             body = {
                 "order_id": order_id,
                 "exchange_code": exchange_code,
             }
             if order_type != "" and order_type != None:
                 body["order_type"] = order_type
             if stoploss != "" and stoploss != None:
@@ -1929,268 +1387,134 @@
                 body["price"] = price
             if validity != "" and validity != None:
                 body["validity"] = validity
             if disclosed_quantity != "" and disclosed_quantity != None:
                 body["disclosed_quantity"] = disclosed_quantity
             if validity_date != "" and validity_date != None:
                 body["validity_date"] = validity_date
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("PUT", "order", body, headers)
+            response = self.make_request(req_type.PUT, api_endpoint.ORDER.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("modify_order() Error - ", e)
+            self.error_exception(self.modify_order.__name__,e)
 
-    def get_portfolio_holdings(
-        self, exchange_code, from_date, to_date, stock_code, portfolio_type
-    ):
+    def get_portfolio_holdings(self, exchange_code, from_date, to_date, stock_code, portfolio_type):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+
             body = {
                 "exchange_code": exchange_code,
             }
             if from_date != "" and from_date != None:
                 body["from_date"] = from_date
             if to_date != "" and to_date != None:
                 body["to_date"] = to_date
             if stock_code != "" and stock_code != None:
                 body["stock_code"] = stock_code
             if portfolio_type != "" and portfolio_type != None:
                 body["portfolio_type"] = portfolio_type
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "portfolioholdings", body, headers)
+            response = self.make_request(
+                req_type.GET, api_endpoint.PORTFOLIO_HOLDING.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_portfolio_holdings() Error - ", e)
+            self.error_exception(self.get_portfolio_holdings.__name__,e)
 
     def get_portfolio_positions(self):
         try:
             body = {}
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "portfoliopositions", body, headers)
+            response = self.make_request(
+                req_type.GET, api_endpoint.PORTFOLIO_POSITION.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_portfolio_positions() Error - ", e)
+            self.error_exception(self.get_portfolio_positions.__name__,e)
 
-    def get_quotes(
-        self, stock_code, exchange_code, expiry_date, product_type, right, strike_price
-    ):
+    def get_quotes(self, stock_code, exchange_code, expiry_date, product_type, right, strike_price):
         try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or stock_code == ""
-                or stock_code == None
-            ):
+            if exchange_code == "" or exchange_code == None or stock_code == "" or stock_code == None:
                 if exchange_code == "" or exchange_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Exchange-Code cannot be empty",
-                    }
-                    return response
+                    return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
                 if stock_code == "" or stock_code == None:
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Stock-Code cannot be empty",
-                    }
-                    return response
-            elif (
-                product_type != ""
-                and product_type != None
-                and product_type.lower()
-                not in [
-                    "futures",
-                    "options",
-                    "futureplus",
-                    "optionplus",
-                    "cash",
-                    "eatm",
-                    "margin",
-                ]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product-type should be either 'futures', 'options', 'futureplus', 'optionplus', 'cash', 'eatm', or 'margin'",
-                }
-                return response
-            elif (
-                right != ""
-                and right != None
-                and right.lower() not in ["call", "put", "others"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Right should be either 'call', 'put', or 'others'",
-                }
-                return response
-            body = {"stock_code": stock_code, "exchange_code": exchange_code}
+                    return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
+            elif product_type != "" and product_type != None and product_type.lower() not in config.PRODUCT_TYPES:
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR.value)
+            elif right != "" and right != None and right.lower() not in config.RIGHT_TYPES:
+                return self.validation_error_response(resp_message.RIGHT_TYPE_ERROR.value)
+
+            body = {
+                "stock_code": stock_code,
+                "exchange_code": exchange_code
+            }
             if expiry_date != "" and expiry_date != None:
                 body["expiry_date"] = expiry_date
             if product_type != "" and product_type != None:
                 body["product_type"] = product_type
             if right != "" and right != None:
                 body["right"] = right
             if strike_price != "" and strike_price != None:
                 body["strike_price"] = strike_price
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "quotes", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.QUOTE.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_quotes() Error - ", e)
+            self.error_exception(self.get_quotes.__name__,e)
 
-    def get_option_chain_quotes(
-        self, stock_code, exchange_code, expiry_date, product_type, right, strike_price
-    ):
+    def get_option_chain_quotes(self,stock_code, exchange_code, expiry_date, product_type, right, strike_price):
         try:
-            if (
-                exchange_code == ""
-                or exchange_code == None
-                or exchange_code.lower() != "nfo"
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "exchange code should be nfo",
-                }
-                return response
-            elif product_type == "" or product_type == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product-Type cannot be empty for Exchange-Code value as 'nfo'.",
-                }
-                return response
-            elif product_type != "future" and product_type != "options":
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product-type should be either 'futures' or 'options' for Exchange-Code value as 'nfo'.",
-                }
-                return response
-            elif stock_code == "" or stock_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "stock code cannot be empty",
-                }
-                return response
-            elif product_type == "options":
-                if (
-                    (expiry_date == "" or expiry_date == None)
-                    and (strike_price == "" or strike_price == None)
-                    and (right == "" or right == None)
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Atleast two inputs are required out of Expiry-Date, Right & Strike-Price. All three cannot be empty'.",
-                    }
-                    return response
-                elif (
-                    (expiry_date != "" or expiry_date != None)
-                    and (strike_price == "" or strike_price == None)
-                    and (right == "" or right == None)
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Either Right or Strike-Price cannot be empty.",
-                    }
-                    return response
-                elif (
-                    (expiry_date == "" or expiry_date == None)
-                    and (strike_price != "" or strike_price != None)
-                    and (right == "" or right == None)
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Either Expiry-Date or Right cannot be empty.",
-                    }
-                    return response
-                elif (
-                    (expiry_date == "" or expiry_date == None)
-                    and (strike_price == "" or strike_price == None)
-                    and (right != None or right != "")
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Either Expiry-Date or Strike-Price cannot be empty.",
-                    }
-                    return response
-                elif (right != "" or right != None) and (
-                    right != "call" and right != "put" and right != "others"
-                ):
-                    response = {
-                        "Success": "",
-                        "Status": 500,
-                        "Error": "Right should be either 'call', 'put', or 'others'.",
-                    }
-                    return response
-            body = {"stock_code": stock_code, "exchange_code": exchange_code}
+            if exchange_code == "" or exchange_code == None or  exchange_code.lower()!="nfo":
+                return self.validation_error_response(resp_message.OPT_CHAIN_EXCH_CODE_ERROR.value)
+            elif product_type=="" or product_type== None:
+                return self.validation_error_response(resp_message.BLANK_PRODUCT_TYPE_NFO.value)
+            elif product_type.lower()!="futures" and product_type.lower()!="options":
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR_NFO.value)
+            elif stock_code=="" or stock_code==None:
+                return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
+            elif product_type.lower() == 'options':
+                if((expiry_date=="" or expiry_date==None)  and (strike_price=="" or strike_price==None) and (right=="" or right==None)):
+                    return self.validation_error_response(resp_message.NFO_FIELDS_MISSING_ERROR.value)
+                elif((expiry_date!="" and expiry_date!=None) and (strike_price=="" or  strike_price==None) and (right=="" or right==None)):
+                    return self.validation_error_response(resp_message.BLANK_RIGHT_STRIKE_PRICE.value)
+                elif((expiry_date == "" or expiry_date == None) and (strike_price!="" or strike_price!=None) and (right=="" or right == None)):
+                    return self.validation_error_response(resp_message.BLANK_RIGHT_EXPIRY_DATE.value)
+                elif((expiry_date=="" or expiry_date==None) and (strike_price=="" or strike_price==None) and (right!=None or right!="")):
+                    return self.validation_error_response(resp_message.BLANK_EXPIRY_DATE_STRIKE_PRICE.value)
+                elif((right!="" and right!=None) and (right.lower()!="call" and right.lower()!="put" and right.lower()!="others")):
+                    return self.validation_error_response(resp_message.RIGHT_TYPE_ERROR.value)
+
+            body = {
+                "stock_code": stock_code,
+                "exchange_code": exchange_code
+            }
             if expiry_date != "" and expiry_date != None:
                 body["expiry_date"] = expiry_date
             if product_type != "" and product_type != None:
                 body["product_type"] = product_type
             if right != "" and right != None:
                 body["right"] = right
             if strike_price != "" and strike_price != None:
                 body["strike_price"] = strike_price
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "optionchain", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.OPT_CHAIN.value, body, headers)
             response = response.json()
             return response
-        except:
-            print("get_option_chain_quotes() Error -", e)
+        except Exception as e:
+            self.error_exception(self.get_option_chain_quotes.__name__,e)
 
-    def square_off(
-        self,
-        source_flag,
-        stock_code,
-        exchange_code,
-        quantity,
-        price,
-        action,
-        order_type,
-        validity,
-        stoploss,
-        disclosed_quantity,
-        protection_percentage,
-        settlement_id,
-        margin_amount,
-        open_quantity,
-        cover_quantity,
-        product_type,
-        expiry_date,
-        right,
-        strike_price,
-        validity_date,
-        trade_password,
-        alias_name,
-        lots,
-    ):
+    def square_off(self, source_flag, stock_code, exchange_code, quantity, price, action, order_type, validity, stoploss, disclosed_quantity, protection_percentage, settlement_id, margin_amount, open_quantity, cover_quantity, product, expiry_date, right, strike_price, validity_date, trade_password, alias_name, order_reference, position_exchange_code, lots):
         try:
             body = {
                 "source_flag": source_flag,
                 "stock_code": stock_code,
                 "exchange_code": exchange_code,
                 "quantity": quantity,
                 "price": price,
@@ -2200,245 +1524,214 @@
                 "stoploss_price": stoploss,
                 "disclosed_quantity": disclosed_quantity,
                 "protection_percentage": protection_percentage,
                 "settlement_id": settlement_id,
                 "margin_amount": margin_amount,
                 "open_quantity": open_quantity,
                 "cover_quantity": cover_quantity,
-                "product_type": product_type,
+                "product_type": product,
                 "expiry_date": expiry_date,
                 "right": right,
                 "strike_price": strike_price,
                 "validity_date": validity_date,
                 "alias_name": alias_name,
                 "trade_password": trade_password,
-                "lots": lots,
+                "order_reference":order_reference,
+                "position_exchange_code":position_exchange_code,
+                "lots": lots
             }
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("POST", "squareoff", body, headers)
+            response = self.make_request(req_type.POST, api_endpoint.SQUARE_OFF.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("square_off() Error - ", e)
+            self.error_exception(self.square_off.__name__,e)
 
-    def get_trade_list(
-        self, from_date, to_date, exchange_code, product_type, action, stock_code
-    ):
+    def get_trade_list(self, from_date, to_date, exchange_code, product_type, action, stock_code):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
-            elif (
-                product_type != ""
-                and product_type != None
-                and product_type.lower()
-                not in [
-                    "futures",
-                    "options",
-                    "futureplus",
-                    "optionplus",
-                    "cash",
-                    "eatm",
-                    "margin",
-                ]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product-type should be either 'futures', 'options', 'futureplus', 'optionplus', 'cash', 'eatm', or 'margin'",
-                }
-                return response
-            elif (
-                action != ""
-                and action != None
-                and action.lower() not in ["buy", "sell"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Action should be either 'buy', or 'sell'",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif product_type != "" and product_type != None and product_type.lower() not in config.PRODUCT_TYPES:
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR.value)
+            elif action != "" and action != None and action.lower() not in config.ACTION_TYPES:
+                return self.validation_error_response(resp_message.ACTION_TYPE_ERROR.value)
+
             body = {
                 "exchange_code": exchange_code,
             }
             if from_date != "" and from_date != None:
                 body["from_date"] = from_date
             if to_date != "" and to_date != None:
                 body["to_date"] = to_date
             if product_type != "" and product_type != None:
                 body["product_type"] = product_type
             if action != "" and action != None:
                 body["action"] = action
             if stock_code != "" and stock_code != None:
                 body["stock_code"] = stock_code
-            body = json.dumps(body, separators=(",", ":"))
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "trades", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.TRADE.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_trade_list() Error - ", e)
+            self.error_exception(self.get_trade_list.__name__s,e)
 
     def get_trade_detail(self, exchange_code, order_id):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
             elif order_id == "" or order_id == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Order-Id cannot be empty",
-                }
-                return response
-            body = {"exchange_code": exchange_code, "order_id": order_id}
-            body = json.dumps(body, separators=(",", ":"))
+                return self.validation_error_response(resp_message.BLANK_ORDER_ID.value)
+ 
+            body = {
+                "exchange_code": exchange_code,
+                "order_id": order_id
+            }
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "trades", body, headers)
+            response = self.make_request(req_type.GET, api_endpoint.TRADE.value, body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("get_trade_detail() Error - ", e)
-
+            self.error_exception(self.get_trade_detail.__name__,e)
+    
     def get_names(self, exchange_code, stock_code):
         try:
             lexchange_code = exchange_code.lower()
             stock_code = stock_code.upper()
-            mapper_exchangecode_to_file = dict()
-            mapper_exchangecode_to_file["nse"] = "NSEScripMaster.txt"
-            mapper_exchangecode_to_file["bse"] = "BSEScripMaster.txt"
-            mapper_exchangecode_to_file["cdnse"] = "CDNSEScripMaster.txt"
-            mapper_exchangecode_to_file["fonse"] = "FONSEScripMaster.txt"
-            required_file = zipfile.open(
-                mapper_exchangecode_to_file.get(lexchange_code)
-            )
-
-            dataframe = pd.read_csv(required_file, sep=",", engine="python")
-
-            print(dataframe.columns)
-            print("length", len(dataframe.columns))
-            df2 = dataframe[dataframe[' "ExchangeCode"'] == stock_code]
-            if len(df2) == 0:
-                df2 = dataframe[dataframe[' "ShortName"'] == stock_code]
-            # print("df",df2)
-
-            requiredresult = df2[
-                [' "ShortName"', ' "ExchangeCode"', "Token", ' "CompanyName"']
-            ]
-
+            mapper_exchangecode_to_file = config.ISEC_NSE_CODE_MAP_FILE
+            required_file = zipfile.open(mapper_exchangecode_to_file.get(lexchange_code))
+    
+            dataframe = pd.read_csv(required_file, sep=',', engine='python')
+             
+            df2 = dataframe[(dataframe[' "ExchangeCode"'] == stock_code) | (dataframe[' "ShortName"'] == stock_code)]
+            if(len(df2)==0):
+                return self.validation_error_response(except_message.ISEC_NSE_STOCK_MAP_EXCEPTION.value)
+            requiredresult = df2[[' "ShortName"',' "ExchangeCode"','Token',' "CompanyName"']]
+    
             isec_stock = requiredresult[' "ShortName"'].to_string().split()[1]
-            token = requiredresult["Token"].to_string().split()[1]
+            token = " ".join(requiredresult['Token'].to_string().split()[1:])
             exchange = requiredresult[' "ExchangeCode"'].to_string()
+            compname = " ".join(requiredresult[' "CompanyName"'].to_string().split()[1:])
+            if(" " in exchange):
+                exchange = " ".join(exchange.split()[1:])
+
+            result = {
+                    'exchange_code':exchange_code,
+                    'exchange_stock_code': exchange,
+                    'isec_stock_code':isec_stock,
+                    'isec_token': token,
+                    'company name':compname,
+                    'isec_token_level1':str('4.1!') + str(token),
+                    'isec_token_level2':str('4.2!') + str(token)
+                }
+    
+            return result
+        except Exception as e:
+            self.error_exception(self.get_names.__name__,e)
 
-            if " " in exchange:
-                exchange = exchange.split()[1]
-
-            # print(value,"val")
-            result = dict()
-            result["exchange_code"] = exchange_code
-            result["exchange_stock_code"] = exchange
-            result["isec_stock_code"] = isec_stock
-            result["isec_token"] = token
-            result["company_name"] = " ".join(
-                requiredresult[' "CompanyName"'].to_string().split()[1:]
-            )
-            response = json.dumps(result, indent=4)
-            return response
-        except Exception as e:
-            print("get_names() Error - ", e)
-
-    def preview_order(
-        self,
-        stock_code="",
-        exchange_code="",
-        product="",
-        order_type="",
-        price="",
-        action="",
-        quantity="",
-        expiry_date="",
-        right="",
-        strike_price="",
-        specialflag="",
-        stoploss="",
-        order_rate_fresh="",
-    ):
+    def limit_calculator(self,strike_price,product_type,expiry_date,underlying,exchange_code,order_flow,stop_loss_trigger,option_type,source_flag,limit_rate,order_reference,available_quantity,market_type,fresh_order_limit):
         try:
             if exchange_code == "" or exchange_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Exchange-Code cannot be empty",
-                }
-                return response
-            elif product == "" or product == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Product cannot be empty",
-                }
-                return response
-            elif stock_code == "" or stock_code == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "stock code cannot be empty",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif strike_price == "" or strike_price == None:
+                return self.validation_error_response(resp_message.BLANK_STRIKE_PRICE.value)
+            elif product_type == "" or product_type == None:
+                return self.validation_error_response(resp_message.BLANK_PRODUCT_TYPE_NFO.value)
+            elif underlying == "" or underlying == None:
+                return self.validation_error_response(resp_message.UNDER_LYING_ERROR.value)
+            elif order_flow == "" or order_flow == None:
+                return self.validation_error_response(resp_message.ORDER_FLOW.value)
+            
+            elif stop_loss_trigger == "" or stop_loss_trigger == None:
+                return self.validation_error_response(resp_message.STOP_LOSS_TRIGGER.value)
+                
+            elif option_type == "" or option_type == None:
+                return self.validation_error_response(resp_message.OPTION_TYPE.value)
+            elif source_flag == "" or source_flag == None:
+                return self.validation_error_response(resp_message.SOURCE_FLAG.value)
+            
+            elif market_type == "" or market_type == None:
+                return self.validation_error_response(resp_message.MARKET_TYPE.value)
+                
+            elif fresh_order_limit == "" or fresh_order_limit == None:
+                return self.validation_error_response(resp_message.FRESH_ORDER_LIMIT.value)
+            body = {                                                                                     
+                "strike_price": strike_price,                                    
+                "product_type":product_type,                 
+                "expiry_date": expiry_date,
+                "underlying" : underlying,
+                "exchange_code":exchange_code,
+                "order_flow" :order_flow,
+                "stop_loss_trigger":stop_loss_trigger,
+                "option_type":option_type,
+                "source_flag" : source_flag,
+                "limit_rate" : limit_rate,
+                "order_reference": order_reference,
+                "available_quantity":available_quantity,
+                "market_type": market_type,
+                "fresh_order_limit":fresh_order_limit
+            }
+            body = json.dumps(body, separators=(',', ':'))
+            headers = self.generate_headers(body)
+            response = self.make_request(req_type.POST, api_endpoint.LIMIT_CALCULATOR.value, body, headers)
+            response = response.json()
+            return response
+            
+        except Exception as e:
+            self.error_exception(self.limit_calculator.__name__, e)
+        
+    def margin_calculator(self,lists,exchange_code):
+        try:
+            body = {
+                "list_of_positions" : lists,
+                "exchange_code" : exchange_code
+            }
+            body = json.dumps(body, separators=(',', ':'))
+            headers = self.generate_headers(body)
+            response = self.make_request(req_type.POST, api_endpoint.MARGIN_CALULATOR.value , body, headers)
+            response = response.json()
+            return response
+        except Exception as e:
+            self.error_exception(self.margin_calculator.__name__, e)
+            
+    def preview_order(self,stock_code="",exchange_code="",product="",order_type="",price="",action="",quantity="",expiry_date="",right="",strike_price="",specialflag="",stoploss="",order_rate_fresh=""):
+        try:
+            if exchange_code == "" or exchange_code == None :
+                return self.validation_error_response(resp_message.BLANK_EXCHANGE_CODE.value)
+            elif product=="" or product == None:
+                return self.validation_error_response(resp_message.PRODUCT_TYPE_ERROR.value)
+            elif stock_code=="" or stock_code==None:
+                return self.validation_error_response(resp_message.BLANK_STOCK_CODE.value)
             elif order_type == "" or order_type == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Order-type cannot be empty",
-                }
-                return response
-            elif action == "" or action == None:
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Action cannot be empty",
-                }
-                return response
-            elif (
-                right != ""
-                and right != None
-                and right.lower() not in ["call", "put", "others"]
-            ):
-                response = {
-                    "Success": "",
-                    "Status": 500,
-                    "Error": "Right should be either 'call', 'put', or 'others'",
-                }
-                return response
+                return self.validation_error_response(resp_message.BLANK_ORDER_TYPE.value)
+            elif action=="" or action == None:
+                return self.validation_error_response(resp_message.BLANK_ACTION.value)
+            elif right != "" and right != None and right.lower() not in config.RIGHT_TYPES:
+                return self.validation_error_response(resp_message.RIGHT_TYPE_ERROR.value)
 
             body = {
                 "stock_code": stock_code,
                 "exchange_code": exchange_code,
                 "product": product,
                 "order_type": order_type,
                 "price": price,
                 "action": action,
                 "quantity": quantity,
                 "expiry_date": expiry_date,
                 "right": right,
                 "strike_price": strike_price,
-                "specialflag": specialflag,
+                "specialflag" : specialflag,
                 "stoploss": stoploss,
-                "order_rate_fresh": order_rate_fresh,
-            }
-            body = json.dumps(body, separators=(",", ":"))
+                "order_rate_fresh": order_rate_fresh
+                }
+            body = json.dumps(body, separators=(',', ':'))
             headers = self.generate_headers(body)
-            response = self.make_request("GET", "preview_order", body, headers)
+            response = self.make_request(req_type.GET, "preview_order", body, headers)
             response = response.json()
             return response
         except Exception as e:
-            print("preview_order Error - ", e)
+            self.error_exception(self.preview_order.__name__,e)
+
+
```

### Comparing `uat_breeze_connect-1.0.14rc38/setup.py` & `uat_breeze_connect-1.0.14rc39/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uat-breeze-connect",
-    version="1.0.14rc38",
+    version="1.0.14rc39",
     author="UAT Breeze Connect",
     author_email="test@mail.com",
     description="UAT Breeze Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['python-socketio[client]','requests','pandas'],
+    install_requires=['python-socketio[client]','requests'],
     url="https://github.com/pypa/sampleproject",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
```

### Comparing `uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/PKG-INFO` & `uat_breeze_connect-1.0.14rc39/uat_breeze_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc38
+Version: 1.0.14rc39
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-socketio[client]
 Requires-Dist: requests
-Requires-Dist: pandas
 
 # Index
 
 <div class="sticky" id="index">
 <ul>
  <li><a href="#Uat_Breeze">UAT_Breeze_Connect_SDK</a></li>
  <li><a href="#Setup_env">Setup Virtual Environment</a></li>
@@ -79,15 +78,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc38
+pip install uat-breeze-connect==1.0.14rc39
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -430,15 +429,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -448,30 +447,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc38 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc39 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
-[client] Requires-Dist: requests Requires-Dist: pandas # Index
+[client] Requires-Dist: requests # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
     * _S_e_t_u_p_ _V_i_r_t_u_a_l_ _E_n_v_i_r_o_n_m_e_n_t
     * _I_n_s_t_a_l_l_i_n_g_ _t_h_e_ _c_l_i_e_n_t
     * _W_e_b_s_o_c_k_e_t_ _U_s_a_g_e
     * _A_P_I_ _U_s_a_g_e
     * _g_e_t___c_u_s_t_o_m_e_r___d_e_t_a_i_l_s
     * _g_e_t___d_e_m_a_t___h_o_l_d_i_n_g_s
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc39 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -291,15 +291,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product_type="margin",
+                    product="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -309,29 +309,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="futures",
+                    product="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product_type="options",
+                    product="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

