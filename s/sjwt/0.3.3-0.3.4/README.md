# Comparing `tmp/sjwt-0.3.3.tar.gz` & `tmp/sjwt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjwt-0.3.3.tar", last modified: Sun May 19 03:54:15 2024, max compression
+gzip compressed data, was "sjwt-0.3.4.tar", last modified: Tue May 28 07:46:10 2024, max compression
```

## Comparing `sjwt-0.3.3.tar` & `sjwt-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:54:15.600878 sjwt-0.3.3/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-19 03:54:15.600878 sjwt-0.3.3/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2024-05-19 03:54:15.600878 sjwt-0.3.3/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)      235 2024-05-19 03:53:57.000000 sjwt-0.3.3/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:54:15.596878 sjwt-0.3.3/sjwt/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      194 2024-05-19 01:52:46.000000 sjwt-0.3.3/sjwt/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     8516 2024-05-19 03:54:06.000000 sjwt-0.3.3/sjwt/models.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3019 2024-05-19 01:52:46.000000 sjwt-0.3.3/sjwt/sjwt.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-19 03:54:15.600878 sjwt-0.3.3/sjwt.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-19 03:54:15.000000 sjwt-0.3.3/sjwt.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2024-05-19 03:54:15.000000 sjwt-0.3.3/sjwt.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-19 03:54:15.000000 sjwt-0.3.3/sjwt.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-19 01:52:46.000000 sjwt-0.3.3/sjwt.egg-info/not-zip-safe
--rw-r--r--   0 andrey    (1000) andrey    (1000)        5 2024-05-19 03:54:15.000000 sjwt-0.3.3/sjwt.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-28 07:46:10.050033 sjwt-0.3.4/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-28 07:46:10.050033 sjwt-0.3.4/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2024-05-28 07:46:10.050033 sjwt-0.3.4/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      235 2024-05-28 07:44:42.000000 sjwt-0.3.4/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-28 07:46:10.046033 sjwt-0.3.4/sjwt/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      194 2024-05-22 16:32:16.000000 sjwt-0.3.4/sjwt/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     9404 2024-05-28 07:44:24.000000 sjwt-0.3.4/sjwt/models.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3019 2024-05-22 16:32:16.000000 sjwt-0.3.4/sjwt/sjwt.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2024-05-28 07:46:10.046033 sjwt-0.3.4/sjwt.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      144 2024-05-28 07:46:09.000000 sjwt-0.3.4/sjwt.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2024-05-28 07:46:10.000000 sjwt-0.3.4/sjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-28 07:46:10.000000 sjwt-0.3.4/sjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2024-05-22 16:32:16.000000 sjwt-0.3.4/sjwt.egg-info/not-zip-safe
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        5 2024-05-28 07:46:10.000000 sjwt-0.3.4/sjwt.egg-info/top_level.txt
```

### Comparing `sjwt-0.3.3/sjwt/models.py` & `sjwt-0.3.4/sjwt/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -186,12 +186,32 @@
     withdrawal_datetime_raw = Column(VARCHAR(98))
     deposit_datetime = Column(TIMESTAMP, nullable=True)
     trading_datetime = Column(TIMESTAMP, nullable=True)
     withdrawal_datetime = Column(TIMESTAMP, nullable=True)
     has_history = Column(Boolean, default=False)
 
 
+class LiquidityDayCandle(BaseModel):
+    __tablename__ = 'liquidity_day'
+    timestamp = Column(TIMESTAMP, nullable=False, index=True)
+    pair_id = Column(ForeignKey('coin_pair.pair_id', ondelete='CASCADE'), index=True, nullable=False)
+    exchange_rate = Column(FLOAT, nullable=True)
+    open = Column(FLOAT, nullable=True)
+    close = Column(FLOAT, nullable=True)
+    high = Column(FLOAT, nullable=True)
+    low = Column(FLOAT, nullable=True)
+    adds = Column(FLOAT, nullable=True)
+    removes = Column(FLOAT, nullable=True)
+    syncs = Column(FLOAT, nullable=True)
+    add_volume = Column(FLOAT, nullable=True)
+    remove_volume = Column(FLOAT, nullable=True)
+    start_block = Column(BigInteger, nullable=True)
+    end_block = Column(BigInteger, nullable=True)
+    liquidity_type = Column(VARCHAR(64), nullable=True)
+    UniqueConstraint("pair_id", "timestamp", name="pair_date")
+
+
 class CoinPased(BaseModel):
     __tablename__ = 'coin_article'
 
     hash = Column(VARCHAR(48), nullable=False, unique=True, index=True)
     is_parsed = Column(Boolean, nullable=False, default=False)
```

### Comparing `sjwt-0.3.3/sjwt/sjwt.py` & `sjwt-0.3.4/sjwt/sjwt.py`

 * *Files identical despite different names*

