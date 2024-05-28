# Comparing `tmp/pawnlib-1.1.8.tar.gz` & `tmp/pawnlib-2.0.tar.gz`

## Comparing `pawnlib-1.1.8.tar` & `pawnlib-2.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
--rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-1.1.8/README.md
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/.DS_Store
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__main__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__version__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/asyncio/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/asyncio/run.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/templates/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/templates/app_with_logging.tmpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/__init__.py
--rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/aws.py
--rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/banner.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/docker.py
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/gs.py
--rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/http.py
--rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/icon.py
--rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/info.py
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/init.py
--rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/main_cli.py
--rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/main_cli_with_required.py__
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/net.py
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/pawns_cli.py__
--rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/proxy.py
--rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/rpc.py
--rwxr-xr-x   0        0        0    11482 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/top.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/wallet.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/docker_echo.tmpl
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/docker_planet.tmpl
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/__fix_import.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/__init__.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/configure.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/console.py
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/first_run_checker.py
--rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/globalconfig.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/docker/__init__.py
--rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/docker/async_docker.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/input/__init__.py
--rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/input/prompt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/__init__.py
--rw-r--r--   0        0        0    55490 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/color_print.py
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/file.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/__init__.py
--rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/net.py
--rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/server.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/__init__.py
--rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/check.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/constants.py
--rw-r--r--   0        0        0    83698 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/converter.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/date_utils.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/defines.py
--rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/generator.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/__init__.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/genesis.py
--rw-r--r--   0        0        0    80276 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/http.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/icx_raw_singer.py
--rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/icx_signer.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/in_memory_zip.py
--rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/log.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/notify.py
--rw-r--r--   0        0        0    25836 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/operate_handler.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-1.1.8/.gitignore
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pawnlib-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-2.0/README.md
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/__main__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/__version__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/asyncio/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/asyncio/run.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/builder/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/builder/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/builder/templates/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/builder/templates/app_with_logging.tmpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/__init__.py
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/aws.py
+-rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/banner.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/docker.py
+-rwxr-xr-x   0        0        0     3579 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/gs.py
+-rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/http.py
+-rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/icon.py
+-rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/info.py
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/init.py
+-rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/main_cli.py
+-rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/main_cli_with_required.py__
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/net.py
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/pawns_cli.py__
+-rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/proxy.py
+-rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/rpc.py
+-rwxr-xr-x   0        0        0    11546 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/top.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/wallet.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/templates/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/templates/docker_echo.tmpl
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/cli/templates/docker_planet.tmpl
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/__fix_import.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/__init__.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/configure.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/console.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/first_run_checker.py
+-rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/config/globalconfig.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/docker/__init__.py
+-rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/docker/async_docker.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/input/__init__.py
+-rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/input/prompt.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/output/__init__.py
+-rw-r--r--   0        0        0    59689 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/output/color_print.py
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/output/file.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/resource/__init__.py
+-rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/resource/net.py
+-rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/resource/server.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/__init__.py
+-rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/check.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/constants.py
+-rw-r--r--   0        0        0    84594 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/converter.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/date_utils.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/defines.py
+-rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/typing/generator.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/__init__.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/genesis.py
+-rw-r--r--   0        0        0    80942 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/http.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/icx_raw_singer.py
+-rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/icx_signer.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/in_memory_zip.py
+-rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/log.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/notify.py
+-rw-r--r--   0        0        0    25836 2020-02-02 00:00:00.000000 pawnlib-2.0/pawnlib/utils/operate_handler.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-2.0/.gitignore
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-2.0/pyproject.toml
+-rw-r--r--   0        0        0    13035 2020-02-02 00:00:00.000000 pawnlib-2.0/PKG-INFO
```

### Comparing `pawnlib-1.1.8/README.md` & `pawnlib-2.0/README.md`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/__init__.py` & `pawnlib-2.0/pawnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/__main__.py` & `pawnlib-2.0/pawnlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/asyncio/run.py` & `pawnlib-2.0/pawnlib/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/builder/generator.py` & `pawnlib-2.0/pawnlib/builder/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/builder/templates/app_with_logging.tmpl` & `pawnlib-2.0/pawnlib/builder/templates/app_with_logging.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/aws.py` & `pawnlib-2.0/pawnlib/cli/aws.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/banner.py` & `pawnlib-2.0/pawnlib/cli/banner.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/docker.py` & `pawnlib-2.0/pawnlib/cli/docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/gs.py` & `pawnlib-2.0/pawnlib/cli/gs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
-from pawnlib.config import  pawn
+from pawnlib.config import pawn
+from pawnlib.output import color_print
+
 try:
     import eth_keys
-except Exception  as e:
-    pawn.console.log("[red]Exception[/red] Required  'eth_keys' module. 'pip3 install eth_keys'" )
+except Exception as e:
+    pawn.console.log("[red]Exception[/red] Required  'eth_keys' module. 'pip3 install eth_keys'")
 
-import argparse
 from pawnlib.builder.generator import generate_banner
 from pawnlib.__version__ import __version__ as _version
 
-from pawnlib.utils.genesis  import genesis_generator, create_cid
+from pawnlib.utils.genesis import genesis_generator, create_cid
 from pawnlib.utils.in_memory_zip import read_genesis_dict_from_zip
 from pawnlib.output import is_file, print_json, open_json
 from pawnlib.typing import get_size
 from pawnlib.input.prompt import CustomArgumentParser, ColoredHelpFormatter
 
-
 __description__ = "Genesis Tool"
 __epilog__ = (
     "Usage examples:\n"
     "1. Generate a genesis file from a genesis.json file:\n"
     "     pawns gs gen -i genesis.json -o icon_genesis.zip\n\n"
     "2. Display information about a genesis zip file: \n"
     "     pawns gs info genesis.zip\n\n"
@@ -37,15 +37,14 @@
         epilog=__epilog__
     )
     parser = get_arguments(parser)
     return parser
 
 
 def get_arguments(parser=None):
-
     parser.add_argument(
         'command',
         help='gen, info',
         nargs="?",
         choices=['gen', 'info']
     )
     parser.add_argument(
@@ -56,14 +55,24 @@
 
     parser.add_argument('-i', '--input-genesis', metavar='genesis.json', help=f'genesis.json', default=None)
     parser.add_argument('-b', '--base-dir', metavar='base_dir', help=f'base dir', default=".")
     parser.add_argument('-o', '--output-file', metavar='output filename', help=f'output filename', default="icon_genesis.zip")
     return parser
 
 
+def print_hex_value(name, value):
+    if value:
+        pawn.console.log(f"{name} = {value} ({int(value, 16)})")
+
+
+def get_hex_value(value):
+    if value:
+        return  f"{value} [bright_black]({int(value, 16)})[/bright_black]"
+
+
 def main():
     banner = generate_banner(
         app_name="Genesis",
         author="jinwoo",
         description="ICON utility",
         font="graffiti",
         version=_version
@@ -82,20 +91,22 @@
     if args.command == "gen":
         genesis_file = f"{args.base_dir}/{args.input_genesis}"
         json_dict = open_json(genesis_file)
         cid = genesis_generator(genesis_json_or_dict=json_dict, base_dir=args.base_dir, genesis_filename=args.output_file)
         pawn.console.log(f"CID = {cid}")
 
     elif args.command == "info" and is_file(args.genesis_zip_file):
-            genesis_json = read_genesis_dict_from_zip(args.genesis_zip_file)
-            print_json(genesis_json)
-            cid = create_cid(genesis_json)
-            nid = genesis_json.get('nid')
-            pawn.console.log(f"FileName  = {args.genesis_zip_file} ({get_size(args.genesis_zip_file)})")
-            pawn.console.log(f"CID       = {cid} ({int(cid, 16)})")
-            pawn.console.log(f"NID       = {nid} ({int(nid, 16)})")
+        genesis_json = read_genesis_dict_from_zip(args.genesis_zip_file)
+        # print_json(genesis_json)
+
+        cid = create_cid(genesis_json)
+        nid = genesis_json.get('nid', "")
 
+        color_print.print_kv("genesis_json", genesis_json)
 
+        color_print.print_kv("FileName", f"{args.genesis_zip_file} ({get_size(args.genesis_zip_file)})")
+        color_print.print_kv("cid", get_hex_value(cid))
+        color_print.print_kv("nid", get_hex_value(nid))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pawnlib-1.1.8/pawnlib/cli/http.py` & `pawnlib-2.0/pawnlib/cli/http.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/icon.py` & `pawnlib-2.0/pawnlib/cli/icon.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/info.py` & `pawnlib-2.0/pawnlib/cli/info.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/init.py` & `pawnlib-2.0/pawnlib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/main_cli.py` & `pawnlib-2.0/pawnlib/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/main_cli_with_required.py__` & `pawnlib-2.0/pawnlib/cli/main_cli_with_required.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/net.py` & `pawnlib-2.0/pawnlib/cli/net.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/pawns_cli.py__` & `pawnlib-2.0/pawnlib/cli/pawns_cli.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/proxy.py` & `pawnlib-2.0/pawnlib/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/rpc.py` & `pawnlib-2.0/pawnlib/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/top.py` & `pawnlib-2.0/pawnlib/cli/top.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/env python3
 import argparse
 from pawnlib.builder.generator import generate_banner
 from pawnlib.__version__ import __version__ as _version
 from pawnlib.config import pawn, pconf
-from pawnlib.typing import StackList, list_to_oneline_string, str2bool
-from pawnlib.resource import SystemMonitor, get_cpu_load, get_interface_ips, get_platform_info, get_mem_info, get_netstat_count
+from pawnlib.typing import StackList, list_to_oneline_string, str2bool, shorten_text
+from pawnlib.resource import (
+    SystemMonitor, get_cpu_load, get_interface_ips, get_platform_info,
+    get_mem_info, get_netstat_count, get_hostname
+)
 from pawnlib.output import is_file
 import os
 import re
 
 from rich.live import Live
 from rich.table import Table
 from rich.align import Align
 from rich.text import Text
+from rich.panel import Panel
+from rich import box
 from pawnlib.typing import todaydate
 import time
 
 __description__ = "This is a tool to measure your server's resources."
 
 __epilog__ = (
     "This tool is designed for monitoring your server's resource usage.\n"
@@ -46,15 +51,15 @@
 else:
     PROCFS_PATH = "/proc"
 
 
 class CustomArgumentParser(argparse.ArgumentParser):
     def error(self, message):
         self.print_help()
-        # sys_exit(message, 2)
+
 
 def get_parser():
     # parser = argparse.ArgumentParser(description='monitor', epilog=epilog_tuple)
     parser = argparse.ArgumentParser(description='monitor', epilog=''.join(__epilog__))
     parser = get_arguments(parser)
     return parser
 
@@ -82,15 +87,15 @@
             "net_out": 100,
             "usr": 80,
             "sys": 80,
             "mem_used": 99.5,
             "disk_read":  100,
             "disk_write":  100,
             "load":  int(cores),
-            "io":  int(cores) * 2,
+            "i/o":  int(cores) * 2,
             "cached":  10,
         }
         self.warning_percent = warning_percent
         self.medium_percent = medium_percent
         self.low_percent = low_percent
 
     @staticmethod
@@ -183,119 +188,116 @@
                 # log_path=f"{args.base_dir}/logs",
                 stdout=stdout,
                 use_hook_exception=True,
                 show_path=False, #hide line numbers
             ),
         )
     print_banner()
-    lines = []
     system_info = get_platform_info()
+    hostname = shorten_text(get_hostname(), width=20, placeholder='...')
     system_monitor = SystemMonitor(interval=args.interval, proc_path=PROCFS_PATH)
-    table_title = f"Server status <{system_info.get('model')},  {system_info.get('cores')} cores, {get_mem_info().get('mem_total')} GB>"
+    table_title = f"🐰 {hostname} <{system_info.get('model')},  {system_info.get('cores')} cores, {get_mem_info().get('mem_total')} GB> 🐰"
 
     if args.print_type == "live":
-        print_live_status(table_title=table_title,  system_info=system_info, system_monitor=system_monitor)
+        print_live_type_status(table_title=table_title,  system_info=system_info, system_monitor=system_monitor)
     # elif args.print_type == "tab":
     #     print_tabulate_status(system_monitor=system_monitor)
     elif args.print_type == "line":
-        count = 0
-        while True:
-            columns, term_rows = os.get_terminal_size()
+        print_line_type_status(table_title=table_title, system_info=system_info, system_monitor=system_monitor, args=args)
 
-            data = get_resources_status(system_monitor=system_monitor, args=args)
-            line = []
-            columns = []
-            for column_key, value in data.items():
-                align_space = max([len(str(value)), len(column_key)]) + 2
-                columns.append(f"[blue][u]{column_key:^{align_space}}[/u][/blue]")
-                _value = CriticalText(column_key, value, cores=system_info.get('cores', 1), align_space=align_space).return_text()
-                line.append(_value)
-            # pawn.console.print(list_to_oneline_string(columns, " | ")) if count % 15 == 0 else None
-            print_line_status(columns) if count % term_rows == 0 else None
-            print_line_status(line)
-            count += 1
+
+def print_line_type_status(table_title, system_info, system_monitor, args):
+    count = 0
+    while True:
+        columns, term_rows = os.get_terminal_size()
+        data = get_resources_status(system_monitor=system_monitor, args=args)
+        line = []
+        columns = []
+        for column_key, value in data.items():
+            align_space = max([len(str(value)), len(column_key)]) + 2
+            columns.append(f"[blue][u]{column_key:^{align_space}}[/u][/blue]")
+            _value = CriticalText(column_key, value, cores=system_info.get('cores', 1), align_space=align_space).return_text()
+            line.append(_value)
+
+        if count % term_rows == 0:
+            # print(f"\t{table_title}")
+
+            pawn.console.print(Panel(table_title, expand=False))
+            print_line_status(columns)
+
+        print_line_status(line)
+
+        count += 1
 
 
 def print_line_status(line):
+    pawn.console.print("", end="│")
     for cell in line:
         pawn.console.print(cell, end="│")
     print()
 
 
-def print_live_status(table_title="",  system_info={}, system_monitor=None):
+def print_live_type_status(table_title="",  system_info={}, system_monitor: SystemMonitor = None):
     lines = []
-
-    with Live(console=pawn.console, refresh_per_second=1) as live_table:
+    with Live(console=pawn.console, refresh_per_second=2) as live_table:
         while True:
             columns, rows = os.get_terminal_size()
             diff_rows = len(lines) - rows
-            table = Table(title=table_title)
+            table = Table(title=table_title, box=box.SIMPLE)
 
             data = get_resources_status(system_monitor=system_monitor)
             line = []
             for column_key, value in data.items():
-                table.add_column(column_key)
+                table.add_column(column_key, justify='right' )
                 line.append(CriticalText(column_key, value, cores=system_info.get('cores', 1)).return_text())
             lines.append(line)
 
             for line in lines:
                 table.add_row(*line)
 
             if len(lines) >= rows - 5:
                 lines.pop(0)
             if diff_rows > -6:
                 del lines[:6]
             live_table.update(Align.center(table))
 
 
-# def print_tabulate_status(system_monitor=None):
-#     _data = []
-#     while True:
-#         data = get_resources_status(system_monitor=system_monitor)
-#         headers = list(data.keys())
-#         values = list(data.values())
-#         _data.append(values)
-#         print(tabulate(_data, headers=headers, tablefmt="grid"))
-#
-#     print()
-
-
-def get_resources_status(system_monitor={}, args=None):
+def get_resources_status(system_monitor: SystemMonitor = None, args=None):
     if not args:
         args = pconf().args
 
     if args.command == "net":
         netstat = get_netstat_count(proc_path=PROCFS_PATH)
         data = {
             "time": todaydate("time_sec"),
         }
         data.update(netstat.get('COUNT'))
         time.sleep(args.interval)
     else:
         memory = system_monitor.get_memory_status()
         network, cpu, disk = system_monitor.get_network_cpu_status()
-        # memory_unit = memory.get('unit').replace('B', "")
+        # memory_unit = memory.get('unit').replace('B', "")w
         memory_unit = memory.get('unit')
 
         data = {
             "time": todaydate("time_sec"),
             "net_in": f"{network['Total'].get('recv'):.2f}M",
             "net_out": f"{network['Total'].get('sent'):.2f}M",
             "pk_in": f"{network['Total'].get('packets_recv')}",
             "pk_out": f"{network['Total'].get('packets_sent')}",
             "load": f"{get_cpu_load()['1min']}",
             "usr": f"{cpu.get('usr')}%",
             "sys": f"{cpu.get('sys')}%",
-            "io": f"{cpu.get('io_wait')}",
+            "i/o": f"{cpu.get('io_wait')}",
             "disk_read":  f"{disk['total'].get('read_mb')}M",
             "disk_write":  f"{disk['total'].get('write_mb')}M",
-            "mem_total": f"{memory.get('total')}{memory_unit}",
+            "mem_total": f"{memory.get('total'):.1f}{memory_unit}",
             # "mem_used": f"{memory.get('percent')}%",
-            "mem_free": f"{memory.get('free')}{memory_unit}",
-            "cached": f"{memory.get('cached')}{memory_unit}",
+            "mem_free": f"{memory.get('free'):.1f}{memory_unit}",
+            "cached": f"{memory.get('cached'):.1f}{memory_unit}",
         }
     return data
 
 
 if __name__ == '__main__':
     try:
         main()
```

