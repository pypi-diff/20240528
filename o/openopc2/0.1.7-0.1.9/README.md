# Comparing `tmp/openopc2-0.1.7.tar.gz` & `tmp/openopc2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openopc2-0.1.7.tar", max compression
+gzip compressed data, was "openopc2-0.1.9.tar", max compression
```

## Comparing `openopc2-0.1.7.tar` & `openopc2-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16490 2022-11-22 14:12:11.979756 openopc2-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     8370 2022-11-22 14:12:11.979756 openopc2-0.1.7/README.md
--rw-r--r--   0        0        0        0 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/__init__.py
--rw-r--r--   0        0        0       69 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/__main__.py
--rw-r--r--   0        0        0    11641 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/cli.py
--rw-r--r--   0        0        0      815 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/config.py
--rw-r--r--   0        0        0    39325 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/da_client.py
--rw-r--r--   0        0        0     8842 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/da_com.py
--rw-r--r--   0        0        0      669 2022-11-22 14:12:11.987756 openopc2-0.1.7/openopc2/exceptions.py
--rw-r--r--   0        0        0     1227 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/gateway_proxy.py
--rw-r--r--   0        0        0     3559 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/gateway_server.py
--rw-r--r--   0        0        0     3852 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/gateway_service.py
--rw-r--r--   0        0        0      209 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/logger.py
--rw-r--r--   0        0        0     4232 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/opc_types.py
--rw-r--r--   0        0        0     1178 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/pythoncom_datatypes.py
--rw-r--r--   0        0        0     5651 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/system_health.py
--rw-r--r--   0        0        0      598 2022-11-22 14:12:11.991756 openopc2-0.1.7/openopc2/utils.py
--rw-r--r--   0        0        0     1137 2022-11-22 14:12:11.991756 openopc2-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openopc2-0.1.7/setup.py
--rw-r--r--   0        0        0     9696 1970-01-01 00:00:00.000000 openopc2-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    16490 2022-11-29 13:35:27.893951 openopc2-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     8370 2022-11-29 13:35:27.897951 openopc2-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/__init__.py
+-rw-r--r--   0        0        0       69 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/__main__.py
+-rw-r--r--   0        0        0    11641 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/cli.py
+-rw-r--r--   0        0        0      815 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/config.py
+-rw-r--r--   0        0        0    39325 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/da_client.py
+-rw-r--r--   0        0        0     8842 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/da_com.py
+-rw-r--r--   0        0        0      669 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/exceptions.py
+-rw-r--r--   0        0        0     1227 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/gateway_proxy.py
+-rw-r--r--   0        0        0     3559 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/gateway_server.py
+-rw-r--r--   0        0        0     3852 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/gateway_service.py
+-rw-r--r--   0        0        0      209 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/logger.py
+-rw-r--r--   0        0        0     4232 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/opc_types.py
+-rw-r--r--   0        0        0     1178 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/pythoncom_datatypes.py
+-rw-r--r--   0        0        0     5651 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/system_health.py
+-rw-r--r--   0        0        0      598 2022-11-29 13:35:27.905951 openopc2-0.1.9/openopc2/utils.py
+-rw-r--r--   0        0        0     1138 2022-11-29 13:35:27.905951 openopc2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openopc2-0.1.9/setup.py
+-rw-r--r--   0        0        0     9696 1970-01-01 00:00:00.000000 openopc2-0.1.9/PKG-INFO
```

### Comparing `openopc2-0.1.7/LICENSE.txt` & `openopc2-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/README.md` & `openopc2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/cli.py` & `openopc2-0.1.9/openopc2/cli.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/config.py` & `openopc2-0.1.9/openopc2/config.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/da_client.py` & `openopc2-0.1.9/openopc2/da_client.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/da_com.py` & `openopc2-0.1.9/openopc2/da_com.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/exceptions.py` & `openopc2-0.1.9/openopc2/exceptions.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/gateway_proxy.py` & `openopc2-0.1.9/openopc2/gateway_proxy.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/gateway_server.py` & `openopc2-0.1.9/openopc2/gateway_server.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/gateway_service.py` & `openopc2-0.1.9/openopc2/gateway_service.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/opc_types.py` & `openopc2-0.1.9/openopc2/opc_types.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/pythoncom_datatypes.py` & `openopc2-0.1.9/openopc2/pythoncom_datatypes.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/system_health.py` & `openopc2-0.1.9/openopc2/system_health.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/openopc2/utils.py` & `openopc2-0.1.9/openopc2/utils.py`

 * *Files identical despite different names*

### Comparing `openopc2-0.1.7/pyproject.toml` & `openopc2-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "openopc2"
-version = "0.1.7"
+version = "0.1.9"
 description = "OPC library with a Windows gateway enabling non-Windows clients to access OPC-DA calls."
 license = "GPL-2.0-or-later"
 readme = "README.md"
 authors = [
     "Lorenz Padberg <lorenz.padberg@iterativ.ch>",
     "Elia Bieri <elia.bieri@iterativ.ch>",
 ]
 repository = "https://github.com/iterativ/openopc2"
 keywords = ["opc", "openopc", "opc-da", "opc classic"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
-    "Intended Audience :: Manufacturing"
+    "Intended Audience :: Manufacturing",
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 pyro5 = "^5.14"
 WMI = { version = "^1.5.1", markers = "sys_platform == 'win32'" }
 pywin32 = { version = "304", markers = "sys_platform == 'win32'" }
```

### Comparing `openopc2-0.1.7/setup.py` & `openopc2-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pyro5>=5.14,<6.0', 'rich>=12.6.0,<13.0.0', 'typer[all]>=0.6.1,<0.7.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['WMI>=1.5.1,<2.0.0', 'pywin32==304']}
 
 setup_kwargs = {
     'name': 'openopc2',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'OPC library with a Windows gateway enabling non-Windows clients to access OPC-DA calls.',
     'long_description': '<p align="center">\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/open-opc.png" alt="LinuxSetup" width="700"/>\n</p>\n\n\n[![PyPI version](https://badge.fury.io/py/openopc2.svg)](https://badge.fury.io/py/openopc2)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openopc2)\n\n\n\n**OpenOPC 2**  is a Python Library for OPC DA. It is Open source and free for everyone. It allows you to use\n[OPC Classic](https://opcfoundation.org/about/opc-technologies/opc-classic/) (OPC Data Access) in \nmodern Python environments. OPC Classic is a pure Windows technology by design, but this library includes a Gateway Server\nthat lets you use OPC Classic on any architecture (Linux, MacOS, Windows, Docker). So this Library creates a gateway \nbetween 2022 and the late 90ties. Like cruising into the sunset with Marty McFly in a Tesla. \n\nOpenOPC 2 is based on the OpenOPC Library that was initially created by Barry Barnleitner and hosted on Source Forge, but\nIt was completely refactorerd and migrated to Python 3.8+\n\n\n# 🔥 Features\n\n* An OpenOPC Gateway Service (a Windows service providing remote access \nto the OpenOPC library, which is useful to avoid DCOM issues).\n* Command Line Interface (CLI)\n* Enables you to use OPC Classic with any Platform\n* CLI and Gateway are independent Executables that do not require Python\n* A system check module (allows you to check the health of your system)\n* A free OPC automation wrapper (required DLL file).\n* General documentation with updated procedures (this file).\n\n# 🐍 OpenOPC vs OpenOPC 2\n\nOpen OPC 2 is based on OpenOPC and should be seen as a successor. If you already have an application that is based on \nOpenOPC, you can migrate with a minimal effort. Our main motivation to build this new version was to improve the developer\nexperience and create a base for other developers that is easier to maintain, test and work with...\n\n* Simpler installation\n* Mostly the same api (but we take the freedom to not be compatible)\n* No memory leak in the OpenOpcService 🎉\n* Python 3.8+ (tested with 3.10)\n* Typings \n* Pyro5, increased security\n* We added tests 😎\n* Refactoring for increased readablity\n* Nicer CLI\n* Pipy Package \n\n\n\n# 🚀 Getting started\n##  Windows local installation\n\nThe quickest way to start is the cli application. Start your OPC server and use the openopc2.exe cli application for test (no python\ninstallation required). \n\n\n\n\n\nNow you know that your OPC server is talking to OpenOPC 2. Then lets get started with python. If you use OpenOPC 2 with \nPython in windows directly you are **limited to a 32bit Python** installation. This is because the dlls of OPC are 32bit.\nIf you prefere working with a 64bit Python version you can simply use the With OpenOPC Gateway. \n\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/WindowsSetup.png" alt="WindowsSetup" width="400"/>\n\nYou must install the gbda_aut.dll (in /lib) which is the GrayboxOpcDa wrapper. \n\nhttp://gray-box.net/daawrapper.php?lang=en\n\n```console\npython -m openopc2 servers\n```\n\n\n\n## Multi plattform installation\nOne of the main benefits of OpenOPC 2 ist the OpenOPC gateway. This enables you to use any modern platform for \ndevelopting your application. Start the OpenOPC service in the Windows environment where the OPC server is running. \nThe Service starts a server (Pyro5) that lets you use the OpenOPC2 OpcDaClient on another machine. Due to the magic of\nPyro (Python Remote Objects) the developer experience and usage of the Library remains the same as if you worke int the \nlocal Windows setup. \n\n\n\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/LinuxSetup.png" alt="LinuxSetup" width="700"/>\n\nOn the Windows Machine open the console as administrator. \n\n```shell\nopenopcservice install\nopenopcservice start\n```\n\nOn your Linux machine\n```\npip install openopc2\nopenopc2 --install`\n```\n\npython\n```python\nfrom openopc2.da_client import OpcDaClient\n\n\n\n```\n\n# ⚙️ Configuration \n\nThe configuration of the OpenOpc 2 libray and the OpenOpcGateway is done via environment variables. To initiate them,\nsimply run:\n\n```shell\nOpenOPC install \n```\n\n```\nOPC_CLASS=Matrikon.OPC.Automation;Graybox.OPC.DAWrapper;HSCOPC.Automation;RSI.OPCAutomation;OPC.Automation\nOPC_CLIENT=OpenOPC\nOPC_GATE_HOST=192.168.1.96    # IMPORTANT: Replace with your IP address\nOPC_GATE_PORT=7766\nOPC_HOST=localhost\nOPC_MODE=dcom\nOPC_SERVER=Hci.TPNServer;HwHsc.OPCServer;opc.deltav.1;AIM.OPC.1;Yokogawa.ExaopcDAEXQ.1;OSI.DA.1;OPC.PHDServerDA.1;Aspen.Infoplus21_DA.1;National Instruments.OPCLabVIEW;RSLinx OPC Server;KEPware.KEPServerEx.V4;Matrikon.OPC.Simulation;Prosys.OPC.Simulation\n```\n\n* If they are not set, open a command prompt window to do that by \ntyping:\n\n```\nC:\\>set ENV_VAR=VALUE\nC:\\>set OPC_GATE_HOST=172.16.4.22    # this is an example\n```\n\n* Make sure the firewall is allowed to keep the port 7766 open. If in \ndoubt, and you\'re doing a quick test, just turn off your firewall \ncompletely.\n\n* For easy testing, make sure an OPC server is installed in your Windows \nbox (i.e. Matrikon OPC Simulation Server).\n\n* The work environment for testing these changes was a remote MacOs with Window10 64bit host and the Matrikon simulation\nserver. \n\n* Register the OPC automation wrapper ( `gbda_aut.dll` ) by typing this \nin the command line:\n\n```shell\nC:\\openopc2\\lib>regsvr32 gbda_aut.dll\n```\n\n* If, for any reason, you want to uninstall this file and remove it from \nyour system registry later, type this in the command line:\n\n```shell\nC:\\openopc2\\lib>regsvr32 gbda_aut.dll -u\n```\n\n\n# CLI\n\nThe CLI (Command Line Interface) lets you use OpenOPC2 in the shell and offers you a quick way to explore your opc server\nand the OpenOPC DA client without the need of writing Python code.\n\nThe documentation of the CLI can be found [here](CLI.md)\n\n<p>\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/cli_server-info.png" alt="WindowsSetup" width="400"/>\n</p>\n\n<p>\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/cli_read.png" alt="WindowsSetup" width="400"/>\n</p>\n\n\n<p>\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/cli_write.png" alt="WindowsSetup" width="400"/>\n</p>\n\n\n<p>\n<img src="https://github.com/iterativ/openopc2/raw/develop/doc/assets/cli_properties.png" alt="WindowsSetup" width="400"/>\n</p>\n\n\n\n# OpenOPC Gateway\n\nThis task can be completed from one of two ways (make sure to have it \ninstalled first):\n\n* By clicking the `Start` link on the "OpenOPC Gateway Service" from the \n"Services" window (Start -> Control Panel -> System and Security -> \nAdministrative Tools).\n* By running the `net start SERVICE` command like this:\n\n```shell\nC:\\openopc2\\bin> zzzOpenOPCService\n```\n\n* If you have problems starting the service, you can also try to start \nthis in "debug" mode:\n\n```shell\nC:\\openopc2\\src>python OpenOPCService.py debug\n```\n\n\n\n```shell\nC:\\openopc2\\>net stop zzzOpenOPCService\n```\n\n### Configure the way the OpenOPC Gateway Service starts\n\nIf you are going to use this service frequently, it would be better to \nconfigure it to start in "automatic" mode. To do this:\n\n* Select the "OpenOPC Gateway Service" from the "Services" window \n(Start -> Control Panel -> System and Security -> Administrative Tools).\n* Right-click and choose "Properties".\n* Change the startup mode to "Automatic". Click "Apply" and "OK" \nbuttons.\n* Start the service (if not already started).\n\n\n\n\n## 🙏 Credits\n\nOpenOPC 2 is based on the OpenOPC python library that was originally created by Barry Barnleitner and its many Forks on\nGithub. Without the great work of all the contributors, this would not be possible. Contribution is open for everyone. \n\nThe authors of the var package are:\n\n\n| Years     |      | Name                | User |\n|-----------|------|---------------------|------|\n| 2008-2012 | 🇺🇸 | Barry Barnreiter    | barry_b@users.sourceforge.net |\n| 2014      | 🇷🇺 | Anton D. Kachalov   | barry_b@users.sourceforge.net |\n| 2017      | 🇻🇪 | José A. Maita       | jose.a.maita@gmail.com|\n| 2022      | 🇨🇭 | Lorenz Padberg      | renzop |\n| 2022      | 🇨🇭 | Elia Bieri          | eliabieri |\n\n\n\n\n## 📜 License\n\nThis software is licensed under the terms of the GNU GPL v2 license plus \na special linking exception for portions of the package. This license is \navailable in the `LICENSE.txt` file.\n',
     'author': 'Lorenz Padberg',
     'author_email': 'lorenz.padberg@iterativ.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/iterativ/openopc2',
```

### Comparing `openopc2-0.1.7/PKG-INFO` & `openopc2-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openopc2
-Version: 0.1.7
+Version: 0.1.9
 Summary: OPC library with a Windows gateway enabling non-Windows clients to access OPC-DA calls.
 Home-page: https://github.com/iterativ/openopc2
 License: GPL-2.0-or-later
 Keywords: opc,openopc,opc-da,opc classic
 Author: Lorenz Padberg
 Author-email: lorenz.padberg@iterativ.ch
 Requires-Python: >=3.8,<3.12
```

