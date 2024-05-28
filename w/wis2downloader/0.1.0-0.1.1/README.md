# Comparing `tmp/wis2downloader-0.1.0.tar.gz` & `tmp/wis2downloader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wis2downloader-0.1.0.tar", last modified: Thu May 16 15:06:53 2024, max compression
+gzip compressed data, was "wis2downloader-0.1.1.tar", last modified: Tue May 28 07:58:29 2024, max compression
```

## Comparing `wis2downloader-0.1.0.tar` & `wis2downloader-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.673789 wis2downloader-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    18431 2024-05-16 15:06:53.673789 wis2downloader-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4646 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/README.md
--rw-rw-rw-   0        0        0      871 2024-05-16 14:56:43.000000 wis2downloader-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 15:06:53.674795 wis2downloader-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.636283 wis2downloader-0.1.0/wis2downloader/
--rw-rw-rw-   0        0        0     1045 2024-05-16 14:58:11.000000 wis2downloader-0.1.0/wis2downloader/__init__.py
--rw-rw-rw-   0        0        0     8696 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/app.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.669849 wis2downloader-0.1.0/wis2downloader/downloader/
--rw-rw-rw-   0        0        0     8790 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/downloader/__init__.py
--rw-rw-rw-   0        0        0     2298 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/log.py
--rw-rw-rw-   0        0        0      619 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.670924 wis2downloader-0.1.0/wis2downloader/queue/
--rw-rw-rw-   0        0        0     2067 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.671839 wis2downloader-0.1.0/wis2downloader/subscriber/
--rw-rw-rw-   0        0        0     6028 2024-05-14 15:11:07.000000 wis2downloader-0.1.0/wis2downloader/subscriber/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:53.672828 wis2downloader-0.1.0/wis2downloader.egg-info/
--rw-rw-rw-   0        0        0    18431 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 15:06:53.000000 wis2downloader-0.1.0/wis2downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.203640 wis2downloader-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    18387 2024-05-28 07:58:29.203640 wis2downloader-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4485 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/README.md
+-rw-rw-rw-   0        0        0      837 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:58:29.203640 wis2downloader-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.173267 wis2downloader-0.1.1/wis2downloader/
+-rw-rw-rw-   0        0        0     1020 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/__init__.py
+-rw-rw-rw-   0        0        0     8642 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/app.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.198128 wis2downloader-0.1.1/wis2downloader/downloader/
+-rw-rw-rw-   0        0        0     8529 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/downloader/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/log.py
+-rw-rw-rw-   0        0        0      602 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.198128 wis2downloader-0.1.1/wis2downloader/queue/
+-rw-rw-rw-   0        0        0     1978 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.198128 wis2downloader-0.1.1/wis2downloader/subscriber/
+-rw-rw-rw-   0        0        0     5860 2024-05-28 07:55:13.000000 wis2downloader-0.1.1/wis2downloader/subscriber/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:58:29.198128 wis2downloader-0.1.1/wis2downloader.egg-info/
+-rw-rw-rw-   0        0        0    18387 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-28 07:58:29.000000 wis2downloader-0.1.1/wis2downloader.egg-info/top_level.txt
```

### Comparing `wis2downloader-0.1.0/LICENSE` & `wis2downloader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wis2downloader-0.1.0/PKG-INFO` & `wis2downloader-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis2downloader
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package to manage subscriptions and downloads from the WIS2.0
 Author: Rory Burke
 Maintainer: Rory Burke
 Maintainer-email: "David I. Berry" <dberry@wmo.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -241,15 +241,15 @@
 
 ## Getting Started
 
 ### 1. Installation
 You can install using Pip:
 
 ```bash
-pip install https://github.com/wmo-im/wis2-downloader/archive/main.zip
+pip install wis2downloader
 ```
 
 ### 2. Configuration
 
 Create a file `config.json` in your local directory, with the following contents:
 
 ```json
```

