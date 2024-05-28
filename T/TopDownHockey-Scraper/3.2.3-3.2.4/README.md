# Comparing `tmp/topdownhockey_scraper-3.2.3.tar.gz` & `tmp/topdownhockey_scraper-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topdownhockey_scraper-3.2.3.tar", last modified: Sat May 18 04:40:51 2024, max compression
+gzip compressed data, was "topdownhockey_scraper-3.2.4.tar", last modified: Tue May 28 18:35:26 2024, max compression
```

## Comparing `topdownhockey_scraper-3.2.3.tar` & `topdownhockey_scraper-3.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.732455 topdownhockey_scraper-3.2.3/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.3/LICENSE
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-18 04:40:51.732409 topdownhockey_scraper-3.2.3/PKG-INFO
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.3/README.md
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.3/pyproject.toml
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-05-18 04:40:51.732734 topdownhockey_scraper-3.2.3/setup.cfg
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-05-18 04:40:29.000000 topdownhockey_scraper-3.2.3/setup.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.730594 topdownhockey_scraper-3.2.3/src/
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.731376 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
--rw-rw-r--   0 patrickbacon   (501) staff       (20)   148269 2024-05-18 04:37:31.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.732187 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/requires.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/top_level.txt
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 18:35:26.330051 topdownhockey_scraper-3.2.4/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.4/LICENSE
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 18:35:26.330001 topdownhockey_scraper-3.2.4/PKG-INFO
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.4/README.md
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.4/pyproject.toml
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-05-28 18:35:26.330303 topdownhockey_scraper-3.2.4/setup.cfg
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-05-28 18:34:52.000000 topdownhockey_scraper-3.2.4/setup.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 18:35:26.327530 topdownhockey_scraper-3.2.4/src/
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 18:35:26.328931 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)   152732 2024-05-28 18:34:21.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-28 18:35:26.329753 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-28 18:35:26.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-05-28 18:35:26.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-05-28 18:35:26.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-05-28 18:35:26.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/requires.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-05-28 18:35:26.000000 topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/top_level.txt
```

### Comparing `topdownhockey_scraper-3.2.3/LICENSE` & `topdownhockey_scraper-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.3/PKG-INFO` & `topdownhockey_scraper-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.3
+Version: 3.2.4
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
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.3 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.4 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `topdownhockey_scraper-3.2.3/README.md` & `topdownhockey_scraper-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.3/setup.cfg` & `topdownhockey_scraper-3.2.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TopDownHockey_Scraper
-version = 3.2.3
+version = 3.2.4
 author = Patrick Bacon
 author_email = patrick.s.bacon@gmail.com
 description = A package built for scraping hockey data from EliteProspects, the NHL's HTML/API reports, and ESPN's XML reports.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TopDownHockey/TopDownHockeyScraper
 project_urls =
```

### Comparing `topdownhockey_scraper-3.2.3/setup.py` & `topdownhockey_scraper-3.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="TopDownHockey_Scraper", # Replace with your own username
-    version="3.2.3",
+    version="3.2.4",
     author="Patrick Bacon",
     author_email="patrick.s.bacon@gmail.com",
     description="The TopDownHockey Scraper",
     long_description=long_description,
     license = 'MIT',
     long_description_content_type="text/markdown",
     url="https://github.com/TopDownHockey/TopDownHockey_Scraper",
```

### Comparing `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py` & `topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py` & `topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1937,17 +1937,87 @@
                     np.where(gamedays.away_team=='S.J', 'SJS',
                     np.where(gamedays.away_team=='SJ', 'SJS',
                     np.where(gamedays.away_team=='N.J', 'NJD',
                     np.where(gamedays.away_team=='NJ', 'NJD',
                     gamedays.away_team)))))))),
         espn_id = gamedays.espn_id.astype(int))
     
