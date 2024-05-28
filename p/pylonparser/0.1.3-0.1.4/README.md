# Comparing `tmp/pylonparser-0.1.3.tar.gz` & `tmp/pylonparser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylonparser-0.1.3.tar", max compression
+gzip compressed data, was "pylonparser-0.1.4.tar", max compression
```

## Comparing `pylonparser-0.1.3.tar` & `pylonparser-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-05-23 19:03:26.231140 pylonparser-0.1.3/LICENSE
--rw-r--r--   0        0        0     1834 2024-05-23 18:45:59.171621 pylonparser-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.3/pylonparser/__init__.py
--rw-r--r--   0        0        0     1666 2024-05-26 18:02:35.771810 pylonparser-0.1.3/pylonparser/matches.py
--rw-r--r--   0        0        0     5736 2024-05-26 18:02:35.771810 pylonparser-0.1.3/pylonparser/scraper.py
--rw-r--r--   0        0        0      758 2024-05-26 18:07:26.701783 pylonparser-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 pylonparser-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-23 19:03:26.231140 pylonparser-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1738 2024-05-26 19:25:53.391342 pylonparser-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.4/pylonparser/__init__.py
+-rw-r--r--   0        0        0     3194 2024-05-26 19:26:04.371341 pylonparser-0.1.4/pylonparser/matches.py
+-rw-r--r--   0        0        0     1158 2024-05-28 18:55:39.025653 pylonparser-0.1.4/pylonparser/schedules.py
+-rw-r--r--   0        0        0     7738 2024-05-28 18:55:39.025653 pylonparser-0.1.4/pylonparser/scraper.py
+-rw-r--r--   0        0        0      758 2024-05-28 18:59:41.955625 pylonparser-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 pylonparser-0.1.4/PKG-INFO
```

### Comparing `pylonparser-0.1.3/LICENSE` & `pylonparser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylonparser-0.1.3/pylonparser/scraper.py` & `pylonparser-0.1.4/pylonparser/scraper.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,42 @@
 import re
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class WebScraper:
+    """
+    A class for scraping and parsing HTML tables from a web page.
+
+    Attributes:
+        url (str): The URL of the web page to scrape.
+
+    Methods:
+        __init__(self, url: str): Initializes a new instance of the WebScraper class.
+        get_page(self, url: str) -> BeautifulSoup: Fetches the web page content and returns it as a BeautifulSoup object.
+        parse_football_table(self, table_id: str) -> list: Parses a football table from the web page and returns it as a list of dictionaries.
+        find_basketball_table_ids(self): Finds the IDs of basketball tables in the web page and returns them as a list.
+        parse_table_type(self, table_type: str) -> tuple: Parses the table type string to determine the partial ID and occurrence.
+        translate_table_id(self, html: HTMLParser, partial_id: str, occurrence: int) -> str: Translates a partial table ID to a full table ID based on its occurrence in the HTML content.
+        parse_basketball_table(self, table_type: str): Parses a basketball table from the web page and returns it as a list of dictionaries.
+    """
+
     def __init__(self, url: str):
         self.url = url
         self.soup = self.get_page(url)
 
     def get_page(self, url: str) -> BeautifulSoup:
+        """
+        Fetches the web page content and returns it as a BeautifulSoup object.
+
+        :param url: The URL of the web page.
+        :return: A BeautifulSoup object representing the web page content.
+        :raises requests.RequestException: If an error occurs while fetching the web page.
+        """
         try:
             response = requests.get(url)
             response.raise_for_status()
             content = response.content
             soup = BeautifulSoup(content, "html.parser")
             for comment in soup.find_all(string=lambda text: isinstance(text, Comment)):
                 if comment.startswith('\n\n<div class="table_container"'):
@@ -25,14 +48,23 @@
                     comment.replace_with(new_tag)
             return soup
         except requests.RequestException as e:
             logger.error(f"Error fetching page {url}: {e}")
             raise
 
     def parse_football_table(self, table_id: str) -> list:
+        """
+        Parses a football table from the HTML document.
+
+        Args:
+            table_id (str): The ID of the table to be parsed.
+
+        Returns:
+            list: A list of dictionaries representing the parsed table.
+        """
         html = HTMLParser(str(self.soup))
         table = html.css_first(f"#{table_id}").css("tbody tr")
         table_list = []
         for row in table:
             table_dict = {}
             header_cell = row.css("th")[0]
             if header_cell.text() not in ["", "Player", "Week"]:
@@ -48,14 +80,20 @@
                     if value.replace(".", "").isdigit():
                         value = int(value) if value.isdigit() else float(value)
                     table_dict[stat.attributes["data-stat"]] = value or 0
                 table_list.append(table_dict)
         return table_list
 
     def find_basketball_table_ids(self):
+        """
+        Finds and returns the IDs of all basketball tables in the HTML document.
+
+        Returns:
+            list: A list of table IDs.
+        """
         html = HTMLParser(str(self.soup))
         tables = html.css("table")
         table_ids = []
         for table in tables:
             table_id = table.attributes.get("id")
             if table_id:
                 table_ids.append(table_id)
@@ -114,26 +152,32 @@
     def parse_basketball_table(self, table_type: str):
         """
         Parses the HTML table based on the given table type and returns the data as a list of dictionaries.
 
         :param table_type: The type of the table (e.g., 'basic-home-stats', 'advanced-away-stats').
         :return: A list of dictionaries with the table data.
         """