### Comparing `pawnlib-1.1.8/pawnlib/cli/wallet.py` & `pawnlib-2.0/pawnlib/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/websocket.py` & `pawnlib-2.0/pawnlib/cli/websocket.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/templates/docker_echo.tmpl` & `pawnlib-2.0/pawnlib/cli/templates/docker_echo.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/cli/templates/docker_planet.tmpl` & `pawnlib-2.0/pawnlib/cli/templates/docker_planet.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/config/__fix_import.py` & `pawnlib-2.0/pawnlib/config/__fix_import.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/config/configure.py` & `pawnlib-2.0/pawnlib/config/configure.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/config/console.py` & `pawnlib-2.0/pawnlib/config/console.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/config/first_run_checker.py` & `pawnlib-2.0/pawnlib/config/first_run_checker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/config/globalconfig.py` & `pawnlib-2.0/pawnlib/config/globalconfig.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/docker/async_docker.py` & `pawnlib-2.0/pawnlib/docker/async_docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/input/__init__.py` & `pawnlib-2.0/pawnlib/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/input/prompt.py` & `pawnlib-2.0/pawnlib/input/prompt.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/output/__init__.py` & `pawnlib-2.0/pawnlib/output/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,14 +41,17 @@
     classdump,
     kvPrint,
     print_json,
     print_syntax,
     pretty_json,
     print_aligned_text,
     print_var,
