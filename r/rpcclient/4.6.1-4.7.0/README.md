# Comparing `tmp/rpcclient-4.6.1.tar.gz` & `tmp/rpcclient-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-4.6.1.tar", last modified: Thu Apr 11 10:51:39 2024, max compression
+gzip compressed data, was "rpcclient-4.7.0.tar", last modified: Tue May 28 11:24:00 2024, max compression
```

## Comparing `rpcclient-4.6.1.tar` & `rpcclient-4.7.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.441916 rpcclient-4.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-11 10:51:21.000000 rpcclient-4.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 10:51:21.000000 rpcclient-4.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-11 10:51:21.000000 rpcclient-4.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 10:51:39.441916 rpcclient-4.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 10:51:21.000000 rpcclient-4.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-11 10:51:21.000000 rpcclient-4.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 10:51:21.000000 rpcclient-4.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.425916 rpcclient-4.6.1/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/protos/
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-11 10:51:28.000000 rpcclient-4.6.1/rpcclient/protos/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-04-11 10:51:28.000000 rpcclient-4.6.1/rpcclient/protos/rpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/protosocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:51:39.441916 rpcclient-4.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.834811 rpcclient-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-28 11:23:44.000000 rpcclient-4.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 11:23:44.000000 rpcclient-4.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-28 11:23:44.000000 rpcclient-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-28 11:24:00.834811 rpcclient-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 11:23:44.000000 rpcclient-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-28 11:23:44.000000 rpcclient-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 11:23:44.000000 rpcclient-4.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.822811 rpcclient-4.7.0/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.826810 rpcclient-4.7.0/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45731 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.826810 rpcclient-4.7.0/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.826810 rpcclient-4.7.0/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.830811 rpcclient-4.7.0/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.830811 rpcclient-4.7.0/rpcclient/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-28 11:23:50.000000 rpcclient-4.7.0/rpcclient/protos/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-05-28 11:23:50.000000 rpcclient-4.7.0/rpcclient/protos/rpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/protosocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.830811 rpcclient-4.7.0/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-05-28 11:23:44.000000 rpcclient-4.7.0/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.830811 rpcclient-4.7.0/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 11:24:00.000000 rpcclient-4.7.0/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:24:00.834811 rpcclient-4.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:24:00.830811 rpcclient-4.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 11:23:44.000000 rpcclient-4.7.0/tests/test_xpc.py
```

### Comparing `rpcclient-4.6.1/CODE_OF_CONDUCT.md` & `rpcclient-4.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/LICENSE` & `rpcclient-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/PKG-INFO` & `rpcclient-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.6.1
+Version: 4.7.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.6.1/pyproject.toml` & `rpcclient-4.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/__main__.py` & `rpcclient-4.7.0/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/client.py` & `rpcclient-4.7.0/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/client_factory.py` & `rpcclient-4.7.0/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/bluetooth.py` & `rpcclient-4.7.0/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/cfpreferences.py` & `rpcclient-4.7.0/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/client.py` & `rpcclient-4.7.0/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/consts.py` & `rpcclient-4.7.0/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/core_graphics.py` & `rpcclient-4.7.0/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/crash_reports.py` & `rpcclient-4.7.0/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/darwin_lief.py` & `rpcclient-4.7.0/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/fs.py` & `rpcclient-4.7.0/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/hid.py` & `rpcclient-4.7.0/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/ioregistry.py` & `rpcclient-4.7.0/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/keychain.py` & `rpcclient-4.7.0/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/location.py` & `rpcclient-4.7.0/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/media.py` & `rpcclient-4.7.0/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/network.py` & `rpcclient-4.7.0/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/objc.py` & `rpcclient-4.7.0/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/objective_c_class.py` & `rpcclient-4.7.0/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-4.7.0/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/power.py` & `rpcclient-4.7.0/rpcclient/darwin/power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/processes.py` & `rpcclient-4.7.0/rpcclient/darwin/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     PROX_FDTYPE_KQUEUE, PROX_FDTYPE_PIPE, PROX_FDTYPE_SOCKET, PROX_FDTYPE_VNODE, TASK_DYLD_INFO_COUNT, \
     THREAD_IDENTIFIER_INFO_COUNT, all_image_infos_t, arm_thread_state64_t, dyld_image_info_t, fat_header, \
     ipc_info_name_t, mach_header_t, mach_port_t, pid_t, pipe_info, proc_fdinfo, proc_taskallinfo, procargs2_t, \
     so_family_t, so_kind_t, socket_fdinfo, task_dyld_info_data_t, thread_identifier_info, vnode_fdinfowithpath, \
     x86_thread_state64_t
 from rpcclient.darwin.symbol import DarwinSymbol
 from rpcclient.exceptions import ArgumentError, BadReturnValueError, MissingLibraryError, ProcessSymbolAbsentError, \
