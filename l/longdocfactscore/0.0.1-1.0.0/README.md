# Comparing `tmp/longdocfactscore-0.0.1.tar.gz` & `tmp/longdocfactscore-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longdocfactscore-0.0.1.tar", last modified: Fri May 24 15:50:58 2024, max compression
+gzip compressed data, was "longdocfactscore-1.0.0.tar", last modified: Tue May 28 08:45:41 2024, max compression
```

## Comparing `longdocfactscore-0.0.1.tar` & `longdocfactscore-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-24 15:50:58.854306 longdocfactscore-0.0.1/
--rw-r--r--   0 User       (501) staff       (20)     1062 2023-09-21 17:25:00.000000 longdocfactscore-0.0.1/LICENSE
--rw-r--r--   0 User       (501) staff       (20)     4570 2024-05-24 15:50:58.853167 longdocfactscore-0.0.1/PKG-INFO
--rw-r--r--   0 User       (501) staff       (20)     3820 2024-05-24 15:41:55.000000 longdocfactscore-0.0.1/README.md
--rw-r--r--   0 User       (501) staff       (20)      699 2024-05-24 04:49:31.000000 longdocfactscore-0.0.1/pyproject.toml
--rw-r--r--   0 User       (501) staff       (20)       38 2024-05-24 15:50:58.854659 longdocfactscore-0.0.1/setup.cfg
--rw-r--r--   0 User       (501) staff       (20)       92 2024-05-24 04:49:31.000000 longdocfactscore-0.0.1/setup.py
-drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-24 15:50:58.722223 longdocfactscore-0.0.1/src/
-drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-24 15:50:58.829840 longdocfactscore-0.0.1/src/longdocfactscore/
--rw-r--r--   0 User       (501) staff       (20)     5877 2024-05-24 04:49:32.000000 longdocfactscore-0.0.1/src/longdocfactscore/ldfacts.py
-drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-24 15:50:58.851623 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/
--rw-r--r--   0 User       (501) staff       (20)     4570 2024-05-24 15:50:58.000000 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/PKG-INFO
--rw-r--r--   0 User       (501) staff       (20)      292 2024-05-24 15:50:58.000000 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/SOURCES.txt
--rw-r--r--   0 User       (501) staff       (20)        1 2024-05-24 15:50:58.000000 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/dependency_links.txt
--rw-r--r--   0 User       (501) staff       (20)       59 2024-05-24 15:50:58.000000 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/requires.txt
--rw-r--r--   0 User       (501) staff       (20)       17 2024-05-24 15:50:58.000000 longdocfactscore-0.0.1/src/longdocfactscore.egg-info/top_level.txt
+drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-28 08:45:41.786896 longdocfactscore-1.0.0/
+-rw-r--r--   0 User       (501) staff       (20)     1062 2023-09-21 17:25:00.000000 longdocfactscore-1.0.0/LICENSE
+-rw-r--r--   0 User       (501) staff       (20)     4788 2024-05-28 08:45:41.785423 longdocfactscore-1.0.0/PKG-INFO
+-rw-r--r--   0 User       (501) staff       (20)     4038 2024-05-28 08:43:22.000000 longdocfactscore-1.0.0/README.md
+-rw-r--r--   0 User       (501) staff       (20)      699 2024-05-28 08:39:53.000000 longdocfactscore-1.0.0/pyproject.toml
+-rw-r--r--   0 User       (501) staff       (20)       38 2024-05-28 08:45:41.787978 longdocfactscore-1.0.0/setup.cfg
+-rw-r--r--   0 User       (501) staff       (20)       92 2024-05-24 04:49:31.000000 longdocfactscore-1.0.0/setup.py
+drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-28 08:45:41.707348 longdocfactscore-1.0.0/src/
+drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-28 08:45:41.755505 longdocfactscore-1.0.0/src/longdocfactscore/
+-rw-r--r--   0 User       (501) staff       (20)     6093 2024-05-28 08:39:25.000000 longdocfactscore-1.0.0/src/longdocfactscore/ldfacts.py
+drwxr-xr-x   0 User       (501) staff       (20)        0 2024-05-28 08:45:41.782717 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/
+-rw-r--r--   0 User       (501) staff       (20)     4788 2024-05-28 08:45:41.000000 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/PKG-INFO
+-rw-r--r--   0 User       (501) staff       (20)      292 2024-05-28 08:45:41.000000 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/SOURCES.txt
+-rw-r--r--   0 User       (501) staff       (20)        1 2024-05-28 08:45:41.000000 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/dependency_links.txt
+-rw-r--r--   0 User       (501) staff       (20)       59 2024-05-28 08:45:41.000000 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/requires.txt
+-rw-r--r--   0 User       (501) staff       (20)       17 2024-05-28 08:45:41.000000 longdocfactscore-1.0.0/src/longdocfactscore.egg-info/top_level.txt
```

### Comparing `longdocfactscore-0.0.1/LICENSE` & `longdocfactscore-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `longdocfactscore-0.0.1/PKG-INFO` & `longdocfactscore-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longdocfactscore
-Version: 0.0.1
+Version: 1.0.0
 Summary: LongDocFACTScore: A framework for evaluating factual consistency of long document abstractive summarisation and the LongSciVerify data set
 Author: Jennifer A Bishop
 Project-URL: Homepage, https://github.com/jbshp/LongDocFACTScore
 Project-URL: Issues, https://github.com/jbshp/LongDocFACTScore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,50 +29,59 @@
 
 ### Method:
 
 LongDocFACTScore is a reference-free framework which can be applied to any reference-free metric for assessing factual consistency. In this repo, it is implemented with BARTScore. The method uses sentence embeddings to calculate similarity between source document sentences and predicted summary sentences, and then applies metrics to the highest similarity text snippets. The scores per sentence in the predicted summary are averaged to give one score per predicted summary. 
 
 In this work, LongDocFACTScore is implemented with [BARTScore](https://github.com/neulab/BARTScore), and some code is copied from the linked repo. 
 
-<img src="ldfacts.png" width="400">
+![longdocfactscore.png](https://github.com/jbshp/LongDocFACTScore/blob/main/ldfacts.png?raw=True)
 
 
 ### Data sets (including LongSciVerify)
 
 In our work, we curate LongSciVerify data set consisting of PubMed and ArXiv papers with human annotations of factual consistency. More information about the data sets we use can be found [here](./data/README.md)
 
 ### Usage of LongDocFACTScore
 
-To run on a piece of text:
+Install:
+```
+pip install longdocfactscore
+```
+or for an editable version
+```
+git clone https://github.com/jbshp/LongDocFACTScore.git
+pip install -e . 
 ```
+
+To run on a piece of text:
+```python
 from longdocfactscore.ldfacts import LongDocFACTScore
 
 predict_summary = "INSERT PREDICTED SUMMARY HERE"
 src_doc = "INSERT SOURCE DOCUMENT HERE"
 
 ldfacts_scorer = LongDocFACTScore(device='cpu')
 
 scores = ldfacts_scorer.score_src_hyp_long([src_doc],[predict_summary])
 ```
 
 To run with some example data:
 ```bash
