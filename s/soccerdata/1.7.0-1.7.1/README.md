# Comparing `tmp/soccerdata-1.7.0.tar.gz` & `tmp/soccerdata-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.7.0.tar", max compression
+gzip compressed data, was "soccerdata-1.7.1.tar", max compression
```

## Comparing `soccerdata-1.7.0.tar` & `soccerdata-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1384 2024-05-09 20:04:25.002545 soccerdata-1.7.0/LICENSE.rst
--rw-r--r--   0        0        0     4017 2024-05-09 20:04:25.002545 soccerdata-1.7.0/README.rst
--rw-r--r--   0        0        0     2361 2024-05-09 20:04:36.218657 soccerdata-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      598 2024-05-09 20:04:36.218657 soccerdata-1.7.0/soccerdata/__init__.py
--rw-r--r--   0        0        0    22163 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/_common.py
--rw-r--r--   0        0        0     5910 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/_config.py
--rw-r--r--   0        0        0     6349 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/clubelo.py
--rw-r--r--   0        0        0    13855 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/espn.py
--rw-r--r--   0        0        0    47579 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fbref.py
--rw-r--r--   0        0        0     8537 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0    17171 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fotmob.py
--rw-r--r--   0        0        0     4658 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/match_history.py
--rw-r--r--   0        0        0    10406 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/sofascore.py
--rw-r--r--   0        0        0    17504 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/sofifa.py
--rw-r--r--   0        0        0    25962 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/understat.py
--rw-r--r--   0        0        0    33035 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/whoscored.py
--rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 soccerdata-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1384 2024-05-27 22:04:44.916546 soccerdata-1.7.1/LICENSE.rst
+-rw-r--r--   0        0        0     4017 2024-05-27 22:04:44.916546 soccerdata-1.7.1/README.rst
+-rw-r--r--   0        0        0     2361 2024-05-27 22:05:00.220620 soccerdata-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      598 2024-05-27 22:05:00.220620 soccerdata-1.7.1/soccerdata/__init__.py
+-rw-r--r--   0        0        0    22380 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/_common.py
+-rw-r--r--   0        0        0     5910 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/_config.py
+-rw-r--r--   0        0        0     6349 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    13855 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/espn.py
+-rw-r--r--   0        0        0    48370 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8537 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0    17171 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/fotmob.py
+-rw-r--r--   0        0        0     4658 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/match_history.py
+-rw-r--r--   0        0        0    10406 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/sofascore.py
+-rw-r--r--   0        0        0    17504 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    25962 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/understat.py
+-rw-r--r--   0        0        0    33575 2024-05-27 22:04:44.932546 soccerdata-1.7.1/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 soccerdata-1.7.1/PKG-INFO
```

### Comparing `soccerdata-1.7.0/LICENSE.rst` & `soccerdata-1.7.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/README.rst` & `soccerdata-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/pyproject.toml` & `soccerdata-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.7.0"
+version = "1.7.1"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -39,15 +39,15 @@
 furo = "^2024.0.0"
 coverage = {version = "^7.0", extras = ["toml"]}
 pre-commit = "^3.0.0"
 flake8 = "^7.0.0"
 flake8-bugbear = "^24.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.3.0"
-pep8-naming = "^0.13.2"
+pep8-naming = "^0.14.0"
 darglint = "^1.8.1"
 pre-commit-hooks = "^4.3.0"
 Pygments = "^2.13.0"
 time-machine = "^2.8.2"
 pytest-mock = "^3.10.0"
 bumpversion = "^0.6.0"
 nbsphinx = "^0.9.0"
