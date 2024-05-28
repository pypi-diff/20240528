# Comparing `tmp/tunein-0.0.4a2-py3-none-any.whl.zip` & `tmp/tunein-0.0.4a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 10693 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3494 b- defN 23-Nov-16 21:37 tunein/__init__.py
--rw-r--r--  2.0 unx     1421 b- defN 23-Nov-16 21:37 tunein/cli.py
--rw-r--r--  2.0 unx     1972 b- defN 23-Nov-16 21:37 tunein/parse.py
--rw-r--r--  2.0 unx      114 b- defN 23-Nov-16 21:37 tunein/version.py
--rw-r--r--  2.0 unx     1683 b- defN 23-Nov-16 21:37 tunein/xml_helper.py
--rw-r--r--  2.0 unx       62 b- defN 23-Nov-16 21:37 tunein/subcommands/__init__.py
--rw-r--r--  2.0 unx     3687 b- defN 23-Nov-16 21:37 tunein/subcommands/search.py
--rw-r--r--  2.0 unx    11431 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      270 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1024 b- defN 23-Nov-16 21:37 tunein-0.0.4a2.dist-info/RECORD
-13 files, 25320 bytes uncompressed, 8991 bytes compressed:  64.5%
+Zip file size: 10222 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     4153 b- defN 24-May-28 21:45 tunein/__init__.py
+-rw-r--r--  2.0 unx     1421 b- defN 24-May-28 21:45 tunein/cli.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-28 21:45 tunein/parse.py
+-rw-r--r--  2.0 unx      114 b- defN 24-May-28 21:45 tunein/version.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-28 21:45 tunein/subcommands/__init__.py
+-rw-r--r--  2.0 unx     4616 b- defN 24-May-28 21:45 tunein/subcommands/search.py
+-rw-r--r--  2.0 unx    11431 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      270 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      947 b- defN 24-May-28 21:45 tunein-0.0.4a3.dist-info/RECORD
+12 files, 25148 bytes uncompressed, 8636 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -6,35 +6,32 @@
 
 Filename: tunein/parse.py
 Comment: 
 
 Filename: tunein/version.py
 Comment: 
 
-Filename: tunein/xml_helper.py
-Comment: 
-
 Filename: tunein/subcommands/__init__.py
 Comment: 
 
 Filename: tunein/subcommands/search.py
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/LICENSE
+Filename: tunein-0.0.4a3.dist-info/LICENSE
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/METADATA
+Filename: tunein-0.0.4a3.dist-info/METADATA
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/WHEEL
+Filename: tunein-0.0.4a3.dist-info/WHEEL
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/entry_points.txt
+Filename: tunein-0.0.4a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/top_level.txt
+Filename: tunein-0.0.4a3.dist-info/top_level.txt
 Comment: 
 
-Filename: tunein-0.0.4a2.dist-info/RECORD
+Filename: tunein-0.0.4a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tunein/__init__.py

