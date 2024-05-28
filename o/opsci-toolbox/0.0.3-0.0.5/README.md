# Comparing `tmp/opsci_toolbox-0.0.3.tar.gz` & `tmp/opsci_toolbox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsci_toolbox-0.0.3.tar", last modified: Thu May 16 09:19:14 2024, max compression
+gzip compressed data, was "opsci_toolbox-0.0.5.tar", last modified: Tue May 28 15:03:51 2024, max compression
```

## Comparing `opsci_toolbox-0.0.3.tar` & `opsci_toolbox-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/
--rw-r--r--   0 erwan     (1000) erwan     (1000)       60 2024-04-18 09:18:21.000000 opsci_toolbox-0.0.3/MANIFEST.in
--rw-r--r--   0 erwan     (1000) erwan     (1000)      198 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/PKG-INFO
--rw-r--r--   0 erwan     (1000) erwan     (1000)       41 2024-03-07 09:27:13.000000 opsci_toolbox-0.0.3/README.md
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/opsci_toolbox/
--rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-17 09:32:00.000000 opsci_toolbox-0.0.3/opsci_toolbox/__init__.py
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/opsci_toolbox/apis/
--rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-18 07:59:34.000000 opsci_toolbox-0.0.3/opsci_toolbox/apis/__init__.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    23183 2024-04-30 14:38:13.000000 opsci_toolbox-0.0.3/opsci_toolbox/apis/rapidapi_helpers.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    12263 2024-04-18 08:59:21.000000 opsci_toolbox-0.0.3/opsci_toolbox/apis/webscraping.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    13115 2024-04-17 10:11:15.000000 opsci_toolbox-0.0.3/opsci_toolbox/apis/youtube_helpers.py
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/opsci_toolbox/helpers/
--rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-17 09:40:17.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/__init__.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    26152 2024-05-16 09:16:42.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/common.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    12403 2024-03-07 09:51:25.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/cv.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    72449 2024-05-03 12:16:49.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/dataviz.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)      996 2024-04-19 08:12:25.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/dates.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)    57966 2024-05-16 08:19:01.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/nlp.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)     9450 2024-05-03 15:40:39.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/nlp_cuml.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)     8053 2024-04-23 13:22:36.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/sna.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)     4606 2024-04-30 15:31:49.000000 opsci_toolbox-0.0.3/opsci_toolbox/helpers/surreaction.py
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/opsci_toolbox/lexicons/
--rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-18 08:58:45.000000 opsci_toolbox-0.0.3/opsci_toolbox/lexicons/__init__.py
--rw-r--r--   0 erwan     (1000) erwan     (1000)     1957 2024-04-18 12:10:22.000000 opsci_toolbox-0.0.3/opsci_toolbox/lexicons/stop_words_en.csv
--rw-r--r--   0 erwan     (1000) erwan     (1000)     6776 2024-04-18 12:12:11.000000 opsci_toolbox-0.0.3/opsci_toolbox/lexicons/stop_words_fr.csv
-drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/
--rw-r--r--   0 erwan     (1000) erwan     (1000)      198 2024-05-16 09:19:14.000000 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 erwan     (1000) erwan     (1000)      786 2024-05-16 09:19:14.000000 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 erwan     (1000) erwan     (1000)        1 2024-05-16 09:19:14.000000 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 erwan     (1000) erwan     (1000)      716 2024-05-16 09:19:14.000000 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/requires.txt
--rw-r--r--   0 erwan     (1000) erwan     (1000)       14 2024-05-16 09:19:14.000000 opsci_toolbox-0.0.3/opsci_toolbox.egg-info/top_level.txt
--rw-r--r--   0 erwan     (1000) erwan     (1000)       38 2024-05-16 09:19:14.209730 opsci_toolbox-0.0.3/setup.cfg
--rw-r--r--   0 erwan     (1000) erwan     (1000)      531 2024-05-16 09:16:24.000000 opsci_toolbox-0.0.3/setup.py
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)       60 2024-04-18 09:18:21.000000 opsci_toolbox-0.0.5/MANIFEST.in
+-rw-r--r--   0 erwan     (1000) erwan     (1000)      198 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/PKG-INFO
+-rw-r--r--   0 erwan     (1000) erwan     (1000)       41 2024-03-07 09:27:13.000000 opsci_toolbox-0.0.5/README.md
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.328895 opsci_toolbox-0.0.5/opsci_toolbox/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-17 09:32:00.000000 opsci_toolbox-0.0.5/opsci_toolbox/__init__.py
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/opsci_toolbox/apis/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-18 07:59:34.000000 opsci_toolbox-0.0.5/opsci_toolbox/apis/__init__.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    23183 2024-04-30 14:38:13.000000 opsci_toolbox-0.0.5/opsci_toolbox/apis/rapidapi_helpers.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    12263 2024-04-18 08:59:21.000000 opsci_toolbox-0.0.5/opsci_toolbox/apis/webscraping.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    13115 2024-04-17 10:11:15.000000 opsci_toolbox-0.0.5/opsci_toolbox/apis/youtube_helpers.py
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/opsci_toolbox/helpers/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-17 09:40:17.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/__init__.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    26152 2024-05-16 09:16:42.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/common.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    12403 2024-03-07 09:51:25.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/cv.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    77393 2024-05-21 15:28:29.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/dataviz.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)      996 2024-04-19 08:12:25.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/dates.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)    57999 2024-05-17 21:02:06.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/nlp.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     9450 2024-05-03 15:40:39.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/nlp_cuml.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     8053 2024-04-23 13:22:36.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/sna.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     4606 2024-04-30 15:31:49.000000 opsci_toolbox-0.0.5/opsci_toolbox/helpers/surreaction.py
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/opsci_toolbox/lexicons/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)        0 2024-04-18 08:58:45.000000 opsci_toolbox-0.0.5/opsci_toolbox/lexicons/__init__.py
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     1957 2024-04-18 12:10:22.000000 opsci_toolbox-0.0.5/opsci_toolbox/lexicons/stop_words_en.csv
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     6776 2024-04-18 12:12:11.000000 opsci_toolbox-0.0.5/opsci_toolbox/lexicons/stop_words_fr.csv
+drwxr-xr-x   0 erwan     (1000) erwan     (1000)        0 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/
+-rw-r--r--   0 erwan     (1000) erwan     (1000)      198 2024-05-28 15:03:51.000000 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 erwan     (1000) erwan     (1000)      786 2024-05-28 15:03:51.000000 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 erwan     (1000) erwan     (1000)        1 2024-05-28 15:03:51.000000 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 erwan     (1000) erwan     (1000)      702 2024-05-28 15:03:51.000000 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/requires.txt
+-rw-r--r--   0 erwan     (1000) erwan     (1000)       14 2024-05-28 15:03:51.000000 opsci_toolbox-0.0.5/opsci_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 erwan     (1000) erwan     (1000)       38 2024-05-28 15:03:51.338895 opsci_toolbox-0.0.5/setup.cfg
+-rw-r--r--   0 erwan     (1000) erwan     (1000)     1638 2024-05-28 15:03:44.000000 opsci_toolbox-0.0.5/setup.py
```

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/apis/rapidapi_helpers.py` & `opsci_toolbox-0.0.5/opsci_toolbox/apis/rapidapi_helpers.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/apis/webscraping.py` & `opsci_toolbox-0.0.5/opsci_toolbox/apis/webscraping.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/apis/youtube_helpers.py` & `opsci_toolbox-0.0.5/opsci_toolbox/apis/youtube_helpers.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/common.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/common.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/cv.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/cv.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/dataviz.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/dataviz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1774,8 +1774,23 @@
                     'width': line_width, 
                     "color": line_color,
                     "dash" : dash,
                     },
                 
             }
         )
+    return fig
+
+def add_image(fig, xref = "paper", yref = "paper", x = 0, y=0, sizex = 0.08, sizey=0.08, xanchor="right", yanchor="bottom", source = "data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDc1IiBoZWlnaHQ9IjM4OCIgdmlld0JveD0iMCAwIDQ3NSAzODgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxwYXRoIGQ9Ik0xMDUuNzI3IDI5My4zOTFDMTA1LjcyNyAyNjYuNzc0IDg0LjEyOTMgMjQ1LjE3NyA1Ny42MDEzIDI0NS4xNzdDMzAuOTg0IDI0NS4xNzcgOS4yOTYgMjY2Ljc3NCA5LjI5NiAyOTMuMzkxQzkuMjk2IDMyMC4wMDkgMzAuOTg0IDM0MS42MDcgNTcuNjAxMyAzNDEuNjA3Qzg0LjEyOTMgMzQxLjYwNyAxMDUuNzI3IDMyMC4wMDkgMTA1LjcyNyAyOTMuMzkxWk0wLjg3MDY2NyAyOTMuMzkxQzAuODcwNjY3IDI2Mi4yMDMgMjYuMzI0IDIzNi43NTMgNTcuNjAxMyAyMzYuNzUzQzg4LjY5ODcgMjM2Ljc1MyAxMTQuMTUxIDI2Mi4yMDMgMTE0LjE1MSAyOTMuMzkxQzExNC4xNTEgMzI0LjU3OSA4OC42OTg3IDM1MC4wMyA1Ny42MDEzIDM1MC4wM0MyNi4zMjQgMzUwLjAzIDAuODcwNjY3IDMyNC41NzkgMC44NzA2NjcgMjkzLjM5MVoiIGZpbGw9ImJsYWNrIi8+CjxwYXRoIGQ9Ik0yMzIuNTMxIDI5My40ODFDMjMyLjUzMSAyNjMuNjM3IDIwOS4zMTkgMjQ1LjI2NSAxODYuMjg2IDI0NS4yNjVDMTY2LjU3IDI0NS4yNjUgMTQ3LjQ4MiAyNTguNjIgMTQ1LjI0MSAyODAuMDM4VjMwNi42NTZDMTQ3LjM5MyAzMjguOTcgMTY2LjM5MSAzNDEuNjk2IDE4Ni4yODYgMzQxLjY5NkMyMDkuMzE5IDM0MS42OTYgMjMyLjUzMSAzMjMuMzI1IDIzMi41MzEgMjkzLjQ4MVpNMjQwLjg2NiAyOTMuNDgxQzI0MC44NjYgMzI4LjA3NCAyMTQuNjk3IDM1MC4xMiAxODcuMTgzIDM1MC4xMkMxNjkuOTc3IDM1MC4xMiAxNTMuNTc1IDM0Mi4zMjQgMTQ1LjI0MSAzMjcuNjI1VjM4Ny40OTNIMTM2Ljk5N1YyMzkuNjJIMTQ0Ljg4M0wxNDUuMjQxIDI1Ny41NDRWMjYwLjE0MkMxNTMuNjY2IDI0NS42MjQgMTcwLjE1NSAyMzYuODQyIDE4Ny4yNzMgMjM2Ljg0MkMyMTQuNjA3IDIzNi44NDIgMjQwLjg2NiAyNTguODg4IDI0MC44NjYgMjkzLjQ4MVoiIGZpbGw9ImJsYWNrIi8+CjxwYXRoIGQ9Ik0yNTUuNjQyIDMyOC40MzNMMjYwLjc1MSAzMjIuNzg4QzI2OC4xMDEgMzM1LjUxMyAyODEuMDk1IDM0MS45NjUgMjk0LjE3OCAzNDEuOTY1QzMwOC41MTggMzQxLjk2NSAzMjMuMTI2IDMzMy42MyAzMjMuMTI2IDMxOS41NjFDMzIzLjEyNiAzMDUuNDkgMzA0LjkzNCAyOTkuNjY1IDI4OS43ODcgMjkzLjc0OUMyODAuMzc4IDI4OS45ODYgMjYwLjc1MSAyODMuMzUzIDI2MC43NTEgMjY0LjYyNEMyNjAuNzUxIDI0OS41NjggMjc0LjI4MyAyMzYuNjYyIDI5NC4yNjkgMjM2LjY2MkMzMDkuODYyIDIzNi42NjIgMzIzLjEyNiAyNDUuMzU0IDMyNy41MTggMjU2LjM3OEwzMjEuNjAzIDI2MS4wMzhDMzE2LjMxNSAyNDkuODM3IDMwNC4yMTcgMjQ0LjkwNiAyOTQuMDAxIDI0NC45MDZDMjc5LjEyMiAyNDQuOTA2IDI2OS4xNzQgMjU0LjEzNyAyNjkuMTc0IDI2NC4yNjVDMjY5LjE3NCAyNzcuNDQgMjg0LjIzMSAyODIuOTA1IDI5OS4xMDkgMjg4LjU1MkMzMTEuMDI3IDI5My4yMTIgMzMxLjU1MSAzMDAuNjUgMzMxLjU1MSAzMTkuMDIyQzMzMS41NTEgMzM4LjExMiAzMTMuMjY5IDM1MC4yMSAyOTQuMDAxIDM1MC4yMUMyNzYuNzAzIDM1MC4yMSAyNjEuODI3IDM0MC40NDIgMjU1LjY0MiAzMjguNDMzWiIgZmlsbD0iYmxhY2siLz4KPHBhdGggZD0iTTM0Ni43OCAyOTMuMzkxQzM0Ni43OCAyNTguNTMgMzc1LjAxMSAyMzYuMDM0IDQwMy4yNDEgMjM2LjAzNEM0MTUuNzg4IDIzNi4wMzQgNDMwLjMwNyAyNDAuNTE3IDQzOS45ODUgMjQ4LjU4Mkw0MzUuMzI1IDI1NS40ODJDNDI4Ljc4MyAyNDkuMjk5IDQxNS41MiAyNDQuNDU5IDQwMy4zMzEgMjQ0LjQ1OUMzNzkuMTMzIDI0NC40NTkgMzU1LjIwNCAyNjMuNDU5IDM1NS4yMDQgMjkzLjM5MUMzNTUuMjA0IDMyMy41OTMgMzc5LjQwMyAzNDIuMzIzIDQwMy4yNDEgMzQyLjMyM0M0MTUuNjA4IDM0Mi4zMjMgNDI5LjIzMSAzMzcuMTI2IDQzNi4yMjEgMzMwLjQ5NEw0NDEuMzI5IDMzNy4xMjZDNDMxLjQ3MiAzNDYuMTc4IDQxNi40MTYgMzUwLjc0OSA0MDMuNDIgMzUwLjc0OUMzNzUuMSAzNTAuNzQ5IDM0Ni43OCAzMjguNDMzIDM0Ni43OCAyOTMuMzkxWiIgZmlsbD0iYmxhY2siLz4KPHBhdGggZD0iTTQ2My42MzcgMjM5LjYxOUg0NzIuMDYxVjM0Ny4xNjNINDYzLjYzN1YyMzkuNjE5Wk00NjEuMTI4IDIxMi40NjRDNDYxLjEyOCAyMDguNzAxIDQ2NC4wODUgMjA1Ljc0MyA0NjcuODQ5IDIwNS43NDNDNDcxLjUyNCAyMDUuNzQzIDQ3NC41NzEgMjA4LjcwMSA0NzQuNTcxIDIxMi40NjRDNDc0LjU3MSAyMTYuMjI4IDQ3MS41MjQgMjE5LjE4NSA0NjcuODQ5IDIxOS4xODVDNDY0LjA4NSAyMTkuMTg1IDQ2MS4xMjggMjE2LjIyOCA0NjEuMTI4IDIxMi40NjRaIiBmaWxsPSJibGFjayIvPgo8cGF0aCBkPSJNMjE3Ljg1MyAzMS4zOTE0TDIzNy43MjEgNTEuMjU4TDI1Ny41ODggMzEuMzkxNEwyMzcuNzIxIDExLjUyNDdMMjE3Ljg1MyAzMS4zOTE0Wk0yMzcuNzIxIDYyLjU3MjdMMjA2LjU0IDMxLjM5MTRMMjM3LjcyMSAwLjIxMDAxNkwyNjguOTAxIDMxLjM5MTRMMjM3LjcyMSA2Mi41NzI3Wk0xNTQuMTAxIDU5Ljc1OTRMMTYxLjQzOSA4Ni45NjQ3TDE4OC42NiA3OS42MjJMMTgxLjMyMyA1Mi41OTU0TDE1NC4xMDEgNTkuNzU5NFpNMTU1Ljc5NyA5Ni43NzE0TDE0NC4yOCA1NC4wNzE0TDE4Ni45NjMgNDIuODM5NEwxOTguNDgxIDg1LjI1OEwxNTUuNzk3IDk2Ljc3MTRaTTI4Ni43ODEgNzkuNjIyTDMxNC4wMDMgODYuOTY0N0wzMjEuMzQxIDU5Ljc1OTRMMjk0LjEyIDUyLjU5NTRMMjg2Ljc4MSA3OS42MjJaTTMxOS42NDMgOTYuNzcxNEwyNzYuOTYxIDg1LjI1OEwyODguNDc5IDQyLjgzOTRMMzMxLjE2MiA1NC4wNzE0TDMxOS42NDMgOTYuNzcxNFpNMTU0LjEwMSAxNTYuMTY5TDE4MS4zMjMgMTYzLjMzM0wxODguNjYgMTM2LjMwN0wxNjEuNDM5IDEyOC45NjVMMTU0LjEwMSAxNTYuMTY5Wk0xODYuOTYzIDE3My4wODlMMTQ0LjI4IDE2MS44NTdMMTU1Ljc5NyAxMTkuMTU3TDE5OC40ODEgMTMwLjY3TDE4Ni45NjMgMTczLjA4OVpNMjg2Ljc3NSAxMzYuMzA5TDI5NC4xMiAxNjMuNTM3TDMyMS4zNDggMTU2LjE5M0wzMTQuMDAzIDEyOC45NjVMMjg2Ljc3NSAxMzYuMzA5Wk0yODguNDc5IDE3My4zNDVMMjc2Ljk2NyAxMzAuNjY5TDMxOS42NDMgMTE5LjE1N0wzMzEuMTU1IDE2MS44MzRMMjg4LjQ3OSAxNzMuMzQ1Wk0yMTcuODUzIDE4NC41MzdMMjM3LjcyMSAyMDQuNDA1TDI1Ny41ODggMTg0LjUzN0wyMzcuNzIxIDE2NC42N0wyMTcuODUzIDE4NC41MzdaTTIzNy43MjEgMjE1LjcxOEwyMDYuNTQgMTg0LjUzN0wyMzcuNzIxIDE1My4zNTdMMjY4LjkwMSAxODQuNTM3TDIzNy43MjEgMjE1LjcxOFoiIGZpbGw9ImJsYWNrIi8+Cjwvc3ZnPgo="):
+    fig.add_layout_image(
+    dict(
+        source=source,
+        xref=xref, 
+        yref=yref,
+        x=x, y=y,
+        sizex=sizex, 
+        sizey=sizey,
+        xanchor=xanchor,
+        yanchor=yanchor
+        )
+    )
     return fig
```

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/dates.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/dates.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/nlp.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1361,11 +1361,11 @@
     """ Calculate sentiment of a text. `return_type` can be 'label', 'score' or 'proba' """
     file_path= os.path.join(dir_json , str(filename)+'.json')
     if not os.path.exists(file_path):
         with torch.no_grad():
             inputs = tokenizer(text, return_tensors='pt', truncation=True, padding=True).to(model.device)
             proba = torch.sigmoid(model(**inputs).logits).cpu().numpy()[0]
             label = model.config.id2label[proba.argmax()]