-pip install -e . 
 python run_example.py
 ```
 
 
 
 ### Repeat evaluation in LongDocFACTScore paper
 
 #### Set up 
 
 1. Run the following
 ```bash
-pip install -e .
+pip install longdocfactscore
 cd evaluation_scripts
 git clone https://github.com/ThomasScialom/QuestEval.git
 git clone https://github.com/neulab/BARTScore.git
 git clone https://github.com/salesforce/factCC.git 
 cp ./utils/factcc_run.py ./factCC/modeling/run.py
 pip install -r requirements.txt
 ```
```

### Comparing `longdocfactscore-0.0.1/README.md` & `longdocfactscore-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,50 +9,59 @@
 
 ### Method:
 
 LongDocFACTScore is a reference-free framework which can be applied to any reference-free metric for assessing factual consistency. In this repo, it is implemented with BARTScore. The method uses sentence embeddings to calculate similarity between source document sentences and predicted summary sentences, and then applies metrics to the highest similarity text snippets. The scores per sentence in the predicted summary are averaged to give one score per predicted summary. 
 
 In this work, LongDocFACTScore is implemented with [BARTScore](https://github.com/neulab/BARTScore), and some code is copied from the linked repo. 
 
-<img src="ldfacts.png" width="400">
+![longdocfactscore.png](https://github.com/jbshp/LongDocFACTScore/blob/main/ldfacts.png?raw=True)
 
 
 ### Data sets (including LongSciVerify)
 
 In our work, we curate LongSciVerify data set consisting of PubMed and ArXiv papers with human annotations of factual consistency. More information about the data sets we use can be found [here](./data/README.md)
 
 ### Usage of LongDocFACTScore
 
-To run on a piece of text:
+Install:
+```
+pip install longdocfactscore
+```
+or for an editable version
+```
+git clone https://github.com/jbshp/LongDocFACTScore.git
+pip install -e . 
 ```
+
+To run on a piece of text:
+```python
 from longdocfactscore.ldfacts import LongDocFACTScore
 
 predict_summary = "INSERT PREDICTED SUMMARY HERE"
 src_doc = "INSERT SOURCE DOCUMENT HERE"
 
 ldfacts_scorer = LongDocFACTScore(device='cpu')
 
 scores = ldfacts_scorer.score_src_hyp_long([src_doc],[predict_summary])
 ```
 
 To run with some example data:
 ```bash
-pip install -e . 
 python run_example.py
 ```
 
 
 
 ### Repeat evaluation in LongDocFACTScore paper
 
 #### Set up 
 
 1. Run the following
 ```bash
-pip install -e .
+pip install longdocfactscore
 cd evaluation_scripts
 git clone https://github.com/ThomasScialom/QuestEval.git
 git clone https://github.com/neulab/BARTScore.git
 git clone https://github.com/salesforce/factCC.git 
 cp ./utils/factcc_run.py ./factCC/modeling/run.py
 pip install -r requirements.txt
 ```
```

### Comparing `longdocfactscore-0.0.1/pyproject.toml` & `longdocfactscore-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longdocfactscore"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Jennifer A Bishop" },
 ]
 description = "LongDocFACTScore: A framework for evaluating factual consistency of long document abstractive summarisation and the LongSciVerify data set"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `longdocfactscore-0.0.1/src/longdocfactscore/ldfacts.py` & `longdocfactscore-1.0.0/src/longdocfactscore/ldfacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# Suppress annoying warnings from this issue which cannot be solved: https://github.com/joblib/threadpoolctl/blob/master/multiple_openmp.md and transformers packages
+import warnings
+warnings.filterwarnings("ignore")
+
 import torch
 import torch.nn as nn
 import traceback
 from transformers import BartTokenizer, BartForConditionalGeneration
 import numpy as np
 from nltk import sent_tokenize
 from sentence_transformers import SentenceTransformer, util
 
-
 class LongDocFACTScore():
     def __init__(self, device="cuda:0", model="BARTScore"):
         self.sent_model = SentenceTransformer("bert-base-nli-mean-tokens")
         self.sent_model.to(device)
         self.device = device
         if model == "BARTScore":
             self.metric = BARTScore(device=self.device)
```