### Comparing `wis2downloader-0.1.0/README.md` & `wis2downloader-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-# The WIS2 Downloader
-### The backend tool for subscribing to the latest data on the WIS2 network.
-
-<a href="https://github.com/wmo-im/wis2-downloader/blob/main/LICENSE" alt="License" ><img src="https://img.shields.io/badge/License-Apache_2.0-blue"></img></a>
-
-The WIS2 Downloader is a Flask-based Python application that allows you to connect to a WIS2 Global Broker, manage subscriptions to topic hierarchies, and configure their associated download directories.
-
-**Note**: This repository does *not* contain the desktop application GUI that can be used to aid maintenance of subscriptions and explore Global Discovery Catalogues. <a href="https://github.com/wmo-im/wis2-downloader-gui">The WIS2 Downloader GUI can be found here.</a>
-
-## Features
-
-- **Dynamic Subscription Management**: Quickly add or remove subscriptions ad hoc without needing to restart the service or change configuration files.
-- **Monitor Download Statistics**: Access the Prometheus metrics through the `/metrics` endpoint, ideal for <a href="https://prometheus.io/docs/visualization/grafana/">Grafana visualization</a>.
-- **Multi-Threading Support**: Configure the number of download workers for more efficient data downloading.
-
-## Demo
-![backend-demo](https://github.com/wmo-im/wis2-downloader/assets/47696929/f9eb9eb3-07bd-49df-9714-61d952000f2e)
-
-*The GET requests are demonstrated here using <a href="https://www.postman.com/">Postman</a>, but the terminal or your browser will suffice too.*
-
-## Getting Started
-
-### 1. Installation
-You can install using Pip:
-
-```bash
-pip install https://github.com/wmo-im/wis2-downloader/archive/main.zip
-```
-
-### 2. Configuration
-
-Create a file `config.json` in your local directory, with the following contents:
-
-```json
-{
-    "broker_url": "replace with url of the global broker, e.g. globalbroker.meteo.fr",
-    "broker_port": "replace with the port to use on the global broker, e.g. 443",
-    "username": "username to use on the global broker, default everyone",
-    "password": "password to use on the global broker, default everyone",
-    "protocol": "transport protocol to use, either tcp or websockets",
-    "topics": {"initial topic 1": "associated download folder", ...},
-    "download_dir": "default base download directory",
-    "flask_host": "127.0.0.1",
-    "flask_port": 8080,
-    "download_workers": 1,
-    "save_logs": false,
-    "log_dir": "default base directory for logs to be saved"
-}
-```
-
-This will be used when starting the WIS2 Downloader service.
-
-### 3. Running
-
-In your terminal, run:
-
-```
-wis2downloader --config <path to configuration file>
-```
-
-The Flask application should now be running. If you need to stop the application, you can do so in the terminal with `Ctrl+C`.
-
-## Maintaining and Monitoring Subscriptions
-
-### Adding subscriptions
-Subscriptions can be added via a GET request to the `./add` endpoint on the Flask app, with the following form:
-
-```bash
-curl http://<flask-host>:<flask-port>/add?topic=<topic-name>&target=<download-directory>
-```
-
-- `topic` specifies the topic to subscribe to. *Special characters (+, #) must be URL encoded, i.e. `+` = `%2B`, `#` = `%23`.*
-- `target` specifies the directory to save the downloads to, relative to `download_dir` from `config.json`. *If this is not provided, the directory will default to that of the topic hierarchy.*
-
-For example:
-```bash
-curl http://localhost:8080/add?topic=cache/a/wis2/%2B/data/core/weather/%23&target=example_data
-```
-
-The list of active subscriptions should be returned as a JSON object.
-
-### Deleting subscriptions
-Subscriptions are deleted similarly via a GET request to the `./delete` endpoint, with the following form:
-```bash
-curl http://<flask-host>:<flask-port>/delete?topic=<topic-name>
-```
-
-For example:
-```bash
-curl http://localhost:8080/delete?topic=cache/a/wis2/%2B/data/core/weather/%23
-```
-
-The list of active subscriptions should be returned as a JSON object.
-### Listing subscriptions
-Subscriptions are listed via a GET request to `./list`:
-
-```bash
-curl http://<flask-host>:<flask-port>/list
-```
-
-The list of active subscriptions should be returned as a JSON object.
-
-### Viewing download metrics
-Prometheus metrics for the downloader are found via a GET request to `./metrics`, e.g.:
-
-```bash
-curl http://<flask-host>:<flask-port>/metrics
-```
-
-## Bugs and Issues
-
-All bugs, enhancements and issues are managed on [GitHub](https://github.com/wmo-im/wis2-downloader/issues).
-
-## Contact
-
-* [Rory Burke](https://github.com/RoryPTB)
-* [David Berry](https://github.com/david-i-berry)
+# The WIS2 Downloader
+### The backend tool for subscribing to the latest data on the WIS2 network.
+
+<a href="https://github.com/wmo-im/wis2-downloader/blob/main/LICENSE" alt="License" ><img src="https://img.shields.io/badge/License-Apache_2.0-blue"></img></a>
+
+The WIS2 Downloader is a Flask-based Python application that allows you to connect to a WIS2 Global Broker, manage subscriptions to topic hierarchies, and configure their associated download directories.
+
+**Note**: This repository does *not* contain the desktop application GUI that can be used to aid maintenance of subscriptions and explore Global Discovery Catalogues. <a href="https://github.com/wmo-im/wis2-downloader-gui">The WIS2 Downloader GUI can be found here.</a>
+
+## Features
+
+- **Dynamic Subscription Management**: Quickly add or remove subscriptions ad hoc without needing to restart the service or change configuration files.
+- **Monitor Download Statistics**: Access the Prometheus metrics through the `/metrics` endpoint, ideal for <a href="https://prometheus.io/docs/visualization/grafana/">Grafana visualization</a>.
+- **Multi-Threading Support**: Configure the number of download workers for more efficient data downloading.
+
+## Demo
+![backend-demo](https://github.com/wmo-im/wis2-downloader/assets/47696929/f9eb9eb3-07bd-49df-9714-61d952000f2e)
+
+*The GET requests are demonstrated here using <a href="https://www.postman.com/">Postman</a>, but the terminal or your browser will suffice too.*
+
+## Getting Started
+
+### 1. Installation
+You can install using Pip:
+
+```bash
+pip install wis2downloader
+```
+
+### 2. Configuration
+
+Create a file `config.json` in your local directory, with the following contents:
+
+```json
+{
+    "broker_url": "replace with url of the global broker, e.g. globalbroker.meteo.fr",
+    "broker_port": "replace with the port to use on the global broker, e.g. 443",
+    "username": "username to use on the global broker, default everyone",
+    "password": "password to use on the global broker, default everyone",
+    "protocol": "transport protocol to use, either tcp or websockets",
+    "topics": {"initial topic 1": "associated download folder", ...},
+    "download_dir": "default base download directory",
+    "flask_host": "127.0.0.1",
+    "flask_port": 8080,
+    "download_workers": 1,
+    "save_logs": false,
+    "log_dir": "default base directory for logs to be saved"
+}
+```
+
+This will be used when starting the WIS2 Downloader service.
+
+### 3. Running
+
+In your terminal, run:
+
+```
+wis2downloader --config <path to configuration file>
+```
+
+The Flask application should now be running. If you need to stop the application, you can do so in the terminal with `Ctrl+C`.
+
+## Maintaining and Monitoring Subscriptions
+
+### Adding subscriptions
+Subscriptions can be added via a GET request to the `./add` endpoint on the Flask app, with the following form:
+
+```bash
+curl http://<flask-host>:<flask-port>/add?topic=<topic-name>&target=<download-directory>
+```
+
+- `topic` specifies the topic to subscribe to. *Special characters (+, #) must be URL encoded, i.e. `+` = `%2B`, `#` = `%23`.*
+- `target` specifies the directory to save the downloads to, relative to `download_dir` from `config.json`. *If this is not provided, the directory will default to that of the topic hierarchy.*
+
+For example:
+```bash
+curl http://localhost:8080/add?topic=cache/a/wis2/%2B/data/core/weather/%23&target=example_data
+```
+
+The list of active subscriptions should be returned as a JSON object.
+
+### Deleting subscriptions
+Subscriptions are deleted similarly via a GET request to the `./delete` endpoint, with the following form:
+```bash
+curl http://<flask-host>:<flask-port>/delete?topic=<topic-name>
+```
+
+For example:
+```bash
+curl http://localhost:8080/delete?topic=cache/a/wis2/%2B/data/core/weather/%23
+```
+
+The list of active subscriptions should be returned as a JSON object.
+### Listing subscriptions
+Subscriptions are listed via a GET request to `./list`:
+
+```bash
+curl http://<flask-host>:<flask-port>/list
+```
+
+The list of active subscriptions should be returned as a JSON object.
+
+### Viewing download metrics
+Prometheus metrics for the downloader are found via a GET request to `./metrics`, e.g.:
+
+```bash
+curl http://<flask-host>:<flask-port>/metrics
+```
+
+## Bugs and Issues
+
+All bugs, enhancements and issues are managed on [GitHub](https://github.com/wmo-im/wis2-downloader/issues).
+
+## Contact
+
+* [Rory Burke](https://github.com/RoryPTB)
+* [David Berry](https://github.com/david-i-berry)
```

#### html2text {}

```diff
@@ -10,23 +10,22 @@
 service or change configuration files. - **Monitor Download Statistics**:
 Access the Prometheus metrics through the `/metrics` endpoint, ideal for
 _G_r_a_f_a_n_a_ _v_i_s_u_a_l_i_z_a_t_i_o_n. - **Multi-Threading Support**: Configure the number of
 download workers for more efficient data downloading. ## Demo ![backend-demo]
 (https://github.com/wmo-im/wis2-downloader/assets/47696929/f9eb9eb3-07bd-49df-
 9714-61d952000f2e) *The GET requests are demonstrated here using _P_o_s_t_m_a_n, but
 the terminal or your browser will suffice too.* ## Getting Started ### 1.
-Installation You can install using Pip: ```bash pip install https://github.com/
-wmo-im/wis2-downloader/archive/main.zip ``` ### 2. Configuration Create a file
-`config.json` in your local directory, with the following contents: ```json
-{ "broker_url": "replace with url of the global broker, e.g.
-globalbroker.meteo.fr", "broker_port": "replace with the port to use on the
-global broker, e.g. 443", "username": "username to use on the global broker,
-default everyone", "password": "password to use on the global broker, default
-everyone", "protocol": "transport protocol to use, either tcp or websockets",
-"topics": {"initial topic 1": "associated download folder", ...},
+Installation You can install using Pip: ```bash pip install wis2downloader ```
+### 2. Configuration Create a file `config.json` in your local directory, with
+the following contents: ```json { "broker_url": "replace with url of the global
+broker, e.g. globalbroker.meteo.fr", "broker_port": "replace with the port to
+use on the global broker, e.g. 443", "username": "username to use on the global
+broker, default everyone", "password": "password to use on the global broker,
+default everyone", "protocol": "transport protocol to use, either tcp or
+websockets", "topics": {"initial topic 1": "associated download folder", ...},
 "download_dir": "default base download directory", "flask_host": "127.0.0.1",
 "flask_port": 8080, "download_workers": 1, "save_logs": false, "log_dir":
 "default base directory for logs to be saved" } ``` This will be used when
 starting the WIS2 Downloader service. ### 3. Running In your terminal, run: ```
 wis2downloader --config ``` The Flask application should now be running. If you
 need to stop the application, you can do so in the terminal with `Ctrl+C`. ##
 Maintaining and Monitoring Subscriptions ### Adding subscriptions Subscriptions
```

### Comparing `wis2downloader-0.1.0/wis2downloader/__init__.py` & `wis2downloader-0.1.1/wis2downloader/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-###############################################################################
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-from threading import Event
-
-__version__ = '0.1.0'
-
-shutdown = Event()
+###############################################################################
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+from threading import Event
+
+__version__ = '0.1.1'
+
+shutdown = Event()
```

### Comparing `wis2downloader-0.1.0/wis2downloader/downloader/__init__.py` & `wis2downloader-0.1.1/wis2downloader/downloader/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-from abc import ABC, abstractmethod
-import urllib3
-from urllib.parse import urlsplit
-import hashlib
-import base64
-import os
-from datetime import datetime as dt
-from pathlib import Path
-import enum
-
-from wis2downloader import shutdown
-from wis2downloader.log import LOGGER
-from wis2downloader.queue import BaseQueue
-from wis2downloader.metrics import (DOWNLOADED_BYTES, DOWNLOADED_FILES,
-                                    FAILED_DOWNLOADS)
-
-
-class BaseDownloader(ABC):
-
-    @abstractmethod
-    def start(self):
-        """Start the download worker to
-        process messages from the queue indefinitely"""
-        pass
-
-    @abstractmethod
-    def process_job(self, job):
-        """Process a single job from the queue"""
-        pass
-
-    @abstractmethod
-    def get_topic_and_centre(self, job):
-        """Extract the topic and centre id from the job"""
-        pass
-
-    @abstractmethod
-    def get_hash_info(self, job):
-        """Extract the hash value and function from the job
-        to be used for verification later"""
-        pass
-
-    @abstractmethod
-    def get_links(self, job):
-        """Extract the download url, update status, and
-        file type from the job links"""
-        pass
-
-    @abstractmethod
-    def extract_filename(self, _url):
-        """Extract the filename and extension from the download link"""
-        pass
-
-    @abstractmethod
-    def validate_data(self, data, expected_hash, hash_function, expected_size):
-        """Validate the hash and size of the downloaded data against
-        the expected values"""
-        pass
-
-    @abstractmethod
-    def save_file(self, data, target, filename, filesize, download_start):
-        """Save the downloaded data to disk"""
-
-
-def get_todays_date():
-    """
-    Returns today's date in the format yyyy/mm/dd.
-    """
-    today = dt.now()
-    yyyy = f"{today.year:04}"
-    mm = f"{today.month:02}"
-    dd = f"{today.day:02}"
-    return yyyy, mm, dd
-
-
-class VerificationMethods(enum.Enum):
-    sha256 = 'sha256'
-    sha384 = 'sha384'
-    sha512 = 'sha512'
-    sha3_256 = 'sha3_256'
-    sha3_384 = 'sha3_384'
-    sha3_512 = 'sha3_512'
-
-
-class DownloadWorker(BaseDownloader):
-    def __init__(self, queue: BaseQueue, basepath: str = "."):
-        self.http = urllib3.PoolManager()
-        self.queue = queue
-        self.basepath = Path(basepath)
-
-    def start(self) -> None:
-        LOGGER.info("Starting download worker")
-        while not shutdown.is_set():
-            # First get the job from the queue
-            job = self.queue.dequeue()
-            if job.get('shutdown', None):
-                break
-
-            self.process_job(job)
-
-            self.queue.task_done()
-
-    def process_job(self, job) -> None:
-        yyyy, mm, dd = get_todays_date()
-        output_dir = self.basepath / yyyy / mm / dd
-
-        # Add target to output directory
-        output_dir = output_dir / job.get("target", ".")
-
-        # Get information about the job for verification later
-        expected_hash, hash_function = self.get_hash_info(job)
-        expected_size = job.get('payload', {}).get('content', {}).get('size')
-
-        # Get the download url, update status, and file type from the job links
-        _url, update, file_type = self.get_links(job)
-
-        if _url is None:
-            LOGGER.info(f"No download link found in job {job}")
-            return
-
-        # Extract the filename and filename ending from the download link
-        filename, filename_ext = self.extract_filename(_url)
-
-        # If the file type is not in the links, use the filename extension
-        if file_type is None:
-            file_type = filename_ext
-
-        target = output_dir / filename
-        # Create parent dir if it doesn't exist
-        target.parent.mkdir(parents=True, exist_ok=True)
-
-        # Only download if file doesn't exist or is an update
-        is_duplicate = target.is_file() and not update
-        if is_duplicate:
-            LOGGER.info(f"Skipping download of {filename}, already exists")
-            return
-
-        # Get information needed for download metric labels
-        topic, centre_id = self.get_topic_and_centre(job)
-
-        # Standardise the file type label, defaulting to 'other'
-        all_type_labels = ['bufr', 'grib', 'json', 'xml', 'png']
-        file_type_label = 'other'
-
-        for label in all_type_labels:
-            if label in file_type:
-                file_type_label = label
-                break
-
-        # Start timer of download time to be logged later
-        download_start = dt.now()
-
-        # Download the file
-        response = None
-        try:
-            response = self.http.request('GET', _url)
-            # Get the filesize in KB
-            filesize = len(response.data)
-        except Exception as e:
-            LOGGER.error(f"Error downloading {_url}")
-            LOGGER.error(e)
-            # Increment failed download counter
-            FAILED_DOWNLOADS.labels(topic=topic, centre_id=centre_id).inc(1)
-            return
-
-        if response is None:
-            return
-
-        # Use the hash function to determine whether to save the data
-        save_data = self.validate_data(
-            response.data, expected_hash, hash_function, expected_size)
-
-        if not save_data:
-            LOGGER.warning(f"Download {filename} failed verification, discarding")  # noqa
-            # Increment failed download counter
-            FAILED_DOWNLOADS.labels(topic=topic, centre_id=centre_id).inc(1)
-            return
-
-        # Now save
-        self.save_file(response.data, target, filename,
-                       filesize, download_start)
-
-        # Increment metrics
-        DOWNLOADED_BYTES.labels(
-            topic=topic, centre_id=centre_id,
-            file_type=file_type_label).inc(filesize)
-        DOWNLOADED_FILES.labels(
-            topic=topic, centre_id=centre_id,
-            file_type=file_type_label).inc(1)
-
-    def get_topic_and_centre(self, job) -> tuple:
-        topic = job.get('topic')
-        return topic, topic.split('/')[3]
-
-    def get_hash_info(self, job):
-        expected_hash = job.get('payload', {}).get(
-            'properties', {}).get('integrity', {}).get('hash')
-        hash_method = job.get('payload', {}).get(
-            'properties', {}).get('integrity', {}).get('method')
-
-        hash_function = None
-
-        # Check if hash method is known using our enumumeration of hash methods
-        if hash_method in VerificationMethods._member_names_:
-            method = VerificationMethods[hash_method].value
-            hash_function = hashlib.new(method)
-
-        return expected_hash, hash_function
-
-    def get_links(self, job) -> tuple:
-        links = job.get('payload', {}).get('links', [])
-        _url = None
-        update = False
-        file_type = None
-        for link in links:
-            if link.get('rel') == 'update':
-                _url = link.get('href')
-                update = True
-                break
-            elif link.get('rel') == 'canonical':
-                _url = link.get('href')
-                app_type = link.get('type')
-                if app_type:
-                    # Remove '.../' prefix and, if present, 'x-' prefix
-                    file_type = app_type.split('/')[1].replace('x-', '')
-                break
-
-        return _url, update, file_type
-
-    def extract_filename(self, _url) -> tuple:
-        path = urlsplit(_url).path
-        filename = os.path.basename(path)
-
-        filename_ext = os.path.splitext(filename)[1][1:]
-
-        return filename, filename_ext
-
-    def validate_data(self, data, expected_hash,
-                      hash_function, expected_size) -> bool:
-        if None in (expected_hash, hash_function,
-                    hash_function):
-            return True
-
-        hash_value = hash_function(data).digest()
-        hash_value = base64.b64encode(hash_value).decode()
-        if (hash_value != expected_hash) or (len(data) != expected_size):
-            return False
-
-        return True
-
-    def save_file(self, data, target, filename, filesize,
-                  download_start) -> None:
-        try:
-            target.write_bytes(data)
-            download_end = dt.now()
-            download_time = download_end - download_start
-            download_seconds = round(download_time.total_seconds(), 2)
-            LOGGER.info(
-                f"Downloaded {filename} of size {filesize} bytes in {download_seconds} seconds")  # noqa
-        except Exception as e:
-            LOGGER.error(f"Error saving to disk: {target}")
-            LOGGER.error(e)
+from abc import ABC, abstractmethod
+import urllib3
+from urllib.parse import urlsplit
+import hashlib
+import base64
+import os
+from datetime import datetime as dt
+from pathlib import Path
+import enum
+
+from wis2downloader import shutdown
+from wis2downloader.log import LOGGER
+from wis2downloader.queue import BaseQueue
+from wis2downloader.metrics import (DOWNLOADED_BYTES, DOWNLOADED_FILES,
+                                    FAILED_DOWNLOADS)
+
+
+class BaseDownloader(ABC):
+
+    @abstractmethod
+    def start(self):
+        """Start the download worker to
+        process messages from the queue indefinitely"""
+        pass
+
+    @abstractmethod
+    def process_job(self, job):
+        """Process a single job from the queue"""
+        pass
+
+    @abstractmethod
+    def get_topic_and_centre(self, job):
+        """Extract the topic and centre id from the job"""
+        pass
+
+    @abstractmethod
+    def get_hash_info(self, job):
+        """Extract the hash value and function from the job
+        to be used for verification later"""
+        pass
+
+    @abstractmethod
+    def get_links(self, job):
+        """Extract the download url, update status, and
+        file type from the job links"""
+        pass
+
+    @abstractmethod
+    def extract_filename(self, _url):
+        """Extract the filename and extension from the download link"""
+        pass
+
+    @abstractmethod
+    def validate_data(self, data, expected_hash, hash_function, expected_size):
+        """Validate the hash and size of the downloaded data against
+        the expected values"""
+        pass
+
+    @abstractmethod
+    def save_file(self, data, target, filename, filesize, download_start):
+        """Save the downloaded data to disk"""
+
+
+def get_todays_date():
+    """
+    Returns today's date in the format yyyy/mm/dd.
+    """
+    today = dt.now()
+    yyyy = f"{today.year:04}"
+    mm = f"{today.month:02}"
+    dd = f"{today.day:02}"
+    return yyyy, mm, dd
+
+
+class VerificationMethods(enum.Enum):
+    sha256 = 'sha256'
+    sha384 = 'sha384'
+    sha512 = 'sha512'
+    sha3_256 = 'sha3_256'
+    sha3_384 = 'sha3_384'
+    sha3_512 = 'sha3_512'
+
+
+class DownloadWorker(BaseDownloader):
+    def __init__(self, queue: BaseQueue, basepath: str = "."):
+        self.http = urllib3.PoolManager()
+        self.queue = queue
+        self.basepath = Path(basepath)
+
+    def start(self) -> None:
+        LOGGER.info("Starting download worker")
+        while not shutdown.is_set():
+            # First get the job from the queue
+            job = self.queue.dequeue()
+            if job.get('shutdown', None):
+                break
+
+            self.process_job(job)
+
+            self.queue.task_done()
+
+    def process_job(self, job) -> None:
+        yyyy, mm, dd = get_todays_date()
+        output_dir = self.basepath / yyyy / mm / dd
+
+        # Add target to output directory
+        output_dir = output_dir / job.get("target", ".")
+
+        # Get information about the job for verification later
+        expected_hash, hash_function = self.get_hash_info(job)
+        expected_size = job.get('payload', {}).get('content', {}).get('size')
+
+        # Get the download url, update status, and file type from the job links
+        _url, update, file_type = self.get_links(job)
+
+        if _url is None:
+            LOGGER.info(f"No download link found in job {job}")
+            return
+
+        # Extract the filename and filename ending from the download link
+        filename, filename_ext = self.extract_filename(_url)
+
+        # If the file type is not in the links, use the filename extension
+        if file_type is None:
+            file_type = filename_ext
+
+        target = output_dir / filename
+        # Create parent dir if it doesn't exist
+        target.parent.mkdir(parents=True, exist_ok=True)
+
+        # Only download if file doesn't exist or is an update
+        is_duplicate = target.is_file() and not update
+        if is_duplicate:
+            LOGGER.info(f"Skipping download of {filename}, already exists")
+            return
+
+        # Get information needed for download metric labels
+        topic, centre_id = self.get_topic_and_centre(job)
+
+        # Standardise the file type label, defaulting to 'other'
+        all_type_labels = ['bufr', 'grib', 'json', 'xml', 'png']
+        file_type_label = 'other'
+
+        for label in all_type_labels:
+            if label in file_type:
+                file_type_label = label
+                break
+
+        # Start timer of download time to be logged later
+        download_start = dt.now()
+
+        # Download the file
+        response = None
+        try:
+            response = self.http.request('GET', _url)
+            # Get the filesize in KB
+            filesize = len(response.data)
+        except Exception as e:
+            LOGGER.error(f"Error downloading {_url}")
+            LOGGER.error(e)
+            # Increment failed download counter
+            FAILED_DOWNLOADS.labels(topic=topic, centre_id=centre_id).inc(1)
+            return
+
+        if response is None:
+            return
+
+        # Use the hash function to determine whether to save the data
+        save_data = self.validate_data(
+            response.data, expected_hash, hash_function, expected_size)
+
+        if not save_data:
+            LOGGER.warning(f"Download {filename} failed verification, discarding")  # noqa
+            # Increment failed download counter
+            FAILED_DOWNLOADS.labels(topic=topic, centre_id=centre_id).inc(1)
+            return
+
+        # Now save
+        self.save_file(response.data, target, filename,
+                       filesize, download_start)
+
+        # Increment metrics
+        DOWNLOADED_BYTES.labels(
+            topic=topic, centre_id=centre_id,
+            file_type=file_type_label).inc(filesize)
+        DOWNLOADED_FILES.labels(
+            topic=topic, centre_id=centre_id,
+            file_type=file_type_label).inc(1)
+
+    def get_topic_and_centre(self, job) -> tuple:
+        topic = job.get('topic')
+        return topic, topic.split('/')[3]
+
+    def get_hash_info(self, job):
+        expected_hash = job.get('payload', {}).get(
+            'properties', {}).get('integrity', {}).get('hash')
+        hash_method = job.get('payload', {}).get(
+            'properties', {}).get('integrity', {}).get('method')
+
+        hash_function = None
+
+        # Check if hash method is known using our enumumeration of hash methods
+        if hash_method in VerificationMethods._member_names_:
+            method = VerificationMethods[hash_method].value
+            hash_function = hashlib.new(method)
+
+        return expected_hash, hash_function
+
+    def get_links(self, job) -> tuple:
+        links = job.get('payload', {}).get('links', [])
+        _url = None
+        update = False
+        file_type = None
+        for link in links:
+            if link.get('rel') == 'update':
+                _url = link.get('href')
+                update = True
+                break
+            elif link.get('rel') == 'canonical':
+                _url = link.get('href')
+                app_type = link.get('type')
+                if app_type:
+                    # Remove '.../' prefix and, if present, 'x-' prefix
+                    file_type = app_type.split('/')[1].replace('x-', '')
+                break
+
+        return _url, update, file_type
+
+    def extract_filename(self, _url) -> tuple:
+        path = urlsplit(_url).path
+        filename = os.path.basename(path)
+
+        filename_ext = os.path.splitext(filename)[1][1:]
+
+        return filename, filename_ext
+
+    def validate_data(self, data, expected_hash,
+                      hash_function, expected_size) -> bool:
+        if None in (expected_hash, hash_function,
+                    hash_function):
+            return True
+
+        hash_value = hash_function(data).digest()
+        hash_value = base64.b64encode(hash_value).decode()
+        if (hash_value != expected_hash) or (len(data) != expected_size):
+            return False
+
+        return True
+
+    def save_file(self, data, target, filename, filesize,
+                  download_start) -> None:
+        try:
+            target.write_bytes(data)
+            download_end = dt.now()
+            download_time = download_end - download_start
+            download_seconds = round(download_time.total_seconds(), 2)
+            LOGGER.info(
+                f"Downloaded {filename} of size {filesize} bytes in {download_seconds} seconds")  # noqa
+        except Exception as e:
+            LOGGER.error(f"Error saving to disk: {target}")
+            LOGGER.error(e)
```

### Comparing `wis2downloader-0.1.0/wis2downloader/log.py` & `wis2downloader-0.1.1/wis2downloader/log.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-###############################################################################
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-# Original source:
-# https://github.com/wmo-im/wis2box/blob/main/wis2box-management/wis2box/log.py
-###############################################################################
-
-"""Logging system"""
-
-import logging
-import sys
-
-LOGGER = logging.getLogger(__name__)
-
-
-def setup_logger(loglevel: str = 'ERROR', logfile: str = 'stdout') -> None:
-    """
-    Setup logger
-
-    :param loglevel: `str`, logging level
-    :param logfile: `str`, logging output file
-
-    :returns: `None` (creates logging instance)
-    """
-
-    log_format = \
-        '[%(asctime)s] %(levelname)s - %(message)s'
-    date_format = '%Y-%m-%dT%H:%M:%SZ'
-
-    loglevels = {
-        'CRITICAL': logging.CRITICAL,
-        'ERROR': logging.ERROR,
-        'WARNING': logging.WARNING,
-        'INFO': logging.INFO,
-        'DEBUG': logging.DEBUG,
-        'NOTSET': logging.NOTSET,
-    }
-
-    loglevel = loglevels[loglevel]
-
-    if logfile is not None:
-        if logfile == 'stdout':
-            logging.basicConfig(level=loglevel, datefmt=date_format,
-                                format=log_format, stream=sys.stdout)
-        else:
-            logging.basicConfig(level=loglevel, datefmt=date_format,
-                                format=log_format, filename=logfile)
-
-    LOGGER.debug('Logging initialized')
+###############################################################################
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+# Original source:
+# https://github.com/wmo-im/wis2box/blob/main/wis2box-management/wis2box/log.py
+###############################################################################
+
+"""Logging system"""
+
+import logging
+import sys
+
+LOGGER = logging.getLogger(__name__)
+
+
+def setup_logger(loglevel: str = 'ERROR', logfile: str = 'stdout') -> None:
+    """
+    Setup logger
+
+    :param loglevel: `str`, logging level
+    :param logfile: `str`, logging output file
+
+    :returns: `None` (creates logging instance)
+    """
+
+    log_format = \
+        '[%(asctime)s] %(levelname)s - %(message)s'
+    date_format = '%Y-%m-%dT%H:%M:%SZ'
+
+    loglevels = {
+        'CRITICAL': logging.CRITICAL,
+        'ERROR': logging.ERROR,
+        'WARNING': logging.WARNING,
+        'INFO': logging.INFO,
+        'DEBUG': logging.DEBUG,
+        'NOTSET': logging.NOTSET,
+    }
+
+    loglevel = loglevels[loglevel]
+
+    if logfile is not None:
+        if logfile == 'stdout':
+            logging.basicConfig(level=loglevel, datefmt=date_format,
+                                format=log_format, stream=sys.stdout)
+        else:
+            logging.basicConfig(level=loglevel, datefmt=date_format,
+                                format=log_format, filename=logfile)
+
+    LOGGER.debug('Logging initialized')
```

### Comparing `wis2downloader-0.1.0/wis2downloader/metrics.py` & `wis2downloader-0.1.1/wis2downloader/metrics.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from prometheus_client import Counter, Gauge
-
-
-QUEUE_SIZE = Gauge(
-    'queue_size', 'Current size of the job queue')
-DOWNLOADED_BYTES = Counter(
-    'downloaded_bytes', 'Total number of downloaded bytes',
-    ['topic', 'centre_id', 'file_type'])
-DOWNLOADED_FILES = Counter(
-    'downloaded_files', 'Total number of downloaded files',
-    ['topic', 'centre_id', 'file_type'])
-FAILED_DOWNLOADS = Counter(
-    'failed_downloads', 'Total number of failed downloads',
-    ['topic', 'centre_id'])
-TOPIC_STATUS = Gauge(
-    'topic_subscription_status', 'Subscription status of a given topic',
-    ['topic'])
+from prometheus_client import Counter, Gauge
+
+
+QUEUE_SIZE = Gauge(
+    'queue_size', 'Current size of the job queue')
+DOWNLOADED_BYTES = Counter(
+    'downloaded_bytes', 'Total number of downloaded bytes',
+    ['topic', 'centre_id', 'file_type'])
+DOWNLOADED_FILES = Counter(
+    'downloaded_files', 'Total number of downloaded files',
+    ['topic', 'centre_id', 'file_type'])
+FAILED_DOWNLOADS = Counter(
+    'failed_downloads', 'Total number of failed downloads',
+    ['topic', 'centre_id'])
+TOPIC_STATUS = Gauge(
+    'topic_subscription_status', 'Subscription status of a given topic',
+    ['topic'])
```

### Comparing `wis2downloader-0.1.0/wis2downloader/subscriber/__init__.py` & `wis2downloader-0.1.1/wis2downloader/subscriber/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-from abc import ABC, abstractmethod
-from fnmatch import fnmatch
-import json
-from pathlib import Path
-import ssl
-
-import paho.mqtt.client as mqtt
-
-from wis2downloader import shutdown
-from wis2downloader.log import LOGGER
-from wis2downloader.queue import BaseQueue
-from wis2downloader.metrics import TOPIC_STATUS
-
-
-class BaseSubscriber(ABC):
-
-    @abstractmethod
-    def _on_connect(self, client, userdata, flags, rc):
-        """Method to handle actions to take on connection to broker"""
-        pass
-
-    @abstractmethod
-    def _on_disconnect(self, client, userdata, rc):
-        """Method to handle actions to take when a connection is lost"""
-        pass
-
-    @abstractmethod
-    def _on_message(self, client, userdata, msg):
-        """Method to handle actions to take when a message is received"""
-        pass
-
-    @abstractmethod
-    def _on_subscribe(self, client, userdata, mid, granted_qos):
-        """Method to handle actions to take when a subscription is made"""
-        pass
-
-    @abstractmethod
-    def add_subscription(self, topic: str, save_path: str):
-        """Method to add subscription to active subscriptions"""
-        pass
-
-    @abstractmethod
-    def delete_subscription(self, topic: str):
-        """Method to remove subscription from active subscriptions"""
-        pass
-
-    @abstractmethod
-    def list_subscriptions(self) -> list:
-        """Method to return list of active subscriptions"""
-        pass
-
-    @abstractmethod
-    def start(self):
-        """Method to start subscriber, e.g. loop_forever in paho-mqtt"""
-        pass
-
-    @abstractmethod
-    def stop(self):
-        """Method to stop subscriber, e.g. disconnect in paho-mqtt"""
-        pass
-
-
-class MQTTSubscriber(BaseSubscriber):
-    def __init__(self, broker: str = "globalbroker.meteo.fr", port: int = 443, uid: str = "everyone", pwd: str = "everyone", protocol: str = "websockets", _queue: BaseQueue = None):
-
-        LOGGER.debug("Initializing MQTT subscriber")
-
-        self.client = mqtt.Client(
-            mqtt.CallbackAPIVersion.VERSION2, transport=protocol)
-        self.client.tls_set(ca_certs=None, certfile=None, keyfile=None,
-                            cert_reqs=ssl.CERT_REQUIRED,
-                            tls_version=ssl.PROTOCOL_TLS,
-                            ciphers=None)
-        self.client.username_pw_set(uid, pwd)
-        self.client.on_connect = self._on_connect
-        self.client.on_disconnect = self._on_disconnect
-        self.client.on_message = self._on_message
-        self.client.on_subscribe = self._on_subscribe
-
-        self.queue = _queue
-        self.active_subscriptions = {}
-
-        # Connect to the broker
-        LOGGER.info("Connecting...")
-        LOGGER.info(f"Host: {broker}, port: {port}")
-        self.client.connect(host=broker, port=port)
-
-    def _on_connect(self, client, userdata, flags, reason_code, properties):
-        if reason_code == 0:
-            LOGGER.info("Connected successfully")
-        elif reason_code > 0:
-            LOGGER.error(f"Connection failed with error code {reason_code}")
-
-    def _on_disconnect(self, client, userdata, disconnect_flags, reason_code, properties):
-        if reason_code == 0:
-            LOGGER.info("Disconnected successfully")
-        elif reason_code > 0:
-            LOGGER.error(f"Disconnection failed with error code {reason_code}")
-
-    def _on_message(self, client, userdata, msg):
-        # first check shutdown is not set
-        if shutdown.is_set():
-            self.client.disconnect()
-        LOGGER.info(f"Message received under topic {msg.topic}")
-        target = self.active_subscriptions.get(msg.topic, {}).get('target')
-        # if a wild card is used in the subs target may not match
-        if target is None:
-            for key, value in self.active_subscriptions.items():
-                if fnmatch(msg.topic, value['pattern']):
-                    target = value['target']
-                    break
-
-        if target == "$TOPIC":
-            target = msg.topic
-
-        if "/" in target:
-            subdirs = target.split("/")
-            target = str(Path(*subdirs))
-
-        if "\\" in target:
-            subdirs = target.split("\\")
-            target = str(Path(*subdirs))
-
-        job = {
-            'topic': msg.topic,
-            'payload': json.loads(msg.payload),
-            'target': target
-        }
-        self.queue.enqueue(job)
-
-    def _on_subscribe(self, client, userdata, mid, reason_codes, properties):
-        for sub_result in reason_codes:
-            if sub_result in [0, 1, 2]:
-                LOGGER.info("Subscription to topic successful")
-            elif sub_result >= 128:
-                LOGGER.error(
-                    f"Subscription to topic failed with error code {sub_result}")  # noqa
-
-    def add_subscription(self, topic: str, save_path: str = "."):
-        self.client.subscribe(topic)
-        self.active_subscriptions[topic] = {
-            'target': save_path,
-            'pattern': topic.replace("+", "*").replace("#", "*")
-        }
-        LOGGER.info(f"Subscribing to {topic}")
-        # Set topic status to subscribed
-        TOPIC_STATUS.labels(topic=topic).set(1)
-        return self.active_subscriptions
-
-    def delete_subscription(self, topic: str):
-        if topic in self.active_subscriptions:
-            self.client.unsubscribe(topic)
-            del self.active_subscriptions[topic]
-            LOGGER.info(f"Unsubscribing from {topic}")
-            # Set topic status to unsubscribed
-            TOPIC_STATUS.labels(topic=topic).set(0)
-        else:
-            LOGGER.info(f"Topic {topic} not found in active subscriptions")
-        return self.active_subscriptions
-
-    def list_subscriptions(self) -> dict:
-        return self.active_subscriptions
-
-    def start(self):
-        self.client.loop_forever()
-
-    def stop(self):
-        self.client.disconnect()
+from abc import ABC, abstractmethod
+from fnmatch import fnmatch
+import json
+from pathlib import Path
+import ssl
+
+import paho.mqtt.client as mqtt
+
+from wis2downloader import shutdown
+from wis2downloader.log import LOGGER
+from wis2downloader.queue import BaseQueue
+from wis2downloader.metrics import TOPIC_STATUS
+
+
+class BaseSubscriber(ABC):
+
+    @abstractmethod
+    def _on_connect(self, client, userdata, flags, rc):
+        """Method to handle actions to take on connection to broker"""
+        pass
+
+    @abstractmethod
+    def _on_disconnect(self, client, userdata, rc):
+        """Method to handle actions to take when a connection is lost"""
+        pass
+
+    @abstractmethod
+    def _on_message(self, client, userdata, msg):
+        """Method to handle actions to take when a message is received"""
+        pass
+
+    @abstractmethod
+    def _on_subscribe(self, client, userdata, mid, granted_qos):
+        """Method to handle actions to take when a subscription is made"""
+        pass
+
+    @abstractmethod
+    def add_subscription(self, topic: str, save_path: str):
+        """Method to add subscription to active subscriptions"""
+        pass
+
+    @abstractmethod
+    def delete_subscription(self, topic: str):
+        """Method to remove subscription from active subscriptions"""
+        pass
+
+    @abstractmethod
+    def list_subscriptions(self) -> list:
+        """Method to return list of active subscriptions"""
+        pass
+
+    @abstractmethod
+    def start(self):
+        """Method to start subscriber, e.g. loop_forever in paho-mqtt"""
+        pass
+
+    @abstractmethod
+    def stop(self):
+        """Method to stop subscriber, e.g. disconnect in paho-mqtt"""
+        pass
+
+
+class MQTTSubscriber(BaseSubscriber):
+    def __init__(self, broker: str = "globalbroker.meteo.fr", port: int = 443, uid: str = "everyone", pwd: str = "everyone", protocol: str = "websockets", _queue: BaseQueue = None):
+
+        LOGGER.debug("Initializing MQTT subscriber")
+
+        self.client = mqtt.Client(
+            mqtt.CallbackAPIVersion.VERSION2, transport=protocol)
+        self.client.tls_set(ca_certs=None, certfile=None, keyfile=None,
+                            cert_reqs=ssl.CERT_REQUIRED,
+                            tls_version=ssl.PROTOCOL_TLS,
+                            ciphers=None)
+        self.client.username_pw_set(uid, pwd)
+        self.client.on_connect = self._on_connect
+        self.client.on_disconnect = self._on_disconnect
+        self.client.on_message = self._on_message
+        self.client.on_subscribe = self._on_subscribe
+
+        self.queue = _queue
+        self.active_subscriptions = {}
+
+        # Connect to the broker
+        LOGGER.info("Connecting...")
+        LOGGER.info(f"Host: {broker}, port: {port}")
+        self.client.connect(host=broker, port=port)
+
+    def _on_connect(self, client, userdata, flags, reason_code, properties):
+        if reason_code == 0:
+            LOGGER.info("Connected successfully")
+        elif reason_code > 0:
+            LOGGER.error(f"Connection failed with error code {reason_code}")
+
+    def _on_disconnect(self, client, userdata, disconnect_flags, reason_code, properties):
+        if reason_code == 0:
+            LOGGER.info("Disconnected successfully")
+        elif reason_code > 0:
+            LOGGER.error(f"Disconnection failed with error code {reason_code}")
+
+    def _on_message(self, client, userdata, msg):
+        # first check shutdown is not set
+        if shutdown.is_set():
+            self.client.disconnect()
+        LOGGER.info(f"Message received under topic {msg.topic}")
+        target = self.active_subscriptions.get(msg.topic, {}).get('target')
+        # if a wild card is used in the subs target may not match
+        if target is None:
+            for key, value in self.active_subscriptions.items():
+                if fnmatch(msg.topic, value['pattern']):
+                    target = value['target']
+                    break
+
+        if target == "$TOPIC":
+            target = msg.topic
+
+        if "/" in target:
+            subdirs = target.split("/")
+            target = str(Path(*subdirs))
+
+        if "\\" in target:
+            subdirs = target.split("\\")
+            target = str(Path(*subdirs))
+
+        job = {
+            'topic': msg.topic,
+            'payload': json.loads(msg.payload),
+            'target': target
+        }
+        self.queue.enqueue(job)
+
+    def _on_subscribe(self, client, userdata, mid, reason_codes, properties):
+        for sub_result in reason_codes:
+            if sub_result in [0, 1, 2]:
+                LOGGER.info("Subscription to topic successful")
+            elif sub_result >= 128:
+                LOGGER.error(
+                    f"Subscription to topic failed with error code {sub_result}")  # noqa
+
+    def add_subscription(self, topic: str, save_path: str = "."):
+        self.client.subscribe(topic)
+        self.active_subscriptions[topic] = {
+            'target': save_path,
+            'pattern': topic.replace("+", "*").replace("#", "*")
+        }
+        LOGGER.info(f"Subscribing to {topic}")
+        # Set topic status to subscribed
+        TOPIC_STATUS.labels(topic=topic).set(1)
+        return self.active_subscriptions
+
+    def delete_subscription(self, topic: str):
+        if topic in self.active_subscriptions:
+            self.client.unsubscribe(topic)
+            del self.active_subscriptions[topic]
+            LOGGER.info(f"Unsubscribing from {topic}")
+            # Set topic status to unsubscribed
+            TOPIC_STATUS.labels(topic=topic).set(0)
+        else:
+            LOGGER.info(f"Topic {topic} not found in active subscriptions")
+        return self.active_subscriptions
+
+    def list_subscriptions(self) -> dict:
+        return self.active_subscriptions
+
+    def start(self):
+        self.client.loop_forever()
+
+    def stop(self):
+        self.client.disconnect()
```

### Comparing `wis2downloader-0.1.0/wis2downloader.egg-info/PKG-INFO` & `wis2downloader-0.1.1/wis2downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis2downloader
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package to manage subscriptions and downloads from the WIS2.0
 Author: Rory Burke
 Maintainer: Rory Burke
 Maintainer-email: "David I. Berry" <dberry@wmo.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -241,15 +241,15 @@
 
 ## Getting Started
 
 ### 1. Installation
 You can install using Pip:
 
 ```bash
-pip install https://github.com/wmo-im/wis2-downloader/archive/main.zip
+pip install wis2downloader
 ```
 
 ### 2. Configuration
 
 Create a file `config.json` in your local directory, with the following contents:
 
 ```json
```