```

### Comparing `soccerdata-1.7.0/soccerdata/__init__.py` & `soccerdata-1.7.1/soccerdata/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A collection of tools to read and process soccer data from various sources."""
 
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 
 __all__ = [
     'ClubElo',
     'ESPN',
     'FBref',
     'FiveThirtyEight',
     'FotMob',
```

### Comparing `soccerdata-1.7.0/soccerdata/_common.py` & `soccerdata-1.7.1/soccerdata/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,29 +448,35 @@
                     raise WebDriverException(
                         "Your IP is blocked. Use tor or a proxy to continue scraping."
                     )
                 if var is None:
                     response = self._driver.execute_script(
                         "return document.body.innerHTML;"
                     ).encode("utf-8")
+                    if response == b"":
+                        raise Exception("Empty response.")
                 else:
                     if not isinstance(var, str):
                         raise NotImplementedError("Only implemented for single variables.")
                     response = json.dumps(self._driver.execute_script("return " + var)).encode(
                         "utf-8"
                     )
                 if not self.no_store and filepath is not None:
                     filepath.parent.mkdir(parents=True, exist_ok=True)
                     with filepath.open(mode="wb") as fh:
                         fh.write(response)
                 return io.BytesIO(response)
             except Exception:
                 logger.exception(
-                    "Error while scraping %s. Retrying... (attempt %d of 5).", url, i + 1
+                    "Error while scraping %s. Retrying in %d seconds... (attempt %d of 5).",
+                    url,
+                    i * 10,
+                    i + 1,
                 )
+                time.sleep(i * 10)
                 self._driver = self._init_webdriver()
                 continue
 
         raise ConnectionError("Could not download %s." % url)
 
 
 def season_code(season: Union[str, int]) -> str:  # noqa: C901
```

### Comparing `soccerdata-1.7.0/soccerdata/_config.py` & `soccerdata-1.7.1/soccerdata/_config.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/clubelo.py` & `soccerdata-1.7.1/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/espn.py` & `soccerdata-1.7.1/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/fbref.py` & `soccerdata-1.7.1/soccerdata/fbref.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,18 @@
                 "leagues='Big 5 European Leagues Combined'.",
                 stacklevel=1,
             )
 
     @property
     def leagues(self) -> List[str]:
         """Return a list of selected leagues."""
+        if "Big 5 European Leagues Combined" in self._leagues_dict:
+            for _, standardized_name in BIG_FIVE_DICT.items():
+                if standardized_name in self._leagues_dict:
+                    del self._leagues_dict[standardized_name]
         return list(self._leagues_dict.keys())
 
     @classmethod
     def _all_leagues(cls) -> Dict[str, str]:
         """Return a dict mapping all canonical league IDs to source league IDs."""
         res = super()._all_leagues()
         res.update({"Big 5 European Leagues Combined": "Big 5 European Leagues Combined"})
@@ -319,15 +323,15 @@
                 )
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
                 df_table.drop("Rk", axis=1, level=1, inplace=True)
             teams.append(df_table)
 
         # return data frame
         df = (
-            _concat(teams, key=['league', 'season'])
+            _concat(teams, key=["league", "season"])
             .rename(columns={"Squad": "team", "# Pl": "players_used"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             # .pipe(standardize_colnames)
             .set_index(["league", "season", "team"])
             .sort_index()
         )
         return df
@@ -422,15 +426,15 @@
             iterator = df_teams
 
         # collect match logs for each team
         stats = []
         for (lkey, skey, team), team_url in iterator.url.items():
             # read html page
             filepath = self.data_dir / filemask.format(team, skey, stat_type)
-            if len(team_url.split('/')) == 6:  # already have season in the url
+            if len(team_url.split("/")) == 6:  # already have season in the url
                 url = (
                     FBREF_API
                     + team_url.rsplit("/", 1)[0]
                     + "/matchlogs"
                     + "/all_comps"
                     + f"/{stat_type}"
                 )
@@ -461,15 +465,15 @@
             for elem in html_table.xpath("//tfoot"):
                 elem.getparent().remove(elem)
             # parse table
             df_table = _parse_table(html_table)
             df_table["season"] = skey
             df_table["team"] = team
             df_table["Time"] = [
-                x.get('csk', None) for x in html_table.xpath(".//td[@data-stat='start_time']")
+                x.get("csk", None) for x in html_table.xpath(".//td[@data-stat='start_time']")
             ]
             df_table["Match Report"] = [
                 (
                     mlink.xpath("./a/@href")[0]
                     if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
                     else None
                 )
@@ -478,15 +482,15 @@
             nb_levels = df_table.columns.nlevels
             if nb_levels == 2:
                 df_table = df_table.drop(["Match Report", "Time"], axis=1, level=1)
             stats.append(df_table)
 
         # return data frame
         df = (
-            _concat(stats, key=['league', 'season', 'team'])
+            _concat(stats, key=["league", "season", "team"])
             .replace(
                 {
                     "Opponent": TEAMNAME_REPLACEMENTS,
                 }
             )
             .rename(columns={"Comp": "league"})
             .pipe(self._translate_league)
@@ -660,15 +664,17 @@
             reader = self.get(url_stats, filepath_stats)
             tree = html.parse(reader)
 
             url_fixtures = FBREF_API + tree.xpath("//a[text()='Scores & Fixtures']")[0].get("href")
             filepath_fixtures = self.data_dir / f"schedule_{lkey}_{skey}.html"
             current_season = not self._is_complete(lkey, skey)
             reader = self.get(
-                url_fixtures, filepath_fixtures, no_cache=current_season and not force_cache
+                url_fixtures,
+                filepath_fixtures,
+                no_cache=current_season and not force_cache,
             )
             tree = html.parse(reader)
             html_table = tree.xpath("//table[contains(@id, 'sched')]")[0]
             df_table = _parse_table(html_table)
             df_table["Match Report"] = [
                 (
                     mlink.xpath("./a/@href")[0]
@@ -795,15 +801,18 @@
             iterator = df_schedule
 
         stats = []
         for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             (home_team, away_team) = self._parse_teams(tree)
             if stat_type == "keepers":
                 id_format = "keeper_stats_{}"
@@ -828,27 +837,29 @@
                 df_table["league"] = game["league"]
                 df_table["season"] = game["season"]
                 df_table["game_id"] = game["game_id"]
                 stats.append(df_table)
             else:
                 logger.warning("No stats found for away team for game with id=%s", game["game_id"])
 
-        df = _concat(stats, key=['game'])
+        df = _concat(stats, key=["game"])
         df = df[~df.Player.str.contains(r"^\d+\sPlayers$")]
         df = (
             df.rename(columns={"#": "jersey_number"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(standardize_colnames, cols=["Player", "Nation", "Pos", "Age", "Min"])
             .set_index(["league", "season", "game", "team", "player"])
             .sort_index()
         )
         return df
 
     def read_lineup(
-        self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
+        self,
+        match_id: Optional[Union[str, List[str]]] = None,
+        force_cache: bool = False,
     ) -> pd.DataFrame:
         """Retrieve lineups for the selected leagues and seasons.
 
         Parameters
         ----------
         match_id : int or list of int, optional
             Retrieve the lineup for a specific game.