+    create_kv_table,
+    print_kv,
+    print_grid,
     debug_logging,
     align_text,
     print_progress_bar,
     get_colorful_object,
     syntax_highlight,
     ProgressTime,
     NoTraceBackException
```

### Comparing `pawnlib-1.1.8/pawnlib/output/color_print.py` & `pawnlib-2.0/pawnlib/output/color_print.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 import json
 import getpass
 import traceback
 import inspect
 import executing
 from contextlib import contextmanager, AbstractContextManager
 
-from pawnlib.typing import converter, date_utils, list_to_oneline_string, const, is_include_list, remove_tags, remove_ascii_color_codes,timestamp_to_string, is_hex
+from pawnlib.typing import (
+    converter, date_utils, list_to_oneline_string, const, is_include_list, remove_tags,
+    remove_ascii_color_codes,timestamp_to_string, is_hex, is_json
+)
 from pawnlib.config import pawnlib_config as pawn, global_verbose
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name
 from pygments.formatters import Terminal256Formatter
 from rich.syntax import Syntax
 from rich.table import Table
+from rich.pretty import Pretty
 from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 from rich import print as rprint
 from typing import Union, Callable
 from datetime import datetime
 import textwrap
 from requests.structures import CaseInsensitiveDict
 
@@ -1494,14 +1498,111 @@
                      f"\t[italic] ({type(data).__name__}), {data_length}", _stack_offset=2)
     if isinstance(data, dict) or isinstance(data, list):
         print(syntax_highlight(data, **kwargs))
     else:
         pawn.console.print(f"\t[white bold]{data}\n")
 
 
