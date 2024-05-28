# Comparing `tmp/PyQuantKit-0.2.2.post6.tar.gz` & `tmp/pyquantkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQuantKit-0.2.2.post6.tar", last modified: Mon Apr 22 08:13:44 2024, max compression
+gzip compressed data, was "pyquantkit-0.3.0.tar", last modified: Tue May 28 02:25:31 2024, max compression
```

## Comparing `PyQuantKit-0.2.2.post6.tar` & `pyquantkit-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1066 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/LICENSE
--rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/PKG-INFO
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.298621 PyQuantKit-0.2.2.post6/PyQuantKit/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    35885 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/ConsoleUtils.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    51884 2024-04-22 08:13:10.000000 PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_lite.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    68097 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_old.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    16240 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/TechnicalAnalysis.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    19560 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/TradeUtils.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     7923 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/_FinanceDecimal.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     2976 2024-04-22 08:13:32.000000 PyQuantKit-0.2.2.post6/PyQuantKit/__init__.py
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/
--rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/PKG-INFO
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      393 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/SOURCES.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)        1 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/dependency_links.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       13 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/requires.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       11 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/top_level.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       53 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/README.md
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       38 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/setup.cfg
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1491 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.216126 pyquantkit-0.3.0/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-28 02:25:31.213126 pyquantkit-0.3.0/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.109828 pyquantkit-0.3.0/PyQuantKit/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    68097 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/PyQuantKit/MarketUtils_old.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    19556 2024-05-27 06:25:36.000000 pyquantkit-0.3.0/PyQuantKit/TradeUtils_old.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7923 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/PyQuantKit/_FinanceDecimal.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3207 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    35847 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/console_utils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    51864 2024-05-27 06:25:36.000000 pyquantkit-0.3.0/PyQuantKit/market_utils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    16197 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/technical_analysis.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    22613 2024-05-27 09:56:50.000000 pyquantkit-0.3.0/PyQuantKit/trade_utils.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.191125 pyquantkit-0.3.0/PyQuantKit.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      421 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       53 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-28 02:25:31.217126 pyquantkit-0.3.0/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1491 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/setup.py
```

### Comparing `PyQuantKit-0.2.2.post6/LICENSE` & `pyquantkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post6/PKG-INFO` & `pyquantkit-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.2.2.post6
+Version: 0.3.0
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/ConsoleUtils.py` & `pyquantkit-0.3.0/PyQuantKit/console_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import time
 import uuid
 from enum import Enum
 from typing import Iterable, Sized
 
 from . import LOGGER
 
-LOGGER = LOGGER.getChild(os.path.basename(os.path.splitext(__file__)[0]))
+LOGGER = LOGGER.getChild('Console')
 __all__ = ['Progress', 'GetInput', 'GetArgs', 'count_ordinal', 'TerminalStyle', 'InteractiveShell', 'ShellTransfer']
 
 
 # noinspection SpellCheckingInspection
 class TerminalStyle(Enum):
     CEND = '\33[0m'
     CBOLD = '\33[1m'
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_lite.py` & `pyquantkit-0.3.0/PyQuantKit/market_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 import math
 import re
 import warnings
 from typing import overload
 
 import numpy as np
 
-from . import LOGGER
+from . import LOGGER, TIME_ZONE
 
 LOGGER = LOGGER.getChild('MarketUtils')
-__all__ = ['TIME_ZONE', 'TransactionSide',
+__all__ = ['TransactionSide',
            'MarketData', 'OrderBook', 'BarData', 'TickData', 'TransactionData', 'TradeData',
            'OrderBookBuffer', 'BarDataBuffer', 'TickDataBuffer', 'TransactionDataBuffer']
 
-TIME_ZONE = None
-
 
 class TransactionSide(enum.Enum):
     ShortOrder = AskOrder = Offer_to_Short = -3
     ShortOpen = Sell_to_Short = -2
     ShortFilled = LongClose = Sell_to_Unwind = ask = -1
     UNKNOWN = CANCEL = 0
     LongFilled = LongOpen = Buy_to_Long = bid = 1
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_old.py` & `pyquantkit-0.3.0/PyQuantKit/MarketUtils_old.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/TechnicalAnalysis.py` & `pyquantkit-0.3.0/PyQuantKit/technical_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 import numpy as np
 import pandas as pd
 
 from . import LOGGER
 
-LOGGER = LOGGER.getChild(os.path.basename(os.path.splitext(__file__)[0]))
+LOGGER = LOGGER.getChild('TA')
 __all__ = ['TechnicalAnalysis']
 
 
 # noinspection PyPep8Naming
 class TechnicalAnalysis(object):
 
     def __getattribute__(self, name):
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/TradeUtils.py` & `pyquantkit-0.3.0/PyQuantKit/TradeUtils_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import datetime
 import json
 import uuid
 from enum import Enum
 
 from . import LOGGER
-from .MarketUtils_lite import TransactionSide, TransactionData
+from .market_utils import TransactionSide, TransactionData
 
 LOGGER = LOGGER.getChild('TradeUtils')
 __all__ = ['OrderState', 'OrderType', 'TradeInstruction', 'TradeReport']
 
 
 class OrderType(Enum):
     UNKNOWN = -2
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/_FinanceDecimal.py` & `pyquantkit-0.3.0/PyQuantKit/_FinanceDecimal.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit/__init__.py` & `pyquantkit-0.3.0/PyQuantKit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
-__version__ = '0.2.2.post6'
+__version__ = '0.3.0'
 
 import logging
 import sys
 import time
 
 LOGGER: logging.Logger | None = None
 LOG_LEVEL = logging.INFO
 LOG_LEVEL_EVENT = LOG_LEVEL - 1
+TIME_ZONE = None
 
 
 class ColoredFormatter(logging.Formatter):
     """Logging Formatter to add colors and count warning / errors"""
 
     def __init__(self, fmt=None, datefmt=None, style='{', validate=True):
         self.format_str = '[{asctime} {name} - {threadName} - {module}:{lineno} - {levelname}] {message}' if fmt is None else fmt
@@ -80,16 +81,21 @@
     return LOGGER
 
 
 def set_logger(logger: logging.Logger):
     global LOGGER
     LOGGER = logger
 
+    market_utils.LOGGER = LOGGER.getChild('MarketUtils')
+    trade_utils.LOGGER = LOGGER.getChild('TradeUtils')
+    technical_analysis.LOGGER = LOGGER.getChild('TA')
+    console_utils.LOGGER = LOGGER.getChild('Console')
+
 
 _ = get_logger()
 
 from ._FinanceDecimal import *
-from .MarketUtils_lite import *
+from .market_utils import *
 # from .MarketUtils2 import *
-from .TechnicalAnalysis import *
-from .TradeUtils import *
-from .ConsoleUtils import *
+from .technical_analysis import *
+from .trade_utils import *
+from .console_utils import *
```

### Comparing `PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/PKG-INFO` & `pyquantkit-0.3.0/PyQuantKit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.2.2.post6
+Version: 0.3.0
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyQuantKit-0.2.2.post6/setup.py` & `pyquantkit-0.3.0/setup.py`

 * *Files identical despite different names*