```diff
@@ -1,9 +1,10 @@
+from urllib.parse import urlparse, urlunparse
+
 import requests
-from tunein.xml_helper import xml2dict
 from tunein.parse import fuzzy_match
 
 
 class TuneInStation:
     def __init__(self, raw):
         self.raw = raw
 
@@ -12,14 +13,22 @@
         return self.raw.get("title", "")
 
     @property
     def artist(self):
         return self.raw.get("artist", "")
 
     @property
+    def bit_rate(self):
+        return self.raw.get("bitrate")
+
+    @property
+    def media_type(self):
+        return self.raw.get("media_type")
+
+    @property
     def image(self):
         return self.raw.get("image")
 
     @property
     def description(self):
         return self.raw.get("description", "")
 
@@ -40,76 +49,91 @@
         return self.title
 
     @property
     def dict(self):
         """Return a dict representation of the station."""
         return {
             "artist": self.artist,
+            "bit_rate": self.bit_rate,
             "description": self.description,
             "image": self.image,
             "match": self.match(),
+            "media_type": self.media_type,
             "stream": self.stream,
             "title": self.title,
         }
 
 
 class TuneIn:
-    search_url = "http://opml.radiotime.com/Search.ashx"
-    featured_url = "http://opml.radiotime.com/Browse.ashx?c=local"  # local stations
+    search_url = "https://opml.radiotime.com/Search.ashx"
+    featured_url = "http://opml.radiotime.com/Browse.ashx"  # local stations
+    stnd_query = {"formats": "mp3,aac,ogg,html,hls", "render": "json"}
 
     @staticmethod
-    def get_stream_url(url):
-        res = requests.get(url)
-        for url in res.text.splitlines():
-            if (len(url) > 4):
-                if url[-3:] == 'm3u':
-                    return url[:-4]
-                if url[-3:] == 'pls':
-                    res2 = requests.get(url)
-                    # Loop through the data looking for the first url
-                    for line in res2.text.splitlines():
-                        if line.startswith("File1="):
-                            return line[6:]
-                else:
-                    return url
+    def get_stream_urls(url):
+        _url = urlparse(url)
+        for scheme in ("http", "https"):
+            url_str = urlunparse(
+                _url._replace(scheme=scheme, query=_url.query + "&render=json")
+            )
+            res = requests.get(url_str)
+            try:
+                res.raise_for_status()
+                break
+            except requests.exceptions.RequestException:
+                continue
+        else:
+            return "Failed to get stream url"
+
+        stations = res.json().get("body", {})
+
+        for station in stations:
+            if station.get("url", "").endswith(".pls"):
+                res = requests.get(station["url"])
+                file1 = [line for line in res.text.split("\n") if line.startswith("File1=")]
+                if file1:
+                    station["url"] = file1[0].split("File1=")[1]
+
+        return stations
 
     @staticmethod
     def featured():
-        res = requests.post(TuneIn.featured_url)
-        return list(TuneIn._get_stations(res))
+        res = requests.post(
+            TuneIn.featured_url,
+            data={**TuneIn.stnd_query, **{"c": "local"}}
+        )
+        stations = res.json().get("body", [{}])[0].get("children", [])
+        return list(TuneIn._get_stations(stations))
 
     @staticmethod
     def search(query):
-        res = requests.post(TuneIn.search_url, data={"query": query, "formats": "mp3,aac,ogg,html,hls"})
-        return list(TuneIn._get_stations(res, query))
+        res = requests.post(
+            TuneIn.search_url,
+            data={**TuneIn.stnd_query, **{"query": query}}
+        )
+        stations = res.json().get("body", [])
+        return list(TuneIn._get_stations(stations, query))
 
     @staticmethod
-    def _get_stations(res: requests.Response, query: str = ""):
-        res = xml2dict(res.text)
-        if not res.get("opml"):
-            return
-        # stations might be nested based on Playlist/Search
-        outline = res['opml']['body']["outline"]
-
-        if not isinstance(outline, list):
-            return
-        if outline[0].get("outline"):
-            stations = outline[0]["outline"]
-        else:
-            stations = outline
-
+    def _get_stations(stations: requests.Response, query: str = ""):
         for entry in stations:
-            try:
-                if not entry.get("key") == "unavailable" \
-                        and entry.get("type") == "audio" \
-                        and entry.get("item") == "station":
-                    yield TuneInStation(
-                        {"stream": TuneIn.get_stream_url(entry["URL"]),
-                         "url": entry["URL"],
-                         "title": entry.get("current_track") or entry.get("text"),
-                         "artist": entry.get("text"),
-                         "description": entry.get("subtext"),
-                         "image": entry.get("image"),
-                         "query": query
-                         })
-            except:
+            if (
+                entry.get("key") == "unavailable"
+                or entry.get("type") != "audio"
+                or entry.get("item") != "station"
+            ):
                 continue
+            streams = TuneIn.get_stream_urls(entry["URL"])
+            for stream in streams:
+                yield TuneInStation(
+                    {
+                        "stream": stream["url"],
+                        "bitrate": stream["bitrate"],
+                        "media_type": stream["media_type"],
+                        "url": entry["URL"],
+                        "title": entry.get("current_track") or entry.get("text"),
+                        "artist": entry.get("text"),
+                        "description": entry.get("subtext"),
+                        "image": entry.get("image"),
+                        "query": query,
+                    }
+                )
```

