# Comparing `tmp/dooc-0.0.1.tar.gz` & `tmp/dooc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dooc-0.0.1.tar", last modified: Fri May 17 08:36:57 2024, max compression
+gzip compressed data, was "dooc-0.0.2.tar", last modified: Tue May 28 12:47:06 2024, max compression
```

## Comparing `dooc-0.0.1.tar` & `dooc-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:57.727938 dooc-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:36:49.000000 dooc-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-17 08:36:57.727938 dooc-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-17 08:36:49.000000 dooc-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:57.723938 dooc-0.0.1/dooc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:57.727938 dooc-0.0.1/dooc/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1396639 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/data/drugcell_ont.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    31866 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/data/gene2ind.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-17 08:36:49.000000 dooc-0.0.1/dooc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:57.727938 dooc-0.0.1/dooc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-17 08:36:57.000000 dooc-0.0.1/dooc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 08:36:57.000000 dooc-0.0.1/dooc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:36:57.000000 dooc-0.0.1/dooc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 08:36:57.000000 dooc-0.0.1/dooc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 08:36:57.000000 dooc-0.0.1/dooc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 08:36:49.000000 dooc-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 08:36:57.727938 dooc-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:36:49.000000 dooc-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:36:57.727938 dooc-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 08:36:49.000000 dooc-0.0.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-17 08:36:49.000000 dooc-0.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 08:36:49.000000 dooc-0.0.1/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-17 08:36:49.000000 dooc-0.0.1/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:47:06.056350 dooc-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 12:46:57.000000 dooc-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-28 12:47:06.056350 dooc-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-28 12:46:57.000000 dooc-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:47:06.052350 dooc-0.0.2/dooc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:46:57.000000 dooc-0.0.2/dooc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 12:46:57.000000 dooc-0.0.2/dooc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:47:06.056350 dooc-0.0.2/dooc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1396639 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/data/drugcell_ont.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31866 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/data/gene2ind.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-28 12:46:58.000000 dooc-0.0.2/dooc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:47:06.056350 dooc-0.0.2/dooc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-28 12:47:06.000000 dooc-0.0.2/dooc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 12:47:06.000000 dooc-0.0.2/dooc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:47:06.000000 dooc-0.0.2/dooc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 12:47:06.000000 dooc-0.0.2/dooc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 12:47:06.000000 dooc-0.0.2/dooc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 12:46:58.000000 dooc-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 12:47:06.056350 dooc-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:46:58.000000 dooc-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:47:06.056350 dooc-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 12:46:58.000000 dooc-0.0.2/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-28 12:46:58.000000 dooc-0.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 12:46:58.000000 dooc-0.0.2/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-28 12:46:58.000000 dooc-0.0.2/tests/test_pipelines.py
```

### Comparing `dooc-0.0.1/LICENSE` & `dooc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/PKG-INFO` & `dooc-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dooc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Digtal Organoid On Chips
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,organoid,AI,deep learning,transformer,drug response,mutations
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: moltx~=1.0.2
+Requires-Dist: moltx~=1.0.4
 Requires-Dist: networkx~=3.1
 Requires-Dist: scikit-learn~=1.3.0
 
 # DOoC
 
 ## Usage
