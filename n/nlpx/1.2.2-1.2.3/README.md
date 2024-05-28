# Comparing `tmp/nlpx-1.2.2.tar.gz` & `tmp/nlpx-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.2.tar", last modified: Mon May 27 13:49:47 2024, max compression
+gzip compressed data, was "nlpx-1.2.3.tar", last modified: Tue May 28 05:09:46 2024, max compression
```

## Comparing `nlpx-1.2.2.tar` & `nlpx-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.575600 nlpx-1.2.2/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:49:47.574928 nlpx-1.2.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.548151 nlpx-1.2.2/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.2/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.556965 nlpx-1.2.2/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.2/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5886 2024-05-27 13:23:10.000000 nlpx-1.2.2/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.2/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.561129 nlpx-1.2.2/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.2/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.2/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.569635 nlpx-1.2.2/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.2/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.2/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.2/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3857 2024-05-27 13:49:43.000000 nlpx-1.2.2/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.552550 nlpx-1.2.2/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.2/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 13:49:47.575844 nlpx-1.2.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 13:49:43.000000 nlpx-1.2.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.572360 nlpx-1.2.2/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.2/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.232011 nlpx-1.2.3/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 05:09:46.231466 nlpx-1.2.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.204450 nlpx-1.2.3/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.3/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.217626 nlpx-1.2.3/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.3/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     6384 2024-05-28 01:52:12.000000 nlpx-1.2.3/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.3/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.220594 nlpx-1.2.3/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.3/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 01:38:11.000000 nlpx-1.2.3/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.226512 nlpx-1.2.3/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.3/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.3/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.3/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3977 2024-05-28 04:51:13.000000 nlpx-1.2.3/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.213017 nlpx-1.2.3/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.3/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 05:09:46.232224 nlpx-1.2.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 05:09:41.000000 nlpx-1.2.3/setup.py
```

### Comparing `nlpx-1.2.2/PKG-INFO` & `nlpx-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.2
+Version: 1.2.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.2/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.3/nlpx/llm/_model_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,67 +78,73 @@
 		self.tokenize_vec = tokenize_vec
 
 	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 			  batch_size=8, eval_batch_size=16,
 			  num_workers=4, num_eval_workers=2,
-			  early_stopping_rounds=10):
+			  early_stopping_rounds=10, n_jobs=-1):
 		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
+		X = self.get_vec(texts, max_length=max_length, n_jobs=n_jobs)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		trainer = SimpleTrainer(model, X, y, eval_size, random_state, collate_fn,
 								 max_iter, optimizer, learning_rate, T_max,
 								 batch_size, eval_batch_size,
 								 num_workers, num_eval_workers,
 								 early_stopping_rounds,
 								 self.device)
 		self.model = trainer.train()
 
-	def predict(self, texts: List[str], max_length: int = 0):
-		logits = self.logits(texts, max_length)
+	def predict(self, texts: List[str], max_length: int = 0, n_jobs=0):
+		logits = self.logits(texts, max_length, n_jobs=n_jobs)
 		return logits.argmax(1)
 
-	def predict_classes(self, texts: List[str], max_length: int = 0):
+	def predict_classes(self, texts: List[str], max_length: int = 0, n_jobs=0):
 		assert self.classes is not None, 'classes must be specified'
-		pred = self.predict(texts, max_length)
+		pred = self.predict(texts, max_length, n_jobs=n_jobs)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 	
-	def predict_proba(self, texts: List[str], max_length: int = 0):
-		logits = self.logits(texts, max_length)
+	def predict_proba(self, texts: List[str], max_length: int = 0, n_jobs=0):
+		logits = self.logits(texts, max_length, n_jobs=n_jobs)
 		result = F.softmax(logits).max(1)
 		return result.indices, result.values
 
-	def predict_classes_proba(self, texts: List[str], max_length: int = 0):
+	def predict_classes_proba(self, texts: List[str], max_length: int = 0, n_jobs=0):
 		assert self.classes is not None, 'classes must be specified'
 		logits = self.logits(texts, max_length)
 		result = F.softmax(logits, dim=1).max(1)
 		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
 