-        partial_id, occurrence = self.parse_table_type(table_type)
         html = HTMLParser(str(self.soup))
-        table_id = self.translate_table_id(html, partial_id, occurrence)
+        if table_type != "schedule":
+            partial_id, occurrence = self.parse_table_type(table_type)
+            table_id = self.translate_table_id(html, partial_id, occurrence)
+        else:
+            table_id = "schedule"
         table = html.css_first(f"#{table_id}").css("tbody tr")
         table_list = []
 
         for row in table:
             table_dict = {}
             header_cell = row.css("th")[0]
             if header_cell.text() not in ["", "Reserves"]:
-                table_dict["id"] = header_cell.attributes["data-append-csv"].strip()
-                table_dict[header_cell.attributes["data-stat"]] = header_cell.text()
+                try:
+                    table_dict["id"] = header_cell.attributes["data-append-csv"].strip()
+                    table_dict[header_cell.attributes["data-stat"]] = header_cell.text()
+                except KeyError:
+                    pass
                 for stat in row.css("td"):
                     value = stat.text()
                     if value.replace(".", "").isdigit():
                         value = int(value) if value.isdigit() else float(value)
                     table_dict[stat.attributes["data-stat"]] = value or 0
                 table_list.append(table_dict)
         return table_list
```

### Comparing `pylonparser-0.1.3/pyproject.toml` & `pylonparser-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylonparser"
-version = "0.1.3"
+version = "0.1.4"
 description = "A tool to parse football game stats."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/traxxo/pylonparser"
 repository = "https://github.com/traxxo/pylonparser"
 documentation = "https://github.com/traxxo/pylonparser/wiki"
```

### Comparing `pylonparser-0.1.3/PKG-INFO` & `pylonparser-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylonparser
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to parse football game stats.
 Home-page: https://github.com/traxxo/pylonparser
 License: MIT
 Keywords: parser,football,stats,nfl,pro-football-by-reference
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.10,<4.0
@@ -31,28 +31,28 @@
 ```sh
 pip install pylonparser
 ```
 
 Usage
 Provide instructions on how to use your project. Include code examples if possible.
 ```sh
-import pandas as pd
-from pylonparser.parser import get_game_stats
+url = "https://www.basketball-reference.com/boxscores/202405220MIN.html"
 
-game_stats = get_game_stats("https://www.pro-football-reference.com/boxscores/202009100kan.htm", "player_offense")
-df = pd.DataFrame(game_stats)
+basketball_match = BasketballMatch(url)
+df = pd.DataFrame(basketball_match.basic_away)
 print(df.head())
 
 ❯
-           player        id team pass_cmp pass_att pass_yds pass_td pass_int pass_sacked  ... rush_td rush_long targets rec rec_yds rec_td rec_long fumbles fumbles_lost
-0  Deshaun Watson  WatsDe00  HOU       20       32      253       1        1           4  ...       1        13       0   0       0      0        0       0            0
-1   David Johnson  JohnDa08  HOU        0        0        0       0        0           0  ...       1        19       4   3      32      0       15       0            0
-2    Duke Johnson  JohnDu00  HOU        0        0        0       0        0           0  ...       0         7       1   0       0      0        0       0            0
-3     Will Fuller  FullWi01  HOU        0        0        0       0        0           0  ...       0         0      10   8     112      0       31       0            0
-4    Jordan Akins  AkinJo00  HOU        0        0        0       0        0           0  ...       0         0       2   2      39      1       20       0            0
+          id             player     mp    fg   fga  fg_pct  fg3  fg3a  fg3_pct   ft  fta  ft_pct  orb  drb  trb  ast  stl  blk  tov   pf   pts plus_minus reason
+0  washipj01    P.J. Washington  40:50   4.0  10.0   0.400  2.0   8.0     0.25  3.0  3.0   1.000  0.0  7.0  7.0  0.0  0.0  2.0  3.0  4.0  13.0        +12    NaN
+1  doncilu01        Luka Dončić  40:45  12.0  26.0   0.462  3.0  10.0     0.30  6.0  7.0   0.857  0.0  6.0  6.0  8.0  3.0  1.0  4.0  2.0  33.0         -9    NaN
+2  irvinky01       Kyrie Irving  40:09  12.0  23.0   0.522  0.0   3.0     0.00  6.0  6.0   1.000  1.0  4.0  5.0  4.0  0.0  1.0  2.0  3.0  30.0         +5    NaN
+3  jonesde02  Derrick Jones Jr.  34:55   4.0   9.0   0.444  0.0   2.0     0.00  0.0  0.0   0.000  2.0  2.0  4.0  2.0  0.0  0.0  0.0  1.0   8.0         -8    NaN
+4  gaffoda01     Daniel Gafford  21:07   5.0   9.0   0.556  0.0   0.0     0.00  0.0  0.0   0.000  4.0  5.0  9.0  0.0  0.0  1.0  2.0  2.0  10.0        -15    NaN
+
 ```
 Testing
 This project uses pytest for testing. To run the tests, use:
 
 Contributing
 Contributions are welcome! Please read the contributing guidelines first.
```