+def create_kv_table(padding=0, key_ratio=2, value_ratio=7):
+    table = Table(
+        padding=padding,
+        pad_edge=False,
+        expand=True,
+        show_header=False,
+        show_footer=False,
+        show_edge=False,
+        show_lines=False,
+        box=None
+    )
+
+    table.add_column("Key", no_wrap=False, justify="left", style="bold yellow", min_width=padding, ratio=key_ratio)
+    table.add_column("Separator", no_wrap=False, justify="left", width=3)
+    table.add_column("Value", no_wrap=True, justify="left", ratio=value_ratio, max_width=50)
+    table.add_column("Debug Info", justify="right", style="grey84")
+
+    return table
+
+
+def get_pretty_value(value):
+    if isinstance(value, (dict, list)):
+        return Syntax(json.dumps(value, indent=4), "json", theme="material", line_numbers=False)
+    else:
+        if value and is_json(value):
+            __loaded_json = json.loads(value)
+            return Pretty(json.loads(value))
+        return value
+
+
+def print_kv(key="", value="", symbol="░",  separator=":", padding=1, key_ratio=1, value_ratio=7):
+    """
+    Print a key-value pair with a symbol, padding, and value size information.
+
+    :param key: The key to print. Defaults to an empty string.
+    :param value: The value associated with the key. Defaults to an empty string.
+    :param symbol: A symbol to prepend to the key. Defaults to a star emoji.
+    :param separator: The separator between the key and the value. Defaults to a colon.
+    :param padding: The padding between columns. Defaults to 5.
+    :param key_ratio: The ratio of the table width allocated for keys. Defaults to 1z.
+    :param value_ratio: The ratio of the table width allocated for values. Defaults to 7.
+
+    Example:
+
+        .. code-block:: python
+
+            print_kv(key="Name", value="John Doe", symbol="👤")
+            # Output:
+            # 👤 Name   :   John Doe   str[bright_black](8)[/bright_black]
+
+            print_kv(key="Age", value=30, symbol="🔢", padding=3)
+            # Output:
+            # 🔢 Age : 30   int[bright_black](2)[/bright_black]
+
+    """
+    table = create_kv_table(padding=padding, key_ratio=key_ratio, value_ratio=value_ratio)
+    value_info = f"{type(value).__name__}[bright_black]({converter.get_value_size(value)})[/bright_black]"
+    table.add_row(f"{symbol} {key}", f"[grey69] {separator} [/grey69]", get_pretty_value(value), value_info)
+    pawn.console.print(table)
+
+
+def print_grid(data: dict = None, title="", symbol="░", separator=":",  padding=0, key_ratio=1, value_ratio=7):
+    """
+    Print a grid layout with a title and optional padding and edge padding.
+
+    :param data: The data to display in the grid. Default is None.
+    :param title: The title of the grid. Default is an empty string.
+    :param symbol: The symbol used for the grid. Default is '░'.  or 🔘★⭐️ ■ ▓  ▒ ░
+    :param separator: The separator between the key and the value. Defaults to a colon.
+    :param padding: The padding around each cell. Default is 0.
+    :param key_ratio: The ratio of the table width allocated for keys. Defaults to 1.
+    :param value_ratio: The ratio of the table width allocated for values. Defaults to 7.
+
+    Example:
+
+        .. code-block:: python
+
+            data = {"Item 1": 123, "Item 2": 456}
+            print_grid(data, title="Inventory", symbol="■", padding=1, pad_edge=False)
+
+            # Output will display a grid with the title "Inventory", using '■' as the symbol,
+            # 1 padding around each cell, and no padding on the edge.
+
+    """
+    table = create_kv_table(padding=padding, key_ratio=key_ratio, value_ratio=value_ratio)
+    pawn.console.rule(f" ✨✨{title}✨✨", style="white")
+    if not isinstance(data, dict):
+        pawn.console.log(f"'{data}' is not dict")
+        return
+
+    for key, value in data.items():
+        value_info = f"{type(value).__name__}[bright_black]({converter.get_value_size(value)})[/bright_black]"
+        table.add_row(f"{symbol} {key}", f"[grey69] {separator} [/grey69]", get_pretty_value(value), value_info)
+    pawn.console.print(table)
+    pawn.console.rule("", style="white")
+
+
 def print_aligned_text(left_text, right_text, filler='.'):
     """
     Print left and right text aligned with filler in between.
 
     :param left_text: The text to be aligned on the left side.
     :param right_text: The text to be aligned on the right side.
     :param filler: The character used to fill the space between left and right text. Default is '.'.
```

### Comparing `pawnlib-1.1.8/pawnlib/output/file.py` & `pawnlib-2.0/pawnlib/output/file.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/resource/__init__.py` & `pawnlib-2.0/pawnlib/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/resource/net.py` & `pawnlib-2.0/pawnlib/resource/net.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/resource/server.py` & `pawnlib-2.0/pawnlib/resource/server.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/typing/__init__.py` & `pawnlib-2.0/pawnlib/typing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     base64ify,
     base64_decode,
     UpdateType,
     convert_hex_to_int,
     convert_dict_hex_to_int,
     hex_to_number,
     get_size,
+    get_value_size,
     convert_bytes,
     str2bool,
     flatten,
     flatten_list,
     flatten_dict,
     recursive_update_dict,
     dict_to_line,
```

### Comparing `pawnlib-1.1.8/pawnlib/typing/check.py` & `pawnlib-2.0/pawnlib/typing/check.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/typing/constants.py` & `pawnlib-2.0/pawnlib/typing/constants.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/typing/converter.py` & `pawnlib-2.0/pawnlib/typing/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1207,14 +1207,56 @@
 
     if attr:
         return [return_size, file_attr]
 
     return return_size
 
 
+def get_value_size(value):
+    """
+    Determine the size of the value based on its type.
+
+    :param value: The value to determine the size of.
+    :type value: Any
+    :return: The size of the value.
+    :rtype: int
+
+    Example:
+
+        .. code-block:: python
+
+            get_value_size(None)
+            # >> 0
+
+            get_value_size([1, 2, 3])
+            # >> 3
+
+            get_value_size({"key1": "value1", "key2": "value2"})
+            # >> 2
+
+            get_value_size("Hello")
+            # >> 5
+
+            get_value_size(True)
+            # >> 1
+    """
+    if value is None:
+        return 0
+    elif isinstance(value, list):
+        return len(value)
+    elif isinstance(value, dict):
+        return len(value.keys())
+    elif isinstance(value, str):
+        return len(value)
+    elif isinstance(value, bool):
+        return 1
+    else:
+        return len(str(value))
+
+
 def convert_bytes(num: Union[int, float]) -> str:
     """
 
     this function will convert bytes to MB.... GB... etc
 
     :param num:
     :return:
