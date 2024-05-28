# Comparing `tmp/aurora_ssg-0.0.2.tar.gz` & `tmp/aurora_ssg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora_ssg-0.0.2.tar", last modified: Tue May 28 10:09:32 2024, max compression
+gzip compressed data, was "aurora_ssg-0.0.3.tar", last modified: Tue May 28 10:23:34 2024, max compression
```

## Comparing `aurora_ssg-0.0.2.tar` & `aurora_ssg-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.647052 aurora_ssg-0.0.2/
--rw-r--r--   0 james      (501) staff       (20)      544 2024-05-28 10:09:29.000000 aurora_ssg-0.0.2/CHANGELOG.md
--rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:09:32.646730 aurora_ssg-0.0.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5787 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.643949 aurora_ssg-0.0.2/aurora/
--rw-r--r--   0 james      (501) staff       (20)       22 2024-05-28 10:07:42.000000 aurora_ssg-0.0.2/aurora/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1250 2024-05-28 09:09:39.000000 aurora_ssg-0.0.2/aurora/cli.py
--rw-r--r--   0 james      (501) staff       (20)      728 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/aurora/date_helpers.py
--rw-r--r--   0 james      (501) staff       (20)    19826 2024-05-28 09:57:26.000000 aurora_ssg-0.0.2/aurora/graph.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.645864 aurora_ssg-0.0.2/aurora_ssg.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      328 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       43 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      153 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        7 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)   923054 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/banner.png
--rw-r--r--   0 james      (501) staff       (20)       38 2024-05-28 10:09:32.647122 aurora_ssg-0.0.2/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1563 2024-05-28 09:57:24.000000 aurora_ssg-0.0.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:23:34.378456 aurora_ssg-0.0.3/
+-rw-r--r--   0 james      (501) staff       (20)     2238 2024-05-28 09:57:50.000000 aurora_ssg-0.0.3/.gitignore
+-rw-r--r--   0 james      (501) staff       (20)      544 2024-05-28 10:09:29.000000 aurora_ssg-0.0.3/CHANGELOG.md
+-rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-28 08:11:52.000000 aurora_ssg-0.0.3/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:23:34.378125 aurora_ssg-0.0.3/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     5787 2024-05-28 08:11:52.000000 aurora_ssg-0.0.3/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:23:34.375388 aurora_ssg-0.0.3/aurora/
+-rw-r--r--   0 james      (501) staff       (20)       22 2024-05-28 10:23:31.000000 aurora_ssg-0.0.3/aurora/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1250 2024-05-28 09:09:39.000000 aurora_ssg-0.0.3/aurora/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      728 2024-05-28 08:11:52.000000 aurora_ssg-0.0.3/aurora/date_helpers.py
+-rw-r--r--   0 james      (501) staff       (20)    20074 2024-05-28 10:23:01.000000 aurora_ssg-0.0.3/aurora/graph.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:23:34.377229 aurora_ssg-0.0.3/aurora_ssg.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      339 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       43 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      153 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        7 2024-05-28 10:23:34.000000 aurora_ssg-0.0.3/aurora_ssg.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)   923054 2024-05-28 08:11:52.000000 aurora_ssg-0.0.3/banner.png
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-28 10:23:34.378521 aurora_ssg-0.0.3/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1563 2024-05-28 09:57:24.000000 aurora_ssg-0.0.3/setup.py
```

### Comparing `aurora_ssg-0.0.2/CHANGELOG.md` & `aurora_ssg-0.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/LICENSE` & `aurora_ssg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/PKG-INFO` & `aurora_ssg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-ssg
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fast static site generator implemented in Python.
 Home-page: https://github.com/capjamesg/aurora
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `aurora_ssg-0.0.2/README.md` & `aurora_ssg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/aurora/cli.py` & `aurora_ssg-0.0.3/aurora/cli.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/aurora/date_helpers.py` & `aurora_ssg-0.0.3/aurora/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/aurora/graph.py` & `aurora_ssg-0.0.3/aurora/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,18 @@
 
             parsed_content["page"]["date"] = parsed_content["post"]["date"]
 
             if "description" not in parsed_content:
                 parsed_content["description"] = pyromark.markdown(
                     parsed_content.content.split("\n")[0]
                 )
+            date_slug = date_slug.replace("-", "/")
+            slug_without_date = re.sub(r"\d{4}-\d{2}-\d{2}-", "", slug)
+
+            parsed_content["url"] = f"{BASE_URL}/{date_slug}/{slug_without_date.replace('.html', '').replace('.md', '')}/"
 
     if "layout" in parsed_content:
         dependencies.add(
             f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/{parsed_content['layout']}.html"
         )
         if not state.get(parsed_content["layout"] + "s"):
             state[parsed_content["layout"] + "s"] = []
```

### Comparing `aurora_ssg-0.0.2/aurora_ssg.egg-info/PKG-INFO` & `aurora_ssg-0.0.3/aurora_ssg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-ssg
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fast static site generator implemented in Python.
 Home-page: https://github.com/capjamesg/aurora
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `aurora_ssg-0.0.2/banner.png` & `aurora_ssg-0.0.3/banner.png`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.2/setup.py` & `aurora_ssg-0.0.3/setup.py`

 * *Files identical despite different names*

