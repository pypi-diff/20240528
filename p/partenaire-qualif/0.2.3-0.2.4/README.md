# Comparing `tmp/partenaire-qualif-0.2.3.tar.gz` & `tmp/partenaire-qualif-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.2.3.tar", last modified: Tue May 14 13:56:18 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.2.4.tar", last modified: Tue May 28 13:54:41 2024, max compression
```

## Comparing `partenaire-qualif-0.2.3.tar` & `partenaire-qualif-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       56 2024-05-14 11:45:10.000000 partenaire-qualif-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3112 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2589 2024-05-13 15:50:34.000000 partenaire-qualif-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-14 13:56:18.000000 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-14 13:56:18.000000 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:56:18.000000 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-14 13:56:18.000000 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 13:56:18.000000 partenaire-qualif-0.2.3/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/qualif/
--rw-rw-rw-   0        0        0       76 2024-05-10 17:15:12.000000 partenaire-qualif-0.2.3/qualif/__init__.py
--rw-rw-rw-   0        0        0     9664 2024-05-14 11:41:05.000000 partenaire-qualif-0.2.3/qualif/qualif.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/qualif/templates/
--rw-rw-rw-   0        0        0        0 2024-05-13 15:47:06.000000 partenaire-qualif-0.2.3/qualif/templates/__init__.py
--rw-rw-rw-   0        0        0     2426 2024-05-10 17:08:42.000000 partenaire-qualif-0.2.3/qualif/templates/prompt_find_website_template.txt
--rw-rw-rw-   0        0        0     1987 2024-05-10 17:12:26.000000 partenaire-qualif-0.2.3/qualif/templates/prompt_qualification_template.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 13:56:18.224129 partenaire-qualif-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-05-14 13:56:17.000000 partenaire-qualif-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:54:41.163800 partenaire-qualif-0.2.4/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       56 2024-05-14 11:45:10.000000 partenaire-qualif-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3112 2024-05-28 13:54:41.163800 partenaire-qualif-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2589 2024-05-13 15:50:34.000000 partenaire-qualif-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 13:54:41.154605 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     3112 2024-05-28 13:54:41.000000 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-28 13:54:41.000000 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:54:41.000000 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-28 13:54:41.000000 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 13:54:41.000000 partenaire-qualif-0.2.4/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 13:54:41.157605 partenaire-qualif-0.2.4/qualif/
+-rw-rw-rw-   0        0        0       76 2024-05-10 17:15:12.000000 partenaire-qualif-0.2.4/qualif/__init__.py
+-rw-rw-rw-   0        0        0     9694 2024-05-28 13:40:07.000000 partenaire-qualif-0.2.4/qualif/qualif.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:54:41.161717 partenaire-qualif-0.2.4/qualif/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-13 15:47:06.000000 partenaire-qualif-0.2.4/qualif/templates/__init__.py
+-rw-rw-rw-   0        0        0     2426 2024-05-10 17:08:42.000000 partenaire-qualif-0.2.4/qualif/templates/prompt_find_website_template.txt
+-rw-rw-rw-   0        0        0     1987 2024-05-10 17:12:26.000000 partenaire-qualif-0.2.4/qualif/templates/prompt_qualification_template.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:54:41.164803 partenaire-qualif-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-05-28 13:54:39.000000 partenaire-qualif-0.2.4/setup.py
```

### Comparing `partenaire-qualif-0.2.3/LICENSE` & `partenaire-qualif-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.3/PKG-INFO` & `partenaire-qualif-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire_qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.2.3/README.md` & `partenaire-qualif-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.3/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.2.4/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire_qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.2.3/qualif/qualif.py` & `partenaire-qualif-0.2.4/qualif/qualif.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
         headers = {
             'Ocp-Apim-Subscription-Key': self.browsing_key
         }
 
         params = {
             'q': query,
             'count': top_k,
-            'responseFilter': 'Webpages'
+            'responseFilter': 'Webpages',
+            'mkt': 'fr-FR',
         }
 
         response = httpx.get(web_search_endpoint, headers=headers, params=params)
         for webpage in response.json()['webPages']['value']:
             webpage_entry = {}
             webpage_entry["url"] = webpage['displayUrl']
             webpage_entry["snippet"] = webpage['snippet']
```

### Comparing `partenaire-qualif-0.2.3/qualif/templates/prompt_find_website_template.txt` & `partenaire-qualif-0.2.4/qualif/templates/prompt_find_website_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.3/qualif/templates/prompt_qualification_template.txt` & `partenaire-qualif-0.2.4/qualif/templates/prompt_qualification_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.2.3/setup.py` & `partenaire-qualif-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version='0.2.3',
+    version='0.2.4',
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire_qualif.git",
     packages=setuptools.find_packages(exclude=("test",)),
```