## tunein/version.py

```diff
@@ -1,6 +1,6 @@
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 4
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## tunein/subcommands/search.py

```diff
@@ -5,14 +5,15 @@
 import argparse
 import json
 import shutil
 import sys
 
 from tunein import TuneIn
 
+
 class Ansi:
     """ANSI escape codes."""
 
     BLUE = "\x1B[34m"
     BOLD = "\x1B[1m"
     CYAN = "\x1B[36m"
     GREEN = "\x1B[32m"
@@ -22,65 +23,97 @@
     RESET = "\x1B[0m"
     REVERSED = "\x1B[7m"
     UNDERLINE = "\x1B[4m"
     WHITE = "\x1B[37m"
     YELLOW = "\x1B[33m"
     GREY = "\x1B[90m"
 
+
 NOPRINT_TRANS_TABLE = {
     i: None for i in range(0, sys.maxunicode + 1) if not chr(i).isprintable()
 }
 
+
 class Search:
     """The search subcommand for tunein."""
 
     def __init__(self: Search, args: argparse.Namespace) -> None:
         """Initialize the search subcommand."""
         self._args: argparse.Namespace = args
-    
+
     def run(self: Search) -> None:
         """Run the search subcommand."""
         tunein = TuneIn()
         results = tunein.search(self._args.station)
         stations = [station.dict for station in results]
         if not stations:
             print(f"No results for {self._args.station}")
             sys.exit(1)
-        stations.sort(key=lambda x: x["match"], reverse=True)
+        stations.sort(key=lambda x: (x["match"], x["bit_rate"]), reverse=True)
         for station in stations:
             station["title"] = self._printable(station["title"])
             station["artist"] = self._printable(station["artist"])
             station["description"] = self._printable(station["description"])
 
         if self._args.format == "json":
             print(json.dumps(stations, indent=4))
         elif self._args.format == "table":
             max_widths = {}
-            columns = ["title", "artist", "description"]
+            columns = ["title", "bit_rate", "media_type", "artist", "description"]
             for column in columns:
-                max_width = max(len(str(station[column])) for station in stations)
+                max_width = max(
+                    [len(str(station[column])) for station in stations] + [len(column)]
+                )
                 if column == "description":
                     term_width = shutil.get_terminal_size().columns
-                    remaining = term_width - max_widths["title"] - max_widths["artist"] - 2
-                    max_width = min(max_width, remaining) 
+                    remaining = (
+                        term_width
+                        - sum(
+                            [
+                                max_widths[column]
+                                for column in columns
+                                if column != "description"
+                            ]
+                        )
+                        - len(columns)
+                        - 1
+                    )
+                    max_width = min(max_width, remaining)
                 max_widths[column] = max_width
 
-            print(" ".join(column.ljust(max_widths[column]).capitalize() for column in columns))
+            print(
+                " ".join(
+                    column.ljust(max_widths[column]).capitalize().replace("_", " ")
+                    for column in columns
+                )
+            )
             print(" ".join("-" * max_widths[column] for column in columns))
             for station in stations:
                 line_parts = []
                 # title as link
                 link = self._term_link(station.get("stream"), station["title"])
-                line_parts.append(f"{link}{' '*(max_widths['title']-len(station['title']))}")
+                line_parts.append(
+                    f"{link}{' '*(max_widths['title']-len(station['title']))}"
+                )
+                # bit rate
+                line_parts.append(
+                    str(station["bit_rate"]).ljust(max_widths["bit_rate"])
+                )
+                # media type
+                line_parts.append(
+                    str(station["media_type"]).ljust(max_widths["media_type"])
+                )
                 # artist
                 line_parts.append(str(station["artist"]).ljust(max_widths["artist"]))
                 # description clipped
-                line_parts.append(str(station["description"])[:max_widths["description"]])
+                line_parts.append(
+                    str(station["description"])[: max_widths["description"]]
+                )
                 print(" ".join(line_parts))