```

### Comparing `pawnlib-1.1.8/pawnlib/typing/date_utils.py` & `pawnlib-2.0/pawnlib/typing/date_utils.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/typing/defines.py` & `pawnlib-2.0/pawnlib/typing/defines.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/typing/generator.py` & `pawnlib-2.0/pawnlib/typing/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/__init__.py` & `pawnlib-2.0/pawnlib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/genesis.py` & `pawnlib-2.0/pawnlib/utils/genesis.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/http.py` & `pawnlib-2.0/pawnlib/utils/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,22 +537,24 @@
         return self._params
 
     def get_params_hint(self):
         return self._params_hint
 
 
 class IconRpcHelper:
-    def __init__(self, url="", wallet=None, network_info: NetworkInfo = None, raise_on_failure=True, debug=False, required_sign_methods=None):
+    def __init__(self, url="", wallet=None, network_info: NetworkInfo = None, raise_on_failure=True, debug=False, required_sign_methods=None, **kwargs):
         self.wallet = wallet
         self.governance_address = None
         self.request_payload = None
         self.response = None
         self.network_info = network_info
         self.raise_on_failure = raise_on_failure
         self.debug = debug
+        self.kwargs = kwargs
+
         if required_sign_methods and isinstance(required_sign_methods, list):
             self.required_sign_methods = required_sign_methods
         else:
             self.required_sign_methods = ["set", "register", "unregister", "claim", "vote", "apply", "remove", "cancel", "acceptScore", "reject"]
 
         if not url and self.network_info:
             url = self.network_info.network_api
