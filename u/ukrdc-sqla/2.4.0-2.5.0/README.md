# Comparing `tmp/ukrdc_sqla-2.4.0.tar.gz` & `tmp/ukrdc_sqla-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukrdc_sqla-2.4.0.tar", max compression
+gzip compressed data, was "ukrdc_sqla-2.5.0.tar", max compression
```

## Comparing `ukrdc_sqla-2.4.0.tar` & `ukrdc_sqla-2.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1095 2024-04-30 15:57:16.478293 ukrdc_sqla-2.4.0/LICENSE
--rw-r--r--   0        0        0      926 2024-05-23 14:51:32.330278 ukrdc_sqla-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1894 2024-04-30 15:57:16.478293 ukrdc_sqla-2.4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.4.0/ukrdc_sqla/__init__.py
--rw-r--r--   0        0        0     9392 2024-05-01 21:42:21.543459 ukrdc_sqla-2.4.0/ukrdc_sqla/empi.py
--rw-r--r--   0        0        0     1690 2024-05-01 21:35:51.375907 ukrdc_sqla-2.4.0/ukrdc_sqla/errorsdb.py
--rw-r--r--   0        0        0      366 2024-05-01 21:35:51.384665 ukrdc_sqla-2.4.0/ukrdc_sqla/pkb.py
--rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.4.0/ukrdc_sqla/py.typed
--rw-r--r--   0        0        0     1109 2024-05-01 21:35:51.391437 ukrdc_sqla-2.4.0/ukrdc_sqla/stats.py
--rw-r--r--   0        0        0    62095 2024-05-01 21:41:35.620165 ukrdc_sqla-2.4.0/ukrdc_sqla/ukrdc.py
--rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.4.0/ukrdc_sqla/utils/__init__.py
--rw-r--r--   0        0        0     4219 2024-05-01 21:42:35.813946 ukrdc_sqla-2.4.0/ukrdc_sqla/utils/links.py
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 ukrdc_sqla-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-30 15:57:16.478293 ukrdc_sqla-2.5.0/LICENSE
+-rw-r--r--   0        0        0      934 2024-05-28 19:55:40.404104 ukrdc_sqla-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1894 2024-04-30 15:57:16.478293 ukrdc_sqla-2.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.5.0/ukrdc_sqla/__init__.py
+-rw-r--r--   0        0        0     9392 2024-05-23 15:58:12.676691 ukrdc_sqla-2.5.0/ukrdc_sqla/empi.py
+-rw-r--r--   0        0        0     1690 2024-05-23 15:58:12.709075 ukrdc_sqla-2.5.0/ukrdc_sqla/errorsdb.py
+-rw-r--r--   0        0        0      366 2024-05-23 15:58:12.730379 ukrdc_sqla-2.5.0/ukrdc_sqla/pkb.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.5.0/ukrdc_sqla/py.typed
+-rw-r--r--   0        0        0     1109 2024-05-23 15:58:12.740615 ukrdc_sqla-2.5.0/ukrdc_sqla/stats.py
+-rw-r--r--   0        0        0    62406 2024-05-28 19:55:40.414454 ukrdc_sqla-2.5.0/ukrdc_sqla/ukrdc.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:57:16.478293 ukrdc_sqla-2.5.0/ukrdc_sqla/utils/__init__.py
+-rw-r--r--   0        0        0     4219 2024-05-23 15:58:12.749002 ukrdc_sqla-2.5.0/ukrdc_sqla/utils/links.py
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 ukrdc_sqla-2.5.0/PKG-INFO
```

### Comparing `ukrdc_sqla-2.4.0/LICENSE` & `ukrdc_sqla-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/pyproject.toml` & `ukrdc_sqla-2.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 authors = ["Joel Collins <joel.collins@renalregistry.nhs.uk>"]
 description = "SQLAlchemy models for the UKRDC"
 name = "ukrdc-sqla"
 readme = "README.md"
-version = "2.4.0"
+version = "2.5.0"
 
 [tool.poetry.dependencies]
 SQLAlchemy = ">=1.4.25,<3.0.0"
 python = ">=3.8.0,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.8.0"
-pytest = "^7.1.3"
+pytest = ">=7.1.3,<9.0.0"
 ruff = "^0.4.2"
 tox = "^4.15.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `ukrdc_sqla-2.4.0/README.md` & `ukrdc_sqla-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/ukrdc_sqla/empi.py` & `ukrdc_sqla-2.5.0/ukrdc_sqla/empi.py`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/ukrdc_sqla/errorsdb.py` & `ukrdc_sqla-2.5.0/ukrdc_sqla/errorsdb.py`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/ukrdc_sqla/stats.py` & `ukrdc_sqla-2.5.0/ukrdc_sqla/stats.py`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/ukrdc_sqla/ukrdc.py` & `ukrdc_sqla-2.5.0/ukrdc_sqla/ukrdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1668,7 +1668,17 @@
     cons = Column(BIT(1), nullable=False)
     rrt = Column(BIT(1), nullable=False)
     equiv_modality = Column(String(8))
     end_of_care = Column(BIT(1), nullable=False)
     is_imprecise = Column(BIT(1), nullable=False)
     nhsbt_transplant_type = Column(String(4))
     transfer_out = Column(BIT(1))
+
+
+class Satellite_map(Base):
+    __tablename__ = "satellite_map"
+
+    satellite_code = Column(String(10), primary_key=True)
+    main_unit_code = Column(String(10), primary_key=True)
+
+    creation_date = Column(DateTime, nullable=False, server_default=text("now()"))
+    update_date = Column(DateTime)
```

### Comparing `ukrdc_sqla-2.4.0/ukrdc_sqla/utils/links.py` & `ukrdc_sqla-2.5.0/ukrdc_sqla/utils/links.py`

 * *Files identical despite different names*

### Comparing `ukrdc_sqla-2.4.0/PKG-INFO` & `ukrdc_sqla-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukrdc-sqla
-Version: 2.4.0
+Version: 2.5.0
 Summary: SQLAlchemy models for the UKRDC
 Author: Joel Collins
 Author-email: joel.collins@renalregistry.nhs.uk
 Requires-Python: >=3.8.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