@@ -883,15 +894,18 @@
             iterator = df_schedule
 
         lineups = []
         for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
             html_tables = tree.xpath("//div[@class='lineup']")
             for i, html_table in enumerate(html_tables):
@@ -910,27 +924,34 @@
                     df_table.drop(bench_idx, inplace=True)
                 # augment with stats
                 html_stats_table = tree.find(
                     "//table[@id='" + "stats_{}_summary".format(teams[i]["id"]) + "']"
                 )
                 df_stats_table = _parse_table(html_stats_table)
                 df_stats_table = df_stats_table.droplevel(0, axis=1)[["Player", "#", "Pos", "Min"]]
-                df_stats_table.columns = ["player", "jersey_number", "position", "minutes_played"]
+                df_stats_table.columns = [
+                    "player",
+                    "jersey_number",
+                    "position",
+                    "minutes_played",
+                ]
                 df_stats_table["jersey_number"] = df_stats_table["jersey_number"].astype("Int64")
                 df_table["jersey_number"] = df_table["jersey_number"].astype("Int64")
                 df_table = pd.merge(
                     df_table, df_stats_table, on=["player", "jersey_number"], how="left"
                 )
                 df_table["minutes_played"] = df_table["minutes_played"].fillna(0)
                 lineups.append(df_table)
         df = pd.concat(lineups).set_index(["league", "season", "game"])
         return df
 
     def read_events(
-        self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
+        self,
+        match_id: Optional[Union[str, List[str]]] = None,
+        force_cache: bool = False,
     ) -> pd.DataFrame:
         """Retrieve match events for the selected seasons or selected matches.
 
         The data returned includes the timing of goals, cards and substitutions.
         Also includes the players who are involved in the event.
 
         Parameters
@@ -969,15 +990,18 @@
 
         events = []
         for i, game in iterator.reset_index().iterrows():
             match_events = []
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
             for team, tid in zip(teams, ["a", "b"]):
                 html_events = tree.xpath(f"////*[@id='events_wrap']/div/div[@class='event {tid}']")
@@ -1017,15 +1041,17 @@
             .set_index(["league", "season", "game"])
             .sort_index()
             .dropna(how="all")
         )
         return df
 
     def read_shot_events(
-        self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
+        self,
+        match_id: Optional[Union[str, List[str]]] = None,
+        force_cache: bool = False,
     ) -> pd.DataFrame:
         """Retrieve shooting data for the selected seasons or selected matches.
 
         The data returned includes who took the shot, when, with which body
         part and from how far away. Additionally, the player creating the
         chance and also the creation before this are included in the data.
 
@@ -1064,15 +1090,18 @@
             iterator = df_schedule
 
         shots = []
         for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league anigd season
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             html_table = tree.find("//table[@id='shots_all']")
             if html_table is not None:
                 df_table = _parse_table(html_table)
@@ -1083,20 +1112,28 @@
             else:
                 logger.warning("No shot data found for game with id=%s", game["game_id"])
 
         if len(shots) == 0:
             return pd.DataFrame()
 
         df = (
-            _concat(shots, key=['game'])
+            _concat(shots, key=["game"])
             .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(
                 standardize_colnames,
-                cols=["Outcome", "Minute", "Distance", "Player", "Body Part", "Notes", "Event"],
+                cols=[
+                    "Outcome",
+                    "Minute",
+                    "Distance",
+                    "Player",
+                    "Body Part",
+                    "Notes",
+                    "Event",
+                ],
             )
             .set_index(["league", "season", "game"])
             .sort_index()
             .dropna(how="all")
         )
         return df
 