@@ -929,26 +931,25 @@
             store_request_payload=False,
         )
 
         error = self.response.get('error')
         if error:
             self.exit_on_failure(error)
             return 0
-
         return response.get('result', [])
 
+
     @staticmethod
     def name_to_params(list_data):
         return {data.get('name'): "" for data in list_data}
 
     @staticmethod
     def make_params_hint(list_data):
         if not list_data:
             return {}
-
         formatted_data = {}
         for data in list_data:
             name = data.get('name')
             data_type = data.get('type', "")
             default = data.get('default', "")
             formatted_data[name] = f"{default}({data_type})"
         return formatted_data
@@ -1026,35 +1027,54 @@
         return response.get('text')
 
     def get_tx_wait(self,  tx_hash=None, url=None,  is_compact=True):
         tx_hash = self._get_tx_hash(tx_hash)
         if not tx_hash:
             return
         self.on_error = False
+
+        if pawn.console._live:
+            if not getattr(pawn, "console_status", None):
+                pawn.console_status = getattr(pawn, "console_status", None)
+            resp = self.check_transaction_loop(tx_hash, url, is_compact, pawn.console_status)
+        else:
+            with pawn.console.status("[magenta] Wait for transaction to be generated.") as status:
+                resp = self.check_transaction_loop(tx_hash, url, is_compact, status)
+
+        return resp
+
+    def check_transaction_loop(self, tx_hash=None, url=None,  is_compact=True, status=None):
         count = 0