### Comparing `longdocfactscore-0.0.1/src/longdocfactscore.egg-info/PKG-INFO` & `longdocfactscore-1.0.0/src/longdocfactscore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longdocfactscore
-Version: 0.0.1
+Version: 1.0.0
 Summary: LongDocFACTScore: A framework for evaluating factual consistency of long document abstractive summarisation and the LongSciVerify data set
 Author: Jennifer A Bishop
 Project-URL: Homepage, https://github.com/jbshp/LongDocFACTScore
 Project-URL: Issues, https://github.com/jbshp/LongDocFACTScore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,50 +29,59 @@
 
 ### Method:
 
 LongDocFACTScore is a reference-free framework which can be applied to any reference-free metric for assessing factual consistency. In this repo, it is implemented with BARTScore. The method uses sentence embeddings to calculate similarity between source document sentences and predicted summary sentences, and then applies metrics to the highest similarity text snippets. The scores per sentence in the predicted summary are averaged to give one score per predicted summary. 
 
 In this work, LongDocFACTScore is implemented with [BARTScore](https://github.com/neulab/BARTScore), and some code is copied from the linked repo. 
 
-<img src="ldfacts.png" width="400">
+![longdocfactscore.png](https://github.com/jbshp/LongDocFACTScore/blob/main/ldfacts.png?raw=True)
 
 
 ### Data sets (including LongSciVerify)
 
 In our work, we curate LongSciVerify data set consisting of PubMed and ArXiv papers with human annotations of factual consistency. More information about the data sets we use can be found [here](./data/README.md)
 
 ### Usage of LongDocFACTScore
 
-To run on a piece of text:
+Install:
+```
+pip install longdocfactscore
+```
+or for an editable version
+```
+git clone https://github.com/jbshp/LongDocFACTScore.git
+pip install -e . 
 ```
+
+To run on a piece of text:
+```python
 from longdocfactscore.ldfacts import LongDocFACTScore
 
 predict_summary = "INSERT PREDICTED SUMMARY HERE"
 src_doc = "INSERT SOURCE DOCUMENT HERE"
 
 ldfacts_scorer = LongDocFACTScore(device='cpu')
 
 scores = ldfacts_scorer.score_src_hyp_long([src_doc],[predict_summary])
 ```
 
 To run with some example data:
 ```bash
-pip install -e . 
 python run_example.py
 ```
 
 
 
 ### Repeat evaluation in LongDocFACTScore paper
 
 #### Set up 
 
 1. Run the following
 ```bash
-pip install -e .
+pip install longdocfactscore
 cd evaluation_scripts
 git clone https://github.com/ThomasScialom/QuestEval.git
 git clone https://github.com/neulab/BARTScore.git
 git clone https://github.com/salesforce/factCC.git 
 cp ./utils/factcc_run.py ./factCC/modeling/run.py
 pip install -r requirements.txt
 ```
```

