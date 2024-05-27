# Comparing `tmp/codal_tsetmc-0.0.7.tar.gz` & `tmp/codal_tsetmc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codal_tsetmc-0.0.7.tar", max compression
+gzip compressed data, was "codal_tsetmc-0.0.8.tar", max compression
```

## Comparing `codal_tsetmc-0.0.7.tar` & `codal_tsetmc-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-0.0.7/LICENSE
--rwxr-xr-x   0        0        0     1773 2023-08-30 12:18:00.105121 codal_tsetmc-0.0.7/README.md
--rwxr-xr-x   0        0        0      881 2023-09-01 22:52:01.837268 codal_tsetmc-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      753 2023-09-01 00:20:39.449669 codal_tsetmc-0.0.7/src/codal_tsetmc/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:46:33.499975 codal_tsetmc-0.0.7/src/codal_tsetmc/config/__init__.py
--rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-0.0.7/src/codal_tsetmc/config/config.default.yml
--rwxr-xr-x   0        0        0     2326 2022-08-31 10:11:07.442885 codal_tsetmc-0.0.7/src/codal_tsetmc/config/engine.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:13:27.157561 codal_tsetmc-0.0.7/src/codal_tsetmc/download/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:20:38.526565 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/__init__.py
--rwxr-xr-x   0        0        0     3836 2023-08-30 22:05:04.261001 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/category.py
--rwxr-xr-x   0        0        0      525 2023-08-30 22:03:38.205743 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/company.py
--rwxr-xr-x   0        0        0     8444 2023-09-01 22:51:43.693855 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/letters.py
--rwxr-xr-x   0        0        0    10194 2023-09-01 12:20:33.670915 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/query.py
--rwxr-xr-x   0        0        0    10507 2023-08-31 20:44:00.586573 codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/report.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:17:32.818433 codal_tsetmc-0.0.7/src/codal_tsetmc/download/other/__init__.py
--rwxr-xr-x   0        0        0     4346 2023-08-31 23:17:29.144931 codal_tsetmc-0.0.7/src/codal_tsetmc/download/other/commodity.py
--rwxr-xr-x   0        0        0        0 2023-08-30 22:17:20.138410 codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/__init__.py
--rwxr-xr-x   0        0        0     4096 2023-08-31 16:56:47.632480 codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/capital.py
--rwxr-xr-x   0        0        0     6421 2023-08-31 16:40:42.333136 codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/price.py
--rwxr-xr-x   0        0        0     4113 2023-08-31 16:56:01.332548 codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/stock.py
--rwxr-xr-x   0        0        0     1585 2023-09-01 00:20:29.525688 codal_tsetmc-0.0.7/src/codal_tsetmc/initializer.py
--rwxr-xr-x   0        0        0        0 2023-08-30 23:17:18.742542 codal_tsetmc-0.0.7/src/codal_tsetmc/models/__init__.py
--rwxr-xr-x   0        0        0     4382 2023-08-30 22:42:01.274702 codal_tsetmc-0.0.7/src/codal_tsetmc/models/companies.py
--rwxr-xr-x   0        0        0      882 2023-08-30 22:53:10.153072 codal_tsetmc-0.0.7/src/codal_tsetmc/models/create.py
--rwxr-xr-x   0        0        0     7788 2023-08-31 00:03:38.442890 codal_tsetmc-0.0.7/src/codal_tsetmc/models/stocks.py
--rwxr-xr-x   0        0        0        1 2023-08-30 22:12:41.957284 codal_tsetmc-0.0.7/src/codal_tsetmc/tools/__init__.py
--rwxr-xr-x   0        0        0     1790 2023-09-01 15:12:06.689260 codal_tsetmc-0.0.7/src/codal_tsetmc/tools/api.py
--rwxr-xr-x   0        0        0      834 2023-08-30 22:53:47.929097 codal_tsetmc-0.0.7/src/codal_tsetmc/tools/database.py
--rwxr-xr-x   0        0        0      891 2023-05-31 12:48:46.815169 codal_tsetmc-0.0.7/src/codal_tsetmc/tools/exception.py
--rwxr-xr-x   0        0        0     9716 2023-07-01 21:22:10.636936 codal_tsetmc-0.0.7/src/codal_tsetmc/tools/string.py
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 codal_tsetmc-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0     3874 2024-05-26 18:07:54.261461 codal_tsetmc-0.0.8/README.md
+-rwxr-xr-x   0        0        0      881 2024-05-26 18:21:35.582076 codal_tsetmc-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      939 2024-05-26 20:11:40.824220 codal_tsetmc-0.0.8/src/codal_tsetmc/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:46:33.499975 codal_tsetmc-0.0.8/src/codal_tsetmc/config/__init__.py
+-rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-0.0.8/src/codal_tsetmc/config/config.default.yml
+-rwxr-xr-x   0        0        0     2281 2024-05-26 19:38:11.337203 codal_tsetmc-0.0.8/src/codal_tsetmc/config/engine.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:13:27.157561 codal_tsetmc-0.0.8/src/codal_tsetmc/download/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:20:38.526565 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/__init__.py
+-rwxr-xr-x   0        0        0     4071 2024-05-26 16:53:41.440402 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/category.py
+-rwxr-xr-x   0        0        0      525 2023-08-30 22:03:38.205743 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/company.py
+-rwxr-xr-x   0        0        0     8343 2024-05-26 17:37:07.978458 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/letters.py
+-rwxr-xr-x   0        0        0    10242 2024-05-26 17:37:08.468597 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/query.py
+-rwxr-xr-x   0        0        0    10615 2024-05-26 17:37:09.202565 codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/report.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:17:32.818433 codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/__init__.py
+-rwxr-xr-x   0        0        0     4370 2024-05-26 22:40:01.079750 codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/commodity.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 22:17:20.138410 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/__init__.py
+-rwxr-xr-x   0        0        0     4112 2024-05-26 22:40:00.827227 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/capital.py
+-rwxr-xr-x   0        0        0     6819 2024-05-27 00:19:09.779013 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/price.py
+-rwxr-xr-x   0        0        0     4397 2024-05-26 22:22:20.459155 codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/stock.py
+-rwxr-xr-x   0        0        0     1483 2024-05-26 20:13:00.609132 codal_tsetmc-0.0.8/src/codal_tsetmc/initializer.py
+-rwxr-xr-x   0        0        0        0 2023-08-30 23:17:18.742542 codal_tsetmc-0.0.8/src/codal_tsetmc/models/__init__.py
+-rwxr-xr-x   0        0        0     4550 2024-05-26 18:40:15.029397 codal_tsetmc-0.0.8/src/codal_tsetmc/models/companies.py
+-rwxr-xr-x   0        0        0      920 2024-05-26 20:11:41.962655 codal_tsetmc-0.0.8/src/codal_tsetmc/models/create.py
+-rwxr-xr-x   0        0        0     7723 2024-05-26 23:55:50.253175 codal_tsetmc-0.0.8/src/codal_tsetmc/models/stocks.py
+-rwxr-xr-x   0        0        0        1 2023-08-30 22:12:41.957284 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/__init__.py
+-rwxr-xr-x   0        0        0     1781 2024-05-26 21:32:15.445757 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/api.py
+-rwxr-xr-x   0        0        0      879 2024-05-26 20:21:43.474048 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/database.py
+-rwxr-xr-x   0        0        0      895 2024-05-26 17:37:09.431876 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/exception.py
+-rwxr-xr-x   0        0        0     9710 2024-05-26 16:28:57.230356 codal_tsetmc-0.0.8/src/codal_tsetmc/tools/string.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 codal_tsetmc-0.0.8/PKG-INFO
```

### Comparing `codal_tsetmc-0.0.7/LICENSE` & `codal_tsetmc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.7/pyproject.toml` & `codal_tsetmc-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codal-tsetmc"
-version = "0.0.7"
+version = "0.0.8"
 description = "Data Downloader for Codal and Tehran stock market"
 authors = ["Mohsen Ebrahimi <mohsenebrahimy.ir@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mohsenebrahimyir.github.io/codal-tsetmc/"
 repository = "https://github.com/mohsenebrahimyir/codal-tsetmc.git"
 packages = [
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/config/engine.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/config/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import contextlib
-from sqlalchemy import Column, Float, Integer, String, create_engine
-from sqlalchemy.ext.declarative import declarative_base, declared_attr
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy import *
 from pathlib import Path
 import os
-import sqlite3
 import logging
 import yaml
 
 
 HOME_PATH = str(Path.home())
 CDL_TSE_FOLDER = ".cdl_tse"
 CONFIG_PATH = f"{os.path.join(HOME_PATH, CDL_TSE_FOLDER)}/config.yml"
 
 
 def create_config():
-    # create config.yml from config.deafult.yml
+    # create config.yml from config.default.yml
     if not os.path.exists(CONFIG_PATH):
         with open(os.path.join(os.path.dirname(__file__), "config.default.yml"), "r") as f:
             config = yaml.full_load(f)
         with contextlib.suppress(FileExistsError):
             path = os.path.join(HOME_PATH, CDL_TSE_FOLDER)
             os.mkdir(path)
         with open(CONFIG_PATH, "w") as f:
@@ -29,19 +27,19 @@
 
 create_config()
 
 
 with open(CONFIG_PATH, "r") as f:
     config = yaml.full_load(f)
 
-defualt_db_path = os.path.join(f"{HOME_PATH}/{CDL_TSE_FOLDER}/companies-stocks.db")
+default_db_path = os.path.join(f"{HOME_PATH}/{CDL_TSE_FOLDER}/companies-stocks.db")
 
 db_path = config.get("database").get("path")
 if db_path is None:
-    db_path = defualt_db_path
+    db_path = default_db_path
 
 default_engine_URI = f"sqlite:///{db_path}"
 engine = config.get("database").get("engine")
 if engine == "sqlite":
     engine_URI = default_engine_URI
 else:
     engine = config.get("database").get("engine")
@@ -78,13 +76,16 @@
     def query(cls):
         return session.query(cls)
 
     def display(self):
         data = self.__dict__
         try:
             del data["_sa_instance_state"]
-        except:
+        except Exception as e:
+            print(e)
+        finally:
             pass
+
         return data
 
 
 Base = declarative_base(cls=QueryMixin)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/category.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/category.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import pandas as pd
 
 from codal_tsetmc.tools.api import get_dict_from_xml_api
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
 
+
 class Categories:
 
     def __init__(self) -> None:
+        self.financial_years = None
+        self.auditors = None
+        self.company_statuses = None
+        self.categories = None
+        self.letter_types = None
+        self.company_types = None
+        self.report_types = None
         self.url = 'https://search.codal.ir/api/search/v1/'
 
     def get_data(self):
         api = get_dict_from_xml_api(self.url + "categories")
         report_types = []
         company_types = []
         letter_types = []
@@ -82,9 +90,10 @@
         fill_table_of_db_with_df(self.financial_years, "financial_years", "date")
 
 
 def fill_categories_table():
     cat = Categories()
     cat.fill_categories_table()
 
+
 if __name__ == '__main__':
     pass
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/company.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/company.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/letters.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/letters.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,251 +2,255 @@
 import asyncio
 import aiohttp
 import pandas as pd
 
 from codal_tsetmc.config.engine import session, engine
 from codal_tsetmc.models.stocks import Stocks
 from codal_tsetmc.tools.string import (
-    FA_TO_EN_DIGITS, LETTERS_CODE_TO_TITLE, 
+    FA_TO_EN_DIGITS, LETTERS_CODE_TO_TITLE,
     datetime_to_num, df_col_to_snake_case, num_to_datetime,
 )
 
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
-from codal_tsetmc.tools.api import get_results_by_asyncio_loop
 from codal_tsetmc.download.codal.query import CodalQuery
 
 """################
-گرفتن اطلاعات از کدال 
+گرفتن اطلاعات از کدال
 ################"""
 
+
 def convert_letter_list_to_df(data) -> pd.DataFrame:
     df = pd.DataFrame(data).replace(regex=FA_TO_EN_DIGITS)
     df["LetterSerial"] = df["Url"].replace(regex={
         r"^.*LetterSerial=": "",
         r"\&.*$": ""
     })
-    df["LetterTypes"]     = df["LetterCode"].replace(regex=LETTERS_CODE_TO_TITLE)
+    df["LetterTypes"] = df["LetterCode"].replace(regex=LETTERS_CODE_TO_TITLE)
     df["PublishDateTime"] = df["PublishDateTime"].apply(datetime_to_num)
-    df["SentDateTime"]    = df["SentDateTime"].apply(datetime_to_num)
-    df["LetterTitle"]     = df["Title"]
-    df["Name"]            = df["CompanyName"]
+    df["SentDateTime"] = df["SentDateTime"].apply(datetime_to_num)
+    df["LetterTitle"] = df["Title"]
+    df["Name"] = df["CompanyName"]
     df = df[[
         "PublishDateTime", "SentDateTime", "TracingNo",
         "LetterSerial", "LetterCode", "LetterTypes", "LetterTitle",
         "Symbol", "Name",
     ]]
     df = df_col_to_snake_case(df)
 
     return df
 
 
-async def get_letters_urls_from_page_100000_async(session, url):
+async def get_letters_urls_from_page_100000_async(ses, url):
     headers = {
-        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 '
+                      'Safari/537.36',
     }
-    async with session.get(url, cookies={}, headers=headers, data="") as response:
+    async with ses.get(url, cookies={}, headers=headers, data="") as response:
         data = await response.json()
-    
+
     u = url.split("100000")
     return [f'{u[0]}{data["Page"] + 1 - i}{u[1]}' for i in range(1, data["Page"] + 1)]
 
 
 async def get_letters_urls_async(urls):
     tasks = []
-    results = []
-    async with aiohttp.ClientSession() as session:
+    async with aiohttp.ClientSession() as ses:
         for url in urls:
-            tasks.append(get_letters_urls_from_page_100000_async(session, url))
+            tasks.append(get_letters_urls_from_page_100000_async(ses, url))
         results = await asyncio.gather(*tasks)
     return results
 
 
 def get_letter_urls_parallel(urls):
-
     if sys.platform == 'win32':
         loop = asyncio.ProactorEventLoop()
         asyncio.set_event_loop(loop)
     else:
         loop = asyncio.get_event_loop()
 
     try:
         results = loop.run_until_complete(get_letters_urls_async(urls))
 
     except RuntimeError:
-        WARNING_COLOR = "\033[93m"
-        ENDING_COLOR = "\033[0m"
-        print(WARNING_COLOR, "Please update stock table", ENDING_COLOR)
+        warning_color = "\033[93m"
+        ending_color = "\033[0m"
+        print(warning_color, "Please update stock table", ending_color)
         print(
-            f"{WARNING_COLOR}If you are using jupyter notebook, please run following command:{ENDING_COLOR}"
+            f"{warning_color}If you are using jupyter notebook, please run following command:{ending_color}"
         )
         print("```")
         print("%pip install nest_asyncio")
         print("import nest_asyncio; nest_asyncio.apply()")
         print("```")
         raise RuntimeError
-    
+
     return results
 
 
 def get_letters_urls_by_symbols(query, symbols, msg=""):
     print(f"update letters urls ", end="\r")
-    
+
     query.set_page_number(100000)
     urls = []
-    
+
     for symbol in symbols:
         query.set_symbol(symbol)
         urls += [query.get_query_url()]
-    
+
     results = get_letter_urls_parallel(urls)
     print(msg, end="\r")
 
     return results
 
-async def update_letters_for_each_url_async(session, url):
+
+async def update_letters_for_each_url_async(ses, url):
     try:
         headers = {
-            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 '
+                          'Safari/537.36',
         }
-        async with session.get(url, cookies={}, headers=headers, data="") as response:
+        async with ses.get(url, cookies={}, headers=headers, data="") as response:
             data = await response.json()
 
             df = convert_letter_list_to_df(data["Letters"])
             fill_table_of_db_with_df(df, "letters", "tracing_no")
 
             return True
 
     except Exception as e:
         return e
 
 
 async def update_letters_for_urls_async(urls):
     tasks = []
-    results = []
-    async with aiohttp.ClientSession() as session:
+    async with aiohttp.ClientSession() as ses:
         for url in urls:
-            tasks.append(update_letters_for_each_url_async(session, url))
+            tasks.append(update_letters_for_each_url_async(ses, url))
         results = await asyncio.gather(*tasks)
 
     return results
 
 
 def update_letter_urls_parallel(urls):
-    
+    results = None
     if sys.platform == 'win32':
         ##############################################################################
         from functools import wraps
 
         from asyncio.proactor_events import _ProactorBasePipeTransport
 
         def silence_event_loop_closed(func):
             @wraps(func)
             def wrapper(self, *args, **kwargs):
                 try:
                     return func(self, *args, **kwargs)
                 except RuntimeError as e:
                     if str(e) != 'Event loop is closed':
                         raise
+
             return wrapper
 
         _ProactorBasePipeTransport.__del__ = silence_event_loop_closed(_ProactorBasePipeTransport.__del__)
-        
+
         ##############################################################################
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    
+
     loop = asyncio.get_event_loop()
-    
+
     try:
         results = loop.run_until_complete(update_letters_for_urls_async(urls))
 
     except RuntimeError:
-        WARNING_COLOR = "\033[93m"
-        ENDING_COLOR = "\033[0m"
-        print(WARNING_COLOR, "Please update stock table", ENDING_COLOR)
+        warning_color = "\033[93m"
+        ending_color = "\033[0m"
+        print(warning_color, "Please update stock table", ending_color)
         print(
-            f"{WARNING_COLOR}If you are using jupyter notebook, please run following command:{ENDING_COLOR}"
+            f"{warning_color}If you are using jupyter notebook, please run following command:{ending_color}"
         )
         print("```")
         print("%pip install nest_asyncio")
         print("import nest_asyncio; nest_asyncio.apply()")
         print("```")
         raise RuntimeError
-    
+
     finally:
         loop.close()
         return results
-  
-
 
 
 def update_letters_table_by_symbols(query, symbols, msg=""):
     print(f"update letters ", end="\r")
     urls_list = get_letters_urls_by_symbols(query, symbols)
 
     letter_urls = []
     for urls in urls_list:
         for url in urls:
             letter_urls += [url]
-    
+
     results = update_letter_urls_parallel(letter_urls)
+    print(msg)
     return results
 
 
 def update_companies_group_letters(query, group_code):
     stocks = session.query(Stocks.symbol).filter_by(group_code=group_code).all()
-    print(f"{' '*25} group: {group_code}", end="\r")
+    print(f"{' ' * 25} group: {group_code}", end="\r")
     symbols = [stock[0] for stock in stocks]
-    msg = "group "+group_code+" updated"
+    msg = "group " + group_code + " updated"
     results = update_letters_table_by_symbols(query, symbols, msg)
     return results
 
 
 def fill_letters_table(query):
     codes = session.query(Stocks.group_code).distinct().all()
     for i, code in enumerate(codes):
-        print(f"{' '*35} total progress: {100*(i+1)/len(codes):.2f}%", end="\r")
+        print(f"{' ' * 35} total progress: {100 * (i + 1) / len(codes):.2f}%", end="\r")
         update_companies_group_letters(query, code[0])
-    
-    print("letters Download Finished.", " "*50)
 
+    print("letters Download Finished.", " " * 50)
 
-def fill_interim_financial_statements_letters(from_date = "1300/01/01", to_date = "1500/01/01"):
+
+def fill_interim_financial_statements_letters(from_date="1300/01/01", to_date="1500/01/01"):
     query = CodalQuery()
     query.set_from_date(from_date)
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
     fill_letters_table(query)
 
-def fill_symbols_interim_financial_statements_letters(symbols, from_date = "1300/01/01", to_date = "1500/01/01"):
+
+def fill_symbols_interim_financial_statements_letters(symbols, from_date="1300/01/01", to_date="1500/01/01"):
     query = CodalQuery()
     query.set_from_date(from_date)
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
     results = update_letters_table_by_symbols(query, symbols)
     return results
 
 
-def update_symbol_interim_financial_statements_letters(symbol, from_date = "1300/01/01", to_date = "1500/01/01"):
+def update_symbol_interim_financial_statements_letters(symbol, from_date="1300/01/01", to_date="1500/01/01"):
     query = CodalQuery()
     query.set_to_date(to_date)
     query.set_category('اطلاعات و صورت مالی سالانه')
     query.set_letter_type('اطلاعات و صورتهای مالی میاندوره ای')
 
-    q = f"SELECT max(publish_date_time) AS date FROM letters WHERE symbol = '{symbol}' AND (letter_code = 'ن-30' OR letter_code = 'ن-31')"
+    q = (
+        f"SELECT max(publish_date_time) AS date FROM letters WHERE symbol = '{symbol}' "
+        f"AND (letter_code = 'ن-30' OR letter_code = 'ن-31')"
+    )
     max_date = pd.read_sql(q, engine)
-    
+
     if max_date.date.iat[0] is None:
         query.set_from_date(from_date)
     else:
-        last_date = num_to_datetime(max_date.date.iat[0], datetime = False)
-        
+        last_date = num_to_datetime(max_date.date.iat[0], datetime=False)
+
         if last_date > from_date:
             query.set_from_date(last_date)
         else:
             query.set_from_date(from_date)
 
     results = update_letters_table_by_symbols(query, [symbol])
     return results
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/query.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 import pandas as pd
 import urllib.parse as urlparse
 from urllib.parse import urlencode
 
 from codal_tsetmc.tools.exception import *
 from codal_tsetmc.tools.string import (
     LETTERS_CODE_TO_TITLE, FA_TO_EN_DIGITS,
@@ -10,18 +12,28 @@
 from codal_tsetmc.tools.api import get_dict_from_xml_api
 from codal_tsetmc.models.companies import (
     CompanyStatuses, CompanyTypes, 
     ReportTypes, LetterTypes, Auditors,
 )
 
 
+def remove_none(dictionary) -> dict:
+    filtered = {k: v for k, v in dictionary.items() if v != -1}
+    dictionary.clear()
+    dictionary.update(filtered)
+
+    return dictionary
+
+
 class CodalQuery:
 
     def __init__(self):
-        # جستوجی اطاعیه‌های سایت کودال
+        # جستجوی اطاعیه‌های سایت کودال
+        self.total = None
+        self.letters = None
         self.base_url = "codal.ir"
         self.report_list_html = f"https://{self.base_url}/ReportList.aspx?"
         self.search_query_xml = f"https://search.{self.base_url}/api/search/v2/q?"
         self.pages = None
         self.params = {
             "PageNumber": 1,
             "Symbol": -1,
@@ -98,62 +110,62 @@
     def set_letter_code(self, code: str = "") -> None:
         BadValueInput(code).int_str_type()
         self.params["LetterCode"] = -1 if code == "" else code
 
     # تنظیم طول دوره
     def set_length_period(self, period=-1) -> None:
         # طول دوره
-        lengthPeriod = {
+        length_period = {
             None: -1, 'همه موارد': -1, '-۱': -1, '۰': -1,
             '۱': 1, '۲': 2, '۳': 3, '۴': 4, '۵': 5, '۶': 6,
             '۷': 7, '۸': 8, '۹': 9, '۱۰': 10, '۱۱': 11, '۱۲': 12,
             -1: -1, 0: -1,
             1: 1, 2: 2, 3: 3, 4: 4, 5: 5, 6: 6,
             7: 7, 8: 8, 9: 9, 10: 10, 11: 11, 12: 12
         }
-        self.params["Length"] = -1 if period == "" else lengthPeriod[period]
+        self.params["Length"] = -1 if period == "" else length_period[period]
 
     # تنظیم از تاریخ
     def set_from_date(self, date: str = "1300/01/01") -> None:
         BadValueInput(date).date_type()
         self.params["FromDate"] = -1 if date == "" else date
 
     # تنظیم تا تاریخ
     def set_to_date(self, date: str = "1500/01/01") -> None:
         BadValueInput(date).date_type()
         self.params["ToDate"] = -1 if date == "" else date
 
     # تنظیم حسابرسی شده
     def set_audited(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+        BadValueInput(status).boolean_type()
         self.params["Audited"] = str(status).lower()
 
     # تنظیم حسابرسی نشده
     def set_not_audited(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+        BadValueInput(status).boolean_type()
         self.params["NotAudited"] = str(status).lower()
 
     # تنظیم اصلی
-    def set_consolidatable(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+    def set_consolidate_table(self, status: bool = True) -> None:
+        BadValueInput(status).boolean_type()
         self.params["Consolidatable"] = str(status).lower()
 
     # تنظیم تلفیقی
-    def set_not_consolidatable(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+    def set_not_consolidate_table(self, status: bool = True) -> None:
+        BadValueInput(status).boolean_type()
         self.params["NotConsolidatable"] = str(status).lower()
 
     # تنظیم فقط زیرمجموعه ها
     def set_childs(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+        BadValueInput(status).boolean_type()
         self.params["Childs"] = str(status).lower()
 
     # تنظیم فقط شرکت اصلی
     def set_mains(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+        BadValueInput(status).boolean_type()
         self.params["Mains"] = str(status).lower()
 
     # تنظیم موسسه حسابرسی شرکت
     def set_auditor_ref(self, name: str = None) -> None:
         BadValueInput(name).string_type()
         code = Auditors.query.filter_by(name=name).first()
         self.params["AuditorRef"] = code.code if bool(code) else -1
@@ -161,24 +173,18 @@
     # سالی مالی منتهی به
     def set_year_end_to_date(self, date: str = "1300/01/01") -> None:
         BadValueInput(date).date_type()
         self.params["YearEndToDate"] = -1 if date == "" else date
 
     # تنظیم فقط اطلاعیه های منتشر شده از طرف سازمان
     def set_publisher(self, status: bool = True) -> None:
-        BadValueInput(status).boolian_type()
+        BadValueInput(status).boolean_type()
         self.params["Publisher"] = str(status).lower()
     
     # حذف تنظیمات
-    def remove_none(self, dictionary) -> dict:
-        filtered = {k: v for k, v in dictionary.items() if v != -1}
-        dictionary.clear()
-        dictionary.update(filtered)
-
-        return dictionary
 
     # تنظیم شماره صفحه
     def set_page_number(self, number: int = 0) -> None:
         if bool(number):
             BadValueInput(number).integer_type()
             self.params['PageNumber'] = number
         else:
@@ -195,19 +201,19 @@
     """################
     گرفتن لینک کوئری کدال 
     ################"""
 
     # گرفتن لینک
     def get_query_url(self, api: bool = True) -> str:
         params = self.params
-        BadValueInput(api).boolian_type()
+        BadValueInput(api).boolean_type()
         url = self.search_query_xml if api else self.report_list_html
         url_parts = list(urlparse.urlparse(url))
         query = dict(urlparse.parse_qsl(url_parts[4]))
-        query.update(self.remove_none(params))
+        query.update(remove_none(params))
         url_parts[4] = f"&{urlencode(query)}&search=true" if api else f"search&{urlencode(query)}"
 
         return urlparse.urlunparse(url_parts)
 
     # گرفتن لیست گزارش
     def get_report_list_url(self) -> str:
         return self.get_query_url(False)
@@ -217,40 +223,40 @@
         return self.get_query_url(True)
     
     """################
     گرفتن اطلاعات از کدال 
     ################"""
 
     # گرفتن اطلاعات کلی در یک صفحه
-    def get_api_sigle_page(self) -> dict:
+    def get_api_single_page(self) -> dict:
         url = self.get_api_search_url()
         response = get_dict_from_xml_api(url)
         self.total = response["Total"]
         self.page = response["Page"]
         
         return response["Letters"]
 
     # گرفتن اطلاعات کلی در همه صفحات
-    def get_api_multi_page(self, pages: int = 0) -> dict:
-        last_letters = self.get_api_sigle_page()
+    def get_api_multi_page(self, pages: int = 0) -> list[Any]:
+        last_letters = self.get_api_single_page()
         letters = []
         pages = pages if bool(pages) else self.page
         reversed_range = list(range(2, pages + 1))
         reversed_range.sort(reverse=True)
         for page in reversed_range:
             print(f"get page {page} of {pages}", end="\r", flush=True)
             self.set_page_number(page)
-            letters += self.get_api_sigle_page()
+            letters += self.get_api_single_page()
         
         letters += last_letters
 
         return letters
 
     # گرفتن اطلاعات کلی تمام صفحات به صورت یک فرمت داده
-    def get_letters(self, pages: int = 0, show = False) -> pd.DataFrame:
+    def get_letters(self, pages: int = 0, show=False) -> pd.DataFrame:
         letters = self.get_api_multi_page(pages)
         df = pd.DataFrame(letters).replace(regex=FA_TO_EN_DIGITS)
         df["LetterSerial"] = df["Url"].replace(regex={
             r"^.*LetterSerial=": "",
             r"\&.*$": ""
         })
         df["LetterTypes"] = df["LetterCode"].replace(regex=LETTERS_CODE_TO_TITLE)
@@ -264,10 +270,7 @@
             "CompanySymbol", "CompanyName",
         ]]
         df = df_col_to_snake_case(df)
         if show:
             return df
         else:
             self.letters = df
-    
-    
-
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/codal/report.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/codal/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,101 +1,109 @@
 import re
 import json
+
 import requests
 import pandas as pd
-import sys
-import asyncio
 import aiohttp
 from bs4 import BeautifulSoup
+from pandas import DataFrame
+
 from codal_tsetmc.tools.api import get_results_by_asyncio_loop
 from codal_tsetmc.tools.string import (
     SHEET_NAME_TO_ID, EMPTY_TO_NONE, AR_TO_FA_LETTER,
     to_snake_case,
     df_col_to_snake_case,
     datetime_to_num,
     replace_all,
 )
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
 from codal_tsetmc.models.companies import Letters
 
+
 def extract_sheet_id(sheet: str) -> str:
     if sheet in SHEET_NAME_TO_ID.keys():
         return f"&sheetId={SHEET_NAME_TO_ID[sheet]}"
     elif sheet in SHEET_NAME_TO_ID.values():
         return f"&sheetId={sheet}"
     else:
         return ""
 
+
 def get_letter(letter_serial: str, sheet: str = "") -> str:
     sheet_id = extract_sheet_id(sheet)
-    headers={
-        "User-Agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36'
+    headers = {
+        "User-Agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 '
+                      'Safari/537.36'
     }
     url = f"https://codal.ir/Reports/Decision.aspx?LetterSerial={letter_serial}&rt=0&let=6&ct=0&ft=-1{sheet_id}"
     response = requests.get(url=url, cookies={}, headers=headers)
     return response.text
 
+
 async def get_letter_async(serial: str, sheet: str = ""):
-    id = extract_sheet_id(sheet)
-    url = f"https://codal.ir/Reports/Decision.aspx?LetterSerial={serial}&rt=0&let=6&ct=0&ft=-1{id}"
-    headers={
-        "User-Agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36'
+    sheet_id = extract_sheet_id(sheet)
+    url = f"https://codal.ir/Reports/Decision.aspx?LetterSerial={serial}&rt=0&let=6&ct=0&ft=-1{sheet_id}"
+    headers = {
+        "User-Agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 '
+                      'Safari/537.36'
     }
     async with aiohttp.ClientSession() as session:
         async with session.get(url, headers=headers, cookies={}) as resp:
             response = await resp.text()
             return response
 
+
 def extract_options(letter_string: str):
     soup = BeautifulSoup(letter_string, 'html.parser')
     return [item.get("value") for item in soup.find_all("option")]
 
-def extract_symbol_and_name(letter_string: str) -> str:
+
+def extract_symbol_and_name(letter_string: str) -> dict[str, str | None | int]:
     soup = BeautifulSoup(letter_string, 'html.parser')
     return {
         "name": soup.find(id="ctl00_txbCompanyName").string,
         "capital": int(soup.find(id="ctl00_lblListedCapital").string.replace(",", "")),
         "symbol": soup.find(id="ctl00_txbSymbol").string,
         "isic": soup.find(id="ctl00_lblISIC").string,
         "company_state": soup.find(id="ctl00_lblCompanyState").string,
-    } 
+    }
 
 
 def edit_datasource_detail(datasource: dict) -> dict:
-    datasource = {to_snake_case(k):v for k,v in datasource.items()}
+    datasource = {to_snake_case(k): v for k, v in datasource.items()}
     dates = [
-        "period_end_to_date", 
+        "period_end_to_date",
         "year_end_to_date",
         "register_date_time",
         "sent_date_time",
         "publish_date_time"
     ]
     for date in dates:
         datasource[date] = datetime_to_num(datasource[date])
 
     return datasource
 
+
 def extract_datasource(letter_string: str) -> dict:
     regex = r"datasource = (.*);\r\n"
     data_json = re.search(regex, letter_string)
     datasource = json.loads(data_json.group(1))
     return edit_datasource_detail(datasource)
 
 
-def update_financial_statment_header(letter_string: str):
-
+def update_financial_statement_header(letter_string: str):
     symbol_and_name = extract_symbol_and_name(letter_string)
     datasource = extract_datasource(letter_string)
 
     df = pd.DataFrame.from_records(
         [{**symbol_and_name, **datasource}]
     )
 
     df = df[[
-        "name", 
+        "name",
         "capital",
         "symbol",
         "isic",
         "company_state",
         "title_fa",
         "title_en",
         "period_end_to_date",
@@ -111,119 +119,125 @@
         "is_for_auditing",
         "period",
         "state"
     ]]
 
     fill_table_of_db_with_df(df, "financial_statement_header", "tracing_no")
 
+
 def edit_sheet_detail(sheet: dict) -> dict:
-    return {to_snake_case(k):v for k,v in sheet.items()}
+    return {to_snake_case(k): v for k, v in sheet.items()}
+
 
 def extract_sheet(datasource, sheet: str = "صورت سود و زیان") -> dict:
     for sht in datasource["sheets"]:
         if sht["title_Fa"] == sheet:
             return edit_sheet_detail(sht)
 
-def extract_sheet_components(sheet: dict) -> dict:
+
+def extract_sheet_components(sheet: dict) -> DataFrame:
     products = pd.DataFrame({"text": [], "value": []})
     # units = pd.DataFrame({"text": [],  "value": []})
-    for id in sheet["sheetComponents"].keys():
-        detail = sheet["sheetComponents"][id][0]
+    for component_id in sheet["sheetComponents"].keys():
+        detail = sheet["sheetComponents"][component_id][0]
         if detail["typeName"] != "Date":
-            if detail["data"][0]["params"] == []:
+            if not detail["data"][0]["params"]:
                 df = pd.DataFrame(detail["data"])
                 products = pd.concat([products, df[["text", "value"]]])
             else:
-                #TODO: add units of products
+                # TODO: add units of products
                 pass
 
     return products
 
+
 def edit_table_detail(table: dict) -> dict:
     if table["title_En"] is not None:
         table["title_En"] = replace_all(table["title_En"], {
             "BalanceSheet": "Balance Sheet",
             "Income Statment": "Income Statement"
         })
     else:
         table["title_En"] = None
-    
-    return {to_snake_case(k):v for k,v in table.items()}
 
-def extract_table(sheet: dict, table: str = "صورت سود و زیان") -> pd.DataFrame:
+    return {to_snake_case(k): v for k, v in table.items()}
+
+
+def extract_table(sheet: dict, table: str = "صورت سود و زیان") -> dict:
     for tbl in sheet["tables"]:
         if tbl["title_Fa"] == table:
             return edit_table_detail(tbl)
 
+
 def extract_cells(table: dict) -> pd.DataFrame:
     df = pd.DataFrame(table["cells"])
     df = df_col_to_snake_case(df)
     df = df.replace(regex=AR_TO_FA_LETTER).replace(regex=EMPTY_TO_NONE)
     df["row"] = df["address"].str.slice(start=1)
     df["col"] = df["address"].str.slice(stop=1)
     df = df[
-        (df['value'].notna()) & 
+        (df['value'].notna()) &
         (df["is_visible"]) &
         (df["cell_group_name"] == "Body")
-    ]
+        ]
 
     return df.drop_duplicates()
 
+
 def extract_items(df: pd.DataFrame) -> pd.DataFrame:
     if "value_type_name" in df.columns:
         df = df[df["value_type_name"].isin(["Fix", "Component"])]
     else:
         df = df[df["col"].isin(["A"])]
 
     df = df.rename(columns={"value": "item"})[["row", "category", "item"]]
 
     return df.drop_duplicates()
 
+
 def extract_values(df: pd.DataFrame) -> pd.DataFrame:
     if "value_type_name" in df.columns:
         df = df[df["value_type_name"].isin(["FormControl", "-1"])]
     else:
         df = df[df["data_type_name"].isin(["Currency"])]
-    
+
     df = df[~pd.isna(df["period_end_to_date"])]
-    
+
     df["period_end_to_date"] = df["period_end_to_date"].apply(datetime_to_num)
 
     if "year_end_to_date" in df.columns:
         df["year_end_to_date"] = df["year_end_to_date"].apply(datetime_to_num)
         df[["period_end_to_date", "year_end_to_date"]] = df[
             ["period_end_to_date", "year_end_to_date"]
         ].fillna(method="ffill", axis=1, limit=1)
     else:
         df["year_end_to_date"] = df["period_end_to_date"]
-    
+
     df["value"] = pd.to_numeric(df["value"])
     df["cell_id"] = (
-        df["meta_table_id"].astype(str) + 
-        '-' + df["meta_table_code"].astype(str) +
-        '-' + df["address"].astype(str) +
-        '-' + df["category"].astype(str) +
-        '-' + df["period_end_to_date"].astype(str)
+            df["meta_table_id"].astype(str) +
+            '-' + df["meta_table_code"].astype(str) +
+            '-' + df["address"].astype(str) +
+            '-' + df["category"].astype(str) +
+            '-' + df["period_end_to_date"].astype(str)
     )
-    
+
     df = df[[
         "row", "value", "cell_id", "category",
         "year_end_to_date", "period_end_to_date",
     ]]
-    return  df.drop_duplicates()
-
-
+    return df.drop_duplicates()
 
 
 def extract_table_with_single_item(table: dict) -> pd.DataFrame:
     cells = extract_cells(table)
     items = extract_items(cells)
     values = extract_values(cells)
     df = pd.merge(values, items)[[
-        "cell_id", "period_end_to_date", 
+        "cell_id", "period_end_to_date",
         "year_end_to_date", "item", "value"
     ]]
 
     return df.drop_duplicates()
 
 
 def add_sheet_and_table_detail(df, datasource, sheet, table):
@@ -235,38 +249,38 @@
     df["table_title_fa"] = table["title_fa"]
     df["description"] = table["description"]
     df["alias_name"] = table["alias_name"]
     return df
 
 
 TABLES_WHIT_SINGLE_ITEM = [
-    "Balance Sheet", 
+    "Balance Sheet",
     "Income Statement",
     "Cash Flow",
     "Sales trend and cost over the last 5 years",
-    "The cost of the sold goods", 
+    "The cost of the sold goods",
     "Staff status",
     "Other operating income",
     "Other operating expenses",
     "Non-operation income and expenses investment income",
     "Non-operation income and expenses miscellaneous items"
 ]
 
+
 def update_financial_statement_table(datasource, sheet, table):
     sheet = edit_sheet_detail(sheet)
     table = edit_table_detail(table)
     if table["title_en"] in TABLES_WHIT_SINGLE_ITEM:
         df = extract_table_with_single_item(table)
         db_table = "financial_statement_table_with_single_item"
         df = add_sheet_and_table_detail(df, datasource, sheet, table)
         fill_table_of_db_with_df(df, db_table, "cell_id")
-    
 
-async def update_stock_financial_statement_table_async(symbol, from_date = 1400, to_date = 1500):
 
+async def update_stock_financial_statement_table_async(symbol, from_date=1400, to_date=1500):
     letter_serials = Letters.query.filter(
         Letters.symbol == symbol,
         Letters.publish_date_time > datetime_to_num(from_date),
         Letters.publish_date_time < datetime_to_num(to_date),
         Letters.letter_types == "صورت های مالی میان دوره ای"
     )
 
@@ -277,30 +291,31 @@
         options = ["0"]
         option_active = True
         while option_active:
             option = options[0]
             letter_string = await get_letter_async(serial, option)
             if option == "0":
                 options = extract_options(letter_string)
-                if "19" in options: options.remove("19")
-            
+                if "19" in options:
+                    options.remove("19")
+
             if "datasource" in letter_string:
-                update_financial_statment_header(letter_string)
+                update_financial_statement_header(letter_string)
 
                 datasource = extract_datasource(letter_string)
                 for sheet in datasource["sheets"]:
                     for table in sheet["tables"]:
-                        if table["cells"] != []:
+                        if table["cells"]:
                             update_financial_statement_table(datasource, sheet, table)
-                
-            options.remove(option)
-            if options == []: option_active = False
 
+            options.remove(option)
+            if not options:
+                option_active = False
 
 
-def update_stocks_financial_statement_table(symbols, from_date = 1400, to_date = 1500, msg=""):
+def update_stocks_financial_statement_table(symbols, from_date=1400, to_date=1500, msg=""):
     if symbols.__class__ != list:
         symbols = [symbols]
-    
+
     tasks = [update_stock_financial_statement_table_async(symbol, from_date, to_date) for symbol in symbols]
     get_results_by_asyncio_loop(tasks)
     print(msg, end="\r")
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/other/commodity.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/other/commodity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from jdatetime import datetime as jdt
-import asyncio
 import aiohttp
-import sys
-import pandas as pd
 import jalali_pandas
+import pandas as pd
 import requests
 
 from codal_tsetmc.config.engine import engine
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
 from codal_tsetmc.tools.api import (
     get_csv_from_github,
     get_results_by_asyncio_loop
@@ -27,99 +25,106 @@
     df["date"] = df["jdate"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
     df["price"] = pd.to_numeric(df["close"].str.replace(",", ""))
 
     df = df.sort_values("date")
 
     return df[["date", "price"]]
 
+
 def get_commodity_price_history(symbol: str) -> pd.DataFrame:
+    df = None
     url = f"https://api.tgju.org/v1/market/indicator/summary-table-data/{symbol}"
-    response = requests.get(url, params=[], headers={}) #('length', '100'),
+    response = requests.get(url, params=[], headers={})  # ('length', '100'),
     new = cleanup_commodity_price_records(response)
     if symbol == "price_dollar_rl":
         old = get_csv_from_github(symbol)
         old["date"] = old["date"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
-        
+
         df = pd.concat(new, old[~old.date.isin(new.date)])
 
     df["symbol"] = symbol
     df.sort_values("date")
     df = df.set_index("date")
 
     return df
 
 
 async def update_commodity_prices(symbol: str):
+    days = None
+    url = ""
     try:
-        jnow = jdt.now()
+        now = jdt.now()
         try:
             query = f"select max(date) as date from commodity_price where symbol = '{symbol}'"
             max_date = pd.read_sql(query, engine)
             last_date = max_date.date.iat[0]
-            days = jnow - jdt.strptime(last_date, "%Y%m%d%H%M%S")
+            days = now - jdt.strptime(last_date, "%Y%m%d%H%M%S")
 
         except Exception as e:
+            print(e)
             last_date = None
         try:
-            if last_date is None: 
+            if last_date is None:
                 url = f"https://api.tgju.org/v1/market/indicator/summary-table-data/{symbol}"
-            elif days.days > 0: 
+            elif days.days > 0:
                 url = f"https://api.tgju.org/v1/market/indicator/summary-table-data/{symbol}?length={days.days}"
-            else:  # The price data for this symbol is updateed
+            else:  # The price data for this symbol is updated
                 return
         except Exception as e:
-            print(f"Error on formating price:{str(e)}")
+            print(f"Error on formatting price:{str(e)}")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
                 response = await resp.json()
 
         df = cleanup_commodity_price_records(response)
         df["symbol"] = symbol
-        df["up_date"] = jnow.strftime("%Y%m%d000000")
+        df["up_date"] = now.strftime("%Y%m%d000000")
 
         fill_table_of_db_with_df(
-            df, 
+            df,
             columns="date",
             table="commodity_price",
             conditions=f"where symbol = '{symbol}'",
             text=f"symbol: {symbol}"
         )
 
         return True, symbol
 
     except Exception as e:
         return e, symbol
 
+
 def update_commodities_prices(symbols, msg=""):
-    print(f"{' '*25} update Commodities ", end="\r")
+    print(f"{' ' * 25} update Commodities ", end="\r")
     tasks = [update_commodity_prices(symbol) for symbol in symbols]
     results = get_results_by_asyncio_loop(tasks)
     print(msg, end="\r")
 
     return results
 
+
 def fill_commodities_prices_table():
     symbols = ["price_dollar_rl"]
     for i, symbol in enumerate(symbols):
-        print(f"{' '*35} total progress: {100*(i+1)/len(symbols):.2f}%", end="\r")
+        print(f"{' ' * 35} total progress: {100 * (i + 1) / len(symbols):.2f}%", end="\r")
         if symbol == "price_dollar_rl":
 
             query = f"select min(date) as date from commodity_price where symbol = '{symbol}'"
             min_date = pd.read_sql(query, engine)
             first_date = min_date.date.iat[0]
             if first_date != "13600707000000":
                 df = get_csv_from_github(symbol)
                 df["date"] = df["date"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
                 df["symbol"] = symbol
                 df["up_date"] = jdt.now().strftime("%Y%m%d000000")
-                
+
                 fill_table_of_db_with_df(
-                    df, 
+                    df,
                     columns="date",
                     table="commodity_price",
                     conditions=f"where symbol = '{symbol}'",
                     text=f"symbol: {symbol}"
                 )
 
         update_commodities_prices([symbol])
-    print("Price Download Finished.", " "*50)
+    print("Price Download Finished.", " " * 50)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/capital.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/capital.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from jdatetime import datetime as jdt
 from datetime import datetime
-import asyncio
+import jalali_pandas
 import aiohttp
 import pandas as pd
-import jalali_pandas
 import requests
 import io
-import sys
 from codal_tsetmc.config.engine import engine, session
 from codal_tsetmc.models.stocks import Stocks
 from codal_tsetmc.tools.database import fill_table_of_db_with_df
 from codal_tsetmc.tools.api import (
     get_data_from_cdn_tsetmec_api,
     get_results_by_asyncio_loop
 )
 from codal_tsetmc.tools.string import value_to_float
 from codal_tsetmc.download.tsetmc.stock import is_stock_in_bourse_or_fara_or_paye
 
 
-def get_stock_capital_daily(code: str, date = None):
+def get_stock_capital_daily(code: str, date=None):
     if date is None:
         date = datetime.now().strftime("%Y%m%d")
-    
+
     data = "Instrument/GetInstrumentHistory"
     dict_data = get_data_from_cdn_tsetmec_api(data, code, date)
     return dict_data["instrumentHistory"]["zTitad"]
 
 
 def cleanup_stock_capitals_records(response):
     df = pd.read_html(io.StringIO(response))[0]
@@ -33,66 +31,69 @@
     df["date"] = df["date"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
     df = df.sort_index(ascending=False)
     df["old"] = df["old"].apply(value_to_float)
     df["new"] = df["new"].apply(value_to_float)
     df = df[
         (df.new > df.new.shift(fill_value=0)) &
         (df.old > df.old.shift(fill_value=0))
-    ]
+        ]
     df = df[
         (df.old == df.new.shift(fill_value=0)) |
         (df.old == min(df.old)) |
         (df.new == max(df.new))
-    ]
+        ]
 
     df = df.sort_values("date")
 
     return df
 
+
 def get_stock_capitals_history(code: str) -> pd.DataFrame:
     url = f"http://old.tsetmc.com/Loader.aspx?ParTree=15131H&i={code}"
     response = requests.get(url).text
     df = cleanup_stock_capitals_records(response)
     df["code"] = code
 
     return df
 
+
 async def update_stock_capitals(code: str):
-    
+    url = ""
     try:
         if not is_stock_in_bourse_or_fara_or_paye(code):
             return
-        
+
         jnow = jdt.now().strftime("%Y%m%d000000")
         try:
             max_date_query = (
                 f"select max(up_date) as up_date from stock_capital where code = '{code}'"
             )
             max_date = pd.read_sql(max_date_query, engine)
             last_up_date = max_date.up_date.iat[0]
 
         except Exception as e:
+            print(e)
             last_up_date = None
         try:
-            # need to updata new capital data
+            # need to update new capital data
             if last_up_date is None or last_up_date < jnow:
                 url = f"http://old.tsetmc.com/Loader.aspx?ParTree=15131H&i={code}"
-            else:  # The capital data for this code is updateed
+            else:  # The capital data for this code is updated
                 return
         except Exception as e:
-            print(f"Error on formating capital:{str(e)}")
+            print(f"Error on formatting capital:{str(e)}")
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as resp:
+        async with aiohttp.ClientSession() as ses:
+            async with ses.get(url) as resp:
                 response = await resp.text()
-        
+
         df = cleanup_stock_capitals_records(response)
 
         df["code"] = code
-        df["up_date"]= jnow
+        df["up_date"] = jnow
 
         fill_table_of_db_with_df(
             df,
             columns="date",
             table="stock_capital",
             conditions=f"where code = '{code}'",
             text=f"stock: {code}"
@@ -104,28 +105,29 @@
         return e, code
 
 
 def update_stocks_capitals(codes, msg=""):
     tasks = [update_stock_capitals(code) for code in codes]
     get_results_by_asyncio_loop(tasks)
     print(msg, end="\r")
+    return True
 
 
 def update_stocks_group_capitals(group_code):
     stocks = session.query(Stocks.code).filter_by(group_code=group_code).all()
-    print(f"{' '*25} group: {group_code}", end="\r")
+    print(f"{' ' * 25} group: {group_code}", end="\r")
     codes = [stock[0] for stock in stocks]
-    msg = "group "+group_code+" updated"
+    msg = "group " + group_code + " updated"
     results = update_stocks_capitals(codes, msg)
     return results
 
 
 def fill_stocks_capitals_table():
     codes = session.query(Stocks.group_code).distinct().all()
     for i, code in enumerate(codes):
         print(
-            f"{' '*35} total progress: {100*(i+1)/len(codes):.2f}%",
+            f"{' ' * 35} total progress: {100 * (i + 1) / len(codes):.2f}%",
             end="\r",
         )
         update_stocks_group_capitals(code[0])
 
-    print("Capital Download Finished.", " "*50)
+    print("Capital Download Finished.", " " * 50)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/price.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/price.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,156 @@
 from jdatetime import datetime as jdt
 from datetime import datetime
-import asyncio
+import jalali_pandas
 import aiohttp
 import pandas as pd
-import jalali_pandas
 import io
 import requests
-import sys
 from codal_tsetmc.config.engine import session
 from codal_tsetmc.models.stocks import Stocks
 from codal_tsetmc.tools.database import (
     fill_table_of_db_with_df,
     read_table_by_conditions
 )
 from codal_tsetmc.tools.api import (
     get_data_from_cdn_tsetmec_api,
     get_results_by_asyncio_loop
 )
-from codal_tsetmc.download.tsetmc.stock import  (
-    is_stock_in_akhza_bond, 
+from codal_tsetmc.download.tsetmc.stock import (
+    is_stock_in_akhza_bond,
     is_stock_in_gam_bond,
     is_stock_in_bourse_or_fara_or_paye
 )
 
+INDEX_CODE = "32097828799138957"
+
+
 def get_index_prices_history():
-    code = "32097828799138957"
-    url = f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{code}'
+    url = f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{INDEX_CODE}'
     headers = {
-        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 '
+                      'Safari/537.36',
     }
     s = requests.get(url, headers=headers, verify=False).json()
     df = pd.DataFrame(s["indexB2"])[["dEven", "xNivInuClMresIbs"]]
     df.columns = ["date", "price"]
     df["date"] = df["date"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
-    df["jdate"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y-%m-%d'))
-    df["code"] = code
+    df["date"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y%m%d000000'))
+    df["code"] = INDEX_CODE
     df["symbol"] = "شاخص كل6"
-    df["ticker"] = "INDEX"
     df["value"] = pd.NA
     df["volume"] = pd.NA
     df = df.sort_values("date")
 
     return df
 
+
 def update_index_prices():
-    index = "32097828799138957"
     df = get_index_prices_history()
-    df["date"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y%m%d000000'))
     df["up_date"] = jdt.now().strftime("%Y%m%d000000")
     fill_table_of_db_with_df(
-        df[["date", "symbol", "ticker", "code", "price", "volume", "value", "up_date"]], 
+        df[["date", "symbol", "code", "price", "volume", "value", "up_date"]],
         columns="date",
         table="stock_price",
-        conditions=f"where code = '{index}'",
-        text=f"stock: {index}"
+        conditions=f"where code = '{INDEX_CODE}'",
+        text=f"stock: {INDEX_CODE}"
     )
 
+
 def get_stock_price_daily(code: str, date: str):
     data = "ClosingPrice/GetClosingPriceDaily"
     dict_data = get_data_from_cdn_tsetmec_api(data, code, date)
-    
+
     return dict_data["closingPriceDaily"]["pClosing"]
 
-def cleanup_stock_prices_records(response):
-    df = pd.read_csv(io.StringIO(response))
-    df.columns = [i[1:-1].lower() for i in df.columns]
-    df["date"] = df["dtyyyymmdd"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
+
+def cleanup_stock_prices_records(data):
+    df = pd.read_csv(io.StringIO(data), delimiter="@", lineterminator=";", engine="c", header=None)
+    df.columns = "date high low price close open yesterday value volume count".split()
+    df["date"] = df["date"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
     df["date"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y%m%d000000'))
     df["price"] = df["close"]
-    df["volume"] = df["vol"]
     df = df.sort_values("date")
 
-    return df[["date", "ticker", "volume", "value", "price"]]
+    return df[["date", "volume", "value", "price"]]
+
 
 def get_stock_prices_history(code: str) -> pd.DataFrame:
     url = f"http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0"
     data = requests.get(url).text
     df = pd.read_csv(io.StringIO(data), delimiter="@", lineterminator=";", engine="c", header=None)
     df.columns = "date high low price close open yesterday value volume count".split()
     df["date"] = df["date"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
-    df["jdate"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y-%m-%d'))
     df["code"] = code
 
     return df
 
+
 async def update_stock_prices(code: str):
+    url = ""
     try:
-        if not is_stock_in_bourse_or_fara_or_paye(code) and not is_stock_in_akhza_bond(code) and not is_stock_in_gam_bond(code):
+        if not is_stock_in_bourse_or_fara_or_paye(code) and not is_stock_in_akhza_bond(
+                code) and not is_stock_in_gam_bond(code):
             return
-        
+
         now = datetime.now().strftime("%Y%m%d")
         try:
 
-            max_date_stock = read_table_by_conditions("stock_price", "code", code, "max(date) AS date")
-            last_date_stock = max_date_stock.date.iat[0]
+            def get_max_date_stock():
+                return read_table_by_conditions(
+                    table="stock_price",
+                    variable="code",
+                    value=code,
+                    columns="max(date) AS date"
+                )
+
+            def get_max_date_index():
+                return read_table_by_conditions(
+                    table="stock_price",
+                    variable="code",
+                    value=INDEX_CODE,
+                    columns="max(date) AS date"
+                )
 
-            max_date_index = read_table_by_conditions("stock_price", "ticker", "INDEX", "max(date) AS date")
-            last_date_index = max_date_index.date.iat[0]
+            last_date_stock = get_max_date_stock().date.iat[0]
+            last_date_index = get_max_date_index().date.iat[0]
 
-            if last_date_index is None or last_date_index < last_date_stock:
+            if last_date_index is None or (last_date_stock is not None and int(last_date_index) < int(last_date_stock)):
                 update_index_prices()
-                max_date_index = read_table_by_conditions("stock_price", "ticker", "INDEX", "max(date) AS date")
-                last_date_index = max_date_index.date.iat[0]
+                last_date_index = get_max_date_index().date.iat[0]
 
         except Exception as e:
-            last_date_stock = None
+            print(e)
+            last_date_stock = "0"
+            last_date_index = "0"
+
         try:
-            if last_date_stock is None:  # no any record added in database
-                url = f"http://old.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom=20000101&DateTo={now}&b=0"
-            elif last_date_stock < last_date_index:  # need to updata new price data
+            if last_date_stock is None:  # Not any record added in database
+                url = (
+                    f"http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0"
+                )
+            elif int(last_date_stock) < int(last_date_index):  # need to update new price data
                 last_date = jdt.strptime(str(int(last_date_stock)), "%Y%m%d%H%M%S").togregorian().strftime("%Y%m%d")
-                url = f"http://old.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom={str(last_date)}&DateTo={now}&b=0"
-            else:  # The price data for this code is updateed
+                url = (
+                    f"http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0"
+                )
+            else:  # The price data for this code is updated
                 return
+
         except Exception as e:
-            print(f"Error on formating price:{str(e)}")
+            print(f"Error on formatting price:{str(e)}")
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 '
+                          'Safari/537.36'
+        }
+        async with aiohttp.ClientSession() as ses:
+            async with ses.get(url, headers=headers) as resp:
+                data = await resp.text()
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as resp:
-                response = await resp.text()
-        
-        df = cleanup_stock_prices_records(response)
+        df = cleanup_stock_prices_records(data)
         df["code"] = code
         stock = Stocks.query.filter_by(code=code).first()
         df["symbol"] = stock.symbol
         df["up_date"] = jdt.now().strftime("%Y%m%d000000")
 
         fill_table_of_db_with_df(
             df,
@@ -135,33 +161,34 @@
         )
 
         return True, code
 
     except Exception as e:
         return e, code
 
+
 def update_stocks_prices(codes, msg=""):
     tasks = [update_stock_prices(code) for code in codes]
     get_results_by_asyncio_loop(tasks)
     print(msg, end="\r")
+    return True
 
 
 def update_stocks_group_prices(group_code):
     stocks = session.query(Stocks.code).filter_by(group_code=group_code).all()
-    print(f"{' '*25} group: {group_code}", end="\r")
+    print(f"{' ' * 25} group: {group_code}", end="\r")
     codes = [stock[0] for stock in stocks]
     msg = "group " + group_code + " updated"
     results = update_stocks_prices(codes, msg)
     return results
 
 
 def fill_stocks_prices_table():
     update_index_prices()
     codes = session.query(Stocks.group_code).distinct().all()
     for i, code in enumerate(codes):
         print(
-            f"{' '*35} total progress: {100*(i+1)/len(codes):.2f}%",
+            f"{' ' * 35} total progress: {100 * (i + 1) / len(codes):.2f}%",
             end="\r",
         )
         update_stocks_group_prices(code[0])
-    print("Price Download Finished.", " "*50)
-
+    print("Price Download Finished.", " " * 50)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/download/tsetmc/stock.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/download/tsetmc/stock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,122 @@
 import requests
-import sys
 import re
-import asyncio
 import aiohttp
 from codal_tsetmc.config.engine import session
 from codal_tsetmc.tools.api import (
     get_csv_from_github,
     get_results_by_asyncio_loop
 )
 from codal_tsetmc.models.stocks import Stocks
 
+
 def is_stock_in_bourse_or_fara_or_paye(code):
     group_type = ["1Z", "91", "C1", "G1", "L1", "N1", "N2", "P1", "V1", "Z1"]
     return Stocks.query.filter_by(code=code).first().group_type in group_type
 
+
 def is_stock_in_akhza_bond(code):
     group_type = ["I1", "I2", "I4"]
     return Stocks.query.filter_by(code=code).first().group_type in group_type
 
+
 def is_stock_in_gam_bond(code):
     stock = Stocks.query.filter_by(code=code).first()
     return stock.group_type in ["N4"] and stock.group_name in ["اوراق تامين مالي"]
 
 
-def get_stock_detail(code: str, timeout = 3):
+def extract_instrumentInfo(data):
+    return {
+        "symbol": data["instrumentInfo"]["lVal18AFC"],
+        "name": data["instrumentInfo"]["lVal30"],
+        "name_en": data["instrumentInfo"]["lVal18"],
+        "isin": data["instrumentInfo"]["cIsin"],
+        "code": data["instrumentInfo"]["insCode"],
+        "capital": data["instrumentInfo"]["zTitad"] if data["instrumentInfo"][
+                                                           "insCode"
+                                                       ] != "32097828799138957" else 1_000_000_000,
+        "instrument_code": data["instrumentInfo"]["insCode"],
+        "instrument_id": data["instrumentInfo"]["instrumentID"],
+        "group_name": data["instrumentInfo"]["sector"]["lSecVal"],
+        "group_code": data["instrumentInfo"]["sector"]["cSecVal"].replace(" ", ""),
+        "group_type": data["instrumentInfo"]["cgrValCot"],
+        "market_name": data["instrumentInfo"]["flowTitle"],
+        "market_code": data["instrumentInfo"]["flow"],
+        "market_type": data["instrumentInfo"]["cgrValCotTitle"],
+    }
+
+
+def get_stock_detail(code: str, timeout=3):
     headers = {
-        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 '
+                      'Safari/537.36',
     }
     url = f"http://cdn.tsetmc.com/api/Instrument/GetInstrumentInfo/{code}"
     r = requests.get(url, headers=headers, verify=False, timeout=timeout)
-    return r.json()
+    return extract_instrumentInfo(r.json())
+
 
 def create_or_update_stock_from_dict(stock):
     print(f"creating stock with code {stock['code']}")
     session.add(Stocks(**stock))
-    
+
     try:
         session.commit()
-    except:
+    except Exception as e:
         print(f"stock {stock['code']} exist", end="\r", flush=True)
+        print(e.__context__)
         session.rollback()
 
-async def update_stock_table(code: str) -> Stocks:
+
+async def update_stock_table(code: str) -> tuple[bool, str] | tuple[Exception, str]:
     try:
-        if exist := Stocks.query.filter_by(code=code).first():
+        stock = Stocks.query.filter_by(code=code).first()
+        if stock.code == code:
             print(f"stock with code {code} exist")
-            return
-        
+            return True, code
+
+        url = f"http://cdn.tsetmc.com/api/Instrument/GetInstrumentInfo/{code}"
         headers = {
-            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 '
+                          'Safari/537.36'
         }
-        url = f"http://cdn.tsetmc.com/api/Instrument/GetInstrumentInfo/{code}"
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as resp:
+        async with aiohttp.ClientSession() as ses:
+            async with ses.get(url, headers=headers) as resp:
                 data = await resp.json()
 
-        stock = {
-            "symbol":          data["instrumentInfo"]["lVal18AFC"],
-            "name":            data["instrumentInfo"]["lVal30"],
-            "name_en":         data["instrumentInfo"]["lVal18"],
-            "isin":            data["instrumentInfo"]["cIsin"],
-            "code":            code,
-            "capital":         data["instrumentInfo"]["zTitad"] if code != "32097828799138957" else 1_000_000_000,
-            "instrument_code": data["instrumentInfo"]["insCode"],
-            "instrument_id":   data["instrumentInfo"]["instrumentID"],
-            "group_name":      data["instrumentInfo"]["sector"]["lSecVal"],
-            "group_code":      data["instrumentInfo"]["sector"]["cSecVal"].replace(" ", ""),
-            "group_type":      data["instrumentInfo"]["cgrValCot"],
-            "market_name":     data["instrumentInfo"]["flowTitle"],
-            "market_code":     data["instrumentInfo"]["flow"],
-            "market_type":     data["instrumentInfo"]["cgrValCotTitle"],
-        }
-
+        stock = extract_instrumentInfo(data)
         create_or_update_stock_from_dict(stock)
 
         return True, code
 
     except Exception as e:
         return e, code
 
+
 def update_stocks_table(codes, msg=""):
     tasks = [update_stock_table(code) for code in codes]
     get_results_by_asyncio_loop(tasks)
     print(msg, end="\r")
 
-def get_stock_ids(timeout = 10):
+
+def get_stock_ids(timeout=10):
     url = "http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx?"
     r = requests.get(url, timeout=timeout)
     ids = set(re.findall(r"\d{15,20}", r.text))
     return list(ids)
 
-def get_stocks_groups(timeout = 10):
+
+def get_stocks_groups(timeout=10):
     url = "http://old.tsetmc.com/Loader.aspx?ParTree=111C1213"
     r = requests.get(url, timeout=timeout)
     return re.findall(r"\d{2}", r.text)
 
-def fill_stocks_table(timeout = 10):
+
+def fill_stocks_table(timeout=10, repeat=30):
     print("This may take several minutes")
     index = ["32097828799138957"]
     bonds = get_csv_from_github("treasury_bill")
     update_stocks_table(index + list(bonds.code))
-    for i in range(30):
-        print(f"Downloading group ids... seris: {i+1}")
+    for i in range(repeat):
+        print(f"Downloading group ids... series: {i + 1}")
         ids = get_stock_ids(timeout=timeout)
         update_stocks_table(ids + index)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/initializer.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/initializer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import os
 
-from codal_tsetmc.config.engine import CDL_TSE_FOLDER, HOME_PATH
-from codal_tsetmc.models.create import create
-from codal_tsetmc.download.codal.company   import fill_companies_table
-from codal_tsetmc.download.codal.category  import fill_categories_table
-from codal_tsetmc.download.tsetmc.stock    import fill_stocks_table
-from codal_tsetmc.download.tsetmc.price    import fill_stocks_prices_table
-from codal_tsetmc.download.tsetmc.capital  import fill_stocks_capitals_table
-from codal_tsetmc.download.other.commodity import fill_commodities_prices_table
-from codal_tsetmc.download.codal.letters   import fill_interim_financial_statements_letters
-
-
+from .config.engine import CDL_TSE_FOLDER, HOME_PATH
+from .models.create import create
+from .download.codal.company import fill_companies_table
+from .download.codal.category import fill_categories_table
+from .download.tsetmc.stock import fill_stocks_table
+from .download.tsetmc.price import fill_stocks_prices_table
+from .download.tsetmc.capital import fill_stocks_capitals_table
+from .download.other.commodity import fill_commodities_prices_table
+from .download.codal.letters import fill_interim_financial_statements_letters
 
 
 def init_db():
     print("creating database")
     path = os.path.join(HOME_PATH, CDL_TSE_FOLDER)
     try:
         os.mkdir(path)
         print("making package folder...")
         print("Includes: config.yml and companies-stocks.db  if you are using sqlite.")
         print("you can change config.yml to your needs.")
     except FileExistsError:
         print("folder already exists")
     create()
-    print(f"DataBase created in: {path}")
+    print(f"Database created in: {path}")
+
+
+def init_table():
     fill_companies_table()
     fill_categories_table()
 
 
 def fill_db():
     print("downloading company and stock details from CODAL and TSETMC")
     print("may take few minutes")
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/models/companies.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/models/companies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from sqlalchemy.orm import relationship
-import pandas as pd
-import jalali_pandas
 
 from codal_tsetmc.config.engine import (
     Column, Integer, String, Boolean, ForeignKey, Base
 )
 
 
 class Companies(Base):
@@ -78,14 +76,24 @@
     code = Column(Integer, unique=True)
     name = Column(String)
 
     def __repr__(self):
         return f"({self.code}, {self.name})"
 
 
+class FinancialYears(Base):
+    __tablename__ = "financial_years"
+
+    id = Column(Integer, primary_key=True)
+    date = Column(Integer, unique=True)
+
+    def __repr__(self):
+        return f"({self.date})"
+
+
 class Letters(Base):
     __tablename__ = "letters"
 
     id = Column(Integer, primary_key=True)
     publish_date_time = Column(Integer)
     sent_date_time = Column(Integer)
     tracing_no = Column(Integer, unique=True)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/models/create.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/models/create.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,39 +5,46 @@
     StockCapital,
     CommodityPrice
 )
 from codal_tsetmc.models.companies import (
     Companies,
     CompanyTypes,
     CompanyStatuses,
+    FinancialYears,
     ReportTypes,
     LetterTypes,
     Auditors,
     Letters,
     FinancialStatementHeader,
     FinancialStatementTableWithSingleItem
 )
 
-def create_table(Model):
+models = [
+    Stocks,
+    StockPrice,
+    StockCapital,
+    Companies,
+    CompanyTypes,
+    CompanyStatuses,
+    FinancialYears,
+    ReportTypes,
+    LetterTypes,
+    Auditors,
+    Letters,
+    FinancialStatementHeader,
+    FinancialStatementTableWithSingleItem,
+    CommodityPrice
+]
+
+
+def create_table(model):
     try:
-        Model.__table__.create(engine)
-    except:
+        model.__table__.create(engine)
+    except Exception as e:
+        print(e.__context__)
+    finally:
         pass
 
+
 def create():
-    models = [
-        Stocks,
-        StockPrice,
-        StockCapital,
-        Companies,
-        CompanyTypes,
-        CompanyStatuses,
-        ReportTypes,
-        LetterTypes,
-        Auditors, 
-        Letters,
-        FinancialStatementHeader, 
-        FinancialStatementTableWithSingleItem,
-        CommodityPrice
-    ]
     for model in models:
         create_table(model)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/models/stocks.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/models/stocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import numpy as np
 import pandas as pd
 import jalali_pandas
+
 from sqlalchemy.orm import relationship
 
 from codal_tsetmc.config.engine import (
     Column, Integer, String, BIGINT, Float, ForeignKey,
     Base, session
 )
 from codal_tsetmc.tools.database import read_table_by_conditions
 
+
 def add_event(df, event, ratio):
     df = df.merge(event[["date", ratio]], how="outer", on="date")
     df = df.sort_values("date").reset_index(drop=True)
     df[ratio] = df[ratio].fillna(method="ffill")
     df = df.dropna(subset=['close'])
     df["cumulative"] = df[ratio].fillna(1).cumprod()
 
-    df[ratio+"_ratio"] = df.cumulative/df.cumulative.iloc[-1]
+    df[ratio + "_ratio"] = df.cumulative / df.cumulative.iloc[-1]
     return df.drop('cumulative', axis=1)
 
 
 class Stocks(Base):
     __tablename__ = "stocks"
 
     id = Column(Integer, primary_key=True)
@@ -48,46 +50,45 @@
     _dollar_cached = False
     _dollar_counter = 0
     _index_cached = False
     _index_counter = 0
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-    
+
     @property
     def price(self) -> pd.DataFrame:
         """dataframe of stock price with date and OHLC"""
         self._price_counter += 1
         if self._price_cached:
             return self._price
-        
+
         df = read_table_by_conditions("stock_price", "code", self.code)
         if df.empty:
             self._price_cached = True
             self._price = df
             return self._price
-        
+
         df["jdate"] = df["date"].replace(regex={"000000$": ""})
         df["date"] = df["date"].jalali.parse_jalali("%Y%m%d%H%M%S").jalali.to_gregorian()
         df.set_index("date", inplace=True)
         self._price_cached = True
         self._price = df[[
             "jdate", "ticker", "symbol", "code", "price", "value", "volume"
         ]].dropna()
 
         return self._price
 
-    
     @property
     def market(self) -> pd.DataFrame:
         """dataframe of stock price with date and OHLC"""
         self._market_counter += 1
         if self._market_cached:
             return self._market
-        
+
         df = self.price
         if df.empty:
             self._market_cached = True
             self._market = df
             return self._market
 
         capital = read_table_by_conditions("stock_capital", "code", self.code).rename(columns={"new": "capital"})
@@ -96,87 +97,84 @@
 
         df = df.join(capital[["capital"]], how="outer").sort_index()
 
         if capital.empty:
             df["capital"].iat[0] = self.capital
         else:
             df["capital"].iat[0] = capital["old"].iloc[0]
-        
+
         df["capital"] = df["capital"].ffill()
-        df["market"]  = df["capital"] * df["price"]
+        df["market"] = df["capital"] * df["price"]
         self._market_cached = True
         self._market = df[["jdate", "symbol", "market", "value"]].dropna()
 
         return self._market
-    
 
     @property
     def dollar(self) -> pd.DataFrame:
         """dataframe of stock price with date and OHLC"""
         self._dollar_counter += 1
         if self._dollar_cached:
             return self._dollar
-        
+
         df = self.market
         if df.empty:
             self._dollar_cached = True
             self._dollar = df
             return self._dollar
 
-        dollar = read_table_by_conditions("commodity_price", "symbol", "price_dollar_rl").rename(columns={"price": "dollar"})
+        dollar = read_table_by_conditions("commodity_price", "symbol", "price_dollar_rl").rename(
+            columns={"price": "dollar"})
         dollar["date"] = dollar["date"].jalali.parse_jalali("%Y%m%d%H%M%S").jalali.to_gregorian()
         dollar.set_index("date", inplace=True)
         df = df.join(dollar[["dollar"]], how="outer").sort_index()
         df["dollar"] = df["dollar"].ffill()
         df["market"] = df["market"] / df["dollar"]
-        df["value"]  = df["value"]  / df["dollar"]
+        df["value"] = df["value"] / df["dollar"]
         self._dollar_cached = True
         self._dollar = df[["jdate", "symbol", "market", "value"]].dropna()
 
         return self._dollar
 
-
     @property
     def index(self) -> pd.DataFrame:
         """dataframe of stock price with date and OHLC"""
         self._index_counter += 1
         if self._index_cached:
             return self._index
-        
+
         df = self.market
         if df.empty:
             self._index_cached = True
             self._index = df
             return self._index
 
         index = read_table_by_conditions("stock_price", "code", "32097828799138957").rename(columns={"price": "index"})
         index["date"] = index["date"].jalali.parse_jalali("%Y%m%d%H%M%S").jalali.to_gregorian()
         index["index"] = index["index"] * 1_000_000_000
         index.set_index("date", inplace=True)
         df = df.join(index[["index"]], how="outer")
-        df["jdate"]  = df["jdate"].ffill()
+        df["jdate"] = df["jdate"].ffill()
         df["symbol"] = df["symbol"].ffill()
         df["market"] = df["market"].ffill()
         self._index_cached = True
         self._index = df[["jdate", "symbol", "market", "index"]].dropna()
 
         return self._index
-    
-    def beta(self, during = 3650):
-        df = self.index[["market", "index"]][-during:].pct_change().dropna()
-        return np.cov(df["market"], df["index"])[0,1] / np.var(df["index"])
 
+    def beta(self, during=3650):
+        df = self.index[["market", "index"]][-during:].pct_change().dropna()
+        return np.cov(df["market"], df["index"])[0, 1] / np.var(df["index"])
 
     def update_price(self):
         from codal_tsetmc.download.tsetmc.price import update_stocks_prices
         try:
             return update_stocks_prices([self.code])
         except:
             return False
-    
 
     def update_capital(self):
         from codal_tsetmc.download.tsetmc.capital import update_stocks_capitals
 
         try:
             return update_stocks_capitals([self.code])
         except:
@@ -192,21 +190,21 @@
     def get_group():
         return (
             session.query(Stocks.group_code, Stocks.group_name)
             .group_by(Stocks.group_code)
             .all()
         )
 
+
 class StockPrice(Base):
     __tablename__ = "stock_price"
 
     id = Column(Integer, primary_key=True)
     code = Column(String, ForeignKey("stocks.code"), index=True)
     symbol = Column(String)
-    ticker = Column(String)
     date = Column(String)
     volume = Column(BIGINT)
     value = Column(BIGINT)
     price = Column(Float)
     up_date = Column(String)
 
     def __repr__(self):
@@ -220,15 +218,15 @@
     code = Column(String, ForeignKey("stocks.code"), index=True)
     date = Column(String)
     old = Column(BIGINT)
     new = Column(BIGINT)
     up_date = Column(String)
 
     def __repr__(self):
-        return f"{self.stock.name}, {max(self.date)}, {max(self.new)}"
+        return f"name: {self.stock.name}, date: {max(self.date)}, capital: {max(self.new)}"
 
 
 class CommodityPrice(Base):
     __tablename__ = "commodity_price"
 
     id = Column(Integer, primary_key=True)
     symbol = Column(String)
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/tools/database.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     conditions: str = "",
     text: str = ""
 ):
     try:
         q = f"SELECT {columns} FROM {table} {conditions}"
         temp = pd.read_sql(q, engine)
         df = df[~df[columns].isin(temp[columns])]
-    except:
+    except Exception as e:
+        print(e)
+    finally:
         pass
 
     df.to_sql(table, engine, if_exists="append", index=False)
     print(text, end="\r", flush=True)
 
 
 def read_table_by_conditions(table, variable="", value="", columns="*", conditions=""):
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/tools/exception.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/exception.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import re
 
 
 class BadValueInput:
     def __init__(self, value):
         self.value = value
 
-    def boolian_type(self):
+    def boolean_type(self):
         if not isinstance(self.value, bool):
             raise TypeError("status must be True or False")
 
     def integer_type(self):
         if not isinstance(self.value, int):
             raise TypeError("status must be Integer")
 
     def string_type(self):
         if not isinstance(self.value, str):
             raise TypeError("status must be String")
 
     def int_str_type(self):
-        pattern = "^\d*$"
+        pattern = "^[0-9]*$"
         if not bool(re.match(pattern, self.value)):
             raise TypeError("status must be Integer String")
 
     def date_type(self):
-        pattern = "^\d{4}\/(0?[1-9]|1[012])\/(0?[1-9]|[12][0-9]|3[01])$"
+        pattern = "^[0-9]{4}/(0?[1-9]|1[012])/(0?[1-9]|[12][0-9]|3[01])$"
         if not bool(re.match(pattern, self.value)):
             raise TypeError("status must be yyyy/mm/dd")
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `codal_tsetmc-0.0.7/src/codal_tsetmc/tools/string.py` & `codal_tsetmc-0.0.8/src/codal_tsetmc/tools/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from jdatetime import datetime as jdt
 
 FA_TO_EN_DIGITS = {
     "۱": "1", "۲": "2", "۳": "3", "۴": "4", "۵": "5",
     "۶": "6", "۷": "7", "۸": "8", "۹": "9", "۰": "0"
 }
 
-
 AR_TO_FA_LETTER = {
     "ي": "ی",
     "ك": "ک"
 }
 
 EMPTY_TO_NONE = {
     "^$": None,
@@ -54,15 +53,15 @@
     "Interpretative Report Summary - Page 3": "22",
     "23": "23",
     "خلاصه اطلاعات گزارش تفسیری - صفحه 4": "23",
     "Interpretative Report Summary - Page 4": "23",
     "24": "24",
     "خلاصه اطلاعات گزارش تفسیری - صفحه 5": "24",
     "Interpretative Report Summary - Page 5": "24",
-    "26": "26",
+    "25": "25",
     "خلاصه اطلاعات گزارش تفسیری - صفحه 6": "25",
     "Interpretative Report Summary - Page 6": "25",
     "26": "26",
     "خلاصه اطلاعات گزارش تفسیری - صفحه 7": "26",
     "Interpretative Report Summary - Page 7": "26",
     "1058": "1058",
     "صورت سود و زیان جامع": "1058",
@@ -104,48 +103,54 @@
 }
 
 
 def replace_all(text, dic):
     text = str(text)
     for k, v in dic.items():
         text = re.sub(k, v, text)
-    
+
     return text
 
+
 def datetime_to_num(dt):
     if dt == "": return None
     try:
         dt = replace_all(dt, {"\D": ""})
         return int(dt) * 10 ** (14 - len(dt))
-    except:
+    finally:
         return dt
 
-def num_to_datetime(num, datetime = True, d = "/", t = ":", sep = " "):
+
+def num_to_datetime(num, datetime=True, d="/", t=":", sep=" "):
     num = str(num)
     date = f"{num[0:4]}{d}{num[4:6]}{d}{num[6:8]}"
     time = f"{num[8:10]}{t}{num[10:12]}{t}{num[12:14]}"
     if datetime:
         return f"{date}{sep}{time}"
     else:
         return date
 
+
 def yyyymmdd_to_shamsi(date):
     date = str(date)
     return jd.fromgregorian(
         day=int(date[-2:]), month=int(date[4:6]), year=int(date[:4])
     ).strftime("%Y/%m/%d")
 
+
 def shamsi_to_yyyymmdd(date: str):
     jdt.strptime(date, "%Y%m%d%H%M%S").togregorian().strftime("%Y%m%d")
 
+
 def removekey(d, key):
     r = dict(d)
     del r[key]
     return r
 
+
 def value_to_float(x):
     x = x.replace(",", "")
     if type(x) == float or type(x) == int:
         return x
     if 'K' in x:
         if len(x) > 1:
             return float(x.replace(' K', '')) * 1000
@@ -154,14 +159,15 @@
         if len(x) > 1:
             return float(x.replace(' M', '')) * 1000000
         return 1000000.0
     if 'B' in x:
         return float(x.replace(' B', '')) * 1000000000
     return 0.0
 
+
 def to_snake_case(name):
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     name = re.sub('__([A-Z])', r'_\1', name)
     name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', name)
     return name.lower()
 
 
@@ -209,8 +215,7 @@
     "ن-70": "تصمیم هیئت مدیره به انجام افزایش سرمایه تفویض شده در مجمع فوق العاده",
     "ن-71": "زمان تشکیل جلسه هیئت‌مدیره در خصوص افزایش سرمایه",
     "ن-72": "لغو اطلاعیه زمان تشکیل جلسه هیئت مدیره در خصوص افزایش سرمایه",
     "ن-73": "تصمیمات هیئت‌مدیره در خصوص افزایش سرمایه",
     "ن-80": "تغییر نشانی",
     "ن-81": "درخواست تکمیل مشخصات سهامداران",
 }
-
```

