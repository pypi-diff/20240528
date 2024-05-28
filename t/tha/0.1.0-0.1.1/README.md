# Comparing `tmp/tha-0.1.0.tar.gz` & `tmp/tha-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tha-0.1.0.tar", last modified: Sun May 26 10:08:23 2024, max compression
+gzip compressed data, was "tha-0.1.1.tar", last modified: Tue May 28 08:24:12 2024, max compression
```

## Comparing `tha-0.1.0.tar` & `tha-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-26 10:08:23.153936 tha-0.1.0/
--rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-26 09:50:16.000000 tha-0.1.0/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-26 10:08:23.153814 tha-0.1.0/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)     5160 2024-05-26 09:59:52.000000 tha-0.1.0/README.md
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-26 10:08:23.153986 tha-0.1.0/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)      759 2024-05-26 10:07:09.000000 tha-0.1.0/setup.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-26 10:08:23.152940 tha-0.1.0/tha/
--rw-r--r--   0 seanghay   (501) staff       (20)        0 2024-05-26 10:06:59.000000 tha-0.1.0/tha/__init__.py
--rw-r--r--   0 seanghay   (501) staff       (20)      144 2024-05-26 10:06:59.000000 tha-0.1.0/tha/ascii_lines.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2027 2024-05-26 10:06:59.000000 tha-0.1.0/tha/cardinals.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2043 2024-05-26 10:06:59.000000 tha-0.1.0/tha/currency.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1127 2024-05-26 10:06:59.000000 tha-0.1.0/tha/datetime.py
--rw-r--r--   0 seanghay   (501) staff       (20)      660 2024-05-26 10:06:59.000000 tha-0.1.0/tha/decimals.py
--rw-r--r--   0 seanghay   (501) staff       (20)      161 2024-05-26 10:06:59.000000 tha-0.1.0/tha/hashtags.py
--rw-r--r--   0 seanghay   (501) staff       (20)      438 2024-05-26 10:06:59.000000 tha-0.1.0/tha/license_plate.py
--rw-r--r--   0 seanghay   (501) staff       (20)    17337 2024-05-26 10:06:59.000000 tha-0.1.0/tha/normalize.py
--rw-r--r--   0 seanghay   (501) staff       (20)      304 2024-05-26 10:06:59.000000 tha-0.1.0/tha/ordinals.py
--rw-r--r--   0 seanghay   (501) staff       (20)      164 2024-05-26 10:06:59.000000 tha-0.1.0/tha/parenthesis.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1018 2024-05-26 10:06:59.000000 tha-0.1.0/tha/phone_numbers.py
--rw-r--r--   0 seanghay   (501) staff       (20)      354 2024-05-26 10:06:59.000000 tha-0.1.0/tha/punctuations.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2309 2024-05-26 10:06:59.000000 tha-0.1.0/tha/repeater.py
--rw-r--r--   0 seanghay   (501) staff       (20)      243 2024-05-26 10:06:59.000000 tha-0.1.0/tha/strings.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1016 2024-05-26 10:06:59.000000 tha-0.1.0/tha/urls.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2957 2024-05-26 10:06:59.000000 tha-0.1.0/tha/verbatim.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-26 10:08:23.153581 tha-0.1.0/tha.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-26 10:08:23.000000 tha-0.1.0/tha.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      449 2024-05-26 10:08:23.000000 tha-0.1.0/tha.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-26 10:08:23.000000 tha-0.1.0/tha.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       35 2024-05-26 10:08:23.000000 tha-0.1.0/tha.egg-info/requires.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-26 10:08:23.000000 tha-0.1.0/tha.egg-info/top_level.txt
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.554610 tha-0.1.1/
+-rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-26 09:50:16.000000 tha-0.1.1/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:24:12.554501 tha-0.1.1/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)     5160 2024-05-26 09:59:52.000000 tha-0.1.1/README.md
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-28 08:24:12.554647 tha-0.1.1/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)      759 2024-05-28 08:24:00.000000 tha-0.1.1/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.553787 tha-0.1.1/tha/
+-rw-r--r--   0 seanghay   (501) staff       (20)        0 2024-05-26 10:06:59.000000 tha-0.1.1/tha/__init__.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      144 2024-05-26 10:06:59.000000 tha-0.1.1/tha/ascii_lines.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2027 2024-05-26 10:06:59.000000 tha-0.1.1/tha/cardinals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2043 2024-05-26 10:06:59.000000 tha-0.1.1/tha/currency.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1127 2024-05-26 10:06:59.000000 tha-0.1.1/tha/datetime.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      824 2024-05-27 13:53:12.000000 tha-0.1.1/tha/decimals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      161 2024-05-26 10:06:59.000000 tha-0.1.1/tha/hashtags.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      438 2024-05-26 10:06:59.000000 tha-0.1.1/tha/license_plate.py
+-rw-r--r--   0 seanghay   (501) staff       (20)    17337 2024-05-26 10:06:59.000000 tha-0.1.1/tha/normalize.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      304 2024-05-26 10:06:59.000000 tha-0.1.1/tha/ordinals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      164 2024-05-26 10:06:59.000000 tha-0.1.1/tha/parenthesis.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1018 2024-05-26 10:06:59.000000 tha-0.1.1/tha/phone_numbers.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      631 2024-05-28 08:19:34.000000 tha-0.1.1/tha/punctuations.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2309 2024-05-26 10:06:59.000000 tha-0.1.1/tha/repeater.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      243 2024-05-26 10:06:59.000000 tha-0.1.1/tha/strings.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1016 2024-05-26 10:06:59.000000 tha-0.1.1/tha/urls.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2957 2024-05-26 10:06:59.000000 tha-0.1.1/tha/verbatim.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.554299 tha-0.1.1/tha.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      449 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       35 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/requires.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/top_level.txt
```

### Comparing `tha-0.1.0/LICENSE` & `tha-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/PKG-INFO` & `tha-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tha
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Khmer Text Normalization and Verbalization Toolkit.
 Home-page: https://github.com/seanghay/tha
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Tha (ថា)
```

### Comparing `tha-0.1.0/README.md` & `tha-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/setup.py` & `tha-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setuptools.setup(
   name="tha",
-  version="0.1.0",
+  version="0.1.1",
   description="A Khmer Text Normalization and Verbalization Toolkit.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/seanghay/tha",
   author="Seanghay Yath",
   author_email="seanghay.dev@gmail.com",
   license="Apache License 2.0",
```

### Comparing `tha-0.1.0/tha/cardinals.py` & `tha-0.1.1/tha/cardinals.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/currency.py` & `tha-0.1.1/tha/currency.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/datetime.py` & `tha-0.1.1/tha/datetime.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/decimals.py` & `tha-0.1.1/tha/decimals.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 from tha.cardinals import processor as cardinals_processor
 
 RE_DECIMALS = re.compile(r"([\-]?[\u17e0-\u17e90-9]+)([\.\,])([\u17e0-\u17e90-9]+)")
 RE_NUM_LEADING_ZEROS = re.compile(
   r"([\-]?[\u17e0-\u17e90-9]+)([\.\,])([\u17e00]+)([\d\u17e0-\u17e9]+)"
 )
 
+def processor(text: str, comma_word="ក្បៀស", point_word="ចុច") -> str:
+  translation = str.maketrans({".": f"▁{point_word}▁", ",": f"▁{comma_word}▁"})
 
-def leading_zeros_replacer(m):
-  return f"{m[1]}{m[2]}{'▁'.join(m[3])}▁{m[4]}"
+  def leading_zeros_replacer(m):
+    return f"{m[1]}{m[2]}{'▁'.join(m[3])}▁{m[4]}".translate(translation)
 
+  def decimals_replacer(m):
+    sep = m[2].translate(translation)
+    return f"{m[1]}{sep}{m[3]}"
 
-def processor(text: str, comma_word="ក្បៀស", point_word="ចុច") -> str:
   text = RE_NUM_LEADING_ZEROS.sub(leading_zeros_replacer, text)
+  text = RE_DECIMALS.sub(decimals_replacer, text)
   text = cardinals_processor(text)
-  text = text.replace(".", f"▁{point_word}▁")
-  text = text.replace(",", f"▁{comma_word}▁")
+
   return text
```

### Comparing `tha-0.1.0/tha/normalize.py` & `tha-0.1.1/tha/normalize.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/phone_numbers.py` & `tha-0.1.1/tha/phone_numbers.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/repeater.py` & `tha-0.1.1/tha/repeater.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/urls.py` & `tha-0.1.1/tha/urls.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha/verbatim.py` & `tha-0.1.1/tha/verbatim.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.0/tha.egg-info/PKG-INFO` & `tha-0.1.1/tha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tha
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Khmer Text Normalization and Verbalization Toolkit.
 Home-page: https://github.com/seanghay/tha
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Tha (ថា)
```

