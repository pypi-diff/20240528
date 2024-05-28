# Comparing `tmp/kahi_impactu_utils-0.0.9.tar.gz` & `tmp/kahi_impactu_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kahi_impactu_utils-0.0.9.tar", last modified: Tue Apr 23 15:20:09 2024, max compression
+gzip compressed data, was "kahi_impactu_utils-0.1.0.tar", last modified: Tue May 28 01:49:55 2024, max compression
```

## Comparing `kahi_impactu_utils-0.0.9.tar` & `kahi_impactu_utils-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 15:20:09.000000 kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/kahi_impactu_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/String.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/kahi_impactu_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:20:09.910932 kahi_impactu_utils-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-23 15:19:58.000000 kahi_impactu_utils-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:49:55.015861 kahi_impactu_utils-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:49:55.015861 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 01:49:54.000000 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 01:49:54.000000 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:49:54.000000 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 01:49:54.000000 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 01:49:54.000000 kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 01:49:55.015861 kahi_impactu_utils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:49:55.015861 kahi_impactu_utils-0.1.0/kahi_impactu_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/kahi_impactu_utils/String.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/kahi_impactu_utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/kahi_impactu_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/kahi_impactu_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:49:55.015861 kahi_impactu_utils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-28 01:49:46.000000 kahi_impactu_utils-0.1.0/setup.py
```

### Comparing `kahi_impactu_utils-0.0.9/Kahi_impactu_utils.egg-info/PKG-INFO` & `kahi_impactu_utils-0.1.0/Kahi_impactu_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Kahi_impactu_utils
-Version: 0.0.9
+Version: 0.1.0
 Summary: Utils for Kahi Impactu project.
 Home-page: https://github.com/colav/Kahi_impactu_utils
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langid==1.1.6
-Requires-Dist: lingua-language-detector==1.3.3
-Requires-Dist: pycld2==0.41
-Requires-Dist: langdetect==1.0.7
-Requires-Dist: fastspell==0.8.0
-Requires-Dist: iso639==0.1.4
+Requires-Dist: langid~=1.1.6
+Requires-Dist: lingua-language-detector~=1.3.3
+Requires-Dist: pycld2~=0.41
+Requires-Dist: langdetect~=1.0.7
+Requires-Dist: fastspell~=0.8.0
+Requires-Dist: iso639~=0.1.4
 Requires-Dist: unidecode
 Requires-Dist: titlecase
 
 
 <center><img src="https://raw.githubusercontent.com/colav/colav.github.io/master/img/Logo.png"/></center>
 
 # Kahi impactu utils
```

### Comparing `kahi_impactu_utils-0.0.9/LICENSE` & `kahi_impactu_utils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kahi_impactu_utils-0.0.9/PKG-INFO` & `kahi_impactu_utils-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Kahi_impactu_utils
-Version: 0.0.9
+Version: 0.1.0
 Summary: Utils for Kahi Impactu project.
 Home-page: https://github.com/colav/Kahi_impactu_utils
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langid==1.1.6
-Requires-Dist: lingua-language-detector==1.3.3
-Requires-Dist: pycld2==0.41
-Requires-Dist: langdetect==1.0.7
-Requires-Dist: fastspell==0.8.0
-Requires-Dist: iso639==0.1.4
+Requires-Dist: langid~=1.1.6
+Requires-Dist: lingua-language-detector~=1.3.3
+Requires-Dist: pycld2~=0.41
+Requires-Dist: langdetect~=1.0.7
+Requires-Dist: fastspell~=0.8.0
+Requires-Dist: iso639~=0.1.4
 Requires-Dist: unidecode
 Requires-Dist: titlecase
 
 
 <center><img src="https://raw.githubusercontent.com/colav/colav.github.io/master/img/Logo.png"/></center>
 
 # Kahi impactu utils
```

### Comparing `kahi_impactu_utils-0.0.9/README.md` & `kahi_impactu_utils-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kahi_impactu_utils-0.0.9/kahi_impactu_utils/String.py` & `kahi_impactu_utils-0.1.0/kahi_impactu_utils/String.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from titlecase import titlecase
 from bs4 import BeautifulSoup