-            results = {"label":label, "score" : proba.max(), col_text : text}
+            results = {"label":label, "score" : float(proba.max()), col_text : text}
+            print(results)
             write_json(results, dir_json , str(filename))
     return results
-
```

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/nlp_cuml.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/nlp_cuml.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/sna.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/sna.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/helpers/surreaction.py` & `opsci_toolbox-0.0.5/opsci_toolbox/helpers/surreaction.py`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/lexicons/stop_words_en.csv` & `opsci_toolbox-0.0.5/opsci_toolbox/lexicons/stop_words_en.csv`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox/lexicons/stop_words_fr.csv` & `opsci_toolbox-0.0.5/opsci_toolbox/lexicons/stop_words_fr.csv`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox.egg-info/SOURCES.txt` & `opsci_toolbox-0.0.5/opsci_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsci_toolbox-0.0.3/opsci_toolbox.egg-info/requires.txt` & `opsci_toolbox-0.0.5/opsci_toolbox.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-Pillow==10.3.0
-Pillow>=9.0.1
+Pillow<11.0.0,>=9.0.1
 Requests==2.31.0
 beautifulsoup4==4.10.0
 chart_studio==1.1.0
-cuml
 eldar==0.0.8
 emoji==2.10.1
 google_api_python_client==2.122.0
-gspread==6.1.0
+gspread==6.1.1
 hdbscan==0.8.33
 jusText==3.0.0
-langchain==0.1.16
-matplotlib==3.8.3
+langchain==0.1.20
 matplotlib>=3.5.1
 networkx==3.2.1
 nltk==3.8.1
-numpy==1.24.4
-numpy>=1.21.5
+numpy<1.25.0,>=1.21.5
 opencv_python_headless==4.9.0.80
 pandas==1.5.3
 plotly==5.19.0
-protobuf
+protobuf==5.26.1
 pyarrow==14.0.2
 python_louvain==0.16
 scikit_learn==1.4.1.post1
-scipy
+scipy<2.0.0,>=1.8.0
 sentence_transformers==2.5.1
 setuptools==59.6.0
 spacy==3.7.4
 spacy_language_detection==0.2.1
 spacymoji==3.1.0
-supervision==0.19.0
+supervision==0.20.0
 textacy==0.13.0
 torch==2.0.1
 tqdm==4.66.2
 trafilatura==1.7.0
 transformers==4.38.2
 umap_learn==0.5.5
 urlextract==1.9.0
```

