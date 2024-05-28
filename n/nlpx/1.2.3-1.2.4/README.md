# Comparing `tmp/nlpx-1.2.3.tar.gz` & `tmp/nlpx-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.3.tar", last modified: Tue May 28 05:09:46 2024, max compression
+gzip compressed data, was "nlpx-1.2.4.tar", last modified: Tue May 28 13:58:19 2024, max compression
```

## Comparing `nlpx-1.2.3.tar` & `nlpx-1.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.232011 nlpx-1.2.3/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 05:09:46.231466 nlpx-1.2.3/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.3/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.204450 nlpx-1.2.3/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.3/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.217626 nlpx-1.2.3/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.3/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     6384 2024-05-28 01:52:12.000000 nlpx-1.2.3/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.3/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.220594 nlpx-1.2.3/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.3/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 01:38:11.000000 nlpx-1.2.3/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.226512 nlpx-1.2.3/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.3/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.3/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.3/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3977 2024-05-28 04:51:13.000000 nlpx-1.2.3/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 05:09:46.213017 nlpx-1.2.3/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.3/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 05:09:46.000000 nlpx-1.2.3/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 05:09:46.232224 nlpx-1.2.3/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 05:09:41.000000 nlpx-1.2.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.248755 nlpx-1.2.4/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 13:58:19.248063 nlpx-1.2.4/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.4/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.218073 nlpx-1.2.4/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.4/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.228086 nlpx-1.2.4/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.4/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     6384 2024-05-28 01:52:12.000000 nlpx-1.2.4/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.4/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.232347 nlpx-1.2.4/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.4/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.4/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.239973 nlpx-1.2.4/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.4/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.4/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.4/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.4/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.222675 nlpx-1.2.4/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 13:58:19.249003 nlpx-1.2.4/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 13:58:13.000000 nlpx-1.2.4/setup.py
```

### Comparing `nlpx-1.2.3/PKG-INFO` & `nlpx-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.3
+Version: 1.2.4
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.3/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.4/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.3/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.4/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.3/nlpx/models/_text_cnn.py` & `nlpx-1.2.4/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.3/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.4/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.3/nlpx/text_token/_utils.py` & `nlpx-1.2.4/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.3/nlpx/training.py` & `nlpx-1.2.4/nlpx/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,34 +67,36 @@
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = evaluate(self.model, self.eval_loader, self.device)
 			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
+
 			if val_acc > best_acc or (val_acc == best_acc and val_loss < min_loss):
 				best_acc = val_acc
 				best_model = self.model
 				cnt = 0
 				cnt2 = 0
-
-			min_loss = min(min_loss, val_loss)
+				last_acc = val_acc
+				min_loss = min(min_loss, val_loss)
+				continue
 
 			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) > self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
 			if last_acc == val_acc:  # val_acc不在变化
 				cnt2 += 1
 			else:
 				cnt2 = 0
 
-			last_acc = val_acc
 			cnt += 1
-
+			last_acc = val_acc
+			min_loss = min(min_loss, val_loss)
 		return best_model
 
 
 class SimpleTrainer(Trainer):
 
 	def __init__(self, model, X, y, eval_size=0.2, random_state=None, collate_fn=None,
 				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
```

### Comparing `nlpx-1.2.3/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.4/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.3
+Version: 1.2.4
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.3/setup.py` & `nlpx-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.3',
+    version='1.2.4',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