-        with pawn.console.status("[magenta] Wait for transaction to be generated.") as status:
-            while True:
-                resp = self._check_transaction(url, tx_hash)
-                if resp.get('error'):
-                    text, exit_loop = self._handle_error_response(resp, count, tx_hash)
-                elif resp.get('result'):
-                    text, exit_loop = self._handle_success_response(resp, count, tx_hash)
-                else:
-                    text = resp
+        while True:
+            resp = self._check_transaction(url, tx_hash)
+            if resp.get('error'):
+                text, exit_loop = self._handle_error_response(resp, count, tx_hash)
+            elif resp.get('result'):
+                text, exit_loop = self._handle_success_response(resp, count, tx_hash)
+            else:
+                text = resp
+
+            wait_callback = self.kwargs.get('wait_callback')
+
+            if wait_callback and callable(wait_callback):
+                wait_callback(text)
+            elif getattr(status, "update", None):
                 status.update(
                     status=text,
                     spinner_style="yellow",
                 )
-                if exit_loop:
-                    self._print_final_result(text, is_compact, resp)
-                    break
-                count += 1
-                time.sleep(1)
-            if self.on_error and tx_hash:
-                self.get_debug_trace(tx_hash, reset_error=False)
+
+            if exit_loop:
+                self._print_final_result(text, is_compact, resp)
+                break
+            count += 1
+            time.sleep(1)
+        if self.on_error and tx_hash:
+            self.get_debug_trace(tx_hash, reset_error=False)
+
         return resp
 
     def _get_tx_hash(self, tx_hash):
         if not tx_hash and isinstance(self.response, dict):
             pawn.console.debug(f"tx_hash not found. It will be found in the self.response")
             if keys_exists(self.response, 'json', 'result', 'txHash'):
                 tx_hash = self.response['json']['result']['txHash']