-    RpcClientException, SymbolAbsentError
+    RpcClientException, SymbolAbsentError, UnrecognizedSelectorError
 from rpcclient.processes import Processes
 from rpcclient.protos.rpc_pb2 import ARCH_ARM64
 from rpcclient.structs.consts import RTLD_NOW, SEEK_SET, SIGKILL, SIGTERM
 from rpcclient.symbol import ADDRESS_SIZE_TO_STRUCT_FORMAT, Symbol
 from rpcclient.sysctl import CTL, KERN
 
 _CF_STRING_ARRAY_PREFIX_LEN = len('    "')
@@ -820,14 +820,35 @@
             for cross_ref_port_info in cross_refs_info[port.ipc_object]:
                 if cross_ref_port_info.has_recv_right:
                     result.append(MachPortCrossRefInfo(name=port.name, ipc_object=port.ipc_object,
                                                        recv_right_pid=cross_ref_port_info.pid,
                                                        recv_right_proc_name=cross_ref_port_info.proc_name))
         return result
 
+    def get_memgraph_snapshot(self) -> bytes:
+        scanner = None
+        try:
+            # first attempt via new API
+            scanner = self._client.symbols.objc_getClass('VMUProcessObjectGraph').objc_call(
+                'createWithTask:', self.task)
+            snapshot_graph = scanner.objc_call('plistRepresentationWithOptions:', 0).py()
+        except UnrecognizedSelectorError:
+            # if failed, attempt with old API
+            scanner = self._client.symbols.objc_getClass('VMUTaskMemoryScanner').objc_call('alloc').objc_call(
+                'initWithTask:', self.task)
+            scanner.objc_call('addRootNodesFromTask')
+            scanner.objc_call('addMallocNodesFromTask')
+            snapshot_graph = scanner.objc_call('processSnapshotGraph').objc_call(
+                'plistRepresentationWithOptions:', 0).py()
+        finally:
+            if scanner is not None:
+                # free object scanner so process can resume
+                scanner.objc_call('release')
+        return snapshot_graph
+
     def __repr__(self):
         return f'<{self.__class__.__name__} PID:{self.pid} PATH:{self.path}>'
 
 
 class DarwinProcesses(Processes):
     """ manage processes """
