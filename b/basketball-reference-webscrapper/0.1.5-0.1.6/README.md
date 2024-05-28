# Comparing `tmp/basketball_reference_webscrapper-0.1.5.tar.gz` & `tmp/basketball_reference_webscrapper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basketball_reference_webscrapper-0.1.5.tar", max compression
+gzip compressed data, was "basketball_reference_webscrapper-0.1.6.tar", max compression
```

## Comparing `basketball_reference_webscrapper-0.1.5.tar` & `basketball_reference_webscrapper-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      120 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/__init__.py
--rw-r--r--   0        0        0     1223 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/team_city_refdata.csv
--rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/data_models/__init_.py
--rw-r--r--   0        0        0      324 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/data_models/feature_model.py
--rw-r--r--   0        0        0        0 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/__init__.py
--rw-r--r--   0        0        0     1083 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/logs.py
--rw-r--r--   0        0        0     7541 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/webscrapping_basketball_reference.py
--rw-r--r--   0        0        0      958 2024-05-27 12:50:32.637539 basketball_reference_webscrapper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/__init__.py
+-rw-r--r--   0        0        0     1223 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/team_city_refdata.csv
+-rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/data_models/__init_.py
+-rw-r--r--   0        0        0      213 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/data_models/feature_model.py
+-rw-r--r--   0        0        0     1769 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/params.yaml
+-rw-r--r--   0        0        0        0 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/__init__.py
+-rw-r--r--   0        0        0     1075 2024-05-28 11:57:13.472094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/logs.py
+-rw-r--r--   0        0        0     7683 2024-05-28 11:57:13.476094 basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/webscrapping_basketball_reference.py
+-rw-r--r--   0        0        0      958 2024-05-28 11:57:13.476094 basketball_reference_webscrapper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.1.6/PKG-INFO
```

### Comparing `basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/constants/team_city_refdata.csv` & `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/constants/team_city_refdata.csv`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/utils/logs.py` & `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/utils/logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides functions to create loggers."""
 
 import logging
-from typing import Text, Union
+from typing import Union
 import sys
 
 
 def get_console_handler() -> logging.StreamHandler:
     """Get console handler.
     Returns:
         logging.StreamHandler which logs into stdout
@@ -17,15 +17,15 @@
     )
     console_handler.setFormatter(formatter)
 
     return console_handler
 
 
 def get_logger(
-    name: Text = __name__, log_level: Union[Text, int] = logging.DEBUG
+    name: str = __name__, log_level: Union[str, int] = logging.DEBUG
 ) -> logging.Logger:
     """Get logger.
     Args:
         name {Text}: logger name
         log_level {Text or int}: logging level; can be string name or integer value
     Returns:
         logging.Logger instance
```

### Comparing `basketball_reference_webscrapper-0.1.5/basketball_reference_webscrapper/webscrapping_basketball_reference.py` & `basketball_reference_webscrapper-0.1.6/basketball_reference_webscrapper/webscrapping_basketball_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,177 +1,197 @@
+"""
+Class that take as inputs url and season and return all games teams stats
+"""
+
 from dataclasses import dataclass
 from urllib.request import urlopen
+import time
 from bs4 import BeautifulSoup
 import pandas as pd
 import requests
-import time
+
 import importlib_resources
+import yaml
 
-from basketball_reference_webscrapper.data_models.feature_model import FeatureIn, FeatureOut
+from basketball_reference_webscrapper.data_models.feature_model import (
+    FeatureIn
+)
 from basketball_reference_webscrapper.utils.logs import get_logger
 
 logger = get_logger("WEB_SCRAPPING_EXECUTION", log_level="INFO")
 
+
 @dataclass
 class WebScrapBasketballReference:
     """
     Class that take as inputs url and season and return all games teams stats
     """
-    
+
     def __init__(self, feature_object: FeatureIn) -> None:
+        """
+        Init function
+        """
         self.feature_object = feature_object