-	def logits(self, texts: List[str], max_length: int = 0):
-		X = self.get_features(texts, max_length)
+	def logits(self, texts: List[str], max_length: int = 0, n_jobs=-1):
+		X = self.get_features(texts, max_length, n_jobs=n_jobs)
 		return super().logits(X)
 
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
-				 max_length: int = 0, collate_fn=None):
-		X = self.get_features(texts, max_length)
+				 max_length: int = 0, collate_fn=None, n_jobs=0):
+		X = self.get_features(texts, max_length, n_jobs=n_jobs)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
 	@staticmethod
 	def get_max_length(texts: List[str], max_length: int = 0) -> int:
 		if max_length and max_length > 0:
 			return max_length
 		return get_texts_max_length(texts, cut_type='char')
 
-	def get_vec(self, texts: List[str], max_length: int):
-		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
-														truncation=True, add_special_tokens=True,
-														return_token_type_ids=True,return_attention_mask=True,
-														return_tensors='pt')
+	def get_vec(self, texts: List[str], max_length: int, n_jobs: int):
+		if n_jobs == 0:
+			return self.tokenize_vec.encode_plus(texts, max_length=max_length, padding='max_length',
+												  truncation=True, add_special_tokens=True,
+												  return_token_type_ids=True, return_attention_mask=True,
+												  return_tensors='pt')
+		else:
+			return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
+															truncation=True, add_special_tokens=True,
+															return_token_type_ids=True,return_attention_mask=True,
+															return_tensors='pt', n_jobs=n_jobs)
 
-	def get_features(self, texts: List[str], max_length: int = 0):
+	def get_features(self, texts: List[str], max_length: int = 0, n_jobs=0):
 		max_length = self.get_max_length(texts, max_length)
-		return self.get_vec(texts, max_length=max_length)
+		return self.get_vec(texts, max_length=max_length, n_jobs=n_jobs)
```

### Comparing `nlpx-1.2.2/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.3/nlpx/llm/_tokenize_vec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import torch
 from pathlib import Path
 from joblib import Parallel, delayed
 from typing import Union, List, Optional
-from transformers import BertTokenizer, BertConfig, BertModel, AutoModel
+from transformers import BertTokenizer, BertConfig, BertModel, AlbertConfig, AlbertModel, ErnieConfig, ErnieModel
 from transformers.tokenization_utils import PaddingStrategy, TruncationStrategy, TensorType
 
 
 class TokenizeVec:
 
-	def __init__(self, pretrained_path: Union[str, Path]):
+	def __init__(self, pretrained_path: Union[str, Path], tokenizer=BertTokenizer):
+		self.config = None
 		self.pretrained = None
-		self.tokenizer = BertTokenizer.from_pretrained(pretrained_path)
+		self.tokenizer = tokenizer.from_pretrained(pretrained_path)
+
+	@property
+	def hidden_size(self):
+		assert self.config is not None, "config must not be None"
+		return self.config.hidden_size
 
 	def encode_plus(self,
 				texts: List[str],
 				add_special_tokens: bool = True,
 				padding: Union[bool, str, PaddingStrategy] = False,
 				truncation: Union[bool, str, TruncationStrategy] = None,
 				max_length: Optional[int] = None,
@@ -241,16 +247,25 @@
 							)
 
 
 class BertTokenizeVec(TokenizeVec):
 
 	def __init__(self, pretrained_path: Union[str, Path]):
 		super().__init__(pretrained_path)
-		bert_config = BertConfig.from_pretrained(pretrained_path)
-		self.pretrained = BertModel.from_pretrained(pretrained_path, config=bert_config)
+		self.config = BertConfig.from_pretrained(pretrained_path)
+		self.pretrained = BertModel.from_pretrained(pretrained_path, config=self.config)
+
+
+class AlbertTokenizeVec(TokenizeVec):
+
+	def __init__(self, pretrained_path: Union[str, Path]):
+		super().__init__(pretrained_path)
+		self.config = AlbertConfig.from_pretrained(pretrained_path)
+		self.pretrained = AlbertModel.from_pretrained(pretrained_path, config=self.config)
 
 
 class ErnieTokenizeVec(TokenizeVec):
 
 	def __init__(self, pretrained_path: Union[str, Path]):
 		super().__init__(pretrained_path)
-		self.pretrained = AutoModel.from_pretrained(pretrained_path)
+		self.config = ErnieConfig.from_pretrained(pretrained_path)
+		self.pretrained = ErnieModel.from_pretrained(pretrained_path, config=self.config)
```

### Comparing `nlpx-1.2.2/nlpx/models/_text_cnn.py` & `nlpx-1.2.3/nlpx/models/_text_cnn.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
     def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels: int = 64, out_features: int = 2,