@@ -1174,36 +1211,36 @@
             columns.loc[mask, 1] = ""
             df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
 
     # throw a warning if not all dataframes have the same length and level 1 columns
     if len(all_columns) and all_columns[0].shape[1] == 2:
         for i, columns in enumerate(all_columns):
             if not columns[1].equals(all_columns[0][1]):
-                res = all_columns[0].merge(columns, indicator=True, how='outer')
+                res = all_columns[0].merge(columns, indicator=True, how="outer")
                 warnings.warn(
                     (
                         "Different columns found for {first} and {cur}.\n\n"
                         + "The following columns are missing in {first}: {extra_cols}.\n\n"
                         + "The following columns are missing in {cur}: {missing_cols}.\n\n"
                         + "The columns of the dataframe with the most columns will be used."
                     ).format(
                         first=dfs[0].iloc[:1][key].values,
                         cur=dfs[i].iloc[:1][key].values,
                         extra_cols=", ".join(
                             map(
                                 str,
-                                res.loc[res['_merge'] == "left_only", [0, 1]]
+                                res.loc[res["_merge"] == "left_only", [0, 1]]
                                 .to_records(index=False)
                                 .tolist(),
                             )
                         ),
                         missing_cols=", ".join(
                             map(
                                 str,
-                                res.loc[res['_merge'] == "right_only", [0, 1]]
+                                res.loc[res["_merge"] == "right_only", [0, 1]]
                                 .to_records(index=False)
                                 .tolist(),
                             )
                         ),
                     ),
                     stacklevel=1,
                 )
```

### Comparing `soccerdata-1.7.0/soccerdata/fivethirtyeight.py` & `soccerdata-1.7.1/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/fotmob.py` & `soccerdata-1.7.1/soccerdata/fotmob.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/match_history.py` & `soccerdata-1.7.1/soccerdata/match_history.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/sofascore.py` & `soccerdata-1.7.1/soccerdata/sofascore.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/sofifa.py` & `soccerdata-1.7.1/soccerdata/sofifa.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/understat.py` & `soccerdata-1.7.1/soccerdata/understat.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.7.0/soccerdata/whoscored.py` & `soccerdata-1.7.1/soccerdata/whoscored.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 import itertools
 import json
 import re
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Callable, Dict, Iterable, List, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 from lxml import html
 from selenium.common.exceptions import (
     ElementClickInterceptedException,
     NoSuchElementException,
-    TimeoutException,
 )
 from selenium.webdriver.common.by import By
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.support import expected_conditions as ec
-from selenium.webdriver.support.ui import WebDriverWait
 
 from ._common import (
     BaseSeleniumReader,
     make_game_id,
     season_code,
     standardize_colnames,
 )
@@ -123,14 +119,52 @@
             "Jumapili": "Sunday",
         }
         for sw, en in {**swahili_months, **swahili_days}.items():
             ts = ts.replace(sw, en)
         return datetime.strptime(ts, "%A, %b %d %Y %H:%M")
 
 
+def _parse_url(url: str) -> Dict:
+    """Parse a URL from WhoScored.
+
+    Parameters
+    ----------
+    url : str
+        URL to parse.
+
+    Raises
+    ------
+    ValueError
+        If the URL could not be parsed.
+
+    Returns
+    -------
+    dict
+    """
+    patt = (
+        r"^(?:https:\/\/www.whoscored.com)?\/"
+        + r"(?:Regions\/(\d+)\/)?"
+        + r"(?:Tournaments\/(\d+)\/)?"
+        + r"(?:Seasons\/(\d+)\/)?"
+        + r"(?:Stages\/(\d+)\/)?"
+        + r"(?:Matches\/(\d+)\/)?"
+    )
+    matches = re.search(patt, url)
+    if matches:
+        return {
+            "region_id": matches.group(1),
+            "league_id": matches.group(2),
+            "season_id": matches.group(3),
+            "stage_id": matches.group(4),
+            "match_id": matches.group(5),
+        }
+    else:
+        raise ValueError(f"Could not parse URL: {url}")
+
+
 class WhoScored(BaseSeleniumReader):
     """Provides pd.DataFrames from data available at http://whoscored.com.
 
     Data will be downloaded as necessary and cached locally in
     ``~/soccerdata/data/WhoScored``.
 
     Parameters
@@ -220,15 +254,14 @@
             for league in region["tournaments"]:
                 leagues.append(
                     {
                         "region_id": region["id"],
                         "region": region["name"],
                         "league_id": league["id"],
                         "league": league["name"],
-                        "url": league["url"],
                     }
                 )
 
         df = (
             pd.DataFrame(leagues)
             .assign(league=lambda x: x.region + " - " + x.league)
             .pipe(self._translate_league)
@@ -245,234 +278,247 @@
         -------
         pd.DataFrame
         """
         df_leagues = self.read_leagues()
 
         seasons = []
         for lkey, league in df_leagues.iterrows():