```

### Comparing `rpcclient-4.6.1/rpcclient/darwin/reports.py` & `rpcclient-4.7.0/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/scpreferences.py` & `rpcclient-4.7.0/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/structs.py` & `rpcclient-4.7.0/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/symbol.py` & `rpcclient-4.7.0/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/syslog.py` & `rpcclient-4.7.0/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/time.py` & `rpcclient-4.7.0/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/darwin/xpc.py` & `rpcclient-4.7.0/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/exceptions.py` & `rpcclient-4.7.0/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/fs.py` & `rpcclient-4.7.0/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/accessibility.py` & `rpcclient-4.7.0/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/amfi.py` & `rpcclient-4.7.0/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/backlight.py` & `rpcclient-4.7.0/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/client.py` & `rpcclient-4.7.0/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/lockdown.py` & `rpcclient-4.7.0/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/mobile_gestalt.py` & `rpcclient-4.7.0/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/processes.py` & `rpcclient-4.7.0/rpcclient/ios/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/screen_capture.py` & `rpcclient-4.7.0/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/sprinboard.py` & `rpcclient-4.7.0/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/telephony.py` & `rpcclient-4.7.0/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/ios/wifi.py` & `rpcclient-4.7.0/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/lief.py` & `rpcclient-4.7.0/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/linux/client.py` & `rpcclient-4.7.0/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/linux/structs.py` & `rpcclient-4.7.0/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/macos/apple_script.py` & `rpcclient-4.7.0/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/macos/client.py` & `rpcclient-4.7.0/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/network.py` & `rpcclient-4.7.0/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/processes.py` & `rpcclient-4.7.0/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/protos/rpc_pb2.py` & `rpcclient-4.7.0/rpcclient/protos/rpc_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: rpc.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x12\x03rpc\"\xb9\x04\n\x07\x43ommand\x12\r\n\x05magic\x18\x01 \x01(\x05\x12\x1c\n\x04\x65xec\x18\x02 \x01(\x0b\x32\x0c.rpc.CmdExecH\x00\x12 \n\x06\x64lopen\x18\x03 \x01(\x0b\x32\x0e.rpc.CmdDlopenH\x00\x12\"\n\x07\x64lclose\x18\x04 \x01(\x0b\x32\x0f.rpc.CmdDlcloseH\x00\x12\x1e\n\x05\x64lsym\x18\x05 \x01(\x0b\x32\r.rpc.CmdDlsymH\x00\x12\x1c\n\x04\x63\x61ll\x18\x06 \x01(\x0b\x32\x0c.rpc.CmdCallH\x00\x12\x1c\n\x04peek\x18\x07 \x01(\x0b\x32\x0c.rpc.CmdPeekH\x00\x12\x1c\n\x04poke\x18\x08 \x01(\x0b\x32\x0c.rpc.CmdPokeH\x00\x12#\n\x08list_dir\x18\t \x01(\x0b\x32\x0f.rpc.CmdListDirH\x00\x12)\n\x0bshow_object\x18\n \x01(\x0b\x32\x12.rpc.CmdShowObjectH\x00\x12\'\n\nshow_class\x18\x0b \x01(\x0b\x32\x11.rpc.CmdShowClassH\x00\x12)\n\x0b\x64ummy_block\x18\x0c \x01(\x0b\x32\x12.rpc.CmdDummyBlockH\x00\x12\x1e\n\x05\x63lose\x18\r \x01(\x0b\x32\r.rpc.CmdCloseH\x00\x12*\n\nclass_list\x18\x0e \x01(\x0b\x32\x14.rpc.CmdGetClassListH\x00\x12\'\n\nexec_chunk\x18\x0f \x01(\x0b\x32\x11.rpc.CmdExecChunkH\x00\x12 \n\x06\x63ustom\x18\x10 \x01(\x0b\x32\x0e.rpc.CmdCustomH\x00\x42\x06\n\x04type\"\xfc\x04\n\x08Response\x12$\n\x04\x65xec\x18\x01 \x01(\x0b\x32\x14.rpc.ResponseCmdExecH\x00\x12/\n\nexec_chunk\x18\x02 \x01(\x0b\x32\x19.rpc.ResponseCmdExecChunkH\x00\x12%\n\x06\x64lopen\x18\x03 \x01(\x0b\x32\x13.rpc.ResponseDlopenH\x00\x12\'\n\x07\x64lclose\x18\x04 \x01(\x0b\x32\x14.rpc.ResponseDlcloseH\x00\x12#\n\x05\x64lsym\x18\x05 \x01(\x0b\x32\x12.rpc.ResponseDlsymH\x00\x12!\n\x04peek\x18\x06 \x01(\x0b\x32\x11.rpc.ResponsePeekH\x00\x12!\n\x04poke\x18\x07 \x01(\x0b\x32\x11.rpc.ResponsePokeH\x00\x12!\n\x04\x63\x61ll\x18\x08 \x01(\x0b\x32\x11.rpc.ResponseCallH\x00\x12#\n\x05\x65rror\x18\t \x01(\x0b\x32\x12.rpc.ResponseErrorH\x00\x12.\n\x0b\x64ummy_block\x18\n \x01(\x0b\x32\x17.rpc.ResponseDummyBlockH\x00\x12.\n\x0bshow_object\x18\x0b \x01(\x0b\x32\x17.rpc.ResponseShowObjectH\x00\x12/\n\nclass_list\x18\x0c \x01(\x0b\x32\x19.rpc.ResponseGetClassListH\x00\x12,\n\nshow_class\x18\r \x01(\x0b\x32\x16.rpc.ResponseShowClassH\x00\x12(\n\x08list_dir\x18\x0e \x01(\x0b\x32\x14.rpc.ResponseListdirH\x00\x12%\n\x06\x63ustom\x18\x0f \x01(\x0b\x32\x13.rpc.ResponseCustomH\x00\x42\x06\n\x04type\"\xd4\x01\n\x12ReturnRegistersArm\x12\n\n\x02x0\x18\x01 \x01(\x04\x12\n\n\x02x1\x18\x02 \x01(\x04\x12\n\n\x02x2\x18\x03 \x01(\x04\x12\n\n\x02x3\x18\x04 \x01(\x04\x12\n\n\x02x4\x18\x05 \x01(\x04\x12\n\n\x02x5\x18\x06 \x01(\x04\x12\n\n\x02x6\x18\x07 \x01(\x04\x12\n\n\x02x7\x18\x08 \x01(\x04\x12\n\n\x02\x64\x30\x18\t \x01(\x01\x12\n\n\x02\x64\x31\x18\n \x01(\x01\x12\n\n\x02\x64\x32\x18\x0b \x01(\x01\x12\n\n\x02\x64\x33\x18\x0c \x01(\x01\x12\n\n\x02\x64\x34\x18\r \x01(\x01\x12\n\n\x02\x64\x35\x18\x0e \x01(\x01\x12\n\n\x02\x64\x36\x18\x0f \x01(\x01\x12\n\n\x02\x64\x37\x18\x10 \x01(\x01\"[\n\x08\x41rgument\x12\x0f\n\x05v_int\x18\x01 \x01(\x04H\x00\x12\x12\n\x08v_double\x18\x02 \x01(\x01H\x00\x12\x0f\n\x05v_str\x18\x03 \x01(\tH\x00\x12\x11\n\x07v_bytes\x18\x04 \x01(\x0cH\x00\x42\x06\n\x04type\"U\n\tHandshake\x12\r\n\x05magic\x18\x01 \x01(\r\x12\x17\n\x04\x61rch\x18\x02 \x01(\x0e\x32\t.rpc.Arch\x12\x0f\n\x07sysname\x18\x03 \x01(\t\x12\x0f\n\x07machine\x18\x04 \x01(\t\"*\n\tObjcClass\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\" \n\rCmdShowObject\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\")\n\x12ResponseShowObject\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\"\x1f\n\x0c\x43mdShowClass\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\"(\n\x11ResponseShowClass\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\"\x1e\n\x0c\x43mdExecChunk\x12\x0e\n\x06\x62uffer\x18\x01 \x01(\x0c\"E\n\x14ResponseCmdExecChunk\x12\x10\n\x06\x62uffer\x18\x01 \x01(\x0cH\x00\x12\x13\n\texit_code\x18\x02 \x01(\rH\x00\x42\x06\n\x04type\"+\n\tCmdDlopen\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0c\n\x04mode\x18\x02 \x01(\x05\" \n\x0eResponseDlopen\x12\x0e\n\x06handle\x18\x01 \x01(\x04\"\x1c\n\nCmdDlclose\x12\x0e\n\x06handle\x18\x01 \x01(\x04\"\x1e\n\x0fResponseDlclose\x12\x0b\n\x03res\x18\x01 \x01(\r\"/\n\x08\x43mdDlsym\x12\x0e\n\x06handle\x18\x01 \x01(\x04\x12\x13\n\x0bsymbol_name\x18\x02 \x01(\t\"\x1c\n\rResponseDlsym\x12\x0b\n\x03ptr\x18\x01 \x01(\x04\"9\n\x07\x43mdExec\x12\x12\n\nbackground\x18\x01 \x01(\x08\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12\x0c\n\x04\x65nvp\x18\x03 \x03(\t\"\x1e\n\x0fResponseCmdExec\x12\x0b\n\x03pid\x18\x01 \x01(\r\"N\n\x07\x43mdCall\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\x12\x15\n\rva_list_index\x18\x02 \x01(\x04\x12\x1b\n\x04\x61rgv\x18\x03 \x03(\x0b\x32\r.rpc.Argument\"i\n\x0cResponseCall\x12\x30\n\rarm_registers\x18\x01 \x01(\x0b\x32\x17.rpc.ReturnRegistersArmH\x00\x12\x16\n\x0creturn_value\x18\x02 \x01(\x04H\x00\x42\x0f\n\rreturn_values\"(\n\x07\x43mdPeek\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\x12\x0c\n\x04size\x18\x02 \x01(\x04\"\x1c\n\x0cResponsePeek\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"(\n\x07\x43mdPoke\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x0e\n\x0cResponsePoke\"\x1a\n\nCmdListDir\x12\x0c\n\x04path\x18\x01 \x01(\t\"\x0f\n\rCmdDummyBlock\"3\n\x12ResponseDummyBlock\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x04\x12\x0c\n\x04size\x18\x02 \x01(\x04\"\x11\n\x0f\x43mdGetClassList\"7\n\x14ResponseGetClassList\x12\x1f\n\x07\x63lasses\x18\x01 \x03(\x0b\x32\x0e.rpc.ObjcClass\"\x0f\n\rResponseError\"R\n\x0fResponseListdir\x12\r\n\x05magic\x18\x01 \x01(\x04\x12\x0c\n\x04\x64irp\x18\x02 \x01(\x04\x12\"\n\x0b\x64ir_entries\x18\x03 \x03(\x0b\x32\r.rpc.DirEntry\"m\n\x08\x44irEntry\x12\x0e\n\x06\x64_type\x18\x01 \x01(\x04\x12\x0e\n\x06\x64_name\x18\x02 \x01(\t\x12 \n\x05lstat\x18\x03 \x01(\x0b\x32\x11.rpc.DirEntryStat\x12\x1f\n\x04stat\x18\x04 \x01(\x0b\x32\x11.rpc.DirEntryStat\"\x83\x02\n\x0c\x44irEntryStat\x12\x0e\n\x06\x65rrno1\x18\x01 \x01(\x04\x12\x0e\n\x06st_dev\x18\x02 \x01(\x04\x12\x0f\n\x07st_mode\x18\x03 \x01(\x04\x12\x10\n\x08st_nlink\x18\x04 \x01(\x04\x12\x0e\n\x06st_ino\x18\x05 \x01(\x04\x12\x0e\n\x06st_uid\x18\x06 \x01(\x04\x12\x0e\n\x06st_gid\x18\x07 \x01(\x04\x12\x0f\n\x07st_rdev\x18\x08 \x01(\x04\x12\x0f\n\x07st_size\x18\t \x01(\x04\x12\x11\n\tst_blocks\x18\n \x01(\x04\x12\x12\n\nst_blksize\x18\x0b \x01(\x04\x12\x11\n\tst_atime1\x18\x0c \x01(\x04\x12\x11\n\tst_mtime1\x18\r \x01(\x04\x12\x11\n\tst_ctime1\x18\x0e \x01(\x04\"\n\n\x08\x43mdClose\"\x1c\n\tCmdCustom\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"!\n\x0eResponseCustom\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c*(\n\x04\x41rch\x12\x10\n\x0c\x41RCH_UNKNOWN\x10\x00\x12\x0e\n\nARCH_ARM64\x10\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_ARCH']._serialized_start=3276
   _globals['_ARCH']._serialized_end=3316
   _globals['_COMMAND']._serialized_start=19
   _globals['_COMMAND']._serialized_end=588
   _globals['_RESPONSE']._serialized_start=591
   _globals['_RESPONSE']._serialized_end=1227
   _globals['_RETURNREGISTERSARM']._serialized_start=1230
```

### Comparing `rpcclient-4.6.1/rpcclient/protos/rpc_pb2.pyi` & `rpcclient-4.7.0/rpcclient/protos/rpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/protosocket.py` & `rpcclient-4.7.0/rpcclient/protosocket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/structs/consts.py` & `rpcclient-4.7.0/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/structs/generic.py` & `rpcclient-4.7.0/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/symbol.py` & `rpcclient-4.7.0/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/symbols_jar.py` & `rpcclient-4.7.0/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/sysctl.py` & `rpcclient-4.7.0/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient/xonshrc.py` & `rpcclient-4.7.0/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/rpcclient.egg-info/PKG-INFO` & `rpcclient-4.7.0/rpcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.6.1
+Version: 4.7.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.6.1/rpcclient.egg-info/SOURCES.txt` & `rpcclient-4.7.0/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/conftest.py` & `rpcclient-4.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_allocation_cleanup.py` & `rpcclient-4.7.0/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_client.py` & `rpcclient-4.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_darwin_client.py` & `rpcclient-4.7.0/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_fs.py` & `rpcclient-4.7.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_objc_symbol.py` & `rpcclient-4.7.0/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_power.py` & `rpcclient-4.7.0/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_preferences.py` & `rpcclient-4.7.0/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_processes.py` & `rpcclient-4.7.0/tests/test_processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     assert len([img for img in server.images if Path(img.path).resolve() == Path(server.path).resolve()]) > 0
     fds = server.fds
     assert fds[0].fd == 0
     assert fds[1].fd == 1
     assert fds[2].fd == 2
 
 
+def test_get_memgraph_snapshot(client):
+    assert len(client.processes.get_self().parent.get_memgraph_snapshot()) > 0
+
+
 @pytest.mark.ios
 def test_launch_process(client):
     client.processes.launch('com.apple.calculator').kill()
 
 
 @pytest.mark.ios
 def test_launch_invalid_process(client):
```

### Comparing `rpcclient-4.6.1/tests/test_socket.py` & `rpcclient-4.7.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_spawn.py` & `rpcclient-4.7.0/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_thread_safe.py` & `rpcclient-4.7.0/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_time.py` & `rpcclient-4.7.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.1/tests/test_xpc.py` & `rpcclient-4.7.0/tests/test_xpc.py`

 * *Files identical despite different names*