-    
-    def _get_team_list_values_validation(self, team_abbrev_list: list):
-        if  (isinstance(self.feature_object.team, list)) and (all(isinstance(s, str) for s in self.feature_object.team)):
-            if set(self.feature_object.team).issubset(team_abbrev_list)==False:
-                raise ValueError(
-                    "team list arg provided is not accepted.\
-                    Value needs to be 'all' or a NBA team abbreviation such as BOS for Boston Celtics.\
-                    More details on all values possible in the GitHub Repo docs"
-                )
-        elif isinstance(self.feature_object.team, str):
-            if (self.feature_object.team != 'all') and (self.feature_object.team not in team_abbrev_list):
-                raise ValueError(
-                    "team arg provided is not accepted.\
-                    Value needs to be 'all' or a NBA team abbreviation such as BOS for Boston Celtics.\
-                    More details on all values possible in the GitHub Repo docs"
-                )
-        else:
-            raise ValueError(
-                    "team args should be a string or a list of string.\
-                    Value needs to be NBA team abbreviation such as BOS for Boston Celtics.\
-                    More details on all values possible in the GitHub Repo docs"
-                )
 
     def webscrappe_nba_games_data(self):
         """
         Webscrappe NBA games data
         """
 
-        #------------------------------------------------------
-        # Get team reference data 
+        # ------------------------------------------------------
+        # User Input check and validation
+        self._get_data_type_validation()
+        self._get_season_validation()
+
+        # ------------------------------------------------------
+        # Import params file
+        with open("basketball_reference_webscrapper/params.yaml", encoding="utf-8") as conf_file:
+            config = yaml.safe_load(conf_file)
+
+        # ------------------------------------------------------
+        # Get team reference data
         ref = (
             importlib_resources.files("basketball_reference_webscrapper")
             / "constants/team_city_refdata.csv"
         )
         with importlib_resources.as_file(ref) as path:
-            team_city_refdata = pd.read_csv(path, sep = ';')
+            team_city_refdata = pd.read_csv(path, sep=";")
 
-        #------------------------------------------------------
-        # User Input check and validation
-        self._get_data_type_validation()
-        self._get_season_validation()
-        self._get_team_list_values_validation(list(team_city_refdata['team_abrev']))
+        # ------------------------------------------------------
+        # Part2 - User Input check and validation
+        self._get_team_list_values_validation(list(team_city_refdata["team_abrev"]))
 
-        #------------------------------------------------------
+        # ------------------------------------------------------
         # Team filtering
         if isinstance(self.feature_object.team, list):
-            team_city_refdata = team_city_refdata[team_city_refdata['team_abrev'].isin(self.feature_object.team)]
+            team_city_refdata = team_city_refdata[
+                team_city_refdata["team_abrev"].isin(self.feature_object.team)
+            ]
         elif isinstance(self.feature_object.team, str):
-            if self.feature_object.team != 'all':
-                team_city_refdata = team_city_refdata[team_city_refdata['team_abrev'] == self.feature_object.team]
-        
-        #------------------------------------------------------
+            if self.feature_object.team != "all":
+                team_city_refdata = team_city_refdata[
+                    team_city_refdata["team_abrev"] == self.feature_object.team
+                ]
+
+        # ------------------------------------------------------
         # Initialization of the dataframe to fill-in
         games = pd.DataFrame()
 
-        #------------------------------------------------------
+        # ------------------------------------------------------
         # For Loop Throught all the team abrev for the given season
         for index, row in team_city_refdata.iterrows():
 
             # URL to scrape
-            team = row['team_abrev']
+            team = row["team_abrev"]
 
-            logger.info(
-                f"Execution for {team}"
-            )
-            
-            url = "https://www.basketball-reference.com/teams/" +\
-                team + "/" +\
-                str(self.feature_object.season) +\
-                "/"+\
-                self.feature_object.data_type
+            logger.info("Execution for: %s", team)
 