-    
+
     @staticmethod
     def _term_link(uri: str, label: str) -> str:
         """Return a link.
 
         Args:
             uri: The URI to link to
             label: The label to use for the link
@@ -93,16 +126,14 @@
         escape_mask = "\x1b]8;{};{}\x1b\\{}\x1b]8;;\x1b\\"
         link_str = escape_mask.format(parameters, uri, label)
         return f"{Ansi.BLUE}{link_str}{Ansi.RESET}"
 
     @staticmethod
     def _printable(string: str) -> str:
         """Replace non-printable characters in a string.
-        
+
         Args:
             string: The string to replace non-printable characters in.
         Returns:
             The string with non-printable characters replaced.
         """
         return string.translate(NOPRINT_TRANS_TABLE)
-
-
```

## Comparing `tunein-0.0.4a2.dist-info/LICENSE` & `tunein-0.0.4a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tunein-0.0.4a2.dist-info/RECORD` & `tunein-0.0.4a3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-tunein/__init__.py,sha256=Wxkz5cUzre5PH9R4_wYIVpJbDDlJ8L2DyquThlF70bk,3494
+tunein/__init__.py,sha256=rbGaPkoZLkVTOzDochXDA_gDcxv5jJuylf0_i_9g29A,4153
 tunein/cli.py,sha256=oVTE33PTR5hNggcOOamD-LmqCr-Mkc2V_CJW0kBuTaI,1421
 tunein/parse.py,sha256=O3h10tIm41wOPtyScbS7HB6H7FZIBpxQw8Tt0p80uBY,1972
-tunein/version.py,sha256=r_gFbUTUjJB6qv0lvHU6jxeFo1eY7xGObelwN97Ok9s,114
-tunein/xml_helper.py,sha256=SiG-8pUlsPJ74oymXhHQrkLEbYYMGeBZF8rLFrAD4tc,1683
+tunein/version.py,sha256=J6Z3IGOGnVrLzAqT_KZW75XpGb1WQRJLYSQgyjuEiSM,114
 tunein/subcommands/__init__.py,sha256=PKQ8DL4wu9k6WpdV2FGm7K-dz24FAoehn7W3JZemDD8,62
-tunein/subcommands/search.py,sha256=WAH6qZ7SqRYfZ2ozu6hgOMQnLGJRLvKaI0pgLP23Bww,3687
-tunein-0.0.4a2.dist-info/LICENSE,sha256=Say7sFhMWFZjsayrsgHilF-61WjPO02-sBrHVI2t34Y,11431
-tunein-0.0.4a2.dist-info/METADATA,sha256=CsCRphZGDjjHRTeSYK8wbgGf9zoQ2Rv8DU9aTMvfcfc,270
-tunein-0.0.4a2.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-tunein-0.0.4a2.dist-info/entry_points.txt,sha256=8O20QAsieAxufCAJpYO-36N03WBtUoezgyXMtRg_ryc,44
-tunein-0.0.4a2.dist-info/top_level.txt,sha256=FtWUQkdFCEWv3fbtXtJHWTwhXK3ZkI-GOTW_Fh4YdPE,26
-tunein-0.0.4a2.dist-info/RECORD,,
+tunein/subcommands/search.py,sha256=k2B_nYJFpEH3p_enJ2zbyOobFFO7sd-RiYzaIvroS-0,4616
+tunein-0.0.4a3.dist-info/LICENSE,sha256=Say7sFhMWFZjsayrsgHilF-61WjPO02-sBrHVI2t34Y,11431
+tunein-0.0.4a3.dist-info/METADATA,sha256=rVFNVjPrfBfiSShJT4prd_MrpLLhFf36UIL3gWmPG-U,270
+tunein-0.0.4a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tunein-0.0.4a3.dist-info/entry_points.txt,sha256=8O20QAsieAxufCAJpYO-36N03WBtUoezgyXMtRg_ryc,44
+tunein-0.0.4a3.dist-info/top_level.txt,sha256=FtWUQkdFCEWv3fbtXtJHWTwhXK3ZkI-GOTW_Fh4YdPE,26
+tunein-0.0.4a3.dist-info/RECORD,,
```

