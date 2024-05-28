# Comparing `tmp/ipyslides-3.9.4.tar.gz` & `tmp/ipyslides-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.4.tar", last modified: Mon May 27 18:32:25 2024, max compression
+gzip compressed data, was "ipyslides-3.9.5.tar", last modified: Tue May 28 02:17:38 2024, max compression
```

## Comparing `ipyslides-3.9.4.tar` & `ipyslides-3.9.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.211819 ipyslides-3.9.4/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.4/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-27 18:32:25.209809 ipyslides-3.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.097909 ipyslides-3.9.4/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.4/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-27 18:31:43.000000 ipyslides-3.9.4/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.204320 ipyslides-3.9.4/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.4/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41105 2024-05-19 04:28:44.000000 ipyslides-3.9.4/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.4/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.4/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.4/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.4/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.4/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0     7917 2024-05-27 17:33:14.000000 ipyslides-3.9.4/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.206259 ipyslides-3.9.4/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.4/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.4/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.4/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.4/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.4/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.4/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.4/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.4/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16285 2024-05-19 17:25:46.000000 ipyslides-3.9.4/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    12585 2024-05-27 18:30:09.000000 ipyslides-3.9.4/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47752 2024-05-27 17:54:56.000000 ipyslides-3.9.4/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.4/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.4/ipyslides/source.py
--rw-rw-rw-   0        0        0    29519 2024-05-19 18:02:34.000000 ipyslides-3.9.4/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.4/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.4/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.166148 ipyslides-3.9.4/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 18:32:25.211819 ipyslides-3.9.4/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.449459 ipyslides-3.9.5/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.5/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-28 02:17:38.446990 ipyslides-3.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.373288 ipyslides-3.9.5/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.5/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-28 02:12:28.000000 ipyslides-3.9.5/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.441356 ipyslides-3.9.5/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.5/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41105 2024-05-28 00:21:37.000000 ipyslides-3.9.5/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.5/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.5/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.5/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.5/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.5/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0     7917 2024-05-27 18:33:15.000000 ipyslides-3.9.5/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.444032 ipyslides-3.9.5/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.5/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1867 2024-05-28 02:16:56.000000 ipyslides-3.9.5/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.5/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2526 2024-05-28 02:12:02.000000 ipyslides-3.9.5/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.5/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.5/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.5/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.5/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16285 2024-05-28 00:22:32.000000 ipyslides-3.9.5/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    12585 2024-05-27 18:30:09.000000 ipyslides-3.9.5/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47752 2024-05-28 00:20:37.000000 ipyslides-3.9.5/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.5/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.5/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29519 2024-05-19 18:02:34.000000 ipyslides-3.9.5/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.5/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.5/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:17:38.409452 ipyslides-3.9.5/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 02:17:37.000000 ipyslides-3.9.5/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 02:17:38.449459 ipyslides-3.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.5/setup.py
```

### Comparing `ipyslides-3.9.4/LICENSE` & `ipyslides-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/PKG-INFO` & `ipyslides-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.4
+Version: 3.9.5
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.4/README.md` & `ipyslides-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.5/ipyslides/_base/_layout_css.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/_widgets.py` & `ipyslides-3.9.5/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/base.py` & `ipyslides-3.9.5/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/export_html.py` & `ipyslides-3.9.5/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/export_template.py` & `ipyslides-3.9.5/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/icons.py` & `ipyslides-3.9.5/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/intro.py` & `ipyslides-3.9.5/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.5/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/navigation.py` & `ipyslides-3.9.5/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/notes.py` & `ipyslides-3.9.5/ipyslides/_base/notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             return f"""<style>
         :root {{
             --primary-bg : {bg};
             --primary-fg : {fg};
             --secondary-bg: {bg2};
         }}
         .columns {{columns: 2 auto;}}
-        .columns > div > * {{background: {bg2};padding:0.2em;font-size:120%;border-left: 2px inset {bg};}}
-        .columns > div:first-child::before {{content:'This Slide';}}
-        .columns > div:last-child::before {{content:'Next Slide';}}
+        .columns > div > * {{background: {bg2};padding:0.2em;font-size:110%;border-left: 2px inset {bg};}}
+        .columns > div:first-child::before {{content:'This Slide';font-size:80%;font-weight:bold;}}
+        .columns > div:last-child::before {{content:'Next Slide';font-size:80%;font-weight:bold;}}
         </style>{content}"""
 
         this_notes = self.main.current.notes 
         next_slide_index = (self.main.current.index + 1) % len(self.main)
         if next_slide_index > 0: # Don't loop notes back
             next_notes = self.main[next_slide_index].notes
         else:
```

### Comparing `ipyslides-3.9.4/ipyslides/_base/screenshot.py` & `ipyslides-3.9.5/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/settings.py` & `ipyslides-3.9.5/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/slide.py` & `ipyslides-3.9.5/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/styles.py` & `ipyslides-3.9.5/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_base/widgets.py` & `ipyslides-3.9.5/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/_demo.py` & `ipyslides-3.9.5/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/core.py` & `ipyslides-3.9.5/ipyslides/core.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/formatters.py` & `ipyslides-3.9.5/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/source.py` & `ipyslides-3.9.5/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/utils.py` & `ipyslides-3.9.5/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/writer.py` & `ipyslides-3.9.5/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides/xmd.py` & `ipyslides-3.9.5/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.5/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.4
+Version: 3.9.5
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.4/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.5/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.4/setup.py` & `ipyslides-3.9.5/setup.py`

 * *Files identical despite different names*

