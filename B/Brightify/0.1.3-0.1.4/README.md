# Comparing `tmp/brightify-0.1.3.tar.gz` & `tmp/brightify-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightify-0.1.3.tar", last modified: Mon May 27 07:40:38 2024, max compression
+gzip compressed data, was "brightify-0.1.4.tar", last modified: Tue May 28 20:44:57 2024, max compression
```

## Comparing `brightify-0.1.3.tar` & `brightify-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/Brightify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 07:40:30.000000 brightify-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-27 07:40:38.310752 brightify-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-27 07:40:30.000000 brightify-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/BaseApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/SensorComm.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/brightylog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/linux/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/log_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorDDCCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorUSB.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/m27q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/res/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/res/icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/res/icon_light.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/sensor_firmware/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/sensor_firmware/platformio.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/sensor_firmware/src/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/sensor_firmware/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/ui_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/WindowsApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/add_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/remove_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-27 07:40:30.000000 brightify-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:40:38.310752 brightify-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/Brightify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-28 20:44:57.000000 brightify-0.1.4/Brightify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-28 20:44:57.000000 brightify-0.1.4/Brightify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:44:57.000000 brightify-0.1.4/Brightify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 20:44:57.000000 brightify-0.1.4/Brightify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 20:44:57.000000 brightify-0.1.4/Brightify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 20:44:52.000000 brightify-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-28 20:44:57.159539 brightify-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-28 20:44:52.000000 brightify-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/BaseApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/SensorComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/brightylog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/linux/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/log_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/monitors/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/monitors/MonitorDDCCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/monitors/MonitorUSB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/monitors/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/monitors/m27q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/res/icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/res/icon_light.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/sensor_firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/sensor_firmware/platformio.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/sensor_firmware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/sensor_firmware/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/ui_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:44:57.159539 brightify-0.1.4/brightify/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/MonitorWMI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/WindowsApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/add_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-28 20:44:52.000000 brightify-0.1.4/brightify/windows/remove_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-28 20:44:52.000000 brightify-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:44:57.163539 brightify-0.1.4/setup.cfg
```

### Comparing `brightify-0.1.3/Brightify.egg-info/PKG-INFO` & `brightify-0.1.4/Brightify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
 Requires-Dist: libusb1
 Requires-Dist: PyQt6
 Requires-Dist: monitorcontrol
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: winshell; platform_system == "Windows"
+Requires-Dist: wmi; platform_system == "Windows"
 
 # Brightify
 This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
 It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
 You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
 The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
 
 ## Getting started
 1. Install brightify by running `pip install Brightify`. This package is regularly uploaded to PyPi. If you want to install the latest version, you can clone this repository from 
 [GitHub](https://github.com/RerikOp/Brightify) and install it with `pip install -e .` in the root directory.
 2. To start the app: `python -m brightify run`. You can exit either by right-clicking the icon in the taskbar and
    selecting "Exit" or by pressing `Ctrl+C` in the terminal.
-3. To start the app at startup (or logon) and add a menu icon, run `python -m add all`. To remove the both, run
-   `python -m remove all`.
+3. To start the app at startup (or logon) and add a menu icon, run `python -m brightify add all`. To remove the both, run
+   `python -m brightify remove all`.
 
 ## Optional arguments
 There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
 - To target add/remove only the startup run `python -m brightify add/remove startup`.
    - To add a task to the task scheduler on Windows, pass `--use-scheduler`. It will request elevated permissions.
    - By default, the terminal will be hidden, but you can change this by passing the `--force-console` argument.
 - To add/remove only the menu icon run `python -m brightify add/remove menu-icon`.
@@ -43,9 +44,11 @@
    see [supported boards](https://docs.platformio.org/en/latest/boards/index.html))
 - Run `pio run -t upload` in the terminal to upload the firmware to the board.
    If everything is working, the *Auto* Checkbox for each supported Monitor should now be clickable
 
 ## Remarks
 - Currently, only the Windows task bar icon is supported, the main part of this app is OS independent.
 - Feel free to create a pull request and add your own USB Monitor
+- Note that a USB Monitor will replace a DDC/CI Monitor with the same name. If you want to use both, you need to change the name of your USB Monitor implementation.
+In case a monitor is found but does not send its name, we cannot distinguish between DDC/CI and USB Monitors. In this case, both will be added.
```

### Comparing `brightify-0.1.3/Brightify.egg-info/SOURCES.txt` & `brightify-0.1.4/Brightify.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 brightify/monitors/MonitorUSB.py
 brightify/monitors/finder.py
 brightify/monitors/m27q.py
 brightify/res/icon_dark.ico
 brightify/res/icon_light.ico
 brightify/sensor_firmware/platformio.ini
 brightify/sensor_firmware/src/main.cpp
+brightify/windows/MonitorWMI.py
 brightify/windows/WindowsApp.py
 brightify/windows/actions.py
 brightify/windows/add_startup_task.py
 brightify/windows/helpers.py
 brightify/windows/remove_startup_task.py
```

### Comparing `brightify-0.1.3/PKG-INFO` & `brightify-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
 Requires-Dist: libusb1
 Requires-Dist: PyQt6
 Requires-Dist: monitorcontrol
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: winshell; platform_system == "Windows"
+Requires-Dist: wmi; platform_system == "Windows"
 
 # Brightify
 This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
 It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
 You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
 The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
 
 ## Getting started
 1. Install brightify by running `pip install Brightify`. This package is regularly uploaded to PyPi. If you want to install the latest version, you can clone this repository from 
 [GitHub](https://github.com/RerikOp/Brightify) and install it with `pip install -e .` in the root directory.
 2. To start the app: `python -m brightify run`. You can exit either by right-clicking the icon in the taskbar and
    selecting "Exit" or by pressing `Ctrl+C` in the terminal.
-3. To start the app at startup (or logon) and add a menu icon, run `python -m add all`. To remove the both, run
-   `python -m remove all`.
+3. To start the app at startup (or logon) and add a menu icon, run `python -m brightify add all`. To remove the both, run
+   `python -m brightify remove all`.
 
 ## Optional arguments
 There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
 - To target add/remove only the startup run `python -m brightify add/remove startup`.
    - To add a task to the task scheduler on Windows, pass `--use-scheduler`. It will request elevated permissions.
    - By default, the terminal will be hidden, but you can change this by passing the `--force-console` argument.
 - To add/remove only the menu icon run `python -m brightify add/remove menu-icon`.
@@ -43,9 +44,11 @@
    see [supported boards](https://docs.platformio.org/en/latest/boards/index.html))
 - Run `pio run -t upload` in the terminal to upload the firmware to the board.
    If everything is working, the *Auto* Checkbox for each supported Monitor should now be clickable
 
 ## Remarks
 - Currently, only the Windows task bar icon is supported, the main part of this app is OS independent.
 - Feel free to create a pull request and add your own USB Monitor
+- Note that a USB Monitor will replace a DDC/CI Monitor with the same name. If you want to use both, you need to change the name of your USB Monitor implementation.
+In case a monitor is found but does not send its name, we cannot distinguish between DDC/CI and USB Monitors. In this case, both will be added.
```

### Comparing `brightify-0.1.3/README.md` & `brightify-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
 
 ## Getting started
 1. Install brightify by running `pip install Brightify`. This package is regularly uploaded to PyPi. If you want to install the latest version, you can clone this repository from 
 [GitHub](https://github.com/RerikOp/Brightify) and install it with `pip install -e .` in the root directory.
 2. To start the app: `python -m brightify run`. You can exit either by right-clicking the icon in the taskbar and
    selecting "Exit" or by pressing `Ctrl+C` in the terminal.
-3. To start the app at startup (or logon) and add a menu icon, run `python -m add all`. To remove the both, run
-   `python -m remove all`.
+3. To start the app at startup (or logon) and add a menu icon, run `python -m brightify add all`. To remove the both, run
+   `python -m brightify remove all`.
 
 ## Optional arguments
 There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
 - To target add/remove only the startup run `python -m brightify add/remove startup`.
    - To add a task to the task scheduler on Windows, pass `--use-scheduler`. It will request elevated permissions.
    - By default, the terminal will be hidden, but you can change this by passing the `--force-console` argument.
 - To add/remove only the menu icon run `python -m brightify add/remove menu-icon`.
@@ -27,9 +27,11 @@
    see [supported boards](https://docs.platformio.org/en/latest/boards/index.html))
 - Run `pio run -t upload` in the terminal to upload the firmware to the board.
    If everything is working, the *Auto* Checkbox for each supported Monitor should now be clickable
 
 ## Remarks
 - Currently, only the Windows task bar icon is supported, the main part of this app is OS independent.
 - Feel free to create a pull request and add your own USB Monitor
+- Note that a USB Monitor will replace a DDC/CI Monitor with the same name. If you want to use both, you need to change the name of your USB Monitor implementation.
+In case a monitor is found but does not send its name, we cannot distinguish between DDC/CI and USB Monitors. In this case, both will be added.
```

### Comparing `brightify-0.1.3/brightify/BaseApp.py` & `brightify-0.1.4/brightify/BaseApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         def run_and_disconnect():
             finished()
             animation.finished.disconnect(run_and_disconnect)
 
         animation.finished.connect(run_and_disconnect)
 
     def __add_reload_button(self):
-
         # add a reload button to the top of self.rows
         reload_button = QPushButton("Reload", self)
         reload_button.clicked.connect(lambda: self.change_state("hide"))
         reload_button.clicked.connect(lambda: self.run_once(self.fade_down_animation, self.redraw))
         reload_button.setStyleSheet(self.ui_config.button_style)
         self.rows.addWidget(reload_button)
```

### Comparing `brightify-0.1.3/brightify/SensorComm.py` & `brightify-0.1.4/brightify/SensorComm.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/__main__.py` & `brightify-0.1.4/brightify/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     logger.exception("An unhandled exception occurred", exc_info=(exc_type, exc_value, exc_tb))
 
 
 def main_win(app: QApplication):
     import win32gui
     from brightify.windows.WindowsApp import WindowsApp
     from brightify.windows.helpers import get_theme
-
     base_app = BaseApp(get_theme)
     WindowsApp(base_app)
     threading.Thread(target=win32gui.PumpMessages, daemon=True).start()
     base_app.show()
     ret_code = app.exec()
     logger.info(f"Exiting with code {ret_code}")
     exit(ret_code)
```

### Comparing `brightify-0.1.3/brightify/brightylog.py` & `brightify-0.1.4/brightify/brightylog.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/linux/helpers.py` & `brightify-0.1.4/brightify/linux/helpers.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/log_config.toml` & `brightify-0.1.4/brightify/log_config.toml`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/monitors/MonitorBase.py` & `brightify-0.1.4/brightify/monitors/MonitorBase.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         """
         pass
 
     @abstractmethod
     def name(self):
         pass
 
+    @staticmethod
+    def get_type():
+        return "ANY"
+
     def convert_sensor_readings(self, readings: Iterable) -> Optional[int]:
         """
         Converts a number of sensor readings to the new brightness of this monitor
         :param readings: an Iterable that contains the most recent readings.
          The first element is the oldest reading
         :return: an int representing a proposed new brightness between self.min_brightness and self.max_brightness
         or None if the sensor data doesn't indicate a brightness switch
```

### Comparing `brightify-0.1.3/brightify/monitors/MonitorDDCCI.py` & `brightify-0.1.4/brightify/monitors/MonitorDDCCI.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,18 @@
             self.vcp_cap, self.__name, self.is_unknown = self.update_cap()
         return self.__name
 
     @staticmethod
     def default_name():
         return "Monitor"
 
+    @staticmethod
+    def get_type():
+        return "DDCCI"
+
     def get_brightness(self, blocking: bool = False, force: bool = False) -> Optional[int]:
         max_tries = 1 if not blocking and not force else self.max_tries
         for _ in range(max_tries):
             with self.monitor:
                 try:
                     return self.monitor.get_luminance()
                 except monitorcontrol.vcp.vcp_abc.VCPError:
```

### Comparing `brightify-0.1.3/brightify/monitors/MonitorUSB.py` & `brightify-0.1.4/brightify/monitors/MonitorUSB.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,13 +48,17 @@
     def pid() -> int:
         pass
 
     @property
     def device(self) -> usb1.USBDevice:
         return self.__device
 
+    @staticmethod
+    def get_type():
+        return "USB"
+
     def __del__(self):
         if self.__device is not None:
             logger.info(f"Closing monitor {self.name()}")
             self.__device.close()
             self.__device = None
             super().__del__()
```

### Comparing `brightify-0.1.3/brightify/monitors/finder.py` & `brightify-0.1.4/brightify/monitors/finder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import timeit
 from typing import List, Type, Tuple
 from pathlib import Path
 
+from brightify import host_os
 from brightify.monitors.MonitorBase import MonitorBase
 from brightify.monitors.MonitorDDCCI import MonitorDDCCI
 from brightify.monitors.MonitorUSB import MonitorUSB
 from brightify.monitors.MonitorBase import logger
 
 
-
 def _supported_usb_impls() -> List[Type[MonitorUSB]]:
     """
     Finds all user implemented MonitorUSB classes in the monitors directory.
     :return: a list of all MonitorUSB implementations
     """
     import importlib, inspect
     monitor_impls = set()
@@ -49,23 +50,44 @@
 
 def _ddcci_monitors() -> List[MonitorDDCCI]:
     """
     Finds all monitors connected to the system and instantiates the MonitorDDCCI class.
     :return: a list of all MonitorDDCCI implementations
     """
     import monitorcontrol
+    # time the operation
     monitors = monitorcontrol.get_monitors()
+    # print the time it took in milliseconds
     return [MonitorDDCCI(monitor) for monitor in monitors]
 
 
+def _internal_monitors() -> List[MonitorBase]:
+    """
+    Finds all internal monitors connected to the system and instantiates the MonitorBase class.
+    :return: a list of all MonitorBase implementations
+    """
+    if host_os == "Windows":
+        from brightify.windows.MonitorWMI import WMIMonitor
+        if WMIMonitor.has_wmi_monitor():
+            return [WMIMonitor()]
+    return []
+
+
 def get_supported_monitors() -> List[MonitorBase]:
     """
     Finds all user implemented MonitorUSB classes and instantiates them with the corresponding USB device.
     If a monitor without a USB device is found or an implementation is missing, we try to connect to the monitor via DDC-CI.
     :return: a list of all MonitorBase implementations
     """
     monitor_impls = _supported_usb_impls()
     usb_monitors = _usb_monitors(monitor_impls)
     logger.info(f"Found {len(usb_monitors)} USB monitor(s) with implementation: {[m.name() for m in usb_monitors]}")
-    ddcci_monitors = _ddcci_monitors()
-    logger.info(f"Found {len(ddcci_monitors)} DDCCI monitor(s)")
-    return usb_monitors + ddcci_monitors
+    all_ddcci_monitors = _ddcci_monitors()
+    internal_monitors = _internal_monitors()
+    logger.info(f"Found {len(internal_monitors)} internal monitor(s)")
+    # remove DD/CCI monitors if they are already connected via USB
+    ddcci_monitors = [m for m in all_ddcci_monitors if not any(m.name() == usb_m.name() for usb_m in usb_monitors)]
+    if (diff := len(all_ddcci_monitors) - len(ddcci_monitors)) > 0:
+        logger.info(f"Removed {diff} DDCCI monitor(s) already connected via USB")
+
+
+    return usb_monitors + ddcci_monitors
```

### Comparing `brightify-0.1.3/brightify/monitors/m27q.py` & `brightify-0.1.4/brightify/monitors/m27q.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/res/icon_dark.ico` & `brightify-0.1.4/brightify/res/icon_dark.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/res/icon_light.ico` & `brightify-0.1.4/brightify/res/icon_light.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/ui_config.py` & `brightify-0.1.4/brightify/ui_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from PyQt6 import QtCore
 from PyQt6.QtCore import QPropertyAnimation, QEasingCurve
 from PyQt6.QtGui import QFont, QFontMetrics
 
 from PyQt6.QtWidgets import QWidget, QSlider, QCheckBox, QLabel, QHBoxLayout
 
-from brightify import icon_light, icon_dark
+from brightify import icon_light, icon_dark, host_os
 from brightify.monitors.MonitorBase import MonitorBase
 from brightify.monitors.MonitorUSB import MonitorUSB
 from brightify.monitors.MonitorDDCCI import MonitorDDCCI
 
 
 @dataclasses.dataclass
 class Theme:
@@ -62,20 +62,16 @@
     @property
     def monitor(self):
         return self.__monitor
 
     @monitor.setter
     def monitor(self, value: MonitorBase):
         self.__monitor = value
-        if isinstance(value, MonitorUSB):
-            self.type_label.setText("[USB]")
-        elif isinstance(value, MonitorDDCCI):
-            self.type_label.setText("[DDCCI]")
-        else:
-            self.type_label.setText("[ANY]")
+        type_label_text = f"[{value.get_type()}]"
+        self.type_label.setText(type_label_text)
 
 
     @staticmethod
     def __slider_style(theme: Theme):
         return f"""
             QSlider {{
                 min-height: 30px;
```

### Comparing `brightify-0.1.3/brightify/windows/WindowsApp.py` & `brightify-0.1.4/brightify/windows/WindowsApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 logger = logging.getLogger("Windows")
 
 
 class WindowsApp:
     # For documentation of objects, see http://timgolden.me.uk/pywin32-docs/objects.html
     # For documentation of functions, see http://timgolden.me.uk/pywin32-docs/win32gui.html
     def __init__(self, base_app: BaseApp):
+        # Listen for taskbar restarts
         WM_TASKBAR_CREATED = win32gui.RegisterWindowMessage("TaskbarCreated")
-        # TODO listen for USB connected
+
         # to receive messages from the os
         self.WM_ICON = win32con.WM_USER + 42
         self.base_app = base_app
 
         self.message_map = {
             # if taskbar is (re)started we must recreate the icon for this program
             WM_TASKBAR_CREATED: self._on_restart,
+            # if the display changes, we must update the top left corner of the app
+            win32con.WM_DISPLAYCHANGE: self._on_restart,
             # on destroy message
             win32con.WM_DESTROY: self._on_destroy,
             # parses the commands that are registers throughout this program
             win32con.WM_COMMAND: self._on_command,
             # if the icon is interacted with
             self.WM_ICON: self._on_icon_notify
         }
@@ -144,15 +147,15 @@
 
         flags = win32gui.NIF_ICON | win32gui.NIF_MESSAGE | win32gui.NIF_TIP
         nid = (self.hwnd, 0, flags, self.WM_ICON, hicon, app_name)
 
         try:
             win32gui.Shell_NotifyIcon(win32gui.NIM_ADD, nid)
         except win32gui.error:
-            logger.critical("Failed to add the icon to the system tray")
+            logger.debug("Failed to add the icon to the system tray, it may already be there")
             pass
 
     def exit(self):
         exit_id = self.cmd_id_map["Exit"]
         try:  # invoke the exit function
             self.cmd_id_map[exit_id]()
         except pywintypes.error as e:
```

### Comparing `brightify-0.1.3/brightify/windows/actions.py` & `brightify-0.1.4/brightify/windows/actions.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/windows/add_startup_task.py` & `brightify-0.1.4/brightify/windows/add_startup_task.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/brightify/windows/helpers.py` & `brightify-0.1.4/brightify/windows/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     raise RuntimeError("This code is designed to run with pywin32")
 except ImportError as e:
     raise RuntimeError("Failed importing pywin32: \n" + e.msg)
 
 # Use OS specific logger
 logger = logging.getLogger("Windows")
 
+
 def get_registry_key(sub_key: str, name: str):
     import winreg
     try:
         key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, sub_key)
         value, reg_type = winreg.QueryValueEx(key, name)
         winreg.CloseKey(key)
         return value, reg_type
```

### Comparing `brightify-0.1.3/brightify/windows/remove_startup_task.py` & `brightify-0.1.4/brightify/windows/remove_startup_task.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.3/pyproject.toml` & `brightify-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Brightify"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Robin S.", email = "brightify@rs-web.net" }
 ]
 description = "Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon."
 
 requires-python = ">= 3.11"
 
@@ -23,9 +23,10 @@
     "platformio",
     "pyserial",
     "libusb1",
     "PyQt6",
     "monitorcontrol",
     # Windows-only dependencies
     'pywin32; platform_system == "Windows"',
-    'winshell; platform_system == "Windows"'
+    'winshell; platform_system == "Windows"',
+    'wmi; platform_system == "Windows"',
 ]
```

