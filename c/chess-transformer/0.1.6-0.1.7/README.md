# Comparing `tmp/chess_transformer-0.1.6.tar.gz` & `tmp/chess_transformer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.6.tar", last modified: Mon May 27 12:31:16 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.7.tar", last modified: Tue May 28 08:45:00 2024, max compression
```

## Comparing `chess_transformer-0.1.6.tar` & `chess_transformer-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      584 2024-05-27 12:31:13.000000 chess_transformer-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-27 08:25:05.000000 chess_transformer-0.1.6/src/chess_transformer/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.714682 chess_transformer-0.1.6/src/chess_transformer/data/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      246 2024-05-27 10:31:51.000000 chess_transformer-0.1.6/src/chess_transformer/data/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.6/src/chess_transformer/data/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1186 2024-05-27 10:12:17.000000 chess_transformer-0.1.6/src/chess_transformer/data/labs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.6/src/chess_transformer/data/parse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.6/src/chess_transformer/data/pytorch.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/src/chess_transformer/data/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer/model/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-05-27 08:26:28.000000 chess_transformer-0.1.6/src/chess_transformer/model/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.6/src/chess_transformer/model/bert.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1455 2024-05-27 08:29:47.000000 chess_transformer-0.1.6/src/chess_transformer/model/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.6/src/chess_transformer/model/loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-27 08:26:17.000000 chess_transformer-0.1.6/src/chess_transformer/model/metrics.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-05-27 09:42:44.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/sans.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1423 2024-05-27 09:43:00.000000 chess_transformer-0.1.6/src/chess_transformer/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 12:31:16.724682 chess_transformer-0.1.6/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       48 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 12:31:16.000000 chess_transformer-0.1.6/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      307 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-05-27 14:59:07.000000 chess_transformer-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      515 2024-05-28 08:44:50.000000 chess_transformer-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.022151 chess_transformer-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      125 2024-05-27 15:03:14.000000 chess_transformer-0.1.7/src/chess_transformer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      302 2024-05-27 18:53:00.000000 chess_transformer-0.1.7/src/chess_transformer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      341 2024-05-27 18:29:49.000000 chess_transformer-0.1.7/src/chess_transformer/_vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer/pytorch/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-27 15:05:21.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-27 19:07:13.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      250 2024-05-27 15:07:20.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/_loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1326 2024-05-27 19:13:32.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/data.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1166 2024-05-28 08:39:47.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/decode.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1375 2024-05-27 19:34:27.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/model.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      909 2024-05-27 19:32:53.000000 chess_transformer-0.1.7/src/chess_transformer/pytorch/pos_enc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1484 2024-05-27 18:58:37.000000 chess_transformer-0.1.7/src/chess_transformer/samples.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:45:00.032151 chess_transformer-0.1.7/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      307 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-28 08:45:00.000000 chess_transformer-0.1.7/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.6/pyproject.toml` & `chess_transformer-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
-description = "Moveread goes smarter, baby"
+description = "package_description"
 dependencies = [
-  "torch", "chess", "jaxtyping", "haskellian", "chess-notation"
+  
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `chess_transformer-0.1.6/src/chess_transformer/data/pytorch.py` & `chess_transformer-0.1.7/src/chess_transformer/pytorch/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import NamedTuple, Sequence
-from haskellian import iter as I
+from typing import Sequence, NamedTuple
 from jaxtyping import Int
+from torch import Tensor
 import torch
-from ..vocab import Vocabulary
-from .parse import parse_line
-from .labs import sample
-
-class TorchSample(NamedTuple):
-  input_ids: Int[torch.Tensor, 'L']
-  labels: Int[torch.Tensor, 'L 5']
-
-class TorchBatch(NamedTuple):
-  input_ids: Int[torch.Tensor, 'B L']
-  labels: Int[torch.Tensor, 'B L 5']
-
-def torch_sample(idx: int, *, lines: Sequence[str], vocab: Vocabulary) -> TorchSample:
-  line = lines[idx]
-  sans = parse_line(line)
-  input_ids, labs = sample(sans, vocab)
-  return TorchSample(torch.tensor(input_ids), torch.tensor(labs))
+from haskellian import iter as I
+from .. import Vocabulary, vocab as default_vocab, parse_sample as _parse_sample
+
+class Sample(NamedTuple):
+  input_ids: Int[Tensor, 'seq_len']
+  word_ends: Sequence[int]
+  labs: Int[Tensor, 'seq_len 5']
+
+class Batch(NamedTuple):
+  input_ids: Int[Tensor, 'batch seq_len']
+  word_ends: Sequence[Sequence[int]]
+  labs: Int[Tensor, 'batch seq_len 5']
+
+def parse_sample(line: str, vocab: Vocabulary = default_vocab) -> Sample:
+  (tokens, ends), labs = _parse_sample(line)
+  input_ids = [vocab[tok] for tok in tokens]
+  return Sample(torch.tensor(input_ids), ends, torch.tensor(labs))
 
-def collate_fn(batch: Sequence[TorchSample], pad_token_id: int, ignore_idx: int = -100) -> TorchBatch:
+def collate_fn(batch: Sequence[Sample], pad_token_id: int, ignore_idx: int = -100) -> Batch:
 
-  input_ids, labs = I.unzip(batch)
+  input_ids, ends, labs = I.unzip(batch)
   batch_size = len(input_ids)
-  maxlen = max(len(x) for x in input_ids)
-  padded_input_ids = torch.full((batch_size, maxlen), fill_value=pad_token_id)
-  padded_labs = torch.full((batch_size, maxlen, 5), fill_value=ignore_idx)
+  max_input_len = max(len(x) for x in input_ids)
+  max_lab_len = max(len(x) for x in labs)
+  padded_input_ids = torch.full((batch_size, max_input_len), fill_value=pad_token_id)
+  padded_labs = torch.full((batch_size, max_lab_len, 5), fill_value=ignore_idx)
 
   for i in range(batch_size):
-    l = len(input_ids[i])
-    padded_input_ids[i, :l] = input_ids[i]
-    padded_labs[i, :l] = labs[i]
+    padded_input_ids[i, :len(input_ids[i])] = input_ids[i]
+    padded_labs[i, :len(labs[i])] = labs[i]
 
-  return TorchBatch(padded_input_ids, padded_labs)
+  return Batch(padded_input_ids, ends, padded_labs)
```

### Comparing `chess_transformer-0.1.6/src/chess_transformer/model/decoding.py` & `chess_transformer-0.1.7/src/chess_transformer/pytorch/decode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 from typing import Sequence
 from jaxtyping import Float
 import torch
-import chess
+import chess_utils as cu
 
 def decode_file(file: int):
   return chr(file + ord('a'))
 
 def decode_rank(rank: int):
   return str(rank + 1)
 
 def decode_uci(from_file: int, from_rank: int, to_file: int, to_rank: int):
   return decode_file(from_file) + decode_rank(from_rank) + decode_file(to_file) + decode_rank(to_rank)
 
-def decode_ucis(logits: Float[torch.Tensor, 'B L 37']) -> Sequence[Sequence[str]]:
+def argmax_ucis(logits: Float[torch.Tensor, 'B L 37']) -> Sequence[Sequence[str]]:
   batch_size = logits.size(0)
   from_files = torch.argmax(logits[:, :, 0:8].reshape(batch_size, -1, 8), dim=-1)
   from_ranks = torch.argmax(logits[:, :, 8:16].reshape(batch_size, -1, 8), dim=-1)
   to_files = torch.argmax(logits[:, :, 16:24].reshape(batch_size, -1, 8), dim=-1)
   to_ranks = torch.argmax(logits[:, :, 24:32].reshape(batch_size, -1, 8), dim=-1)
   
   return [
     [
       decode_uci(*[int(i.item()) for i in idxs])
       for idxs in zip(from_files[b], from_ranks[b], to_files[b], to_ranks[b])
     ]
     for b in range(batch_size)
   ]
 
-def ucis2pgn(ucis: Sequence[str]) -> Sequence[str]:
-  """Parses UCIs into SAN. Stops whenever it finds an illegal move."""
-  pgn = []
-  board = chess.Board()
-  try:
-    for uci in ucis:
-      move = chess.Move.from_uci(uci)
-      pgn.append(board.san(move))
-      board.push(move)
-  finally:
-    return pgn
-  
-def decode_pgns(logits: Float[torch.Tensor, 'B L 37']) -> Sequence[Sequence[str]]:
-  return [ucis2pgn(ucis) for ucis in decode_ucis(logits)]
+def greedy_pgn(logits: Float[torch.Tensor, 'B L 37']) -> Sequence[Sequence[str]]:
+  return [list(cu.ucis2sans(ucis)) for ucis in argmax_ucis(logits)]
```

