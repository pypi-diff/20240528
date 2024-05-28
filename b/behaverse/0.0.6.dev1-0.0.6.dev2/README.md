# Comparing `tmp/behaverse-0.0.6.dev1.tar.gz` & `tmp/behaverse-0.0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.6.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.6.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.6.dev1.tar` & `behaverse-0.0.6.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1781 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/.github/workflows/docs-publish.yml
--rw-r--r--   0        0        0     1243 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      160 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/.gitignore
--rw-r--r--   0        0        0      158 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/.pypirc
--rw-r--r--   0        0        0      375 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/LICENSE
--rw-r--r--   0        0        0      984 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/README.md
--rw-r--r--   0        0        0       54 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/docs/.gitignore
--rw-r--r--   0        0        0       22 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2024-05-24 10:46:55.276388 behaverse-0.0.6.dev1/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0     1366 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/docs/_quarto.yml
--rw-r--r--   0        0        0     1156 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/docs/getting_started.qmd
--rw-r--r--   0        0        0      261 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/docs/index.qmd
--rw-r--r--   0        0        0     1255 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/docs/system_design.qmd
--rw-r--r--   0        0        0      209 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/environment.yml
--rw-r--r--   0        0        0     7910 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/examples/1 Getting Started.ipynb
--rw-r--r--   0        0        0     1788 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/pyproject.toml
--rw-r--r--   0        0        0      494 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/__init__.py
--rw-r--r--   0        0        0      284 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/additional_storage/huggingface.py
--rw-r--r--   0        0        0      276 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/additional_storage/osf.py
--rw-r--r--   0        0        0      278 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/additional_storage/ulhpc.py
--rw-r--r--   0        0        0      279 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/additional_storage/zenodo.py
--rw-r--r--   0        0        0       27 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/conftest.py
--rw-r--r--   0        0        0     7093 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/dataset.py
--rw-r--r--   0        0        0      238 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/dataset_description.py
--rw-r--r--   0        0        0     1699 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/dataset_test.py
--rw-r--r--   0        0        0     1619 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/dvc_storage.py
--rw-r--r--   0        0        0      535 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/dvc_storage_test.py
--rw-r--r--   0        0        0     2533 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/functional.py
--rw-r--r--   0        0        0       28 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/functions_test.py
--rw-r--r--   0        0        0     2571 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/http_storage.py
--rw-r--r--   0        0        0     1918 2024-05-24 10:46:55.280387 behaverse-0.0.6.dev1/src/behaverse/utils.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 behaverse-0.0.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1781 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1243 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      160 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/README.md
+-rw-r--r--   0        0        0       54 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1366 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/_quarto.yml
+-rw-r--r--   0        0        0     1222 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/getting_started.qmd
+-rw-r--r--   0        0        0      261 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/index.qmd
+-rw-r--r--   0        0        0     1255 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/docs/system_design.qmd
+-rw-r--r--   0        0        0      221 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/environment.yml
+-rw-r--r--   0        0        0    10649 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/examples/1 Getting Started.ipynb
+-rw-r--r--   0        0        0     1788 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/pyproject.toml
+-rw-r--r--   0        0        0      494 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/huggingface.py
+-rw-r--r--   0        0        0      276 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/osf.py
+-rw-r--r--   0        0        0      278 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/ulhpc.py
+-rw-r--r--   0        0        0      279 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/additional_storage/zenodo.py
+-rw-r--r--   0        0        0       27 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/conftest.py
+-rw-r--r--   0        0        0     8702 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset.py
+-rw-r--r--   0        0        0      238 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset_description.py
+-rw-r--r--   0        0        0     1714 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dataset_test.py
+-rw-r--r--   0        0        0     1619 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dvc_storage.py
+-rw-r--r--   0        0        0      535 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/dvc_storage_test.py
+-rw-r--r--   0        0        0     2520 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/functional.py
+-rw-r--r--   0        0        0       28 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/functions_test.py
+-rw-r--r--   0        0        0     2571 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/http_storage.py
+-rw-r--r--   0        0        0     1918 2024-05-28 10:54:10.099794 behaverse-0.0.6.dev2/src/behaverse/utils.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 behaverse-0.0.6.dev2/PKG-INFO
```

### Comparing `behaverse-0.0.6.dev1/.github/workflows/docs-publish.yml` & `behaverse-0.0.6.dev2/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/.github/workflows/pypi-publish.yml` & `behaverse-0.0.6.dev2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/LICENSE` & `behaverse-0.0.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/README.md` & `behaverse-0.0.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/docs/_extensions/machow/interlinks/interlinks.lua` & `behaverse-0.0.6.dev2/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/docs/_quarto.yml` & `behaverse-0.0.6.dev2/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/docs/getting_started.qmd` & `behaverse-0.0.6.dev2/docs/getting_started.qmd`

 * *Files 14% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 ---
 
 # Getting Started
 
 To access datasets via the API, you first need to install the `behaverse` Python package. You can do this by running the following command:
 
 ```bash