-            if '200' in str(requests.get(url)):
+            if self.feature_object.data_type == "gamelog":
+                url = (
+                    config[self.feature_object.data_type]["url"]
+                    + team
+                    + "/"
+                    + str(self.feature_object.season)
+                    + "/"
+                    + self.feature_object.data_type
+                )
+            else:
+                url = (
+                    config[self.feature_object.data_type]["url"]
+                    + team
+                    + "/"
+                    + str(self.feature_object.season)
+                    + "_games.html"
+                )
+
+            # url = f'https://www.basketball-reference.com/players/{player_id}/gamelog/{id_season}'
+            # url = f"https://www.basketball-reference.com/teams/{team}/{SEASON}.html"
+            # url = f"https://www.basketball-reference.com/teams/BRK/2001.html"
 
+            if "200" in str(requests.get(url, timeout=60)):
                 # collect HTML data and create beautiful soup object:
-                html = urlopen(url)
-                        
-                # create beautiful soup object from HTML
-                soup = BeautifulSoup(html, "html.parser")
-
-                rows = soup.findAll('tr')[2:]
-
-                rows_data = [[td.getText() for td in rows[i].findAll('td')]
-                                    for i in range(len(rows))]
-
-                if len(rows_data) != 0:
-                    # create the dataframe
-                    games_tmp = pd.DataFrame(rows_data)
-                    cols = ["game_nb", "game_date", "extdom", "opp", "results",
-                            "pts_tm","pts_opp",
-                            "fg_tm", "fga_tm","fg_prct_tm",
-                            "3p_tm","3pa_tm", "3p_prct_tm","ft_tm","fta_tm","ft_prct_tm",
-                            "orb_tm","trb_tm", "ast_tm","stl_tm","blk_tm" ,"tov_tm","pf_tm",
-                            "nc",
-                            "fg_opp","fga_opp","fg_prct_opp",
-                            "3p_opp", "3pa_opp", "3p_prct_opp", "ft_opp", "fta_opp","ft_prct_opp",
-                            "orb_opp", "trb_opp","ast_opp", "stl_opp", "blk_opp","tov_opp", "pf_opp"]
-
-                    games_tmp.columns =  cols
-                    games_tmp = games_tmp.dropna()
-                    games_tmp['id_season'] = self.feature_object.season
-                    games_tmp['tm'] = team
-                    games = pd.concat([games, games_tmp], axis=0)
-            
+                # html = urlopen(url)
+
+                with urlopen(url) as html:
+
+                    # create beautiful soup object from HTML
+                    soup = BeautifulSoup(html, "html.parser")
+
+                    rows = soup.findAll("tr")[
+                        config[self.feature_object.data_type]["beautifulsoup_tr_index"] :
+                    ]
+
+                    rows_data = [
+                        [td.getText() for td in rows[i].findAll("td")]
+                        for i in range(len(rows))
+                    ]
+
+                    if len(rows_data) != 0:
+
+                        games_tmp = pd.DataFrame(rows_data)
+                        games_tmp.columns = config[self.feature_object.data_type]["list_columns"]
+                        games_tmp = games_tmp.dropna()
+                        games_tmp.loc[:, "id_season"] = self.feature_object.season
+                        games_tmp.loc[:, "tm"] = team
+                        games = pd.concat([games, games_tmp], axis=0)
+
             time.sleep(5)
 
-        games = games[[
-            'id_season', 'game_nb', 'game_date', 'extdom', 'tm','opp', 'results', 'pts_tm', 'pts_opp',
-            'fg_tm', 'fga_tm', 'fg_prct_tm', '3p_tm', '3pa_tm', '3p_prct_tm',
-            'ft_tm', 'fta_tm', 'ft_prct_tm', 'orb_tm', 'trb_tm', 'ast_tm', 'stl_tm',
-            'blk_tm', 'tov_tm', 'pf_tm', 'fg_opp', 'fga_opp', 'fg_prct_opp',
-            '3p_opp', '3pa_opp', '3p_prct_opp', 'ft_opp', 'fta_opp', 'ft_prct_opp',
-            'orb_opp', 'trb_opp', 'ast_opp', 'stl_opp', 'blk_opp', 'tov_opp',
-            'pf_opp']]
+        games = games[config[self.feature_object.data_type]["list_columns_to_select"]]
 
         return games
