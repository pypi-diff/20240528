# Comparing `tmp/chess_transformer-0.1.5.tar.gz` & `tmp/chess_transformer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.5.tar", last modified: Mon May 27 09:48:49 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.6.tar", last modified: Mon May 27 12:31:16 2024, max compression
```

## Comparing `chess_transformer-0.1.5.tar` & `chess_transformer-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      584 2024-05-27 09:48:47.000000 chess_transformer-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.204679 chess_transformer-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.204679 chess_transformer-0.1.5/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-27 08:25:05.000000 chess_transformer-0.1.5/src/chess_transformer/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.204679 chess_transformer-0.1.5/src/chess_transformer/data/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      224 2024-05-27 09:38:45.000000 chess_transformer-0.1.5/src/chess_transformer/data/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.5/src/chess_transformer/data/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1114 2024-05-27 09:36:55.000000 chess_transformer-0.1.5/src/chess_transformer/data/labs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.5/src/chess_transformer/data/parse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.5/src/chess_transformer/data/pytorch.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.5/src/chess_transformer/data/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/src/chess_transformer/model/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-05-27 08:26:28.000000 chess_transformer-0.1.5/src/chess_transformer/model/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.5/src/chess_transformer/model/bert.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1455 2024-05-27 08:29:47.000000 chess_transformer-0.1.5/src/chess_transformer/model/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.5/src/chess_transformer/model/loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-27 08:26:17.000000 chess_transformer-0.1.5/src/chess_transformer/model/metrics.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/src/chess_transformer/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-05-27 09:42:44.000000 chess_transformer-0.1.5/src/chess_transformer/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.5/src/chess_transformer/vocab/sans.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1423 2024-05-27 09:43:00.000000 chess_transformer-0.1.5/src/chess_transformer/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 09:48:49.214679 chess_transformer-0.1.5/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 09:48:49.000000 chess_transformer-0.1.5/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-27 09:48:49.000000 chess_transformer-0.1.5/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 09:48:49.000000 chess_transformer-0.1.5/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       48 2024-05-27 09:48:49.000000 chess_transformer-0.1.5/src/chess_transformer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 09:48:49.000000 chess_transformer-0.1.5/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      584 2024-05-27 12:31:13.000000 chess_transformer-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-27 08:25:05.000000 chess_transformer-0.1.6/src/chess_transformer/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/chess_transformer/data/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      246 2024-05-27 10:31:51.000000 chess_transformer-0.1.6/src/chess_transformer/data/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.6/src/chess_transformer/data/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1186 2024-05-27 10:12:17.000000 chess_transformer-0.1.6/src/chess_transformer/data/labs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.6/src/chess_transformer/data/parse.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.6/src/chess_transformer/data/pytorch.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/src/chess_transformer/data/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer/model/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-05-27 08:26:28.000000 chess_transformer-0.1.6/src/chess_transformer/model/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.6/src/chess_transformer/model/bert.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1455 2024-05-27 08:29:47.000000 chess_transformer-0.1.6/src/chess_transformer/model/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.6/src/chess_transformer/model/loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-27 08:26:17.000000 chess_transformer-0.1.6/src/chess_transformer/model/metrics.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-05-27 09:42:44.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/sans.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1423 2024-05-27 09:43:00.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       48 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.5/pyproject.toml` & `chess_transformer-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread goes smarter, baby"
 dependencies = [
   "torch", "chess", "jaxtyping", "haskellian", "chess-notation"
 ]
```

### Comparing `chess_transformer-0.1.5/src/chess_transformer/data/dataset.py` & `chess_transformer-0.1.6/src/chess_transformer/data/dataset.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/data/labs.py` & `chess_transformer-0.1.6/src/chess_transformer/data/labs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Sequence, NamedTuple
+from typing import Literal, Sequence, NamedTuple, Iterable
 import chess
 from ..vocab import Vocabulary
 
 promotion_ids = dict(n=1, b=2, r=3, q=4)
 def parse_promotion(piece: Literal['n', 'b', 'r', 'q'] | None) -> int:
   return 0 if piece is None else promotion_ids[piece]
 
@@ -10,23 +10,23 @@
   from_file = ord(e2e4q[0]) - ord('a')
   from_rank = int(e2e4q[1]) - 1
   to_file = ord(e2e4q[2]) - ord('a')
   to_rank = int(e2e4q[3]) - 1
   promotion = parse_promotion(e2e4q[4] if len(e2e4q) == 5 else None) # type: ignore
   return from_file, from_rank, to_file, to_rank, promotion
 
-def uci_labels(sans: Sequence[str]) -> Sequence[tuple[int, int, int, int, int]]:
+def sans2ucis(sans: Sequence[str]) -> Iterable[str]:
   board = chess.Board()
-  labs = []
   for san in sans:
     move = board.parse_san(san)
-    labs.append(parse_uci(move.uci()))
+    yield move.uci()
     board.push(move)
 
-  return labs
+def uci_labels(sans: Sequence[str]) -> Sequence[tuple[int, int, int, int, int]]:
+  return [parse_uci(uci) for uci in sans2ucis(sans)]
 
 class Sample(NamedTuple):
   input_ids: Sequence[int]
   labs: Sequence[tuple[int, int, int, int, int]]
 
 def sample(sans: Sequence[str], vocab: Vocabulary) -> Sample:
   labs = uci_labels(sans)
```

### Comparing `chess_transformer-0.1.5/src/chess_transformer/data/pytorch.py` & `chess_transformer-0.1.6/src/chess_transformer/data/pytorch.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/data/random.py` & `chess_transformer-0.1.6/src/chess_transformer/data/random.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/model/bert.py` & `chess_transformer-0.1.6/src/chess_transformer/model/bert.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/model/decoding.py` & `chess_transformer-0.1.6/src/chess_transformer/model/decoding.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/model/loss.py` & `chess_transformer-0.1.6/src/chess_transformer/model/loss.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/vocab/sans.py` & `chess_transformer-0.1.6/src/chess_transformer/vocab/sans.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer/vocab/vocab.py` & `chess_transformer-0.1.6/src/chess_transformer/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.5/src/chess_transformer.egg-info/SOURCES.txt` & `chess_transformer-0.1.6/src/chess_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

