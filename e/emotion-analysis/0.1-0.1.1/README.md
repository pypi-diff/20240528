# Comparing `tmp/emotion_analysis-0.1.tar.gz` & `tmp/emotion_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_analysis-0.1.tar", last modified: Mon May 27 19:51:16 2024, max compression
+gzip compressed data, was "emotion_analysis-0.1.1.tar", last modified: Tue May 28 02:31:27 2024, max compression
```

## Comparing `emotion_analysis-0.1.tar` & `emotion_analysis-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 19:51:16.011077 emotion_analysis-0.1/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      302 2024-05-27 19:51:16.011077 emotion_analysis-0.1/PKG-INFO
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 19:51:16.011077 emotion_analysis-0.1/emotion_analysis/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1/emotion_analysis/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4287 2024-05-27 16:54:30.000000 emotion_analysis-0.1/emotion_analysis/bert_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14768 2024-05-27 16:39:22.000000 emotion_analysis-0.1/emotion_analysis/data_preprocessing.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      901 2024-05-27 19:27:24.000000 emotion_analysis-0.1/emotion_analysis/dataset_upload.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1/emotion_analysis/frnn.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4443 2024-05-27 16:54:17.000000 emotion_analysis-0.1/emotion_analysis/roberta_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1907 2024-05-27 19:16:17.000000 emotion_analysis-0.1/emotion_analysis/tweets_embedding.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 19:51:16.011077 emotion_analysis-0.1/emotion_analysis.egg-info/
--rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      302 2024-05-27 19:51:16.000000 emotion_analysis-0.1/emotion_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      495 2024-05-27 19:51:16.000000 emotion_analysis-0.1/emotion_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-27 19:51:16.000000 emotion_analysis-0.1/emotion_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-27 19:51:16.000000 emotion_analysis-0.1/emotion_analysis.egg-info/requires.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-27 19:51:16.000000 emotion_analysis-0.1/emotion_analysis.egg-info/top_level.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-27 19:51:16.011077 emotion_analysis-0.1/setup.cfg
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      563 2024-05-27 19:49:36.000000 emotion_analysis-0.1/setup.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 19:51:16.011077 emotion_analysis-0.1/tests/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1/tests/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     8271 2024-05-27 17:00:40.000000 emotion_analysis-0.1/tests/test.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/PKG-INFO
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/emotion_analysis/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.1/emotion_analysis/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4287 2024-05-27 16:54:30.000000 emotion_analysis-0.1.1/emotion_analysis/bert_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14768 2024-05-27 16:39:22.000000 emotion_analysis-0.1.1/emotion_analysis/data_preprocessing.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      421 2024-05-28 02:25:32.000000 emotion_analysis-0.1.1/emotion_analysis/dataset_upload.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.1/emotion_analysis/frnn.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4443 2024-05-27 21:14:04.000000 emotion_analysis-0.1.1/emotion_analysis/roberta_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2381 2024-05-28 02:28:21.000000 emotion_analysis-0.1.1/emotion_analysis/tweets_embedding.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/emotion_analysis.egg-info/
+-rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      495 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/requires.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/setup.cfg
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      558 2024-05-28 02:30:56.000000 emotion_analysis-0.1.1/setup.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/tests/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.1/tests/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    10136 2024-05-27 21:13:11.000000 emotion_analysis-0.1.1/tests/test.py
```

### Comparing `emotion_analysis-0.1/emotion_analysis/bert_pcc_score_emotions.py` & `emotion_analysis-0.1.1/emotion_analysis/bert_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1/emotion_analysis/data_preprocessing.py` & `emotion_analysis-0.1.1/emotion_analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1/emotion_analysis/frnn.py` & `emotion_analysis-0.1.1/emotion_analysis/frnn.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1/emotion_analysis/roberta_pcc_score_emotions.py` & `emotion_analysis-0.1.1/emotion_analysis/roberta_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1/emotion_analysis/tweets_embedding.py` & `emotion_analysis-0.1.1/emotion_analysis/tweets_embedding.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 # Define the functions for extracting vector representations
 
 print("TWEETS EMBEDDING BERT AND ROBERTA IMPORT START!")
 
 
 def get_vector_bert(text):
     # Load pre-trained BERT model and tokenizer
-    tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
-    model = BertModel.from_pretrained("bert-base-uncased")
+    tokenizer = BertTokenizer.from_pretrained(
+        "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/emotion_analysis/bert-base-uncased"
+    )
+    model = BertModel.from_pretrained(
+        "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/emotion_analysis/bert-base-uncased"
+    )
 
     # Tokenize input text
     inputs = tokenizer(text, return_tensors="pt", max_length=512, truncation=True)
 
     # Forward pass through BERT model
     with torch.no_grad():
         outputs = model(**inputs)
@@ -43,16 +47,20 @@
     cls_embedding_list = cls_embedding.squeeze().tolist()
 
     return cls_embedding_list
 
 
 def get_vector_roberta(text):
     try:
-        tokenizer = RobertaTokenizer.from_pretrained("twitter-roberta-base-emotion")
-        model = RobertaModel.from_pretrained("twitter-roberta-base-emotion")
+        tokenizer = RobertaTokenizer.from_pretrained(
+            "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/twitter-roberta-base-emotion"
+        )
+        model = RobertaModel.from_pretrained(
+            "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/twitter-roberta-base-emotion"
+        )
         inputs = tokenizer(text, return_tensors="pt", max_length=512, truncation=True)
         with torch.no_grad():
             outputs = model(**inputs)
         cls_embedding = outputs.last_hidden_state[:, 0, :]
         cls_embedding_list = cls_embedding.squeeze()
         return cls_embedding_list.numpy()
     except Exception as e:
```

### Comparing `emotion_analysis-0.1/tests/test.py` & `emotion_analysis-0.1.1/tests/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,38 @@
 from emotion_analysis.data_preprocessing import *
 from emotion_analysis.dataset_upload import *
 from emotion_analysis.tweets_embedding import *
 from emotion_analysis.frnn import *
 from emotion_analysis.bert_pcc_score_emotions import *
 from emotion_analysis.roberta_pcc_score_emotions import *
 
+anger_train, anger_dev, anger_data, anger_test = upload_datasets(
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-anger-dev.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-anger-train.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-anger-test.txt",
+)
+
+fear_train, fear_dev, fear_data, fear_test = upload_datasets(
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-fear-train.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-fear-dev.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-fear-test.txt",
+)
+
+joy_train, joy_dev, joy_data, joy_test = upload_datasets(
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-joy-train.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-joy-dev.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-joy-test.txt",
+)
+
+sad_train, sad_dev, sad_data, sad_test = upload_datasets(
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/EI-oc-En-sadness-train.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-sadness-dev.txt",
+    "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-sadness-test.txt",
+)
+
 
 generate_wordclouds(anger_train, anger_dev, anger_data, anger_test, "Anger")
 plot_statistics(anger_train, anger_dev, anger_data, anger_test, "Anger")
 plot_additional_statistics(anger_train, anger_dev, anger_test, "Anger")
 plot_top_n_words(anger_train, n=20, title="Top 20 Frequent Words in Anger Train Data")
 plot_ngrams_frequency(
     anger_train, n=2, top_n=10, title="Bigram Frequency in Anger Train Data"
```