-from re import sub
+from re import sub, findall
+import html
 
 
 def abbreviations(word, **kwargs):
     """
     Function to handle abbreviations in the titlecase function
 
     Parameters:
@@ -60,7 +61,31 @@
     str
         The parsed title.
     """
     if [tag.name for tag in BeautifulSoup(string, 'lxml').find_all() if tag.name.find('math') > -1]:
         string = sub('\n', ' ', BeautifulSoup(
             sub(r"([a-zA-Z])<", r"\1 <", string), 'lxml').text.strip())
     return string
+
+
+def parse_html(string):
+    """
+    Function to parse the string of a html element,
+    only if html code is found in the string.
+
+    Parameters:
+    -----------
+    string : str
+        The string to be parsed.
+
+    Returns:
+    --------
+    str
+        The parsed title.
+    """
+    if "&lt;" in string:
+        string = html.unescape(string)
+    found = findall(r'<[^>]+>', string)
+    if found:
+        soup = BeautifulSoup(string, 'html.parser')
+        return soup.get_text()
+    return string
```

### Comparing `kahi_impactu_utils-0.0.9/kahi_impactu_utils/Utils.py` & `kahi_impactu_utils-0.1.0/kahi_impactu_utils/Utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,14 +257,20 @@
         return "researchgate"
     if "linkedin" in url:
         return "linkedin"
     if "scholar.google" in url:
         return "scholar"
     if "scopus" in url:
         return "scopus"
+    if "publons" in url:
+        return "wos"
+    if "webofscience" in url:
+        return "wos"
+    if "ssrn" in url:
+        return "ssrn"
     return None
 
 
 def parse_scholar_id_from_url(value):
     """
     Parse the google scholar id from the url,
     the id is the value of the user parameter.
@@ -280,15 +286,15 @@
         The google scholar id
     """
     value = value.replace("authuser", "")
     value = findall(r"user=([^&]{1,12})", value)
     if value:
         value = value[-1]
         if len(value) == 12:
-            return value
+            return "https://scholar.google.com/citations?user=" + value
     return None
 
 
 def parse_researchgate_id_from_url(value):
     """
     Function to parse the researchgate id from the url,
     it is the value of the profile path in the url
@@ -302,15 +308,15 @@
     --------
     str
         The researchgate id
     """
     value = search(
         r"https://www\.researchgate\.net/profile/([^\s/?&]+)", value)
     if value:
-        return value.group(1)
+        return "https://www.researchgate.net/profile/" + value.group(1)
     return None
 
 
 def parse_linkedin_id_from_url(value):
     """
     Function to parse the linkedin id from the url,
     it is the value of the "in" parameter in the url.
@@ -323,15 +329,15 @@
     Returns:
     --------
     str
         The linkedin id
     """
     value = search(r"linkedin\.com/in/([^/?&]+)", value)
     if value:
-        return value.group(1)
+        return "https://www.linkedin.com/in/" + value.group(1)
     return None
 
 
 def parse_orcid_id_from_url(value):
     """
     Function to parse the orcid id from the url,
     it is the value of the orcid parameter in the url.
@@ -343,20 +349,19 @@
         The url of the orcid profile
 
     Returns:
     --------
     str
         The orcid id
     """
-    value = value.replace("-", "")
-    value = value.replace("_", "")
+    value = value.replace("-", "").replace("_", "").replace(" ", "")
     value = search(
         r"(?:ORCID\s?)?([a-zA-Z0-9]{4})-?([a-zA-Z0-9]{4})-?([a-zA-Z0-9]{4})-?([a-zA-Z0-9]{4})", value)
     if value:
-        return "-".join(value.groups())
+        return "https://orcid.org/" + "-".join(value.groups())
     return None
 
 
 def parse_scopus_id_from_url(value):
     """
     Function to parse the scopus id from the url,
     it is the value of the authorID or authorId parameter in the url.
@@ -370,22 +375,67 @@
         The url of the scopus profile
 
     Returns:
     --------
     str
         The scopus id
     """