-    # Might need to fix later; don't have right home/away teams right now 
+    gamedays = gamedays.assign(
+        away_team = np.where(gamedays.away_team=='DUCKS', 'ANA',
+                    np.where(gamedays.away_team=='COYOTES', 'ARI',
+                    np.where(gamedays.away_team=='BRUINS', 'BOS',
+                    np.where(gamedays.away_team=='SABRES', 'BUF',
+                    np.where(gamedays.away_team=='FLAMES', 'CGY',
+                    np.where(gamedays.away_team=='HURRICANES', 'CAR',
+                    np.where(gamedays.away_team=='BLACKHAWKS', 'CHI',
+                    np.where(gamedays.away_team=='AVALANCHE', 'COL',
+                    np.where(gamedays.away_team=='BLUE JACKETS', 'CBJ',
+                    np.where(gamedays.away_team=='STARS', 'DAL',
+                    np.where(gamedays.away_team=='RED WINGS', 'DET',
+                    np.where(gamedays.away_team=='OILERS', 'EDM',
+                    np.where(gamedays.away_team=='PANTHERS', 'FLA',
+                    np.where(gamedays.away_team=='KINGS', 'LAK',
+                    np.where(gamedays.away_team=='WILD', 'MIN',
+                    np.where(gamedays.away_team=='CANADIENS', 'MTL',
+                    np.where(gamedays.away_team=='PREDATORS', 'NSH',
+                    np.where(gamedays.away_team=='DEVILS', 'NJD',
+                    np.where(gamedays.away_team=='ISLANDERS', 'NYI',
+                    np.where(gamedays.away_team=='RANGERS', 'NYR',
+                    np.where(gamedays.away_team=='SENATORS', 'OTT',
+                    np.where(gamedays.away_team=='FLYERS', 'PHI',
+                    np.where(gamedays.away_team=='PENGUINS', 'PIT',
+                    np.where(gamedays.away_team=='SHARKS', 'SJS',
+                    np.where(gamedays.away_team=='KRAKEN', 'SEA',
+                    np.where(gamedays.away_team=='BLUES', 'STL',
+                    np.where(gamedays.away_team=='LIGHTNING', 'TBL',
+                    np.where(gamedays.away_team=='MAPLE LEAFS', 'TOR',
+                    np.where(gamedays.away_team=='CANUCKS', 'VAN',
+                    np.where(gamedays.away_team=='GOLDEN KNIGHTS', 'VGK',
+                    np.where(gamedays.away_team=='CAPITALS', 'WSH',
+                    np.where(gamedays.away_team=='JETS', 'WPG', 'mistake'
+                            ))))))))))))))))))))))))))))))))
+    )
+
+    gamedays = gamedays.assign(
+        home_team = np.where(gamedays.home_team=='DUCKS', 'ANA',
+                    np.where(gamedays.home_team=='COYOTES', 'ARI',
+                    np.where(gamedays.home_team=='BRUINS', 'BOS',
+                    np.where(gamedays.home_team=='SABRES', 'BUF',
+                    np.where(gamedays.home_team=='FLAMES', 'CGY',
+                    np.where(gamedays.home_team=='HURRICANES', 'CAR',
+                    np.where(gamedays.home_team=='BLACKHAWKS', 'CHI',
+                    np.where(gamedays.home_team=='AVALANCHE', 'COL',
+                    np.where(gamedays.home_team=='BLUE JACKETS', 'CBJ',
+                    np.where(gamedays.home_team=='STARS', 'DAL',
+                    np.where(gamedays.home_team=='RED WINGS', 'DET',
+                    np.where(gamedays.home_team=='OILERS', 'EDM',
+                    np.where(gamedays.home_team=='PANTHERS', 'FLA',
+                    np.where(gamedays.home_team=='KINGS', 'LAK',
+                    np.where(gamedays.home_team=='WILD', 'MIN',
+                    np.where(gamedays.home_team=='CANADIENS', 'MTL',
+                    np.where(gamedays.home_team=='PREDATORS', 'NSH',
+                    np.where(gamedays.home_team=='DEVILS', 'NJD',
+                    np.where(gamedays.home_team=='ISLANDERS', 'NYI',
+                    np.where(gamedays.home_team=='RANGERS', 'NYR',
+                    np.where(gamedays.home_team=='SENATORS', 'OTT',
+                    np.where(gamedays.home_team=='FLYERS', 'PHI',
+                    np.where(gamedays.home_team=='PENGUINS', 'PIT',
+                    np.where(gamedays.home_team=='SHARKS', 'SJS',
+                    np.where(gamedays.home_team=='KRAKEN', 'SEA',
+                    np.where(gamedays.home_team=='BLUES', 'STL',
+                    np.where(gamedays.home_team=='LIGHTNING', 'TBL',
+                    np.where(gamedays.home_team=='MAPLE LEAFS', 'TOR',
+                    np.where(gamedays.home_team=='CANUCKS', 'VAN',
+                    np.where(gamedays.home_team=='GOLDEN KNIGHTS', 'VGK',
+                    np.where(gamedays.home_team=='CAPITALS', 'WSH',
+                    np.where(gamedays.home_team=='JETS', 'WPG', 'mistake'
+                            ))))))))))))))))))))))))))))))))
+    )
     
-    #gamedays = gamedays[(gamedays.game_date==this_date) & (gamedays.home_team==home_team) & (gamedays.away_team==away_team)] 
+    gamedays = gamedays[(gamedays.game_date==this_date) & (gamedays.home_team==home_team) & (gamedays.away_team==away_team)] 
         
     return(gamedays)
 
 def merge_and_prepare(events, shifts):
     
     season = str(int(str(events.game_id.iloc[0])[:4])) + str(int(str(events.game_id.iloc[0])[:4]) + 1)
     small_id = str(events.game_id.iloc[0])[5:]
```

### Comparing `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/PKG-INFO` & `topdownhockey_scraper-3.2.4/src/TopDownHockey_Scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.3
+Version: 3.2.4
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
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.3 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.4 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