-            url = WHOSCORED_URL + league.url
+            url = (
+                WHOSCORED_URL
+                + f"/Regions/{league['region_id']}"
+                + f"/Tournaments/{league['league_id']}"
+            )
             filemask = "seasons/{}.html"
             filepath = self.data_dir / filemask.format(lkey)
             reader = self.get(url, filepath, var=None)
 
             # extract team links
             tree = html.parse(reader)
             for node in tree.xpath("//select[contains(@id,'seasons')]/option"):
                 # extract team IDs from links
+                season_url = node.get("value")
+                season_id = _parse_url(season_url)["season_id"]
                 seasons.append(
                     {
-                        "url": node.get("value"),
                         "league": lkey,
-                        "league_id": league.league_id,
                         "season": season_code(node.text),
+                        "region_id": league.region_id,
+                        "league_id": league.league_id,
+                        "season_id": season_id,
                     }
                 )
 
         df = (
             pd.DataFrame(seasons)
             .set_index(["league", "season"])
             .sort_index()
             .loc[itertools.product(self.leagues, self.seasons)]
         )
         return df
 
-    def _parse_season_stages(self) -> List[Dict]:
-        match_selector = (
-            "//div[contains(@id,'tournament-fixture')]//div[contains(@class,'divtable-row')]"
-        )
-        WebDriverWait(self._driver, 30, poll_frequency=1).until(
-            ec.presence_of_element_located((By.XPATH, match_selector))
-        )
-        node_stages_selector = "//select[contains(@id,'stages')]/option"
-        node_stages = self._driver.find_elements(By.XPATH, node_stages_selector)
-        stages = []
-        for stage in node_stages:
-            if not re.search(r"Grp. ([A-Z])$", stage.text):
-                # there is always a page with all group stage games combined
-                stages.append({"url": stage.get_attribute("value"), "name": stage.text})
-        return stages
-
-    def _parse_schedule_page(self) -> Tuple[List[Dict], Optional[WebElement]]:
-        match_selector = (
-            "//div[contains(@id,'tournament-fixture')]//div[contains(@class,'divtable-row')]"
-        )
-        date_selector = "./div[contains(@class,'divtable-header')]"
-        time_selector = "./div[contains(@class,'time')]"
-        home_team_selector = "./div[contains(@class,'team home')]//a"
-        away_team_selector = "./div[contains(@class,'team away')]//a"
-        result_selector = "./div[contains(@class,'result')]//a"
-
-        try:
-            WebDriverWait(self._driver, 30, poll_frequency=1).until(
-                ec.presence_of_element_located((By.XPATH, match_selector))
+    def read_season_stages(self, force_cache: bool = False) -> pd.DataFrame:
+        """Retrieve the season stages for the selected leagues.
+
+        Parameters
+        ----------
+        force_cache : bool
+             By default no cached data is used for the current season.
+             If True, will force the use of cached data anyway.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        df_seasons = self.read_seasons()
+        filemask = "seasons/{}_{}.html"
+
+        season_stages = []
+        for (lkey, skey), season in df_seasons.iterrows():
+            current_season = not self._is_complete(lkey, skey)
+
+            # get season page
+            url = (
+                WHOSCORED_URL
+                + f"/Regions/{season['region_id']}"
+                + f"/Tournaments/{season['league_id']}"
+                + f"/Seasons/{season['season_id']}"
             )
-            date_str = None
-            schedule_page = []
-            for node in self._driver.find_elements(By.XPATH, match_selector):
-                if node.get_attribute("data-id"):
-                    match_id = int(node.get_attribute("data-id"))
-                    time_str = node.find_element(By.XPATH, time_selector).get_attribute(
-                        "textContent"
-                    )
-                    match_url = node.find_element(By.XPATH, result_selector).get_attribute("href")
-                    schedule_page.append(
-                        {
-                            "date": _parse_datetime(f"{date_str} {time_str}"),
-                            "home_team": node.find_element(By.XPATH, home_team_selector).text,
-                            "away_team": node.find_element(By.XPATH, away_team_selector).text,
-                            "game_id": match_id,
-                            "url": match_url,
-                        }
-                    )
-                else:
-                    date_str = node.find_element(By.XPATH, date_selector).text
-                    logger.info("Scraping game schedule for %s", date_str)
-        except TimeoutException:
-            schedule_page = []
-
-        try:
-            next_page_selector = (
-                "//div[contains(@id,'date-controller')]"
-                "/a[contains(@class,'previous') and not(contains(@class, 'is-disabled'))]"
+            filepath = self.data_dir / filemask.format(lkey, skey)
+            reader = self.get(url, filepath, var=None, no_cache=current_season and not force_cache)
+            tree = html.parse(reader)
+
+            # get default season stage
+            fixtures_url = tree.xpath("//a[text()='Fixtures']/@href")[0]
+            stage_id = _parse_url(fixtures_url)["stage_id"]
+            season_stages.append(
+                {
+                    "league": lkey,
+                    "season": skey,
+                    "region_id": season.region_id,
+                    "league_id": season.league_id,
+                    "season_id": season.season_id,
+                    "stage_id": stage_id,
+                    "stage": None,
+                }
             )
-            next_page = self._driver.find_element(By.XPATH, next_page_selector)
-        except NoSuchElementException:
-            next_page = None
-        return schedule_page, next_page
-
-    def _parse_schedule(self, stage: Optional[str] = None) -> List[Dict]:
-        schedule = []
-        # Parse first page
-        page_schedule, next_page = self._parse_schedule_page()
-        schedule.extend(page_schedule)
-        # Go to next page
-        while next_page is not None:
-            try:
-                next_page.click()
-                time.sleep(5)
-                logger.debug("Next page")
-            except ElementClickInterceptedException:
-                self._handle_banner()
-            # Parse next page
-            page_schedule, next_page = self._parse_schedule_page()
-            schedule.extend(page_schedule)
-        schedule = [dict(item, stage=stage) for item in schedule]
-        return schedule
+
+            # extract additional stages
+            for node in tree.xpath("//select[contains(@id,'stages')]/option"):
+                stage_url = node.get("value")
+                stage_id = _parse_url(stage_url)["stage_id"]
+                season_stages.append(
+                    {
+                        "league": lkey,
+                        "season": skey,
+                        "region_id": season.region_id,
+                        "league_id": season.league_id,
+                        "season_id": season.season_id,
+                        "stage_id": stage_id,
+                        "stage": node.text,
+                    }
+                )
+
+        df = (
+            pd.DataFrame(season_stages)
+            .drop_duplicates(subset=["league", "season", "stage_id"], keep="last")
+            .set_index(["league", "season"])
+            .sort_index()
+            .loc[itertools.product(self.leagues, self.seasons)]
+        )
+        return df
 
     def read_schedule(self, force_cache: bool = False) -> pd.DataFrame:  # noqa: C901
         """Retrieve the game schedule for the selected leagues and seasons.
 
         Parameters
         ----------
         force_cache : bool
              By default no cached data is used for the current season.
              If True, will force the use of cached data anyway.
 
         Returns
         -------
         pd.DataFrame
         """
-        df_seasons = self.read_seasons()
-        filemask = "matches/{}_{}.csv"
+        df_season_stages = self.read_season_stages(force_cache=force_cache)
+        filemask_schedule = "matches/{}_{}_{}_{}.json"
 
         all_schedules = []
-        for (lkey, skey), season in df_seasons.iterrows():
-            filepath = self.data_dir / filemask.format(lkey, skey)
-            url = WHOSCORED_URL + season.url
-
-            schedule = []
-            is_current_season = not self._is_complete(lkey, skey)
-            no_cache = (not filepath.exists()) or self.no_cache
-            if (is_current_season and not force_cache) or no_cache:
-                # Scrape the season's schedule
-                self._driver.get(url)
-
-                # Check if season consists of multiple stages
-                stages = self._parse_season_stages()
-
-                # Handle a multi-stage season
-                if len(stages) > 0:
-                    for stage in stages:
-                        url = WHOSCORED_URL + stage["url"].replace("Show", "Fixtures")
-                        self._driver.get(url)
-                        try:
-                            WebDriverWait(self._driver, 30, poll_frequency=1).until(
-                                ec.presence_of_element_located(
-                                    (By.XPATH, "//div[@id='tournament-fixture']")
-                                )
-                            )
-                        except TimeoutException:
-                            # Tournaments sometimes do not have a fixtures page,
-                            # the summary page has to be used instead
-                            url = WHOSCORED_URL + stage["url"]
-                            self._driver.get(url)
-                        logger.info("Scraping game schedule with stage=%s from %s", stage, url)
-                        schedule.extend(self._parse_schedule(stage=stage["name"]))
+        for (lkey, skey), stage in df_season_stages.iterrows():
+            current_season = not self._is_complete(lkey, skey)
+            stage_id = stage["stage_id"]
+            stage_name = stage["stage"]
+
+            # get the calendar of the season stage
+            season_stage_url = (
+                WHOSCORED_URL
+                + f"/Regions/{stage['region_id']}"
+                + f"/Tournaments/{stage['league_id']}"
+                + f"/Seasons/{stage['season_id']}"
+                + f"/Stages/{stage['stage_id']}"
+            )
+            if stage_name is not None:
+                calendar_filepath = self.data_dir / "matches/{}_{}_{}.html".format(
+                    lkey, skey, stage_id
+                )
+                logger.info(
+                    "Retrieving calendar for %s %s (%s)",
+                    lkey,
+                    skey,
+                    stage_name,
+                )
+            else:
+                calendar_filepath = self.data_dir / f"matches/{lkey}_{skey}.html"
+                logger.info(
+                    "Retrieving calendar for %s %s",
+                    lkey,
+                    skey,
+                )
+            calendar = self.get(
+                season_stage_url,
+                calendar_filepath,
+                var="wsCalendar",
+                no_cache=current_season and not force_cache,
+            )
+            mask = json.load(calendar)["mask"]
 
-                # Handle a single-stage season
+            # get the fixtures for each month
+            it = [(year, month) for year in mask.keys() for month in mask[year].keys()]
+            for i, (year, month) in enumerate(it):
+                filepath = self.data_dir / filemask_schedule.format(lkey, skey, stage_id, month)
+                url = WHOSCORED_URL + f"/tournaments/{stage_id}/data/?d={year}{(int(month)+1):02d}"
+
+                if stage_name is not None:
+                    logger.info(
+                        "[%s/%s] Retrieving fixtures for %s %s (%s)",
+                        i + 1,
+                        len(it),
+                        lkey,
+                        skey,
+                        stage_name,
+                    )
                 else:
-                    fixtures_nav_selector = "//a[text()='Fixtures']"
-                    fixtures_nav = self._driver.find_element(By.XPATH, fixtures_nav_selector)
-                    self._driver.get(fixtures_nav.get_attribute("href"))
-                    try:
-                        WebDriverWait(self._driver, 30, poll_frequency=1).until(
-                            ec.presence_of_element_located(
-                                (By.XPATH, "//div[@id='tournament-fixture']")
-                            )
-                        )
-                    except TimeoutException:
-                        # Tournaments sometimes do not have a fixtures page,
-                        # the summary page has to be used instead
-                        summary_nav_selector = "//a[text()='Fixtures']"
-                        summary_nav = self._driver.find_element(By.XPATH, summary_nav_selector)
-                        self._driver.get(summary_nav.get_attribute("href"))
-                    logger.info("Scraping game schedule from %s", url)
-                    schedule.extend(self._parse_schedule())
-
-                # Cache the data
-                df_schedule = pd.DataFrame(schedule).assign(league=lkey, season=skey)
-                if not self.no_store:
-                    df_schedule.to_csv(filepath, index=False)
-
-            else:
-                # Load cached data
-                logger.info("Retrieving game schedule of %s - %s from the cache", lkey, skey)
-                df_schedule = pd.read_csv(filepath)
+                    logger.info(
+                        "[%s/%s] Retrieving fixtures for %s %s",
+                        i + 1,
+                        len(it),
+                        lkey,
+                        skey,
+                    )
 
-            all_schedules.append(df_schedule)
+                reader = self.get(
+                    url, filepath, var=None, no_cache=current_season and not force_cache
+                )
+                data = json.load(reader)
+                for tournament in data["tournaments"]:
+                    df_schedule = pd.DataFrame(tournament["matches"])
+                    df_schedule["league"] = lkey
+                    df_schedule["season"] = skey
+                    df_schedule["stage"] = stage_name
+                    all_schedules.append(df_schedule)
 
         if len(all_schedules) == 0:
             return pd.DataFrame(index=["league", "season", "game"])
 
         # Construct the output dataframe
         df = (
             pd.concat(all_schedules)
-            .drop_duplicates()
+            .drop_duplicates(subset=["id"])
             .replace(
                 {
-                    "home_team": TEAMNAME_REPLACEMENTS,
-                    "away_team": TEAMNAME_REPLACEMENTS,
+                    "homeTeamName": TEAMNAME_REPLACEMENTS,
+                    "awayTeamName": TEAMNAME_REPLACEMENTS,
+                }
+            )
+            .rename(
+                columns={
+                    "homeTeamName": "home_team",
+                    "awayTeamName": "away_team",
+                    "id": "game_id",
+                    "startTimeUtc": "date",
                 }
             )
             .assign(date=lambda x: pd.to_datetime(x["date"]))
             .assign(game=lambda df: df.apply(make_game_id, axis=1))
+            .pipe(standardize_colnames)
             .set_index(["league", "season", "game"])
             .sort_index()
         )
         return df
 
     def _read_game_info(self, game_id: int) -> Dict:
         """Return game info available in the header."""
         urlmask = WHOSCORED_URL + "/Matches/{}"
         url = urlmask.format(game_id)
         data = {}
         self._driver.get(url)
         # league and season
         breadcrumb = self._driver.find_elements(
-            By.XPATH, "//div[@id='breadcrumb-nav']/*[not(contains(@class, 'separator'))]"
+            By.XPATH,
+            "//div[@id='breadcrumb-nav']/*[not(contains(@class, 'separator'))]",
         )
         country = breadcrumb[0].text
         league, season = breadcrumb[1].text.split(" - ")
         data["league"] = {v: k for k, v in self._all_leagues().items()}[f"{country} - {league}"]
         data["season"] = season_code(season)
         # match header
         match_header = self._driver.find_element(By.XPATH, "//div[@id='match-header']")
@@ -492,15 +538,17 @@
                 for desc_def in desc_list.find_elements(By.TAG_NAME, "dt"):
                     desc_val = desc_def.find_element(By.XPATH, "./following-sibling::dd")
                     data[desc_def.text] = desc_val.text
 
         return data
 
     def read_missing_players(
-        self, match_id: Optional[Union[int, List[int]]] = None, force_cache: bool = False
+        self,
+        match_id: Optional[Union[int, List[int]]] = None,
+        force_cache: bool = False,
     ) -> pd.DataFrame:
         """Retrieve a list of injured and suspended players ahead of each game.
 
         Parameters
         ----------
         match_id : int or list of int, optional
             Retrieve the missing players for a specific game.
@@ -533,15 +581,18 @@
 
         match_sheets = []
         for i, (_, game) in enumerate(iterator.iterrows()):
             url = urlmask.format(game.game_id)
             filepath = DATA_DIR / filemask.format(game["league"], game["season"], game["game_id"])
 
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             reader = self.get(url, filepath, var=None)
 
             # extract missing players
             tree = html.parse(reader)
             for node in tree.xpath("//div[@id='missing-players']/div[2]/table/tbody/tr"):
                 # extract team IDs from links
@@ -598,14 +649,16 @@
 
     def read_events(  # noqa: C901
         self,
         match_id: Optional[Union[int, List[int]]] = None,
         force_cache: bool = False,
         live: bool = False,
         output_fmt: Optional[str] = "events",
+        retry_missing: bool = True,
+        on_error: Literal["raise", "skip"] = "raise",
     ) -> Optional[Union[pd.DataFrame, Dict[int, List], "OptaLoader"]]:  # type: ignore  # noqa: F821
         """Retrieve the the event data for each game in the selected leagues and seasons.
 
         Parameters
         ----------
         match_id : int or list of int, optional
             Retrieve the event stream for a specific game.
@@ -627,19 +680,26 @@
                   of the original events.
                   See https://socceraction.readthedocs.io/en/latest/documentation/SPADL.html#atomic-spadl
                 - 'loader': Returns a socceraction.data.opta.OptaLoader
                   instance, which can be used to retrieve the actual data.
                   See https://socceraction.readthedocs.io/en/latest/modules/generated/socceraction.data.opta.OptaLoader.html#socceraction.data.opta.OptaLoader  # noqa: E501
                 - None: Doesn't return any data. This is useful to just cache
                   the data without storing the events in memory.
+        retry_missing : bool
+            If no events were found for a game in a previous attempt, will
+            retry to scrape the events
+        on_error : "raise" or "skip", default: "raise"
+            Wheter to raise an exception or to skip the game if an error occurs.
 
         Raises
         ------
         ValueError
             If the given match_id could not be found in the selected seasons.
+        ConnectionError
+            If the match page could not be retrieved.
         ImportError
             If the requested output format is 'spadl', 'atomic-spadl' or
             'loader' but the socceraction package is not installed.
 
         Returns
         -------
         See the description of the ``output_fmt`` parameter.
@@ -688,33 +748,42 @@
         events = {}
         player_names = {}
         team_names = {}
         for i, (_, game) in enumerate(iterator.iterrows()):
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
-                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+                "[%s/%s] Retrieving game with id=%s",
+                i + 1,
+                len(iterator),
+                game["game_id"],
             )
             filepath = self.data_dir / filemask.format(
                 game["league"], game["season"], game["game_id"]
             )
 
-            reader = self.get(
-                url,
-                filepath,
-                var="requirejs.s.contexts._.config.config.params.args.matchCentreData",
-                no_cache=live,
-            )
-            if reader.read(4) == b'null':
+            try:
                 reader = self.get(
                     url,
                     filepath,
                     var="requirejs.s.contexts._.config.config.params.args.matchCentreData",
-                    no_cache=True,
+                    no_cache=live,
                 )
+                if retry_missing and reader.read(4) == b"null":
+                    reader = self.get(
+                        url,
+                        filepath,
+                        var="requirejs.s.contexts._.config.config.params.args.matchCentreData",
+                        no_cache=True,
+                    )
+            except ConnectionError as e:
+                if on_error == "skip":
+                    logger.warning("Error while scraping game %s: %s", game["game_id"], e)
+                    continue
+                raise
             reader.seek(0)
             json_data = json.load(reader)
             if json_data is not None:
                 player_names.update(
                     {int(k): v for k, v in json_data["playerIdNameDictionary"].items()}
                 )
                 team_names.update(
```

### Comparing `soccerdata-1.7.0/PKG-INFO` & `soccerdata-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.7.0
+Version: 1.7.1
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.9,<3.13
```

