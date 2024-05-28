# Comparing `tmp/benchnirs-1.2.3.tar.gz` & `tmp/benchnirs-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchnirs-1.2.3.tar", last modified: Tue May 21 10:40:24 2024, max compression
+gzip compressed data, was "benchnirs-1.2.4.tar", last modified: Tue May 28 15:13:02 2024, max compression
```

## Comparing `benchnirs-1.2.3.tar` & `benchnirs-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:40:24.603469 benchnirs-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-21 10:40:16.000000 benchnirs-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7996 2024-05-21 10:40:24.603469 benchnirs-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7457 2024-05-21 10:40:16.000000 benchnirs-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:40:24.602469 benchnirs-1.2.3/benchnirs/
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-21 10:40:16.000000 benchnirs-1.2.3/benchnirs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49450 2024-05-21 10:40:16.000000 benchnirs-1.2.3/benchnirs/learn.py
--rw-rw-rw-   0 root         (0) root         (0)    25530 2024-05-21 10:40:16.000000 benchnirs-1.2.3/benchnirs/load.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-21 10:40:16.000000 benchnirs-1.2.3/benchnirs/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-21 10:40:16.000000 benchnirs-1.2.3/benchnirs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:40:24.603469 benchnirs-1.2.3/benchnirs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7996 2024-05-21 10:40:24.000000 benchnirs-1.2.3/benchnirs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-21 10:40:24.000000 benchnirs-1.2.3/benchnirs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:40:24.000000 benchnirs-1.2.3/benchnirs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-21 10:40:24.000000 benchnirs-1.2.3/benchnirs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 10:40:24.000000 benchnirs-1.2.3/benchnirs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 10:40:24.603469 benchnirs-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-21 10:40:16.000000 benchnirs-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.641823 benchnirs-1.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-28 15:12:54.000000 benchnirs-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8063 2024-05-28 15:13:02.640823 benchnirs-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7524 2024-05-28 15:12:54.000000 benchnirs-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.639823 benchnirs-1.2.4/benchnirs/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50444 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/learn.py
+-rw-rw-rw-   0 root         (0) root         (0)    25857 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2024-05-28 15:12:54.000000 benchnirs-1.2.4/benchnirs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:13:02.640823 benchnirs-1.2.4/benchnirs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8063 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 15:13:02.000000 benchnirs-1.2.4/benchnirs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:13:02.641823 benchnirs-1.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-28 15:12:54.000000 benchnirs-1.2.4/setup.py
```

### Comparing `benchnirs-1.2.3/LICENSE` & `benchnirs-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.3/PKG-INFO` & `benchnirs-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.2.3
+Version: 1.2.4
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 *Benchmarking framework for machine learning with fNIRS*
 
 **Quick links**  
 &rarr; [*Journal article*](https://www.frontiersin.org/articles/10.3389/fnrgo.2023.994969)  
 &rarr; [*BenchNIRS source code*](https://gitlab.com/HanBnrd/benchnirs)  
 &rarr; [*Install BenchNIRS*](https://hanbnrd.gitlab.io/benchnirs/install.html)  
 &rarr; [*Documentation*](https://hanbnrd.gitlab.io/benchnirs)  
+&rarr; [*Examples*](https://hanbnrd.gitlab.io/benchnirs/examples.html)  
 &rarr; [*Issue tracker*](https://gitlab.com/HanBnrd/benchnirs/-/issues)  
 
 
 [![DOI](https://img.shields.io/badge/doi-10.3389%2Ffnrgo.2023.994969-blue)](https://doi.org/10.3389/fnrgo.2023.994969)
 [![License](https://img.shields.io/badge/license-GNU%20GPLv3%2b-lightgrey)](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/LICENSE)
 [![Pipeline](https://gitlab.com/HanBnrd/benchnirs/badges/main/pipeline.svg)](https://gitlab.com/HanBnrd/benchnirs)
 [![PyPI version](https://img.shields.io/pypi/v/benchnirs)](https://pypi.org/project/benchnirs/)
@@ -53,15 +54,15 @@
 
 
 ## Recommendation checklist
 A checklist of recommendations towards good practice for machine learning with fNIRS (for brain-computer interface applications) can be found [here](./CHECKLIST.md). We welcome contributions from the community in order to improve it, please see below for more information on how to contribute.
 
 
 ## Setting up *BenchNIRS*
-1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+1. Download and install Python 3.9 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
 
 2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
 ```bash
 pip install benchnirs
 ```
 
 3. Download the datasets (see below).
@@ -88,17 +89,17 @@
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
-epochs = bn.load_dataset('bak_2019_me', dataset_path)
+epochs = bn.load_dataset('bak_2019_me', path)
 data = bn.process_epochs(epochs['right', 'left', 'foot'])
-results = bn.deep_learn(*data, 'lstm')
+results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
```

### Comparing `benchnirs-1.2.3/README.md` & `benchnirs-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 *Benchmarking framework for machine learning with fNIRS*
 
 **Quick links**  
 &rarr; [*Journal article*](https://www.frontiersin.org/articles/10.3389/fnrgo.2023.994969)  
 &rarr; [*BenchNIRS source code*](https://gitlab.com/HanBnrd/benchnirs)  
 &rarr; [*Install BenchNIRS*](https://hanbnrd.gitlab.io/benchnirs/install.html)  
 &rarr; [*Documentation*](https://hanbnrd.gitlab.io/benchnirs)  
+&rarr; [*Examples*](https://hanbnrd.gitlab.io/benchnirs/examples.html)  
 &rarr; [*Issue tracker*](https://gitlab.com/HanBnrd/benchnirs/-/issues)  
 
 
 [![DOI](https://img.shields.io/badge/doi-10.3389%2Ffnrgo.2023.994969-blue)](https://doi.org/10.3389/fnrgo.2023.994969)
 [![License](https://img.shields.io/badge/license-GNU%20GPLv3%2b-lightgrey)](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/LICENSE)
 [![Pipeline](https://gitlab.com/HanBnrd/benchnirs/badges/main/pipeline.svg)](https://gitlab.com/HanBnrd/benchnirs)
 [![PyPI version](https://img.shields.io/pypi/v/benchnirs)](https://pypi.org/project/benchnirs/)
@@ -37,15 +38,15 @@
 
 
 ## Recommendation checklist
 A checklist of recommendations towards good practice for machine learning with fNIRS (for brain-computer interface applications) can be found [here](./CHECKLIST.md). We welcome contributions from the community in order to improve it, please see below for more information on how to contribute.
 
 
 ## Setting up *BenchNIRS*
-1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+1. Download and install Python 3.9 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
 
 2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
 ```bash
 pip install benchnirs
 ```
 
 3. Download the datasets (see below).
@@ -72,17 +73,17 @@
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
-epochs = bn.load_dataset('bak_2019_me', dataset_path)
+epochs = bn.load_dataset('bak_2019_me', path)
 data = bn.process_epochs(epochs['right', 'left', 'foot'])
-results = bn.deep_learn(*data, 'lstm')
+results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
```

### Comparing `benchnirs-1.2.3/benchnirs/__init__.py` & `benchnirs-1.2.4/benchnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.3/benchnirs/learn.py` & `benchnirs-1.2.4/benchnirs/learn.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from sklearn.metrics import (accuracy_score, precision_recall_fscore_support,
                              confusion_matrix)
 from sklearn.model_selection import (KFold, StratifiedKFold, GroupKFold,
                                      GridSearchCV, train_test_split)
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import LinearSVC
 from sklearn.utils import shuffle
+from sys import stdout
+from tqdm import trange
 
 
 OUTER_K = 5
 INNER_K = 3
 
 # Standard machine learning parameters
 MAX_ITER = 250000  # for support vector classifier
@@ -74,15 +76,15 @@
 
     output_folder : string
         Path to the directory into which the figures will be saved. Defaults to
         ``'./outputs'``.
 
     Returns
     -------
-    accuracies : list of floats
+    accuracies : array of floats
         List of accuracies on the test sets (one for each iteration of the
         outer cross-validation).
 
     all_hps : list of floats | list of None
         List of regularization parameters for the SVC or a list of None for the
         LDA (one for each iteration of the outer cross-validation).
 
@@ -109,15 +111,15 @@
     all_y_true = []
     all_y_pred = []
     accuracies = []
     additional_metrics = []
     all_hps = []
     out_split = out_kf.split(nirs, labels, groups)
     for k, out_idx in enumerate(out_split):
-        print(f'\tFOLD #{k}')
+        print(f'    FOLD #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_train, labels_test = labels[out_idx[0]], labels[out_idx[1]]
 
         if groups is None:
             groups_train = None
             nirs_train, labels_train = shuffle(
                 nirs_train, labels_train, random_state=random_state)
@@ -179,14 +181,16 @@
     cm = confusion_matrix(all_y_true, all_y_pred, normalize='true')
     sns.heatmap(cm, annot=True, cmap='crest', vmin=0.1, vmax=0.8)
     plt.xlabel('Predicted')
     plt.ylabel('Ground truth')
     plt.savefig(f'{output_folder}/confusion_matrix.png')
     plt.close()
 
+    accuracies = np.array(accuracies)
+
     return accuracies, all_hps, additional_metrics
 
 
 class _DatasetFromNumPy(Dataset):
     """
     Dataset loader from NumPy arrays for PyTorch.
     """
@@ -271,22 +275,18 @@
         x = x[:, -1, :]  # last output of the sequence
         x = F.relu(self.fc1(x))
         x = self.fc2(x)
         return x
 
 
 def _train_dl(nirs_train, labels_train, clf, batch_size, lr, max_epoch,
-              early_stop, random_state):
+              early_stop, random_state, device):
     """
     Train a deep learning classifier with PyTorch.
     """
-    # Set device
-    device_count = torch.cuda.device_count()
-    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-
     # Load data
     if early_stop:
         split = train_test_split(nirs_train, labels_train, shuffle=True,
                                  train_size=0.80, stratify=labels_train,
                                  random_state=random_state)
         nirs_train, labels_train = split[0], split[2]
         nirs_val, labels_val = split[1], split[3]
@@ -294,26 +294,36 @@
         val_loader = DataLoader(dataset=dataset_val, batch_size=1,
                                 shuffle=False)
     dataset_train = _DatasetFromNumPy(nirs_train, labels_train)
     train_loader = DataLoader(dataset=dataset_train, batch_size=batch_size,
                               shuffle=True)
 
     # Instantiate model and hyperparameters
+    device_count = torch.cuda.device_count()
     if device_count > 1:
         clf = nn.DataParallel(clf)  # use multiple GPUs
     clf.to(device)
     criterion = nn.CrossEntropyLoss()  # LogSoftmax() & NLLLoss()
     optimizer = optim.Adam(clf.parameters(), lr=lr)
     # scheduler = optim.lr_scheduler.StepLR(optimizer, step_size=25, gamma=0.5)
 
     train_losses = []
     train_accuracies = []
     val_losses = []
     val_accuracies = []
-    for epoch in range(max_epoch):  # loop over the data multiple times
+    bf = "    > Model training: {l_bar}{bar}| Epoch {n_fmt}/{total_fmt}"
+    disable = False
+    if not stdout.isatty():
+        try:
+            __IPYTHON__
+        except NameError:
+            disable = True
+    pbar = trange(
+        max_epoch, bar_format=bf, leave=False, disable=disable, ascii=True)
+    for epoch in pbar:
         # Train
         clf.train()
         running_loss = 0.0
         correct = 0.0
         total = 0.0
         for i, data in enumerate(train_loader):
             # Get the inputs
@@ -359,42 +369,38 @@
                     total += y.size(0)
                     correct += (predicted == y).sum()
                     correct = int(correct)
                 val_losses.append(running_loss / (i+1))
                 val_accuracies.append(correct / total)
                 last_sorted = sorted(val_losses[-PATIENCE:])
                 if epoch >= PATIENCE and val_losses[-PATIENCE:] == last_sorted:
-                    print(f'\t\t>Early stopping after {epoch+1} epochs')
+                    print(f'    > Early stopping after {epoch+1} epochs')
                     break
         # scheduler.step()
 
     if device_count > 1:
         clf = clf.module
 
     results = {'train_losses': train_losses,
                'train_accuracies': train_accuracies,
                'val_losses': val_losses,
                'val_accuracies': val_accuracies}
     return clf, results
 
 
-def _test_dl(nirs_test, labels_test, clf):
+def _test_dl(nirs_test, labels_test, clf, device):
     """
     Test a deep learning classifier with PyTorch.
     """
-    # Set device
-    device_count = torch.cuda.device_count()
-    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-
     # Load data sets
     dataset_test = _DatasetFromNumPy(nirs_test, labels_test)
     test_loader = DataLoader(dataset=dataset_test, batch_size=1,
                              shuffle=False)
 
-    if device_count > 1:
+    if torch.cuda.device_count() > 1:
         clf = nn.DataParallel(clf)  # use multiple GPUs
     clf.to(device)
     criterion = nn.CrossEntropyLoss()  # LogSoftmax() & NLLLoss()
 
     # Test
     clf.eval()
     with torch.no_grad():
@@ -472,15 +478,15 @@
 
     output_folder : string
         Path to the directory into which the figures will be saved. Defaults to
         ``'./outputs'``.
 
     Returns
     -------
-    accuracies : list of floats
+    accuracies : array of floats
         List of accuracies on the test sets (one for each iteration of the
         outer cross-validation).
 
     all_hps : list of tuples
         List of best hyperparameters (one tuple for each iteration of the outer
         cross-validation). Each tuple will be `(batch size, learning rate)`.
 
@@ -501,19 +507,28 @@
     if model_class == 'ann':
         model_class = _ANNClassifier
     elif model_class == 'cnn':
         model_class = _CNNClassifier
     elif model_class == 'lstm':
         model_class = _LSTMClassifier
 
-    print(f'Deep learning: {model_class.__name__}')
+    print(f'Deep learning: {model_class.__name__}', end=' ')
+
+    # Set device
+    if torch.cuda.is_available():
+        device = torch.device('cuda:0')
+        device_count = torch.cuda.device_count()
+        print(f"(using {device_count} GPU{'s' if device_count > 1 else ''})")
+    else:
+        device = torch.device('cpu')
+        print("(using CPU)")
 
     # Outer split
     if os.path.isfile(f'{output_folder}/split.pickle'):
-        print('\tSaved k-fold split found, loading it...', end=' ')
+        print('    Saved k-fold split found, loading it...', end=' ')
         with open(f'{output_folder}/split.pickle', 'rb') as f:
             out_split = pickle.load(f)
         print('Done!')
     else:
         if groups is None:
             out_kf = StratifiedKFold(n_splits=OUTER_K)
         else:
@@ -528,15 +543,15 @@
     # Inner split
     if groups is None:
         in_kf = StratifiedKFold(n_splits=INNER_K)
     else:
         in_kf = GroupKFold(n_splits=INNER_K)
 
     for k, out_idx in enumerate(out_split):
-        print(f'\tTraining outer fold #{k}')
+        print(f'    Training outer fold #{k}')
         nirs_train = nirs[out_idx[0]]
         labels_train = labels[out_idx[0]]
 
         if groups is None:
             groups_train = None
             nirs_train, labels_train = shuffle(
                 nirs_train, labels_train, random_state=random_state)
@@ -549,51 +564,50 @@
         # Min-max scaling
         if normalize:
             maxs = nirs_train.max(axis=normalize, keepdims=True)
             mins = nirs_train.min(axis=normalize, keepdims=True)
             nirs_train = (nirs_train - mins) / (maxs - mins)
 
         if os.path.isfile(f'{output_folder}/model_k{k}.pt'):
-            print('\t\tClassifier checkpoint found, skipping training')
+            print('    > Classifier checkpoint found, skipping training')
         else:
             # Train classifier for each combination of hyperparameters
             hp_list = list(itertools.product(batch_sizes, lrs))
             if len(hp_list) > 1:
+                print('    > Hyperparameter selection')
                 in_accuracies = [[] for _ in hp_list]
                 for i, hp in enumerate(hp_list):
                     batch_size, lr = hp[0], hp[1]
                     in_split = in_kf.split(nirs_train, labels_train,
                                            groups_train)
                     for in_idx in in_split:
                         nirs_in_train = nirs_train[in_idx[0]]
                         labels_in_train = labels_train[in_idx[0]]
                         nirs_val = nirs_train[in_idx[1]]
                         labels_val = labels_train[in_idx[1]]
 
                         clf = model_class(n_classes).double()
                         clf, _ = _train_dl(nirs_in_train, labels_in_train,
                                            clf, batch_size, lr, max_epoch,
-                                           early_stop=False,
-                                           random_state=random_state)
-                        results = _test_dl(nirs_val, labels_val, clf)
+                                           False, random_state, device)
+                        results = _test_dl(nirs_val, labels_val, clf, device)
                         in_accuracies[i].append(results['test_accuracy'])
 
                 # Get best hyperparameters
                 in_average_accuracies = np.mean(in_accuracies, axis=1)
                 index_best = np.argmax(in_average_accuracies)
                 best_hps = hp_list[index_best]
             else:
                 best_hps = (batch_sizes[0], lrs[0])
 
             # Retrain with best hyperparameters
             clf = model_class(n_classes).double()
             clf, results = _train_dl(nirs_train, labels_train,
                                      clf, best_hps[0], best_hps[1], max_epoch,
-                                     early_stop=True,
-                                     random_state=random_state)
+                                     True, random_state, device)
 
             # Save trained model and training results
             clf.cpu()
             torch.save(clf.state_dict(), f'{output_folder}/model_k{k}.pt')
             with open(f'{output_folder}/hps_k{k}.pickle', 'wb') as f:
                 pickle.dump(best_hps, f)
             with open(f'{output_folder}/results_k{k}.pickle', 'wb') as f:
@@ -617,15 +631,15 @@
 
     all_ks, all_epochs = [], []
     all_train_losses, all_val_losses = [], []
     all_train_accuracies, all_val_accuracies = [], []
     all_y_true, all_y_pred = [], []
     accuracies, all_hps, additional_metrics = [], [], []
     for k, out_idx in enumerate(out_split):
-        print(f'\tTesting outer fold #{k}')
+        print(f'    Testing outer fold #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_test = labels[out_idx[1]]
 
         # Min-max scaling of test set using training set only to avoid leakage
         if normalize:
             maxs = nirs_train.max(axis=normalize, keepdims=True)
             mins = nirs_train.min(axis=normalize, keepdims=True)
@@ -645,15 +659,15 @@
         all_epochs += [epoch for epoch in range(len(results['train_losses']))]
         all_train_losses += results['train_losses']
         all_val_losses += results['val_losses']
         all_train_accuracies += results['train_accuracies']
         all_val_accuracies += results['val_accuracies']
 
         # Test model
-        results = _test_dl(nirs_test, labels_test, clf)
+        results = _test_dl(nirs_test, labels_test, clf, device)
         all_y_true += results['y_true']
         all_y_pred += results['y_pred']
         accuracies.append(results['test_accuracy'])
         prfs = precision_recall_fscore_support(
             results['y_true'], results['y_pred'], average='weighted')
         additional_metrics.append(prfs[:-1])
 
@@ -675,62 +689,71 @@
     df_accuracies = df_accuracies.melt(id_vars=['k', 'Epoch'],
                                        value_vars=['Training', 'Validation'],
                                        var_name='Condition',
                                        value_name='Accuracy')
     sns.lineplot(ax=axes[1], data=df_accuracies, y='Accuracy', x='Epoch',
                  hue='Condition', units='k', estimator=None)
     plt.savefig(f'{output_folder}/graphs.png', bbox_inches='tight')
+    plt.show()
     plt.close()
 
     # Figures
     cm = confusion_matrix(all_y_true, all_y_pred, normalize='true')
     sns.heatmap(cm, annot=True, cmap='crest', vmin=0.1, vmax=0.8)
     plt.xlabel('Predicted')
     plt.ylabel('Ground truth')
     plt.savefig(f'{output_folder}/confusion_matrix.png')
     plt.close()
 
+    accuracies = np.array(accuracies)
+
     return accuracies, all_hps, additional_metrics
 
 
 def _train_encdec(x_train, y_train, encoder, decoder, batch_size, lr,
-                  max_epoch, early_stop, random_state):
+                  max_epoch, early_stop, random_state, device):
     """
     Train a deep learning encoder-decoder with PyTorch.
     """
-    # Set device
-    device_count = torch.cuda.device_count()
-    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-
     # Load data
     if early_stop:
         split = train_test_split(x_train, y_train, shuffle=True,
                                  train_size=0.80, random_state=random_state)
         x_train, y_train = split[0], split[2]
         x_val, y_val = split[1], split[3]
         dataset_val = _DatasetFromNumPy(x_val, y_val)
         val_loader = DataLoader(dataset=dataset_val, batch_size=1,
                                 shuffle=False)
     dataset_train = _DatasetFromNumPy(x_train, y_train)
     train_loader = DataLoader(dataset=dataset_train, batch_size=batch_size,
                               shuffle=True)
 
     # Instantiate model and hyperparameters
+    device_count = torch.cuda.device_count()
     if device_count > 1:  # use multiple GPUs
         encoder = nn.DataParallel(encoder)
         decoder = nn.DataParallel(decoder)
     encoder.to(device)
     decoder.to(device)
     criterion = nn.MSELoss()
     params = list(encoder.parameters()) + list(decoder.parameters())
     optimizer = optim.Adam(params, lr=lr)
 
     train_losses = []
     val_losses = []
-    for epoch in range(max_epoch):  # loop over the data multiple times
+    bf = "    > Model training: {l_bar}{bar}| Epoch {n_fmt}/{total_fmt}"
+    disable = False
+    if not stdout.isatty():
+        try:
+            __IPYTHON__
+        except NameError:
+            disable = True
+    pbar = trange(
+        max_epoch, bar_format=bf, leave=False, disable=disable, ascii=True)
+    for epoch in pbar:
         # Train
         encoder.train()
         decoder.train()
         running_loss = 0.0
         for i, data in enumerate(train_loader):
             # Get the inputs
             x, y = data[0].to(device), data[1].to(device)
@@ -765,40 +788,36 @@
                     features = encoder(x)
                     outputs = decoder(features)
                     loss = criterion(outputs, y)
                     running_loss += loss.item()
                 val_losses.append(running_loss / (i+1))
                 last_sorted = sorted(val_losses[-PATIENCE:])
                 if epoch >= PATIENCE and val_losses[-PATIENCE:] == last_sorted:
-                    print(f'\t\t>Early stopping after {epoch+1} epochs')
+                    print(f'    > Early stopping after {epoch+1} epochs')
                     break
 
     if device_count > 1:
         encoder = encoder.module
         decoder = decoder.module
 
     results = {'train_losses': train_losses,
                'val_losses': val_losses}
     return encoder, decoder, results
 
 
-def _test_encdec(x_test, y_test, encoder, decoder):
+def _test_encdec(x_test, y_test, encoder, decoder, device):
     """
     Test a deep learning encoder-decoder with PyTorch.
     """
-    # Set device
-    device_count = torch.cuda.device_count()
-    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-
     # Load data sets
     dataset_test = _DatasetFromNumPy(x_test, y_test)
     test_loader = DataLoader(dataset=dataset_test, batch_size=1,
                              shuffle=False)
 
-    if device_count > 1:  # use multiple GPUs
+    if torch.cuda.device_count() > 1:  # use multiple GPUs
         encoder = nn.DataParallel(encoder)
         decoder = nn.DataParallel(decoder)
     encoder.to(device)
     decoder.to(device)
     criterion = nn.MSELoss()
 
     # Test
@@ -818,62 +837,65 @@
 
 
 def _proxy_optim(nirs_train, targets_train, groups_train, enc_class, dec_class,
                  batch_sizes, lrs, max_epoch, random_state, output_folder):
     """
     Train and optimise encoder-decoder.
     """
+    # Set device
+    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
+
     if random_state:
         torch.manual_seed(random_state)
 
     if not os.path.isdir(output_folder):
         os.makedirs(output_folder)
 
     if groups_train is None:
         in_kf = KFold(n_splits=INNER_K)
     else:
         in_kf = GroupKFold(n_splits=INNER_K)
 
     # Encoder-decoder optimization
     hp_list = list(itertools.product(batch_sizes, lrs))
     if len(hp_list) > 1:
+        print('    > Hyperparameter selection')
         in_losses = [[] for _ in hp_list]
         for i, hp in enumerate(hp_list):
             batch_size, lr = hp[0], hp[1]
             in_split = in_kf.split(nirs_train, targets_train, groups_train)
             for in_idx in in_split:
                 nirs_in_train = nirs_train[in_idx[0]]
                 targets_in_train = targets_train[in_idx[0]]
                 nirs_val = nirs_train[in_idx[1]]
                 targets_val = targets_train[in_idx[1]]
 
                 encoder = enc_class().double()
                 decoder = dec_class().double()
                 encoder, decoder, _ = _train_encdec(
                     nirs_in_train, targets_in_train, encoder, decoder,
-                    batch_size, lr, max_epoch, early_stop=False,
-                    random_state=random_state)
+                    batch_size, lr, max_epoch, False, random_state, device)
 
-                results = _test_encdec(nirs_val, targets_val, encoder, decoder)
+                results = _test_encdec(nirs_val, targets_val, encoder, decoder,
+                                       device)
                 in_losses[i].append(results['test_loss'])
 
         # Get best hyperparameters
         in_average_losses = np.mean(in_losses, axis=1)
         index_best = np.argmin(in_average_losses)
         best_hps = hp_list[index_best]
     else:
         best_hps = (batch_sizes[0], lrs[0])
 
     # Retrain with best hyperparameters
     encoder = enc_class().double()
     decoder = dec_class().double()
     encoder, decoder, results = _train_encdec(
         nirs_train, targets_train, encoder, decoder,
-        best_hps[0], best_hps[1], max_epoch, early_stop=True,
-        random_state=random_state)
+        best_hps[0], best_hps[1], max_epoch, True, random_state, device)
 
     # Save trained model and training results
     encoder.cpu()
     decoder.cpu()
     torch.save(encoder.state_dict(), f'{output_folder}/encoder.pt')
     torch.save(decoder.state_dict(), f'{output_folder}/decoder.pt')
     with open(f'{output_folder}/hps.pickle', 'wb') as f:
@@ -960,15 +982,15 @@
 
     output_folder : string
         Path to the directory into which the figures will be saved. Defaults to
         ``'./outputs'``.
 
     Returns
     -------
-    accuracies : list of floats
+    accuracies : array of floats
         List of accuracies for the overall classifier on the test sets (one for
         each iteration of the outer cross-validation).
 
     all_hps : list of tuples
         List of best hyperparameters for the overall classifier (one tuple for
         each iteration of the outer cross-validation). Each tuple will be
         `(batch size, learning rate)`.
@@ -989,24 +1011,33 @@
     print(f'Labels: {set(labels)}')
     if 8 in set(labels):
         n_classes = len(set(labels)) - 1  # minus unlabelled
     else:
         n_classes = len(set(labels))
 
     print(f'Deep transfer learning: {enc_class.__name__}/'
-          f'{dec_class.__name__}-{model_class.__name__}')
+          f'{dec_class.__name__}-{model_class.__name__}', end=' ')
+
+    # Set device
+    if torch.cuda.is_available():
+        device = torch.device('cuda:0')
+        device_count = torch.cuda.device_count()
+        print(f"(using {device_count} GPU{'s' if device_count > 1 else ''})")
+    else:
+        device = torch.device('cpu')
+        print("(using CPU)")
 
     # Get index to split channel types
     mid_idx = nirs.shape[1] / 2
     if mid_idx.is_integer():
         mid_idx = int(mid_idx)
 
     # Outer split
     if os.path.isfile(f'{output_folder}/split.pickle'):
-        print('\tSaved k-fold split found, loading it...', end=' ')
+        print('    Saved k-fold split found, loading it...', end=' ')
         with open(f'{output_folder}/split.pickle', 'rb') as f:
             out_split = pickle.load(f)
         print('Done!')
     else:
         if groups is None:
             out_kf = StratifiedKFold(n_splits=OUTER_K)
         else:
@@ -1021,15 +1052,15 @@
     # Inner split
     if groups is None:
         in_kf = StratifiedKFold(n_splits=INNER_K)
     else:
         in_kf = GroupKFold(n_splits=INNER_K)
 
     for k, out_idx in enumerate(out_split):
-        print(f'\tTraining outer fold #{k}')
+        print(f'    Training outer fold #{k}')
         nirs_train = nirs[out_idx[0]]
         labels_train = labels[out_idx[0]]
 
         if groups is None:
             groups_train = None
             nirs_train, labels_train = shuffle(
                 nirs_train, labels_train, random_state=random_state)
@@ -1046,45 +1077,46 @@
             nirs_train = (nirs_train - mins) / (maxs - mins)
 
         # Train and optimise self-supervised models
         nirs_train_hbo = nirs_train[:, mid_idx:, :]
         nirs_train_hbr = nirs_train[:, :mid_idx, :]
         # HbO -> HbR
         if os.path.isfile(f'{output_folder}/k{k}/hbo/encoder.pt'):
-            print('\t\tSaved HbO encoder found, loading it...', end=' ')
+            print('    > HbO encoder checkpoint found, loading it...', end=' ')
             enc_hbo = enc_class().double()
             enc_hbo.load_state_dict(
                 torch.load(f'{output_folder}/k{k}/hbo/encoder.pt'))
             print('Done!')
         else:
             enc_hbo, _ = _proxy_optim(
                 nirs_train_hbo, nirs_train_hbr, groups_train,
                 enc_class, dec_class, batch_sizes=batch_sizes, lrs=lrs,
                 max_epoch=max_epoch, random_state=random_state,
                 output_folder=f'{output_folder}/k{k}/hbo')
         # HbR -> HbO
         if os.path.isfile(f'{output_folder}/k{k}/hbr/encoder.pt'):
-            print('\t\tSaved HbR encoder found, loading it...', end=' ')
+            print('    > HbR encoder checkpoint found, loading it...', end=' ')
             enc_hbr = enc_class().double()
             enc_hbr.load_state_dict(
                 torch.load(f'{output_folder}/k{k}/hbr/encoder.pt'))
             print('Done!')
         else:
             enc_hbr, _ = _proxy_optim(
                 nirs_train_hbr, nirs_train_hbo, groups_train,
                 enc_class, dec_class, batch_sizes=batch_sizes, lrs=lrs,
                 max_epoch=max_epoch, random_state=random_state,
                 output_folder=f'{output_folder}/k{k}/hbr')
 
         if os.path.isfile(f'{output_folder}/k{k}/clf.pt'):
-            print('\t\tClassifier checkpoint found, skipping training')
+            print('    > Classifier checkpoint found, skipping training')
         else:
             # Train classifier for each combination of hyperparameters
             hp_list = list(itertools.product(batch_sizes, lrs))
             if len(hp_list) > 1:
+                print('    > Hyperparameter selection')
                 in_accuracies = [[] for _ in hp_list]
                 for i, hp in enumerate(hp_list):
                     batch_size, lr = hp[0], hp[1]
                     in_split = in_kf.split(nirs_train, labels_train,
                                            groups_train)
                     for in_idx in in_split:
                         nirs_in_train = nirs_train[in_idx[0]]
@@ -1099,17 +1131,16 @@
                         idx_val = np.where(np.array(labels_val) != 8)
                         labels_val = labels_val[idx_val]
                         nirs_val = nirs_val[idx_val]
 
                         clf = model_class(n_classes, enc_hbo, enc_hbr).double()
                         clf, _ = _train_dl(nirs_in_train, labels_in_train,
                                            clf, batch_size, lr, max_epoch,
-                                           early_stop=False,
-                                           random_state=random_state)
-                        results = _test_dl(nirs_val, labels_val, clf)
+                                           False, random_state, device)
+                        results = _test_dl(nirs_val, labels_val, clf, device)
                         in_accuracies[i].append(results['test_accuracy'])
 
                 # Get best hyperparameters
                 in_average_accuracies = np.mean(in_accuracies, axis=1)
                 index_max = np.argmax(in_average_accuracies)
                 best_hps = hp_list[index_max]
             else:
@@ -1118,16 +1149,15 @@
             # Retrain with best hyperparameters
             idx_train = np.where(np.array(labels_train) != 8)
             labels_train = labels_train[idx_train]
             nirs_train = nirs_train[idx_train]
             clf = model_class(n_classes, enc_hbo, enc_hbr).double()
             clf, results = _train_dl(nirs_train, labels_train,
                                      clf, best_hps[0], best_hps[1], max_epoch,
-                                     early_stop=True,
-                                     random_state=random_state)
+                                     True, random_state, device)
 
             # Save trained model and training results
             clf.cpu()
             torch.save(clf.state_dict(), f'{output_folder}/k{k}/clf.pt')
             with open(f'{output_folder}/k{k}/hps.pickle', 'wb') as f:
                 pickle.dump(best_hps, f)
             with open(f'{output_folder}/k{k}/results.pickle', 'wb') as f:
@@ -1151,15 +1181,15 @@
 
     all_ks, all_epochs = [], []
     all_train_losses, all_val_losses = [], []
     all_train_accuracies, all_val_accuracies = [], []
     all_y_true, all_y_pred = [], []
     accuracies, all_hps, additional_metrics = [], [], []
     for k, out_idx in enumerate(out_split):
-        print(f'\tTesting outer fold #{k}')
+        print(f'    Testing outer fold #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_test = labels[out_idx[1]]
 
         # Min-max scaling of test set using training set only to avoid leakage
         if normalize:
             maxs = nirs_train.max(axis=normalize, keepdims=True)
             mins = nirs_train.min(axis=normalize, keepdims=True)
@@ -1188,15 +1218,15 @@
         all_train_accuracies += results['train_accuracies']
         all_val_accuracies += results['val_accuracies']
 
         # Test model
         idx_test = np.where(np.array(labels_test) != 8)
         labels_test = labels_test[idx_test]
         nirs_test = nirs_test[idx_test]
-        results = _test_dl(nirs_test, labels_test, clf)
+        results = _test_dl(nirs_test, labels_test, clf, device)
         all_y_true += results['y_true']
         all_y_pred += results['y_pred']
         accuracies.append(results['test_accuracy'])
         prfs = precision_recall_fscore_support(
             results['y_true'], results['y_pred'], average='weighted')
         additional_metrics.append(prfs[:-1])
 
@@ -1218,18 +1248,21 @@
     df_accuracies = df_accuracies.melt(id_vars=['k', 'Epoch'],
                                        value_vars=['Training', 'Validation'],
                                        var_name='Condition',
                                        value_name='Accuracy')
     sns.lineplot(ax=axes[1], data=df_accuracies, y='Accuracy', x='Epoch',
                  hue='Condition', units='k', estimator=None)
     plt.savefig(f'{output_folder}/graphs.png', bbox_inches='tight')
+    plt.show()
     plt.close()
 
     # Figures
     cm = confusion_matrix(all_y_true, all_y_pred, normalize='true')
     sns.heatmap(cm, annot=True, cmap='crest', vmin=0.1, vmax=0.8)
     plt.xlabel('Predicted')
     plt.ylabel('Ground truth')
     plt.savefig(f'{output_folder}/confusion_matrix.png')
     plt.close()
 
+    accuracies = np.array(accuracies)
+
     return accuracies, all_hps, additional_metrics
```

### Comparing `benchnirs-1.2.3/benchnirs/load.py` & `benchnirs-1.2.4/benchnirs/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import mne
 import nirsimple as ns
 import numpy as np
 import scipy.io
 
 from mne.channels import combine_channels
 from pandas import DataFrame
+from sys import stdout
+from tqdm import tqdm
 
 
 PATH_HERFF_2014 = '../../data/dataset_herff_2014/'
 PATH_SHIN_2018 = '../../data/dataset_shin_2018/'
 PATH_SHIN_2016 = '../../data/dataset_shin_2016/'
 PATH_BAK_2019 = '../../data/dataset_bak_2019/'
 
@@ -179,15 +181,15 @@
                          'Left PFC HbO': [8, 10, 12, 14],
                          'Left PFC HbR': [9, 11, 13, 15]}
         data['event_id'] = {'1-back': 1, '2-back': 2, '3-back': 3}
         data['tmin'] = -5
         data['tmax'] = 44
 
         # Load data matrix
-        mat = scipy.io.loadmat(f'{path}{subject}.mat')
+        mat = scipy.io.loadmat(f'{path}/{subject}.mat')
 
         # Get Hb data
         delta_c = mat['data']  # in uM
         delta_c = delta_c * 1e-6  # convert uM to M
         data['delta_c'] = delta_c
 
         # Get labels
@@ -221,16 +223,16 @@
                          'Left PFC HbO': [0, 1, 2, 3, 4, 5, 6],
                          'Left PFC HbR': [36, 37, 38, 39, 40, 41, 42]}
         data['event_id'] = {'0-back': 1, '2-back': 2, '3-back': 3}
         data['tmin'] = -2
         data['tmax'] = 40
 
         # Load data matrices
-        cnt = scipy.io.loadmat(f'{path}{subject}/cnt_nback.mat')
-        mrk = scipy.io.loadmat(f'{path}{subject}/mrk_nback.mat')
+        cnt = scipy.io.loadmat(f'{path}/{subject}/cnt_nback.mat')
+        mrk = scipy.io.loadmat(f'{path}/{subject}/mrk_nback.mat')
 
         # Get sampling frequency (in Hz)
         data['sfreq'] = cnt['cnt_nback']['oxy'][0, 0]['fs'][0, 0][0][0]
 
         # Get channel info
         ch_oxy = cnt['cnt_nback']['oxy'][0, 0]['clab'][0, 0][0]
         ch_deoxy = cnt['cnt_nback']['deoxy'][0, 0]['clab'][0, 0][0]
@@ -290,16 +292,16 @@
                          'Left PFC HbO': [0, 1, 2, 3, 4, 5, 6],
                          'Left PFC HbR': [36, 37, 38, 39, 40, 41, 42]}
         data['event_id'] = {'baseline': 1, 'word generation': 2}
         data['tmin'] = -2
         data['tmax'] = 10
 
         # Load data matrices
-        cnt = scipy.io.loadmat(f'{path}{subject}/cnt_wg.mat')
-        mrk = scipy.io.loadmat(f'{path}{subject}/mrk_wg.mat')
+        cnt = scipy.io.loadmat(f'{path}/{subject}/cnt_wg.mat')
+        mrk = scipy.io.loadmat(f'{path}/{subject}/mrk_wg.mat')
 
         # Get sampling frequency (in Hz)
         data['sfreq'] = cnt['cnt_wg']['oxy'][0, 0]['fs'][0, 0][0][0]
 
         # Get channel info
         ch_oxy = cnt['cnt_wg']['oxy'][0, 0]['clab'][0, 0][0]
         ch_deoxy = cnt['cnt_wg']['deoxy'][0, 0]['clab'][0, 0][0]
@@ -357,16 +359,16 @@
                          'Left PFC HbO': [0, 2, 8, 62],
                          'Left PFC HbR': [1, 3, 9, 63]}
         data['event_id'] = {'baseline': 1, 'mental arithmetic': 2}
         data['tmin'] = -2
         data['tmax'] = 10
 
         # Load data matrices
-        cnt = scipy.io.loadmat(f'{path}{subject}/cnt.mat')
-        mrk = scipy.io.loadmat(f'{path}{subject}/mrk.mat')
+        cnt = scipy.io.loadmat(f'{path}/{subject}/cnt.mat')
+        mrk = scipy.io.loadmat(f'{path}/{subject}/mrk.mat')
 
         # Get sampling frequency (in Hz)
         data['sfreq'] = cnt['cnt'][0, 1]['fs'][0, 0][0][0]
 
         # Get original channel info
         wls = cnt['cnt'][0, 1]['wavelengths'][0, 0][0].tolist()
         dpfs = [6., 6.]
@@ -453,15 +455,15 @@
                          'Left MC HbO': range(0, 10),
                          'Left MC HbR': range(20, 30)}
         data['event_id'] = {'right': 1, 'left': 2, 'foot': 3}
         data['tmin'] = -2
         data['tmax'] = 10
 
         # Load data matrices
-        mat = scipy.io.loadmat(f'{path}{subject}.mat')
+        mat = scipy.io.loadmat(f'{path}/{subject}.mat')
 
         # Get sampling frequency (in Hz)
         data['sfreq'] = mat['dat']['fs'][0, 0][0, 0]
 
         # Get channel info
         ch_names = [ch.tolist()[0] for ch in mat['dat']['clab'][0, 0][0]]
         ch_names = [ch.replace('deoxy', ' HbR') for ch in ch_names]
@@ -511,15 +513,16 @@
         (epoch interval: -2 to 10 seconds).
         ``'shin_2016_ma'`` for mental arithmetic from Shin et al., 2016
         (epoch interval: -2 to 10 seconds).
         ``'bak_2019_me'`` for motor execution from Bak et al., 2019
         (epoch interval: -2 to 10 seconds).
 
     path : string
-        Path of the dataset selected with the ``dataset`` parameter.
+        Path of the directory of the dataset selected with the ``dataset``
+        parameter.
 
     bandpass : list of floats | None
         Cutoff frequencies of the bandpass Butterworth filter (in Hz). Defaults
         to ``None`` for no filtering.
 
     order : integer
         Order of the bandpass Butterworth filter.
@@ -548,15 +551,14 @@
 
     Returns
     -------
     epochs : MNE Epochs object
         MNE epochs data with associated labels. Subject IDs are contained in
         the ``metadata`` property.
     """
-    print('Loading epochs...')
     raws = None
     groups = []
 
     if dataset == 'herff_2014_nb':
         loader = _DatasetHerff2014NB()
     elif dataset == 'shin_2018_nb':
         loader = _DatasetShin2018NB()
@@ -565,15 +567,24 @@
     elif dataset == 'shin_2016_ma':
         loader = _DatasetShin2016MA()
     elif dataset == 'bak_2019_me':
         loader = _DatasetBak2019ME()
     else:
         loader = None
 
-    for subj_id, subj in enumerate(loader.subject_list):
+    bf = "Loading data: {l_bar}{bar}| Subject {n_fmt}/{total_fmt}"
+    disable = False
+    if not stdout.isatty():
+        try:
+            __IPYTHON__
+        except NameError:
+            disable = True
+    pbar = tqdm(
+        loader.subject_list, bar_format=bf, disable=disable, ascii=True)
+    for subj_id, subj in enumerate(pbar):
         try:
             data = loader.load(subj, path)
         except FileNotFoundError:
             raise FileNotFoundError(
                 f"dataset not found, please make sure the dataset has been "
                 f"downloaded and the proper path has been provided (cf. "
                 f"https://hanbnrd.gitlab.io/benchnirs/install.html)")
```

### Comparing `benchnirs-1.2.3/benchnirs/process.py` & `benchnirs-1.2.4/benchnirs/process.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.3/benchnirs/viz.py` & `benchnirs-1.2.4/benchnirs/viz.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.3/benchnirs.egg-info/PKG-INFO` & `benchnirs-1.2.4/benchnirs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.2.3
+Version: 1.2.4
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BenchNIRS
 
 <img title="BenchNIRS" align="right" width="150" height="150" src="https://hanbnrd.gitlab.io/assets/img/logos/benchnirs.png" alt="BenchNIRS">
 
 *Benchmarking framework for machine learning with fNIRS*
 
 **Quick links**  
 &rarr; [*Journal article*](https://www.frontiersin.org/articles/10.3389/fnrgo.2023.994969)  
 &rarr; [*BenchNIRS source code*](https://gitlab.com/HanBnrd/benchnirs)  
 &rarr; [*Install BenchNIRS*](https://hanbnrd.gitlab.io/benchnirs/install.html)  
 &rarr; [*Documentation*](https://hanbnrd.gitlab.io/benchnirs)  
+&rarr; [*Examples*](https://hanbnrd.gitlab.io/benchnirs/examples.html)  
 &rarr; [*Issue tracker*](https://gitlab.com/HanBnrd/benchnirs/-/issues)  
 
 
 [![DOI](https://img.shields.io/badge/doi-10.3389%2Ffnrgo.2023.994969-blue)](https://doi.org/10.3389/fnrgo.2023.994969)
 [![License](https://img.shields.io/badge/license-GNU%20GPLv3%2b-lightgrey)](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/LICENSE)
 [![Pipeline](https://gitlab.com/HanBnrd/benchnirs/badges/main/pipeline.svg)](https://gitlab.com/HanBnrd/benchnirs)
 [![PyPI version](https://img.shields.io/pypi/v/benchnirs)](https://pypi.org/project/benchnirs/)
@@ -53,15 +54,15 @@
 
 
 ## Recommendation checklist
 A checklist of recommendations towards good practice for machine learning with fNIRS (for brain-computer interface applications) can be found [here](./CHECKLIST.md). We welcome contributions from the community in order to improve it, please see below for more information on how to contribute.
 
 
 ## Setting up *BenchNIRS*
-1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+1. Download and install Python 3.9 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
 
 2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
 ```bash
 pip install benchnirs
 ```
 
 3. Download the datasets (see below).
@@ -88,17 +89,17 @@
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
-epochs = bn.load_dataset('bak_2019_me', dataset_path)
+epochs = bn.load_dataset('bak_2019_me', path)
 data = bn.process_epochs(epochs['right', 'left', 'foot'])
-results = bn.deep_learn(*data, 'lstm')
+results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
```

### Comparing `benchnirs-1.2.3/setup.py` & `benchnirs-1.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="benchnirs",
-    version="1.2.3",
+    version="1.2.4",
     author="Johann Benerradi",
     author_email="johann.benerradi@gmail.com",
     description="Benchmarking framework for machine learning with fNIRS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/HanBnrd/benchnirs",
     license="GNU GPLv3+",
     packages=setuptools.find_packages(),
     install_requires=[
-        "importlib",
         "lazy_loader",
+        "tqdm",
         "numpy",
         "pandas",
         "scipy",
         "mne",
         "matplotlib",
         "seaborn",
         "scikit-learn",
@@ -28,9 +28,9 @@
         "nirsimple"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

