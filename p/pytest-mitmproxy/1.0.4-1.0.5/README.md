# Comparing `tmp/pytest-mitmproxy-1.0.4.tar.gz` & `tmp/pytest_mitmproxy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mitmproxy-1.0.4.tar", last modified: Thu Mar  7 03:35:00 2024, max compression
+gzip compressed data, was "pytest_mitmproxy-1.0.5.tar", last modified: Tue May 28 09:50:03 2024, max compression
```

## Comparing `pytest-mitmproxy-1.0.4.tar` & `pytest_mitmproxy-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 03:35:00.824311 pytest-mitmproxy-1.0.4/
--rw-rw-rw-   0        0        0      343 2024-03-07 03:35:00.824311 pytest-mitmproxy-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       20 2024-02-27 03:04:33.000000 pytest-mitmproxy-1.0.4/README.md
--rw-rw-rw-   0        0        0      544 2024-03-07 03:34:42.000000 pytest-mitmproxy-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-07 03:35:00.824311 pytest-mitmproxy-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-07 03:35:00.805361 pytest-mitmproxy-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-07 03:35:00.817330 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/
--rw-rw-rw-   0        0        0        0 2024-02-27 02:38:41.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-02-27 04:15:35.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/addon.py
--rw-rw-rw-   0        0        0     1438 2024-02-27 04:14:28.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/install_cert.py
--rw-rw-rw-   0        0        0     2314 2024-03-07 03:33:17.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/plugin.py
--rw-rw-rw-   0        0        0     1533 2024-02-27 05:01:25.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/system_proxy.py
-drwxrwxrwx   0        0        0        0 2024-03-07 03:35:00.823314 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/
--rw-rw-rw-   0        0        0      343 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-07 03:35:00.000000 pytest-mitmproxy-1.0.4/src/pytest_mitmproxy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 09:50:03.372330 pytest_mitmproxy-1.0.5/
+-rw-rw-rw-   0        0        0      343 2024-05-28 09:50:03.371332 pytest_mitmproxy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2024-02-27 03:04:33.000000 pytest_mitmproxy-1.0.5/README.md
+-rw-rw-rw-   0        0        0      544 2024-05-28 09:49:32.000000 pytest_mitmproxy-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:50:03.372330 pytest_mitmproxy-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 09:50:03.359400 pytest_mitmproxy-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:50:03.364352 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/
+-rw-rw-rw-   0        0        0        0 2024-02-27 02:38:41.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-02-27 04:15:35.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/addon.py
+-rw-rw-rw-   0        0        0     1438 2024-02-27 04:14:28.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/install_cert.py
+-rw-rw-rw-   0        0        0     2329 2024-05-28 09:49:32.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/plugin.py
+-rw-rw-rw-   0        0        0     1533 2024-02-27 05:01:25.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/system_proxy.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:50:03.370406 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 09:50:03.000000 pytest_mitmproxy-1.0.5/src/pytest_mitmproxy.egg-info/top_level.txt
```

### Comparing `pytest-mitmproxy-1.0.4/pyproject.toml` & `pytest_mitmproxy-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pytest-mitmproxy"
 description = "pytest plugin for mitmproxy tests"
-version = "1.0.4"
+version = "1.0.5"
 requires-python = ">=3.10"
 dependencies = [
     "pytest>=7.0",
     "mitmproxy>=10.0",
     "psutil>=5.0",
 ]
```

### Comparing `pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/addon.py` & `pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/addon.py`

 * *Files identical despite different names*

### Comparing `pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/install_cert.py` & `pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/install_cert.py`

 * *Files identical despite different names*

### Comparing `pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/plugin.py` & `pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         sock.bind(('localhost', 0))
         _, port = sock.getsockname()
         sock.close()
         return port if port != start_port else self._get_available_port(start_port=start_port + 1)
 
     def _start_mitmproxy(self):
         self._kill_existing_mitmproxy_processes()
-        proxy_port = self._get_available_port()
-        set_proxy(enable_proxy=True, proxy_address=f"http://127.0.0.1:{proxy_port}")
-        mitmproxy_command = ['mitmdump', '-p', str(proxy_port), '-s', self._addon_file, '-q', '--set',
+        self.proxy_port = self._get_available_port()
+        set_proxy(enable_proxy=True, proxy_address=f"http://127.0.0.1:{self.proxy_port}")
+        mitmproxy_command = ['mitmdump', '-p', str(self.proxy_port), '-s', self._addon_file, '-q', '--set',
                              f'url_filter={self.url_filter}']
         # 启动mitmproxy
         logger.debug("启动mitmproxy")
         self._mitmproxy_process = subprocess.Popen(mitmproxy_command)
 
     def _stop_mitmproxy(self):
         if self._mitmproxy_process:
```

### Comparing `pytest-mitmproxy-1.0.4/src/pytest_mitmproxy/system_proxy.py` & `pytest_mitmproxy-1.0.5/src/pytest_mitmproxy/system_proxy.py`

 * *Files identical despite different names*

