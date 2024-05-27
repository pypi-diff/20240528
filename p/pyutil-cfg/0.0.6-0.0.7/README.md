# Comparing `tmp/pyutil-cfg-0.0.6.tar.gz` & `tmp/pyutil_cfg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutil-cfg-0.0.6.tar", last modified: Wed Aug 23 19:22:42 2023, max compression
+gzip compressed data, was "pyutil_cfg-0.0.7.tar", last modified: Mon May 27 22:30:24 2024, max compression
```

## Comparing `pyutil-cfg-0.0.6.tar` & `pyutil_cfg-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2023-08-23 19:22:42.551141 pyutil-cfg-0.0.6/
--rw-r--r--   0 chhsiao    (501) staff       (20)     1064 2023-08-18 20:12:22.000000 pyutil-cfg-0.0.6/LICENSE
--rw-r--r--   0 chhsiao    (501) staff       (20)     1758 2023-08-23 19:22:42.550961 pyutil-cfg-0.0.6/PKG-INFO
--rw-r--r--   0 chhsiao    (501) staff       (20)     1340 2023-08-18 20:12:22.000000 pyutil-cfg-0.0.6/README.md
-drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2023-08-23 19:22:42.548113 pyutil-cfg-0.0.6/pyutil_cfg/
--rw-r--r--   0 chhsiao    (501) staff       (20)       47 2023-02-20 19:06:45.000000 pyutil-cfg-0.0.6/pyutil_cfg/__init__.py
--rw-r--r--   0 chhsiao    (501) staff       (20)     2594 2023-08-23 19:20:02.000000 pyutil-cfg-0.0.6/pyutil_cfg/cfg.py
-drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2023-08-23 19:22:42.550114 pyutil-cfg-0.0.6/pyutil_cfg.egg-info/
--rw-r--r--   0 chhsiao    (501) staff       (20)     1758 2023-08-23 19:22:42.000000 pyutil-cfg-0.0.6/pyutil_cfg.egg-info/PKG-INFO
--rw-r--r--   0 chhsiao    (501) staff       (20)      221 2023-08-23 19:22:42.000000 pyutil-cfg-0.0.6/pyutil_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 chhsiao    (501) staff       (20)        1 2023-08-23 19:22:42.000000 pyutil-cfg-0.0.6/pyutil_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 chhsiao    (501) staff       (20)       11 2023-08-23 19:22:42.000000 pyutil-cfg-0.0.6/pyutil_cfg.egg-info/top_level.txt
--rw-r--r--   0 chhsiao    (501) staff       (20)       38 2023-08-23 19:22:42.551186 pyutil-cfg-0.0.6/setup.cfg
--rw-r--r--   0 chhsiao    (501) staff       (20)      675 2023-08-23 19:21:30.000000 pyutil-cfg-0.0.6/setup.py
-drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2023-08-23 19:22:42.550486 pyutil-cfg-0.0.6/tests/
--rw-r--r--   0 chhsiao    (501) staff       (20)     1539 2023-08-18 20:12:22.000000 pyutil-cfg-0.0.6/tests/test_cfg.py
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:24.000850 pyutil_cfg-0.0.7/
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1064 2023-08-18 20:12:22.000000 pyutil_cfg-0.0.7/LICENSE
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1708 2024-05-27 22:30:23.999661 pyutil_cfg-0.0.7/PKG-INFO
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1340 2023-08-18 20:12:22.000000 pyutil_cfg-0.0.7/README.md
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:23.972374 pyutil_cfg-0.0.7/__/
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:23.978629 pyutil_cfg-0.0.7/__/bin/
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1200 2024-05-27 21:54:47.000000 pyutil_cfg-0.0.7/__/bin/activate_this.py
+-rw-r--r--   0 chhsiao    (501) staff       (20)      708 2024-05-27 22:27:11.000000 pyutil_cfg-0.0.7/pyproject.toml
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:23.981082 pyutil_cfg-0.0.7/pyutil_cfg/
+-rw-r--r--   0 chhsiao    (501) staff       (20)       47 2023-02-20 19:06:45.000000 pyutil_cfg-0.0.7/pyutil_cfg/__init__.py
+-rw-r--r--   0 chhsiao    (501) staff       (20)     2946 2024-05-27 22:26:49.000000 pyutil_cfg-0.0.7/pyutil_cfg/cfg.py
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:23.989192 pyutil_cfg-0.0.7/pyutil_cfg.egg-info/
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1708 2024-05-27 22:30:23.000000 pyutil_cfg-0.0.7/pyutil_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 chhsiao    (501) staff       (20)      260 2024-05-27 22:30:23.000000 pyutil_cfg-0.0.7/pyutil_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 chhsiao    (501) staff       (20)        1 2024-05-27 22:30:23.000000 pyutil_cfg-0.0.7/pyutil_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 chhsiao    (501) staff       (20)       27 2024-05-27 22:30:23.000000 pyutil_cfg-0.0.7/pyutil_cfg.egg-info/top_level.txt
+-rw-r--r--   0 chhsiao    (501) staff       (20)       38 2024-05-27 22:30:24.001080 pyutil_cfg-0.0.7/setup.cfg
+-rw-r--r--   0 chhsiao    (501) staff       (20)       38 2024-05-27 22:26:49.000000 pyutil_cfg-0.0.7/setup.py
+drwxr-xr-x   0 chhsiao    (501) staff       (20)        0 2024-05-27 22:30:23.987373 pyutil_cfg-0.0.7/tests/
+-rw-r--r--   0 chhsiao    (501) staff       (20)     1539 2023-08-18 20:12:22.000000 pyutil_cfg-0.0.7/tests/test_cfg.py
```

### Comparing `pyutil-cfg-0.0.6/LICENSE` & `pyutil_cfg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutil-cfg-0.0.6/PKG-INFO` & `pyutil_cfg-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: pyutil-cfg
-Version: 0.0.6
+Version: 0.0.7
 Summary: python util for cfg (configurations)
