# Comparing `tmp/higgsml-0.0.6.tar.gz` & `tmp/higgsml-0.0.7.tar.gz`

## Comparing `higgsml-0.0.6.tar` & `higgsml-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/__init__.py
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/datasets.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/ingestion.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/score.py
--rw-r--r--   0        0        0    20064 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/systematics.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.6/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.6/LICENSE
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 higgsml-0.0.6/README.md
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 higgsml-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 higgsml-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/__init__.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/score.py
+-rw-r--r--   0        0        0    20059 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/systematics.py
+-rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 higgsml-0.0.7/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.7/LICENSE
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 higgsml-0.0.7/README.md
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 higgsml-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 higgsml-0.0.7/PKG-INFO
```

### Comparing `higgsml-0.0.6/HiggsML/ingestion.py` & `higgsml-0.0.7/HiggsML/ingestion.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.6/HiggsML/score.py` & `higgsml-0.0.7/HiggsML/score.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.6/HiggsML/systematics.py` & `higgsml-0.0.7/HiggsML/systematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,21 +567,20 @@
     for key in data_set.keys():
         if key is not "data":
             data_syst_set[key] = data_syst.pop(key)
     data_syst_set["data"] = data_syst
 
     return data_syst_set
 
-
 LHC_NUMBERS = {
-    "ztautau": 6177943,
-    "wjets": 2704182,
-    "diboson": 2192528,
-    "ttbar": 617402,
-    "htautau": 14139
+    "ztautau": 823327,
+    "wjets": 710190,
+    "diboson": 40590,
+    "ttbar": 158761,
+    "htautau": 3639,
 }
 
 def get_bootstraped_dataset(
     test_set,
     mu=1.0,
     seed=31415,
     w_scale=1.0,
```

### Comparing `higgsml-0.0.6/HiggsML/visualization.py` & `higgsml-0.0.7/HiggsML/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         print("[*] --- Examples of all features")
         display(self.dfall.head())
 
         print("[*] --- Description of all features")
         display(self.dfall.describe())
 
     def histogram_dataset(self, columns=None):
-        fig = plt.figure()
         if columns == None:
             columns = self.columns
         sns.set_theme(rc={"figure.figsize": (40, 40)}, style="whitegrid")
 
         dfplot = pd.DataFrame(self.dfall, columns=columns)
 
         nbins = 25
@@ -73,15 +72,17 @@
             alpha=0.5,
             density=True,
             ax=ax,
             bins=nbins,
             label="S",
         )
 
-        plt.legend(loc="best")
+        for i in range(len(ax)):
+            ax[i].set_title(columns[i])
+            ax[i].legend(["Background", "Signal"])
         plt.title("Histograms of features in" + self.name)
         plt.show()
 
     def correlation_plots(self, columns=None):
         caption = ["Signal feature", "Background feature"]
         if columns == None:
             columns = self.columns
@@ -129,15 +130,15 @@
             lh._sizes = [10]
 
         plt.rcParams["figure.facecolor"] = "w"  # Set the figure facecolor to white
         ax.figure.suptitle("Pair plots of features in" + self.name)
         plt.show()
         plt.close()
 
-    def stacked_histogram(self, field_name, mu_hat=1.0, bins=30, detailedlabel=None):
+    def stacked_histogram(self, field_name, mu_hat=1.0, bins=30):
         field = self.dfall[field_name]
         sns.set_theme(rc={"figure.figsize": (8, 7)}, style="whitegrid")
 
         bins = 30
 
         detailed_label = np.array(self.detailed_label)
```

### Comparing `higgsml-0.0.6/.gitignore` & `higgsml-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.6/LICENSE` & `higgsml-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.6/README.md` & `higgsml-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.6/pyproject.toml` & `higgsml-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HiggsML"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
   { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
   { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
   { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
```

### Comparing `higgsml-0.0.6/PKG-INFO` & `higgsml-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HiggsML
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Black Swan test package
 Project-URL: Homepage, https://github.com/blackSwanCS/black_swan_pkg
 Project-URL: Issues, https://github.com/blackSwanCS/black_swan_pkg/issues
 Author-email: Ragansu Chakkappai <ragansu.chakkappai@universite-paris-saclay.fr>, David Rousseau <david.rousseau@uijclab.in2p3.fr>, "V. Estrade" <v.estrade@centralesupelec.fr>, Ihsan Ullah <ihsan.ullah@universite-paris-saclay.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

