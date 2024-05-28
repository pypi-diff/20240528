# Comparing `tmp/openai-cost-logger-0.4.1.tar.gz` & `tmp/openai-cost-logger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-cost-logger-0.4.1.tar", last modified: Fri May 10 08:58:19 2024, max compression
+gzip compressed data, was "openai-cost-logger-0.5.0.tar", last modified: Tue May 28 14:07:03 2024, max compression
```

## Comparing `openai-cost-logger-0.4.1.tar` & `openai-cost-logger-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:03.982782 openai-cost-logger-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-28 14:07:03.982782 openai-cost-logger-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:03.982782 openai-cost-logger-0.5.0/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:03.982782 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-28 14:07:03.000000 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-28 14:07:03.000000 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:07:03.000000 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 14:07:03.000000 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 14:07:03.000000 openai-cost-logger-0.5.0/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:07:03.982782 openai-cost-logger-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 14:07:00.000000 openai-cost-logger-0.5.0/setup.py
```

### Comparing `openai-cost-logger-0.4.1/LICENSE` & `openai-cost-logger-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.4.1/PKG-INFO` & `openai-cost-logger-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.4.1
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
@@ -33,25 +33,31 @@
       pip install openai-cost-logger
 
 * .. code-block:: python
 
       from openai_cost_logger import OpenAICostLogger
       from openai_cost_logger import OpenAICostLoggerViz
       from openai_cost_logger import OpenAICostLoggerUtils
+      from openai_cost_logger import OpenAICostLogger_Singleton
       from openai_cost_logger import DEFAULT_LOG_PATH, MODELS_COST
 
 Key Features:
 -------------
 * Track the cost of every request you make and save them in a JSON file.
 * Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
 * Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
 Models supported:
 -------------------
-* The response generation is totally up to the user. The library support every model which response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
+* The generation of responses is totally up to the user. The library supports every model whose response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
+
+Multithreading:
+---------------
+* Be aware that the classic cost logger is not thread-safe.
+* If you want to use it in a multithreading environment, you should use the **thread-safe** version of the logger: ``OpenAICostLogger_Singleton``. The interface is the same as the classic logger. This will prevent multiple threads from writing to the same file at the same time.
 
 Note:
 -----
 * Every cost is specified per **million tokens**.
 * If you don't specify the cost, the library will look to the **MODELS_COST** dictionary and get the cost of the model you are using. Be aware that if the model is not in the dictionary, an exception will be raised.
 
 Viz example:
```

### Comparing `openai-cost-logger-0.4.1/openai_cost_logger/constants.py` & `openai-cost-logger-0.5.0/openai_cost_logger/constants.py`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger.py` & `openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger.py`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_viz.py` & `openai-cost-logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.4.1/openai_cost_logger.egg-info/PKG-INFO` & `openai-cost-logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.4.1
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
@@ -33,25 +33,31 @@
       pip install openai-cost-logger
 
 * .. code-block:: python
 
       from openai_cost_logger import OpenAICostLogger
       from openai_cost_logger import OpenAICostLoggerViz
       from openai_cost_logger import OpenAICostLoggerUtils
+      from openai_cost_logger import OpenAICostLogger_Singleton
       from openai_cost_logger import DEFAULT_LOG_PATH, MODELS_COST
 
 Key Features:
 -------------
 * Track the cost of every request you make and save them in a JSON file.
 * Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
 * Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
 Models supported:
 -------------------
-* The response generation is totally up to the user. The library support every model which response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
+* The generation of responses is totally up to the user. The library supports every model whose response contains the fields **usage.prompt_tokens** and **usage.total_tokens** (e.g. chat completions, embeddings, etc.).
+
+Multithreading:
+---------------
+* Be aware that the classic cost logger is not thread-safe.
+* If you want to use it in a multithreading environment, you should use the **thread-safe** version of the logger: ``OpenAICostLogger_Singleton``. The interface is the same as the classic logger. This will prevent multiple threads from writing to the same file at the same time.
 
 Note:
 -----
 * Every cost is specified per **million tokens**.
 * If you don't specify the cost, the library will look to the **MODELS_COST** dictionary and get the cost of the model you are using. Be aware that if the model is not in the dictionary, an exception will be raised.
 
 Viz example:
```

### Comparing `openai-cost-logger-0.4.1/setup.py` & `openai-cost-logger-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read the README file (reStructuredText format)
 with open('README.rst') as f:
     long_description = f.read()
 
-version_number = '0.4.1'
+version_number = '0.5.0'
 
 setup(
     name='openai-cost-logger',
     version=version_number,
     author='Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov',
     description='OpenAI Cost Logger',
     author_email='lorenzodrudi11@gmail.com',
```