-Home-page: https://github.com/chhsiao1981/pyutil_cfg
-Author: chhsiao
-Author-email: hsiao.chuanheng@gmail.com
+Author-email: Chuan-Heng Hsiao <hsiao.chuanheng@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyutil_cfg
```

### Comparing `pyutil-cfg-0.0.6/README.md` & `pyutil_cfg-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyutil-cfg-0.0.6/pyutil_cfg/cfg.py` & `pyutil_cfg-0.0.7/pyutil_cfg/cfg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 
-from configparser import SafeConfigParser
+from typing import Optional, Any
+from configparser import ConfigParser
 import logging
 import logging.config
 
 import json
 
 
-def init(name, ini_filename, log_ini_filename='', params=None):
+def init(name: str, ini_filename: str, log_ini_filename: str = '', params: Optional[dict] = None) -> tuple[logging.Logger, dict]:
     logger = _init_logger(name, log_ini_filename, ini_filename)
     config = _init_ini_file(name, ini_filename, logger)
     config = _post_init_config(params, config, logger)
 
-    logger.debug('pyutil_cfg: to return: name: %s logger: %s config: %s', name, logger, config)
+    logger.debug('pyutil_cfg.init: to return: name: %s logger: %s config: %s', name, logger, config)
 
     return logger, config
 
 
-def _init_logger(name, log_ini_filename, ini_filename):
+def _init_logger(name: str, log_ini_filename: str, ini_filename: str) -> logging.Logger:
     logger = logging.getLogger(name)
 
     if not log_ini_filename:
         log_ini_filename = ini_filename
 
     if not log_ini_filename:
         return logger
@@ -30,55 +31,55 @@
         logging.config.fileConfig(log_ini_filename, disable_existing_loggers=False)
     except:
         pass
 
     return logger
 
 
-def _init_ini_file(name, ini_filename, logger):
+def _init_ini_file(name: str, ini_filename: str, logger: logging.Logger) -> dict:
     '''
     setup name:main config
     '''
-    section = name + ':main'
+    section_name = name + ':main'
 
-    config = _init_ini_file_core(ini_filename, section, logger)
+    config = _init_ini_file_core(ini_filename, section_name, logger)
 
     return config
 
 
-def _init_ini_file_core(ini_filename, section, logger):
+def _init_ini_file_core(ini_filename: str, section_name: str, logger: logging.Logger) -> dict:
     '''
     get ini conf from section
     return: config: {key: val} val: json_loaded
     '''
     if not ini_filename:
         return {}
 
-    config_parser = SafeConfigParser()
+    config_parser = ConfigParser()
     config_parser.read(ini_filename)
     sections = config_parser.sections()
-    if section not in sections:
+    if section_name not in sections:
         return {}
 
-    options = config_parser.options(section)
-    config = {option: _init_ini_file_parse_option(option, section, config_parser, logger) for option in options}
+    options = config_parser.options(section_name)
+    config = {option: _init_ini_file_parse_option(option, section_name, config_parser, logger) for option in options}
 
     return config
 
 
-def _init_ini_file_parse_option(option, section, config_parser, logger):
+def _init_ini_file_parse_option(option: str, section_name: str, config_parser: ConfigParser, logger: logging.Logger) -> Any:
     try:
-        val = config_parser.get(section, option)
+        val = config_parser.get(section_name, option)
     except Exception as e:
-        logger.exception('unable to get option: section: %s option: %s e: %s', section, option, e)
+        logger.exception('unable to get option: section: %s option: %s e: %s', section_name, option, e)
         val = ''
     return _init_ini_file_val_to_json(option, val)
 
 
-def _init_ini_file_val_to_json(option, val):
+def _init_ini_file_val_to_json(option: str, val: Any) -> Any:
     '''
     try to do json load on value
     '''
 
     if val.__class__.__name__ != 'str':
         return val
 
@@ -90,15 +91,15 @@
 
     if option.endswith('_set'):
         val = set(val)
 
     return val
 
 
-def _post_init_config(params, config, logger):
+def _post_init_config(params: Optional[dict], config: dict, logger: logging.Logger) -> dict:
     '''
     add additional parameters into config
     '''
 
     if not params:
         return config
```

### Comparing `pyutil-cfg-0.0.6/pyutil_cfg.egg-info/PKG-INFO` & `pyutil_cfg-0.0.7/pyutil_cfg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: pyutil-cfg
-Version: 0.0.6
+Version: 0.0.7
 Summary: python util for cfg (configurations)
-Home-page: https://github.com/chhsiao1981/pyutil_cfg
-Author: chhsiao
-Author-email: hsiao.chuanheng@gmail.com
+Author-email: Chuan-Heng Hsiao <hsiao.chuanheng@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyutil_cfg
```

### Comparing `pyutil-cfg-0.0.6/tests/test_cfg.py` & `pyutil_cfg-0.0.7/tests/test_cfg.py`

 * *Files identical despite different names*

