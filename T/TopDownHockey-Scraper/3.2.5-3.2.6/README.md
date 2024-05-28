# Comparing `tmp/topdownhockey_scraper-3.2.5.tar.gz` & `tmp/topdownhockey_scraper-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topdownhockey_scraper-3.2.5.tar", last modified: Tue May 28 19:07:05 2024, max compression
+gzip compressed data, was "topdownhockey_scraper-3.2.6.tar", last modified: Tue May 28 19:13:58 2024, max compression
```

## Comparing `topdownhockey_scraper-3.2.5.tar` & `topdownhockey_scraper-3.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:07:05.777731 topdownhockey_scraper-3.2.5/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.5/LICENSE
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 19:07:05.777675 topdownhockey_scraper-3.2.5/PKG-INFO
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.5/README.md
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.5/pyproject.toml
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-05-28 19:07:05.777995 topdownhockey_scraper-3.2.5/setup.cfg
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-05-28 19:05:56.000000 topdownhockey_scraper-3.2.5/setup.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:07:05.775766 topdownhockey_scraper-3.2.5/src/
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:07:05.776531 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
--rw-rw-r--   0 patrickbacon   (501) staff       (20)   152676 2024-05-28 19:05:02.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:07:05.777452 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 19:07:05.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-05-28 19:07:05.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-05-28 19:07:05.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-05-28 19:07:05.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/requires.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-05-28 19:07:05.000000 topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/top_level.txt
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:13:58.987801 topdownhockey_scraper-3.2.6/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.6/LICENSE
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 19:13:58.987740 topdownhockey_scraper-3.2.6/PKG-INFO
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.6/README.md
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.6/pyproject.toml
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-05-28 19:13:58.988058 topdownhockey_scraper-3.2.6/setup.cfg
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-05-28 19:13:36.000000 topdownhockey_scraper-3.2.6/setup.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:13:58.985936 topdownhockey_scraper-3.2.6/src/
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:13:58.986714 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)   152677 2024-05-28 19:13:15.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 19:13:58.987544 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 19:13:58.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-05-28 19:13:58.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-05-28 19:13:58.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-05-28 19:13:58.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/requires.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-05-28 19:13:58.000000 topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/top_level.txt
```

### Comparing `topdownhockey_scraper-3.2.5/LICENSE` & `topdownhockey_scraper-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.5/PKG-INFO` & `topdownhockey_scraper-3.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.5
+Version: 3.2.6
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.5 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.6 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `topdownhockey_scraper-3.2.5/README.md` & `topdownhockey_scraper-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.5/setup.cfg` & `topdownhockey_scraper-3.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TopDownHockey_Scraper
-version = 3.2.5
+version = 3.2.6
 author = Patrick Bacon
 author_email = patrick.s.bacon@gmail.com
 description = A package built for scraping hockey data from EliteProspects, the NHL's HTML/API reports, and ESPN's XML reports.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TopDownHockey/TopDownHockeyScraper
 project_urls =
```

### Comparing `topdownhockey_scraper-3.2.5/setup.py` & `topdownhockey_scraper-3.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="TopDownHockey_Scraper", # Replace with your own username
-    version="3.2.5",
+    version="3.2.6",
     author="Patrick Bacon",
     author_email="patrick.s.bacon@gmail.com",
     description="The TopDownHockey Scraper",
     long_description=long_description,
     license = 'MIT',
     long_description_content_type="text/markdown",
     url="https://github.com/TopDownHockey/TopDownHockey_Scraper",
```

### Comparing `topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py` & `topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py` & `topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1895,15 +1895,15 @@
     at = []
     ht = []
     gids = []
     fax = pd.DataFrame()
     #print(str(i))
     for i in range (0, ((len(soup_found)))):
         away = soup_found[i]['href'].rsplit('/')[-1].split('-')[0].upper()
-        home = soup_found[i]['href'].rsplit('/')[-1].split('-')[1].upper()
+        home = soup_found[i]['href'].rsplit('/')[-1].split('-')[-1].upper()
         espnid = soup_found[i]['href'].rsplit('/')[-2]
         at.append(away)
         ht.append(home)
         gids.append(espnid)
     
     fax = fax.assign(
     away_team = at,
```

### Comparing `topdownhockey_scraper-3.2.5/src/TopDownHockey_Scraper.egg-info/PKG-INFO` & `topdownhockey_scraper-3.2.6/src/TopDownHockey_Scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.5
+Version: 3.2.6
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.5 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.6 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

