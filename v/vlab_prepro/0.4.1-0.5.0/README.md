# Comparing `tmp/vlab_prepro-0.4.1.tar.gz` & `tmp/vlab_prepro-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlab_prepro-0.4.1.tar", max compression
+gzip compressed data, was "vlab_prepro-0.5.0.tar", max compression
```

## Comparing `vlab_prepro-0.4.1.tar` & `vlab_prepro-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.4.1/LICENSE
--rw-r--r--   0        0        0      513 2024-05-05 21:03:32.977874 vlab_prepro-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.4.1/vlab_prepro/__init__.py
--rw-r--r--   0        0        0     8330 2024-05-05 21:03:14.910985 vlab_prepro-0.4.1/vlab_prepro/preprocess.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 vlab_prepro-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.5.0/LICENSE
+-rw-r--r--   0        0        0      513 2024-05-28 01:54:00.080400 vlab_prepro-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.5.0/vlab_prepro/__init__.py
+-rw-r--r--   0        0        0     8330 2024-05-28 01:53:26.466713 vlab_prepro-0.5.0/vlab_prepro/preprocess.py
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 vlab_prepro-0.5.0/PKG-INFO
```

### Comparing `vlab_prepro-0.4.1/LICENSE` & `vlab_prepro-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlab_prepro-0.4.1/pyproject.toml` & `vlab_prepro-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vlab_prepro"
-version = "0.4.1"
+version = "0.5.0"
 description = ""
 authors = ["Nandan Rao <nandanmarkrao@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 toolz = "^0.11.1"
 pandas = "^2.0.3"
```

### Comparing `vlab_prepro-0.4.1/vlab_prepro/preprocess.py` & `vlab_prepro-0.5.0/vlab_prepro/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     return df
 
 
 def add_final_answer(df):
     df = df.sort_values("timestamp")
     df["final_answer"] = True
     df.loc[
-        df.duplicated(["userid", "surveyid", "question_idx"], keep="last"),
+        df.duplicated(["userid", "surveyid", "question_ref"], keep="last"),
         "final_answer",
     ] = False
     return df
 
 
 @curry
 def _assign(name, fn, tindex, d):
```