-pip install behaverse
+pip install -U behaverse
 ```
 
 Make sure you have Python 3.10 or later installed on your system. We recommend using a virtual environment such as Mamba to manage your dependencies.
 
 
 # Usage
 
 The `behaverse` package provides a simple API to access datasets. You can use the `behaverse` package to download datasets, load them into memory, and access the data. Here is an example of how to use the package to list available datasets, download a dataset, select a subset of the dataset, and load it into memory:
 
 ```{python}
-from behaverse import list_datasets, download_dataset, load_dataset
+from behaverse import list_datasets, download_dataset, load_dataset, open_dataset, describe_dataset
 from IPython.display import display
 
 # List available datasets
-print(list_datasets())
+display(list_datasets())
 
 # Open a dataset, select a subset of the data, and load it into memory
 dataset = open_dataset('P500_9subjects/L1m').where(subject_id=['001', '002']).load()
-display(dataset.subjects)
-display(dataset.study_flow)
-display(dataset.response)
+display('subjects', dataset.subjects)
+display('study flow', dataset.study_flow)
+
+# print dataset description
 describe_dataset(dataset)
 ```
```

### Comparing `behaverse-0.0.6.dev1/docs/system_design.qmd` & `behaverse-0.0.6.dev2/docs/system_design.qmd`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/pyproject.toml` & `behaverse-0.0.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/src/behaverse/dataset.py` & `behaverse-0.0.6.dev2/src/behaverse/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,26 +33,26 @@
     def __init__(self, name: str, **kwargs) -> None:
         """Initialize the Dataset class."""
         if not kwargs.get('allow_instantiation', False):
             raise NotImplementedError('You cannot instantiate this class. Use the class methods instead.')
 
         self.name = name
 
-        self.db_path = Path.home() / '.behaverse' / 'datasets' / self.name
+        self.path = Path.home() / '.behaverse' / 'datasets' / self.name
 
-        if not self.db_path.exists():
-            raise FileNotFoundError(f'Dataset not found: {self.db_path}')
+        if not self.path.exists():
+            raise FileNotFoundError(f'Dataset not found: {self.path}')
 
         # SECTION subjects table