-
-    ##
     value = search(r"(?:authorId=|authorID=)(\d+)", value)
     if value:
         return f"https://www.scopus.com/authid/detail.uri?authorId={value.group(1)}"
     return None
 
 
+def parse_ssrn_id_from_url(value):
+    """
+    Function to parse the ssrn id from the url,
+    it is the value of the profile path in the url
+
+    Parameters:
+    ----------
+    value: str
+        The url of the web of ssrn profile
+
+    Returns:
+    --------
+    str
+        The ssrn id
+    """
+    value = search(r'(?:per_id|partid|partID|author)=([\d]+)', value)
+    if value:
+        return "https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=" + value.group(1)
+    return None
+
+
+def parse_wos_id_from_url(value):
+    """
+    Function to parse the wos id from the url,
+    it is the value of the profile path in the url
+
+    Parameters:
+    ----------
+    value: str
+        The url of the web of science profile
+
+    Returns:
+    --------
+    str
+        The wos id
+    """
+    if "publons" in value:
+        _value = search(r'/(\d+)/', value)
+        if _value:
+            return _value.group(1)
+    if "webofscience" in value:
+        _value = search(r'/(\d+)', value)
+        if _value:
+            return "https://www.webofscience.com/wos/author/record/" + _value.group(1)
+    return None
+
+
 def get_id_from_url(value):
     """
     Function to get the id from the url, it uses the get_id_type function to get the type of the id
     and then uses the corresponding function to parse the id from the url.
     Returns the ids without url encoding, without spaces and without url path.
 
     Parameters:
@@ -406,14 +456,18 @@
         return parse_researchgate_id_from_url(value)
     if get_id_type_from_url(value) == "linkedin":
         return parse_linkedin_id_from_url(value)
     if get_id_type_from_url(value) == "orcid":
         return parse_orcid_id_from_url(value)
     if get_id_type_from_url(value) == "scopus":
         return parse_scopus_id_from_url(value)
+    if get_id_type_from_url(value) == "wos":
+        return parse_wos_id_from_url(value)
+    if get_id_type_from_url(value) == "ssrn":
+        return parse_ssrn_id_from_url(value)
 
     return None
 
 
 def compare_author(author_id, comparison_name, author_full_name):
     """
     Compares the given author's full name with a comparison name and returns the comparison method used.
@@ -472,7 +526,31 @@
         return {'author_full_name': author_full_name, 'author_id': author_id, 'method': 'all'}
     elif some(comparison_parts, lambda part: part in full_name_clean, 2):
         return {'author_full_name': author_full_name, 'author_id': author_id, 'method': 'some'}
     # elif any(part in full_name_clean for part in comparison_parts):
         # return {'author_full_name': author_full_name, 'author_id': author_id, 'method': 'any'}
 
     return False
+
+
+def parse_sex(sex: str, lang: str = "es") -> str:
+    """
+    Function to normalize sex name
+
+    Parameters:
+    ----------
+    sex:str
+        The sex to be normalized
+
+    Returns:
+    --------
+    str
+        The sex normalized
+    """
+    sex = sex.strip().lower()
+    if sex == "m" or sex == 'masculino':
+        return "Hombre" if lang == "es" else "Men"
+    if sex == "f" or sex == 'femenino':
+        return "Mujer" if lang == "es" else "Woman"
+    if sex == "i" or "intersexual":
+        return "Intersexual"
+    return sex
```

### Comparing `kahi_impactu_utils-0.0.9/setup.py` & `kahi_impactu_utils-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,20 @@
 
         long_description=open("README.md").read(),
 
         long_description_content_type="text/markdown",
 
         # Dependent packages (distributions)
         install_requires=[
-            'langid==1.1.6',
-            'lingua-language-detector==1.3.3',
-            'pycld2==0.41',
-            'langdetect==1.0.7',
-            'fastspell==0.8.0',
-            'iso639==0.1.4',
+            'langid~=1.1.6',
+            'lingua-language-detector~=1.3.3',
+            'pycld2~=0.41',
+            'langdetect~=1.0.7',
+            'fastspell~=0.8.0',
+            'iso639~=0.1.4',
             'unidecode',
             'titlecase'
         ],
     )
 
 
 if __name__ == "__main__":
```

