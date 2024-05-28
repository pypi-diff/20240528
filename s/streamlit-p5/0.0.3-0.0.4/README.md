# Comparing `tmp/streamlit_p5-0.0.3.tar.gz` & `tmp/streamlit_p5-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_p5-0.0.3.tar", last modified: Sun May 26 23:25:13 2024, max compression
+gzip compressed data, was "streamlit_p5-0.0.4.tar", last modified: Tue May 28 11:05:53 2024, max compression
```

## Comparing `streamlit_p5-0.0.3.tar` & `streamlit_p5-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 23:25:13.045836 streamlit_p5-0.0.3/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       35 2024-05-25 08:26:39.000000 streamlit_p5-0.0.3/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2283 2024-05-26 23:25:13.041836 streamlit_p5-0.0.3/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1665 2024-05-26 23:24:20.000000 streamlit_p5-0.0.3/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-26 23:25:13.045836 streamlit_p5-0.0.3/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      897 2024-05-26 23:23:42.000000 streamlit_p5-0.0.3/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 23:25:13.041836 streamlit_p5-0.0.3/streamlit_p5/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1317 2024-05-26 23:12:41.000000 streamlit_p5-0.0.3/streamlit_p5/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 23:25:13.041836 streamlit_p5-0.0.3/streamlit_p5/p5/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2112 2024-05-26 23:12:26.000000 streamlit_p5-0.0.3/streamlit_p5/p5/index.html
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)  1034532 2024-05-24 21:32:33.000000 streamlit_p5-0.0.3/streamlit_p5/p5/p5.min.js
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-26 23:25:13.041836 streamlit_p5-0.0.3/streamlit_p5.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2283 2024-05-26 23:25:12.000000 streamlit_p5-0.0.3/streamlit_p5.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      287 2024-05-26 23:25:13.000000 streamlit_p5-0.0.3/streamlit_p5.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-26 23:25:12.000000 streamlit_p5-0.0.3/streamlit_p5.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      140 2024-05-26 23:25:12.000000 streamlit_p5-0.0.3/streamlit_p5.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2024-05-26 23:25:12.000000 streamlit_p5-0.0.3/streamlit_p5.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       35 2024-05-25 08:26:39.000000 streamlit_p5-0.0.4/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2657 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1828 2024-05-28 11:05:42.000000 streamlit_p5-0.0.4/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1108 2024-05-28 11:01:04.000000 streamlit_p5-0.0.4/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/streamlit_p5/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1317 2024-05-26 23:12:41.000000 streamlit_p5-0.0.4/streamlit_p5/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/streamlit_p5/p5/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2112 2024-05-26 23:12:26.000000 streamlit_p5-0.0.4/streamlit_p5/p5/index.html
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)  1034532 2024-05-24 21:32:33.000000 streamlit_p5-0.0.4/streamlit_p5/p5/p5.min.js
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-28 11:05:53.395320 streamlit_p5-0.0.4/streamlit_p5.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2657 2024-05-28 11:05:53.000000 streamlit_p5-0.0.4/streamlit_p5.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      287 2024-05-28 11:05:53.000000 streamlit_p5-0.0.4/streamlit_p5.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-28 11:05:53.000000 streamlit_p5-0.0.4/streamlit_p5.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      140 2024-05-28 11:05:53.000000 streamlit_p5-0.0.4/streamlit_p5.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2024-05-28 11:05:53.000000 streamlit_p5-0.0.4/streamlit_p5.egg-info/top_level.txt
```

### Comparing `streamlit_p5-0.0.3/PKG-INFO` & `streamlit_p5-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: streamlit_p5
-Version: 0.0.3
-Summary: Embed the power of Processing.org in your Streamlit app
-Home-page: 
+Version: 0.0.4
+Summary: Bring the power of ProcessingJS (aka P5) to Streamlit. This module allows you to create Processing sketches, interact with those sketches using the mouse and keyboard, and share data between your Processing Sketch and Stremalit.
+Home-page: https://streamlit-p5-examples.fly.dev/
 Author: Neal Riley
 Author-email: neal.riley@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
@@ -14,15 +14,17 @@
 Requires-Dist: playwright==1.39.0; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
 
 # streamlit_p5
 
-Embed your processing sketches in Streamlit!
+Embed your processing sketches in Streamlit! Check out the demo [here](https://streamlit-p5-examples.fly.dev/)
+
+You can find the source code at: [https://github.com/salable/streamlit-p5](https://github.com/salable/streamlit-p5)
 
 ## Installation instructions
 
 ```sh
 pip install streamlit streamlit_p5
 ```
 
@@ -98,9 +100,8 @@
 }, width=700, height=500)
 ```
 
 Wanna build this from source? just run: 
 
 ```sh
 python setup.py sdist bdist_wheel && twine upload dist/*
-twine upload dist/*
 ```
```

### Comparing `streamlit_p5-0.0.3/README.md` & `streamlit_p5-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # streamlit_p5
 
-Embed your processing sketches in Streamlit!
+Embed your processing sketches in Streamlit! Check out the demo [here](https://streamlit-p5-examples.fly.dev/)
+
+You can find the source code at: [https://github.com/salable/streamlit-p5](https://github.com/salable/streamlit-p5)
 
 ## Installation instructions
 
 ```sh
 pip install streamlit streamlit_p5
 ```
 
@@ -80,9 +82,8 @@
 }, width=700, height=500)
 ```
 
 Wanna build this from source? just run: 
 
 ```sh
 python setup.py sdist bdist_wheel && twine upload dist/*
-twine upload dist/*
 ```
```

### Comparing `streamlit_p5-0.0.3/streamlit_p5/__init__.py` & `streamlit_p5-0.0.4/streamlit_p5/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.3/streamlit_p5/p5/index.html` & `streamlit_p5-0.0.4/streamlit_p5/p5/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.3/streamlit_p5/p5/p5.min.js` & `streamlit_p5-0.0.4/streamlit_p5/p5/p5.min.js`

 * *Files identical despite different names*

### Comparing `streamlit_p5-0.0.3/streamlit_p5.egg-info/PKG-INFO` & `streamlit_p5-0.0.4/streamlit_p5.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: streamlit_p5
-Version: 0.0.3
-Summary: Embed the power of Processing.org in your Streamlit app
-Home-page: 
+Version: 0.0.4
+Summary: Bring the power of ProcessingJS (aka P5) to Streamlit. This module allows you to create Processing sketches, interact with those sketches using the mouse and keyboard, and share data between your Processing Sketch and Stremalit.
+Home-page: https://streamlit-p5-examples.fly.dev/
 Author: Neal Riley
 Author-email: neal.riley@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
@@ -14,15 +14,17 @@
 Requires-Dist: playwright==1.39.0; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
 
 # streamlit_p5
 
-Embed your processing sketches in Streamlit!
+Embed your processing sketches in Streamlit! Check out the demo [here](https://streamlit-p5-examples.fly.dev/)
+
+You can find the source code at: [https://github.com/salable/streamlit-p5](https://github.com/salable/streamlit-p5)
 
 ## Installation instructions
 
 ```sh
 pip install streamlit streamlit_p5
 ```
 
@@ -98,9 +100,8 @@
 }, width=700, height=500)
 ```
 
 Wanna build this from source? just run: 
 
 ```sh
 python setup.py sdist bdist_wheel && twine upload dist/*
-twine upload dist/*
 ```
```