-        self.subjects = pd.read_csv(self.db_path / 'subjects.csv',
+        self.subjects = pd.read_csv(self.path / 'subjects.csv',
                                     dtype={'subject_id': str})
         # !SECTION subjects table
 
         # SECTION study flow table
-        study_flow_files = list(self.db_path.glob('**/study_flow.csv'))
+        study_flow_files = list(self.path.glob('**/study_flow.csv'))
 
         self.study_flow = pd.concat(
             [pd.read_csv(f, dtype={'subject_id': str, 'session_id': str})
              for f in study_flow_files], axis=0, ignore_index=True)
         # !SECTION study flow table
 
     def where(self, **conditions: Any) -> 'Dataset':
@@ -112,41 +112,78 @@
     def load(self) -> 'Dataset':
         """Load the dataset with the given name.
 
         Returns:
             Dataset: The newly loaded dataset.
 
         """
+        # TODO single progress bar for all the tables
+        # TODO refactor as load_table method
+
         # SECTION response table
         response_files = self.study_flow.apply(lambda s:
-            (self.db_path /
+            (self.path /
             f'subject_{s["subject_id"]}' /
             f'session_{s["session_id"]}' /
             f'{s["activity"]}' /
             f'response_{s["attempt"]}.csv').absolute().as_posix(), axis=1).to_list()
 
         response_dfs = []
-        for f in tqdm(response_files):
+        for f in tqdm(response_files, desc='Loading responses'):
             if Path(f).exists():
                 try:
-                    df = pd.read_csv(f)
+                    df = pd.read_csv(f, dtype={'subject_id': str})
                     if not df.empty and len(df.columns) > 1:
                         response_dfs.append(df)
                 except pd.errors.EmptyDataError:
                     logger.warning(f'Empty response file: {f}')
 
-        self.response = pd.concat(response_dfs, axis=0, ignore_index=True)
+        self.response_table = pd.concat(response_dfs, axis=0, ignore_index=True)
         # !SECTION response table
 
-        # TODO SECTION stimulus table
-        self.stimulus = ...
+        # SECTION stimulus table
+        stimulus_files = self.study_flow.apply(lambda s:
+            (self.path /
+            f'subject_{s["subject_id"]}' /
+            f'session_{s["session_id"]}' /
+            f'{s["activity"]}' /
+            f'stimulus_{s["attempt"]}.csv').absolute().as_posix(), axis=1).to_list()
+
+        stimulus_dfs = []
+        for f in tqdm(stimulus_files, desc='Loading stimuli'):
+            if Path(f).exists():
+                try:
+                    df = pd.read_csv(f)
+                    if not df.empty and len(df.columns) > 1:
+                        stimulus_dfs.append(df)
+                except pd.errors.EmptyDataError:
+                    logger.warning(f'Empty stimulus file: {f}')
+
+        self.stimulus_table = pd.concat(stimulus_dfs, axis=0, ignore_index=True)
         # !SECTION stimulus table
 
-        # TODO SECTION option table
-        self.option = ...
+        # SECTION option table
+        option_files = self.study_flow.apply(lambda s:
+            (self.path /
+            f'subject_{s["subject_id"]}' /
+            f'session_{s["session_id"]}' /
+            f'{s["activity"]}' /
+            f'option_{s["attempt"]}.csv').absolute().as_posix(), axis=1).to_list()
+
+        option_dfs = []
+        for f in tqdm(option_files, desc='Loading options'):
+            if Path(f).exists():
+                try:
+                    df = pd.read_csv(f)
+                    if not df.empty and len(df.columns) > 1:
+                        option_dfs.append(df)
+                except pd.errors.EmptyDataError:
+                    logger.warning(f'Empty option file: {f}')
+
+        self.option_table = pd.concat(option_dfs, axis=0, ignore_index=True)
         # !SECTION option table
 
         return self
 
     @classmethod
     def open(cls, name: str, download: bool = True, storage: str='http') -> 'Dataset':
         """Open the dataset with the given name, and optionally download it if it does not exist.
```

### Comparing `behaverse-0.0.6.dev1/src/behaverse/dataset_test.py` & `behaverse-0.0.6.dev2/src/behaverse/dataset_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     from .dataset import Dataset
 
     dataset = Dataset.open('P500_9subjects/L1m').load()
 
     assert dataset.name == 'P500_9subjects/L1m'
     assert len(dataset.subjects) > 0
     assert len(dataset.study_flow) > 0
-    assert len(dataset.response) > 0
+    assert len(dataset.response_table) > 0
 
 
 def test_load_dataset_with_condition():
     """Partially load a behaverse dataset."""
     from .dataset import Dataset
 
     subject_ids = ['001', '002']
@@ -48,8 +48,8 @@
     dataset = Dataset.open('P500_9subjects/L1m').where(subject_id=subject_ids).load()
 
     assert dataset.name == 'P500_9subjects/L1m'
     assert len(dataset.subjects) == len(subject_ids)
     assert len(dataset.study_flow.subject_id.unique()) == len(subject_ids)
 
     # FIXME subject_index in response table must be renamed to subject_id
-    assert len(dataset.response.subject_index.unique()) == len(subject_ids)
+    assert len(dataset.response_table['subject_index'].unique()) == len(subject_ids)
```

### Comparing `behaverse-0.0.6.dev1/src/behaverse/dvc_storage.py` & `behaverse-0.0.6.dev2/src/behaverse/dvc_storage.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/src/behaverse/dvc_storage_test.py` & `behaverse-0.0.6.dev2/src/behaverse/dvc_storage_test.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/src/behaverse/functional.py` & `behaverse-0.0.6.dev2/src/behaverse/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,25 @@
         dataset = load_dataset('P500_9subjects/L1m', subject_id=['001', '002'])
         ```
 
     """
     return Dataset.open(name).where(**conditions).load()
 
 
-def describe_dataset(name: str) -> DatasetDescription:
+def describe_dataset(dataset: Dataset) -> DatasetDescription:
     """Describe the dataset with the given name.
 
     Args:
-        name: Name of the dataset to describe.
+        dataset: Dataset to describe.
 
     Returns:
         DatasetDescription: Metadata and description of the dataset.
 
     """
-    return Dataset.open(name).describe()
+    return dataset.describe()
 
 
 def validate_dataset(name: str) -> bool:
     """Validate the dataset with the given name.
 
     Args:
         name: Name of the dataset to validate.
```

### Comparing `behaverse-0.0.6.dev1/src/behaverse/http_storage.py` & `behaverse-0.0.6.dev2/src/behaverse/http_storage.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/src/behaverse/utils.py` & `behaverse-0.0.6.dev2/src/behaverse/utils.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.6.dev1/PKG-INFO` & `behaverse-0.0.6.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behaverse
-Version: 0.0.6.dev1
+Version: 0.0.6.dev2
 Summary: Behaverse Python Package.
 Author-email: xCIT Development Team <contact@xcit.org>
 Maintainer-email: Morteza Ansarinia <ansarinia@me.com>, Hoorieh Afkari <hoorieh.afkari@uni.lu>, Pedro Cardoso-Leite <pedro.cardosoleite@uni.lu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