```

### Comparing `dooc-0.0.1/README.md` & `dooc-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/dooc/data/drugcell_ont.txt` & `dooc-0.0.2/dooc/data/drugcell_ont.txt`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/dooc/data/gene2ind.txt` & `dooc-0.0.2/dooc/data/gene2ind.txt`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/dooc/datasets.py` & `dooc-0.0.2/dooc/datasets.py`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/dooc/models.py` & `dooc-0.0.2/dooc/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -45,56 +45,61 @@
 
 
 class MutSmiXAttention(MutSmi):
     """Regression model using transformer cross attention."""
 
     def __init__(
         self,
-        d_model: int,
+        nhead: int = 2,
+        num_layers: int = 2,
         gene_conf: nets.GeneGNNConfig = nets.GeneGNN.DEFAULT_CONFIG,
         smiles_conf: AbsPosEncoderDecoderConfig = AdaMR.CONFIG_BASE,
     ) -> None:
         super().__init__(gene_conf, smiles_conf)
-        self.d_model = d_model
+        d_model = self.smiles_conf.d_model
+        d_hidden = d_model // 2
+        layer = nn.TransformerDecoderLayer(d_model, nhead, batch_first=True)
+        self.cross_att = nn.TransformerDecoder(layer, num_layers)
+        self.reg = nn.Sequential(
+            nn.Linear(d_model, d_hidden),
+            nn.ReLU(),
+            nn.Dropout(0.1),
+            nn.Linear(d_hidden, 1),
+        )
 
     def forward(
         self, smiles_src: torch.Tensor, smiles_tgt: torch.Tensor, gene_src: torch.Tensor
     ) -> torch.Tensor:
-        pass
+        smiles_out = self.smiles_encoder.forward_feature(smiles_src, smiles_tgt).unsqueeze(-2)  # [b, 1, dmodel]
+        gene_out = self.gene_encoder(gene_src).unsqueeze(-2)  # [b, 1, dmodel]
+
+        feat = self.cross_att(smiles_out, gene_out)  # [b, 1, dmodel]
+
+        return self.reg(feat.squeeze(-2))  # [b, 1]
 
 
 class MutSmiFullConnection(MutSmi):
     """Regression model using fully connection."""
 
     def __init__(
         self,
-        d_model: int,
         gene_conf: nets.GeneGNNConfig = nets.GeneGNN.DEFAULT_CONFIG,
         smiles_conf: AbsPosEncoderDecoderConfig = AdaMR.CONFIG_BASE,
     ) -> None:
         super().__init__(gene_conf, smiles_conf)
-        self.d_model = d_model
-
+        d_model = self.smiles_conf.d_model
         d_hidden = d_model // 2
-        self.gene_fc = nn.Linear(self.gene_conf.num_hiddens_genotype, self.d_model)
         self.reg = nn.Sequential(
-            nn.Linear(self.d_model, d_hidden),
+            nn.Linear(d_model, d_hidden),
             nn.ReLU(),
             nn.Dropout(0.1),
             nn.Linear(d_hidden, 1),
         )
 
     def forward(
         self, smiles_src: torch.Tensor, smiles_tgt: torch.Tensor, gene_src: torch.Tensor
     ) -> torch.Tensor:
-        is_batched = smiles_src.dim() == 2
-
-        smiles_out = self.smiles_encoder.forward_feature(smiles_src, smiles_tgt)
-        gene_out = self.gene_encoder(gene_src).unsqueeze(1)
-
-        feat = None
-        if is_batched:
-            feat = smiles_out + self.gene_fc(gene_out)[:, 0]
-        else:
-            feat = smiles_out[0] + self.gene_fc(gene_out)[0]
+        smiles_out = self.smiles_encoder.forward_feature(smiles_src, smiles_tgt)  # [b, dmodel]
+        gene_out = self.gene_encoder(gene_src)  # [b, dmodel]
+        feat = smiles_out + gene_out
 
-        return self.reg(feat)
+        return self.reg(feat)  # [b, 1]
```

### Comparing `dooc-0.0.1/dooc/nets.py` & `dooc-0.0.2/dooc/nets.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from torch import nn
 from dataclasses import dataclass
 from dooc.utils import load_gene_mapping, load_ontology
 
 
 @dataclass
 class GeneGNNConfig:
+    d_model: int
     gene_dim: int
     drug_dim: int
     num_hiddens_genotype: int
     num_hiddens_drug: list
     num_hiddens_final: int
     gene2ind_path: str
     ont_path: str
@@ -20,39 +21,43 @@
     """GNN for mutations embeddings.
 
     reference: https://github.com/idekerlab/DrugCell/
 
     """
 
     DEFAULT_CONFIG = GeneGNNConfig(
+        d_model=768,
         gene_dim=3008,
         drug_dim=2048,
         num_hiddens_genotype=6,
         num_hiddens_drug=[100, 50, 6],
         num_hiddens_final=6,
         gene2ind_path=os.path.join(os.path.dirname(__file__), "data", "gene2ind.txt"),
         ont_path=os.path.join(os.path.dirname(__file__), "data", "drugcell_ont.txt"),
     )
 
     def __init__(self, conf: GeneGNNConfig = DEFAULT_CONFIG) -> None:
         super().__init__()
         self.conf = conf