-    
 
     def _get_data_type_validation(self):
         if self.feature_object.data_type is not None:
-            print(self.feature_object.data_type)
-            if str(self.feature_object.data_type) != 'gamelog':
+            if str(self.feature_object.data_type) not in ["gamelog", "schedule"]:
                 raise ValueError(
-                    "data_type value provided is not supported by the package. Accepted values are: 'gamelog'\
+                    "data_type value provided is not supported by the package.\
+                    Accepted values are: 'gamelog', 'schedule'.\
                     Read documentation for more details"
                 )
         else:
             raise ValueError(
-                    "data_type is a required argument. it accepts the following values: 'gamelog'.\
+                "data_type is a required argument.\
+                    Accepted values are: 'gamelog', 'schedule'.\
                     Read documentation for more details"
-                )
-    
+            )
+
     def _get_season_validation(self):
         if isinstance(self.feature_object.season, int):
-            if (
-                self.feature_object.season < 1999
-            ):
+            if self.feature_object.season < 1999:
                 raise ValueError(
                     "season value provided is a year not supported by the package. \
                     it should be between 2000 and current NBA season."
                 )
         else:
             raise ValueError(
-                    "season is a required argument and should be an int value between 2000 and current NBA season."
-                )
-    
-
-    
-if __name__ == "__main__":
-    webscrapping_class = WebScrapBasketballReference(
-        url = "test",
-        season = 2022
-    )
-
-    nba_games = webscrapping_class.webscrappe_nba_games_data()
+                "season is a required argument and should be an int value between 2000\
+                    and current NBA season."
+            )
 
+    def _get_team_list_values_validation(self, team_abbrev_list: list):
+        if (isinstance(self.feature_object.team, list)) and (
+            all(isinstance(s, str) for s in self.feature_object.team)
+        ):
+            if set(self.feature_object.team).issubset(team_abbrev_list) is False:
+                raise ValueError(
+                    "team list arg provided is not accepted.\
+                    Value needs to be 'all' or a NBA team abbreviation\
+                    such as BOS for Boston Celtics.\
+                    More details on all values possible in the GitHub Repo docs"
+                )
+        elif isinstance(self.feature_object.team, str):
+            if (self.feature_object.team != "all") and (
+                self.feature_object.team not in team_abbrev_list
+            ):
+                raise ValueError(
+                    "team arg provided is not accepted.\
+                    Value needs to be 'all' or a NBA team abbreviation\
+                    such as BOS for Boston Celtics.\
+                    More details on all values possible in the GitHub Repo docs"
+                )
+        else:
+            raise ValueError(
+                "team args should be a string or a list of string.\
+                    Value needs to be NBA team abbreviation such as BOS for Boston Celtics.\
+                    More details on all values possible in the GitHub Repo docs"
+            )
```

### Comparing `basketball_reference_webscrapper-0.1.5/pyproject.toml` & `basketball_reference_webscrapper-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basketball-reference-webscrapper"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python package for Basketball Reference that gathers data by scraping the website"
 authors = ["Yannick Flores <yannick.flores1992@gmail.com>"]
 readme = "README.md"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -19,15 +19,15 @@
 [tool.poetry.dev-dependencies]
 coverage = {extras = ["toml"], version = "6.5.*"}
 black = {version = "22.10.*", allow-prereleases = true}
 pytest = "7.2.*"
 pytest-html = "3.1.*"
 pytest-cov = "2.12.*"
 py = "1.11.*"
-pylint = "2.15.*"
+pylint = "2.17.*"
 python-decouple = "3.6"
 mkdocs = "1.4.*"
 importlib-resources="6.0.1"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
```

### Comparing `basketball_reference_webscrapper-0.1.5/PKG-INFO` & `basketball_reference_webscrapper-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basketball-reference-webscrapper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for Basketball Reference that gathers data by scraping the website
 Author: Yannick Flores
 Author-email: yannick.flores1992@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

