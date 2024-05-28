# Comparing `tmp/nlpx-1.2.1.tar.gz` & `tmp/nlpx-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.1.tar", last modified: Mon May 27 13:23:47 2024, max compression
+gzip compressed data, was "nlpx-1.2.2.tar", last modified: Mon May 27 13:49:47 2024, max compression
```

## Comparing `nlpx-1.2.1.tar` & `nlpx-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.653709 nlpx-1.2.1/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:23:47.652850 nlpx-1.2.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.626460 nlpx-1.2.1/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.1/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.633610 nlpx-1.2.1/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.1/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5886 2024-05-27 13:23:10.000000 nlpx-1.2.1/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.1/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.637465 nlpx-1.2.1/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.1/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.1/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.646211 nlpx-1.2.1/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.1/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.1/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.1/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3901 2024-05-27 13:08:01.000000 nlpx-1.2.1/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.630632 nlpx-1.2.1/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.1/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 13:23:47.654141 nlpx-1.2.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 13:23:44.000000 nlpx-1.2.1/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.650649 nlpx-1.2.1/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.1/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.575600 nlpx-1.2.2/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:49:47.574928 nlpx-1.2.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.548151 nlpx-1.2.2/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.2/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.556965 nlpx-1.2.2/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.2/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5886 2024-05-27 13:23:10.000000 nlpx-1.2.2/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.2/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.561129 nlpx-1.2.2/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.2/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.2/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.569635 nlpx-1.2.2/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.2/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.2/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.2/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3857 2024-05-27 13:49:43.000000 nlpx-1.2.2/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.552550 nlpx-1.2.2/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.2/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 13:49:47.000000 nlpx-1.2.2/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 13:49:47.575844 nlpx-1.2.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 13:49:43.000000 nlpx-1.2.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:49:47.572360 nlpx-1.2.2/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.2/test/test.py
```

### Comparing `nlpx-1.2.1/PKG-INFO` & `nlpx-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.1
+Version: 1.2.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.1/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.2/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.1/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.2/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.1/nlpx/models/_text_cnn.py` & `nlpx-1.2.2/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.1/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.2/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.1/nlpx/text_token/_utils.py` & `nlpx-1.2.2/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.1/nlpx/training.py` & `nlpx-1.2.2/nlpx/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,27 @@
 			val_loss, val_acc = evaluate(self.model, self.eval_loader, self.device)
 			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
 			if val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
-
-			if val_acc >= best_acc:  # val_acc提升
 				cnt = 0
 
+			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) > self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
+				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
+				break
+
 			if last_acc == val_acc:  # val_acc不在变化
 				cnt2 += 1
 			else:
 				cnt2 = 0
 
 			last_acc = val_acc
 			cnt += 1
-			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) > self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
-				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
-				break
 
 		return best_model
 
 
 class SimpleTrainer(Trainer):
 
 	def __init__(self, model, X, y, eval_size=0.2, random_state=None, collate_fn=None,
```

### Comparing `nlpx-1.2.1/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.2/nlpx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.1
+Version: 1.2.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.1/setup.py` & `nlpx-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.1',
+    version='1.2.2',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