+        d_model = self.conf.d_model
 
         dg, dg_root, term_size_map, term_direct_gene_map = self._get_params()
         self.dg, self.dg_root = dg, dg_root
         self.term_size_map, self.term_direct_gene_map = (
             term_size_map,
             term_direct_gene_map,
         )
 
         self._cal_term_dim()
         self._contruct_direct_gene_layer()
         self._construct_nn_graph()
         self._construct_nn_drug()
         self._construct_final_layer()
+        self.out_fc = nn.Linear(self.conf.num_hiddens_genotype,
+                                d_model)
 
     def _contruct_direct_gene_layer(self):
         """
         build a layer for forwarding gene that are directly annotated with the term
         """
         for term, gene_set in self.term_direct_gene_map.items():
             if len(gene_set) == 0:
@@ -177,15 +182,16 @@
             torch.load(ckpt_files[0], map_location=torch.device("cpu")), strict=False
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         removed drug layer
         """
-
+        x_dim = x.dim()
+        x = x.unsqueeze(0) if x_dim == 1 else x
         gene_input = x.narrow(1, 0, self.conf.gene_dim)
         # drug_input = x.narrow(1, self.conf.gene_dim, self.conf.drug_dim)
 
         # define forward function for genotype dcell #############################################
         term_gene_out_map = {}
 
         for term, _ in self.term_direct_gene_map.items():
@@ -219,8 +225,12 @@
                 aux_layer1_out = torch.tanh(
                     self._modules[term + "_aux_linear_layer1"](term_nn_out_map[term])
                 )
                 aux_out_map[term] = self._modules[term + "_aux_linear_layer2"](
                     aux_layer1_out
                 )
 
-        return term_nn_out_map[self.dg_root]
+        out = term_nn_out_map[self.dg_root]
+        out = self.out_fc(out)
+        if x_dim == 1:
+            out = out.squeeze(0)
+        return out
```

### Comparing `dooc-0.0.1/dooc/pipelines.py` & `dooc-0.0.2/dooc/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         smi_tokenizer: tokenizers.MoltxTokenizer,
         model: models.MutSmiXAttention,
         device: torch.device = torch.device("cpu"),
     ) -> None:
         super().__init__(smi_tokenizer, model, device)
 
     def __call__(self, gene: typing.Sequence[int], smiles: str) -> float:
-        return
+        smi_src, smi_tgt, gene_src = self._model_args(gene, smiles)
+        pred = self.model(smi_src, smi_tgt, gene_src)
+        return pred.item()
 
 
 class MutSmiFullConnection(MutSmi):
     def __init__(
         self,
         smi_tokenizer: tokenizers.MoltxTokenizer,
         model: models.MutSmiFullConnection,
```

### Comparing `dooc-0.0.1/dooc/utils.py` & `dooc-0.0.2/dooc/utils.py`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/dooc.egg-info/PKG-INFO` & `dooc-0.0.2/dooc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dooc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Digtal Organoid On Chips
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,organoid,AI,deep learning,transformer,drug response,mutations
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: moltx~=1.0.2
+Requires-Dist: moltx~=1.0.4
 Requires-Dist: networkx~=3.1
 Requires-Dist: scikit-learn~=1.3.0
 
 # DOoC
 
 ## Usage
```

### Comparing `dooc-0.0.1/setup.cfg` & `dooc-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dooc-0.0.1/tests/test_datasets.py` & `dooc-0.0.2/tests/test_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 from moltx.models import AdaMRTokenizerConfig
 
 
 def test_MutSmi():
     return
 
 
-# def test_MutSmiXAttention():
-#     tokenizer = tkz.MoltxTokenizer.from_pretrain(
-#         conf=AdaMRTokenizerConfig.Prediction
-#         )
-#     ds = datasets.MutSmiXAttention(tokenizer)
-#     smiles = ["CC[N+]CCBr", "Cc1ccc1"]
-#     values = [0.88, 0.89]
-#     mutations = [[random.choice([0, 1]) for _ in range(3008)],
-#                  [random.choice([0, 1]) for _ in range(3008)]]
-#     with pytest.raises(RuntimeError):
-#         ds(smiles, mutations, values[:1])
-#     smiles_src, smiles_tgt, mutations_src, out = ds(smiles,
-#                                                     mutations,
-#                                                     values)
-#     assert smiles_src.shape == (2, 4)
-#     assert smiles_tgt.shape == (2, 6)
-#     assert mutations_src.shape == (2, 3008)
-#     assert out.shape == (2, 1)
+def test_MutSmiXAttention():
+    tokenizer = tkz.MoltxTokenizer.from_pretrain(
+        conf=AdaMRTokenizerConfig.Prediction
+        )
+    ds = datasets.MutSmiXAttention(tokenizer)
+    smiles = ["CC[N+]CCBr", "Cc1ccc1"]
+    values = [0.88, 0.89]
+    mutations = [[random.choice([0, 1]) for _ in range(3008)],
+                 [random.choice([0, 1]) for _ in range(3008)]]
+    with pytest.raises(RuntimeError):
+        ds(smiles, mutations, values[:1])
+    smiles_src, smiles_tgt, mutations_src, out = ds(smiles,
+                                                    mutations,
+                                                    values)
+    assert smiles_src.shape == (2, 200)
+    assert smiles_tgt.shape == (2, 200)
+    assert mutations_src.shape == (2, 3008)
+    assert out.shape == (2, 1)
 
 
 def test_MutSmiFullConnection():
     tokenizer = tkz.MoltxTokenizer.from_pretrain(
         conf=AdaMRTokenizerConfig.Prediction
         )
     ds = datasets.MutSmiFullConnection(tokenizer)
```

### Comparing `dooc-0.0.1/tests/test_pipelines.py` & `dooc-0.0.2/tests/test_pipelines.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 import random
-from dooc import pipelines, models, nets
+from dooc import pipelines, models
 from moltx import tokenizers as tkz
 from moltx.models import AdaMRTokenizerConfig
 
  
-# def test_MutSmiXAttention():
-#     tokenizer = tkz.MoltxTokenizer.from_pretrain(
-#         conf=AdaMRTokenizerConfig.Prediction
-#         )
-#     d_model = 768
-#     model = models.MutSmiXAttention(d_model)
-#     model.load_ckpt('/path/to/mutsmixattention.ckpt')
-#     pipeline = pipelines.MutSmiXAttention(tokenizer, model)
-#     mutation = [random.choice([1, 0]) for _ in range(3008)]
-#     smiles = "CC[N+](C)(C)Cc1ccccc1Br"
-#     predict = pipeline(mutation, smiles)
-#     assert isinstance(predict, float)
+def test_MutSmiXAttention():
+    tokenizer = tkz.MoltxTokenizer.from_pretrain(
+        conf=AdaMRTokenizerConfig.Prediction
+        )
+    model = models.MutSmiXAttention()
+    # model.load_ckpt('/path/to/mutsmixattention.ckpt')
+    pipeline = pipelines.MutSmiXAttention(smi_tokenizer=tokenizer,
+                                          model=model)
+    mutation = [random.choice([1, 0]) for _ in range(3008)]
+    smiles = "CC[N+](C)(C)Cc1ccccc1Br"
+    predict = pipeline(mutation, smiles)
+    assert isinstance(predict, float)
 
 
-def test_MutSmiFullConnection(datadir):
+def test_MutSmiFullConnection():
     tokenizer = tkz.MoltxTokenizer.from_pretrain(
         conf=AdaMRTokenizerConfig.Prediction
         )
-    d_model = 768
-    gene_conf = nets.GeneGNNConfig(
-        gene_dim=3008,
-        drug_dim=2048,
-        num_hiddens_genotype=6,
-        num_hiddens_drug=[100, 50, 6],
-        num_hiddens_final=6,
-        gene2ind_path=f"{datadir}/gene2ind.txt",
-        ont_path=f"{datadir}/drugcell_ont.txt",
-    )
-    model = models.MutSmiFullConnection(d_model, gene_conf)
+    model = models.MutSmiFullConnection()
     # model.load_ckpt('/path/to/mutsmifullconnection.ckpt')
     pipeline = pipelines.MutSmiFullConnection(smi_tokenizer=tokenizer,
                                               model=model)
-    mutation = [[random.choice([1, 0]) for _ in range(3008)]]
+    mutation = [random.choice([1, 0]) for _ in range(3008)]
     smiles = "CC[N+](C)(C)Cc1ccccc1Br"
     predict = pipeline(mutation, smiles)
     assert isinstance(predict, float)
```