```

### Comparing `pawnlib-1.1.8/pawnlib/utils/icx_raw_singer.py` & `pawnlib-2.0/pawnlib/utils/icx_raw_singer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/icx_signer.py` & `pawnlib-2.0/pawnlib/utils/icx_signer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/in_memory_zip.py` & `pawnlib-2.0/pawnlib/utils/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/log.py` & `pawnlib-2.0/pawnlib/utils/log.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/notify.py` & `pawnlib-2.0/pawnlib/utils/notify.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pawnlib/utils/operate_handler.py` & `pawnlib-2.0/pawnlib/utils/operate_handler.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/.gitignore` & `pawnlib-2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/pyproject.toml` & `pawnlib-2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.8/PKG-INFO` & `pawnlib-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pawnlib
-Version: 1.1.8
+Version: 2.0
 Summary: pawnlib is a collection of libraries for IaC.
 Project-URL: Changelog, https://github.com/jinwoo-j/pawnlib
 Project-URL: Documentation, https://pawnlib.readthedocs.io
 Project-URL: Homepage, https://pawnlib.readthedocs.io
 Project-URL: Source, https://github.com/jinwoo-j/pawnlib
 Author-email: Jinwoo <jinwoo@parametacorp.com>
 License-Expression: MIT
@@ -43,16 +43,16 @@
 Requires-Dist: rich>=12.0.1
 Requires-Dist: six>=1.15.0
 Requires-Dist: tabulate>=0.8.7
 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: urllib3~=1.26.0
 Requires-Dist: websocket-client>=0.59.0
 Provides-Extra: brotli
-Requires-Dist: brotli; platform_python_implementation == 'CPython' and extra == 'brotli'
-Requires-Dist: brotlicffi; platform_python_implementation != 'CPython' and extra == 'brotli'
+Requires-Dist: brotli; (platform_python_implementation == 'CPython') and extra == 'brotli'
+Requires-Dist: brotlicffi; (platform_python_implementation != 'CPython') and extra == 'brotli'
 Provides-Extra: docker
 Requires-Dist: aiodocker~=0.21.0; extra == 'docker'
 Provides-Extra: full
 Requires-Dist: aiodocker~=0.21.0; extra == 'full'
 Requires-Dist: coincurve~=18.0.0; extra == 'full'
 Requires-Dist: eth-keyfile>=0.6.1; extra == 'full'
 Requires-Dist: rich<14,>=10; extra == 'full'
```

