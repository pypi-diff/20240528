# Comparing `tmp/dj-database-url-2.0.0.tar.gz` & `tmp/dj-database-url-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-database-url-2.0.0.tar", last modified: Thu Apr 27 15:31:20 2023, max compression
+gzip compressed data, was "dj-database-url-2.1.0.tar", last modified: Tue Aug 15 13:12:53 2023, max compression
```

## Comparing `dj-database-url-2.0.0.tar` & `dj-database-url-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/dj_database_url/
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/dj_database_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/dj_database_url/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/dj_database_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/tests/test_dj_database_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/dj_database_url/
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/dj_database_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/dj_database_url/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/dj_database_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-08-15 13:12:53.000000 dj-database-url-2.1.0/dj_database_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-15 13:12:53.000000 dj-database-url-2.1.0/dj_database_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 13:12:53.000000 dj-database-url-2.1.0/dj_database_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-15 13:12:53.000000 dj-database-url-2.1.0/dj_database_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-15 13:12:53.000000 dj-database-url-2.1.0/dj_database_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 13:12:53.640774 dj-database-url-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-08-15 13:12:39.000000 dj-database-url-2.1.0/tests/test_dj_database_url.py
```

### Comparing `dj-database-url-2.0.0/LICENSE` & `dj-database-url-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-database-url-2.0.0/PKG-INFO` & `dj-database-url-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-database-url
-Version: 2.0.0
+Version: 2.1.0
 Summary: Use Database URLs in your Django Application.
 Home-page: https://github.com/jazzband/dj-database-url
 Author: Original Author: Kenneth Reitz, Maintained by: JazzBand Community
 License: BSD
 Project-URL: GitHub, https://github.com/jazzband/dj-database-url/
 Project-URL: Release log, https://github.com/jazzband/dj-database-url/blob/master/CHANGELOG.md
 Platform: any
```

### Comparing `dj-database-url-2.0.0/README.rst` & `dj-database-url-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dj-database-url-2.0.0/dj_database_url/__init__.py` & `dj-database-url-2.1.0/dj_database_url/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,18 @@
     # Pass the query string into OPTIONS.
     options: Dict[str, Any] = {}
     for key, values in query.items():
         if spliturl.scheme == "mysql" and key == "ssl-ca":
             options["ssl"] = {"ca": values[-1]}
             continue
 
-        options[key] = values[-1]
+        try:
+            options[key] = int(values[-1])
+        except (TypeError, ValueError):
+            options[key] = values[-1]
 
     if ssl_require:
         options["sslmode"] = "require"
 
     # Support for Postgres Schema URLs
     if "currentSchema" in options and engine in (
         "django.contrib.gis.db.backends.postgis",
```

### Comparing `dj-database-url-2.0.0/dj_database_url.egg-info/PKG-INFO` & `dj-database-url-2.1.0/dj_database_url.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-database-url
-Version: 2.0.0
+Version: 2.1.0
 Summary: Use Database URLs in your Django Application.
 Home-page: https://github.com/jazzband/dj-database-url
 Author: Original Author: Kenneth Reitz, Maintained by: JazzBand Community
 License: BSD
 Project-URL: GitHub, https://github.com/jazzband/dj-database-url/
 Project-URL: Release log, https://github.com/jazzband/dj-database-url/blob/master/CHANGELOG.md
 Platform: any
```

### Comparing `dj-database-url-2.0.0/setup.py` & `dj-database-url-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 readme = Path("README.rst").read_text()
 
 setup(
     name="dj-database-url",
-    version="2.0.0",
+    version="2.1.0",
     url="https://github.com/jazzband/dj-database-url",
     license="BSD",
     author="Original Author: Kenneth Reitz, Maintained by: JazzBand Community",
     description="Use Database URLs in your Django Application.",
     long_description=readme,
     long_description_content_type="text/x-rst",
     packages=["dj_database_url"],
```

### Comparing `dj-database-url-2.0.0/tests/test_dj_database_url.py` & `dj-database-url-2.1.0/tests/test_dj_database_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,10 +581,17 @@
         os.environ,
         {"DATABASE_URL": "postgres://user:password@instance.amazonaws.com:5431/d8r8?"},
     )
     def test_ssl_require(self):
         url = dj_database_url.config(ssl_require=True)
         assert url["OPTIONS"] == {'sslmode': 'require'}
 
+    def test_options_int_values(self):
+        """Ensure that options with integer values are parsed correctly."""
+        url = dj_database_url.parse(
+            "mysql://user:pw@127.0.0.1:15036/db?connect_timout=3"
+        )
+        assert url["OPTIONS"] == {'connect_timout': 3}
+
 
 if __name__ == "__main__":
     unittest.main()
```