-                 activation=nn.ReLU(inplace=True), num_hidden_layer: int = 0, drop_out: float = 0.0):
+                 activation=nn.ReLU(inplace=True), num_hidden_layer: int = 0, batch_norm=False, layer_norm=False,
+                 drop_out: float = 0.0):
         """ TextCNN model
         Parameters
         ----------
         word_dim: int, dim of word, in_channels of cnn
         cnn_channels: int, out_channels of cnn
         kernel_sizes: size of each cnn kernel
         out_features: dim of output
@@ -25,33 +26,50 @@
         >>> X = torch.randn(batch_size, 10, word_dim)
         >>> targets = torch.randint(0, num_classes, (batch_size,))
         >>> model = TextCNN(word_dim, cnn_channels=64, kernel_sizes=(2, 3, 4), out_features=num_classes)
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
         super().__init__()
-        self.convs = nn.ModuleList([
-            nn.Sequential(
-                nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
-                nn.BatchNorm1d(num_features=cnn_channels),
-                activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
-                nn.AdaptiveMaxPool1d(1)
-            ) for kernel_size in kernel_sizes
-        ])
+        if batch_norm:
+            self.convs = nn.ModuleList([
+                nn.Sequential(
+                    nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                    nn.BatchNorm1d(num_features=cnn_channels),
+                    activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
+                    nn.AdaptiveMaxPool1d(1)
+                ) for kernel_size in kernel_sizes
+            ])
+        else:
+            self.convs = nn.ModuleList([
+                nn.Sequential(
+                    nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
+                    activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
+                    nn.AdaptiveMaxPool1d(1)
+                ) for kernel_size in kernel_sizes
+            ])
 
         self.num_hidden_layer = num_hidden_layer
         num_features = cnn_channels * len(kernel_sizes)
         if num_hidden_layer and num_hidden_layer > 0:
-            self.hidden_layers = nn.ModuleList([
-                nn.Sequential(
-                    nn.Linear(in_features=num_features, out_features=num_features),
-                    nn.LayerNorm(normalized_shape=num_features),
-                    activation
-                ) for _ in range(num_hidden_layer)
-            ])
+            if layer_norm:
+                self.hidden_layers = nn.ModuleList([
+                    nn.Sequential(
+                        nn.Linear(in_features=num_features, out_features=num_features),
+                        nn.LayerNorm(normalized_shape=num_features),
+                        activation
+                    ) for _ in range(num_hidden_layer)
+                ])
+            else:
+                self.hidden_layers = nn.ModuleList([
+                    nn.Sequential(
+                        nn.Linear(in_features=num_features, out_features=num_features),
+                        activation
+                    ) for _ in range(num_hidden_layer)
+                ])
 
         self.fc = nn.Linear(in_features=num_features, out_features=out_features)
         if 0.0 < drop_out < 1.0:
             self.fc = nn.Sequential(
                 nn.Dropout(drop_out),
                 self.fc
             )
```

### Comparing `nlpx-1.2.2/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.3/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.2/nlpx/text_token/_utils.py` & `nlpx-1.2.3/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.2/nlpx/training.py` & `nlpx-1.2.3/nlpx/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 		self.device = device
 
 	def train(self):
 		cnt = 0
 		cnt2 = 0
 		best_acc = 0.0
 		last_acc = 0.0
+		min_loss = 100.0
 		best_model = None
 		if self.T_max and self.T_max > 0:
 			scheduler = CosineAnnealingLR(self.optimizer, T_max=self.T_max)
 		for epoch in range(self.max_iter):
 			total = 0.0
 			losses = 0.0
 			correct = 0.0
@@ -66,18 +67,21 @@
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = evaluate(self.model, self.eval_loader, self.device)
 			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
-			if val_acc > best_acc:
+			if val_acc > best_acc or (val_acc == best_acc and val_loss < min_loss):
 				best_acc = val_acc
 				best_model = self.model
 				cnt = 0
+				cnt2 = 0
+
+			min_loss = min(min_loss, val_loss)
 
 			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) > self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
 			if last_acc == val_acc:  # val_acc不在变化
 				cnt2 += 1
```

### Comparing `nlpx-1.2.2/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.3/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.2
+Version: 1.2.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.2/setup.py` & `nlpx-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.2',
+    version='1.2.3',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

