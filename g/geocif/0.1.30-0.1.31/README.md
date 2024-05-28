# Comparing `tmp/geocif-0.1.30.tar.gz` & `tmp/geocif-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.30.tar", last modified: Sun May 26 14:57:26 2024, max compression
+gzip compressed data, was "geocif-0.1.31.tar", last modified: Mon May 27 01:51:06 2024, max compression
```

## Comparing `geocif-0.1.30.tar` & `geocif-0.1.31.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.872530 geocif-0.1.30/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.30/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.30/MANIFEST.in
--rw-rw-rw-   0        0        0     1586 2024-05-26 14:57:26.866878 geocif-0.1.30/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.30/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.407786 geocif-0.1.30/geocif/
--rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.549939 geocif-0.1.30/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.30/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.30/geocif/agmet/utils.py
--rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.30/geocif/analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.627091 geocif-0.1.30/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.30/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.30/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.30/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.30/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.30/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.30/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.654883 geocif-0.1.30/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.30/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.30/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.30/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    42711 2024-05-26 14:55:15.000000 geocif-0.1.30/geocif/geocif.py
--rw-rw-rw-   0        0        0     6660 2024-05-25 01:23:08.000000 geocif-0.1.30/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.30/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.791637 geocif-0.1.30/geocif/ml/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    12623 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5098 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    13882 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     9120 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0    10035 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.30/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.30/geocif/ml/output.py
--rw-rw-rw-   0        0        0     5139 2024-05-26 02:21:56.000000 geocif-0.1.30/geocif/ml/spatial_autocorrelation.py
--rw-rw-rw-   0        0        0     8348 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     9038 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9515 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3171 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.30/geocif/ml/xai.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.816876 geocif-0.1.30/geocif/playground/
--rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.30/geocif/playground/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.30/geocif/playground/automl.py
--rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.30/geocif/playground/misc.py
--rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.30/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.840642 geocif-0.1.30/geocif/viz/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/viz/__init__.py
--rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.30/geocif/viz/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.521676 geocif-0.1.30/geocif.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-05-26 14:57:25.000000 geocif-0.1.30/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.30/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.30/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-26 14:57:26.902391 geocif-0.1.30/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-26 14:57:15.000000 geocif-0.1.30/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.855306 geocif-0.1.30/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.30/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.956912 geocif-0.1.31/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.31/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-27 01:51:06.956013 geocif-0.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.31/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.826002 geocif-0.1.31/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.31/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.871644 geocif-0.1.31/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.31/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.31/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.31/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.31/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.31/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.893355 geocif-0.1.31/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.31/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.31/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.31/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.31/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.31/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.31/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.31/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.899881 geocif-0.1.31/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.31/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.31/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.31/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    42901 2024-05-26 15:50:48.000000 geocif-0.1.31/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6660 2024-05-25 01:23:08.000000 geocif-0.1.31/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.31/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.933119 geocif-0.1.31/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.31/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12623 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5098 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    13882 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     9120 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0    10035 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.31/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.31/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     5701 2024-05-27 01:23:59.000000 geocif-0.1.31/geocif/ml/spatial_autocorrelation.py
+-rw-rw-rw-   0        0        0     8348 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     9038 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9515 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3171 2024-05-25 18:55:01.000000 geocif-0.1.31/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.31/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.938634 geocif-0.1.31/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.31/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.31/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.31/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.31/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.942644 geocif-0.1.31/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.31/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.31/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.861010 geocif-0.1.31/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-27 01:51:04.000000 geocif-0.1.31/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-05-27 01:51:06.000000 geocif-0.1.31/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:51:04.000000 geocif-0.1.31/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.31/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-27 01:51:04.000000 geocif-0.1.31/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.31/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-27 01:51:06.976191 geocif-0.1.31/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-27 01:50:56.000000 geocif-0.1.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:51:06.953449 geocif-0.1.31/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.31/tests/test_geocif.py
```

### Comparing `geocif-0.1.30/LICENSE` & `geocif-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/PKG-INFO` & `geocif-0.1.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.30
+Version: 0.1.31
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.30/README.md` & `geocif-0.1.31/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/agmet/geoagmet.py` & `geocif-0.1.31/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/agmet/plot.py` & `geocif-0.1.31/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/agmet/utils.py` & `geocif-0.1.31/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/analysis.py` & `geocif-0.1.31/geocif/analysis.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/backup/features.py` & `geocif-0.1.31/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/backup/geo.py` & `geocif-0.1.31/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/backup/geocif.py` & `geocif-0.1.31/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/backup/metadata.py` & `geocif-0.1.31/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/cei/definitions.py` & `geocif-0.1.31/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/cei/indices.py` & `geocif-0.1.31/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/geocif.py` & `geocif-0.1.31/geocif/geocif.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,14 +351,16 @@
                 )[0]
 
         # Create a dataframe with forecast results
         shp = len(X_test)
         experiment_id = f"{self.country}_{self.crop}"
         now = ar.utcnow().to("America/New_York").format("MMMM-DD-YYYY HH:mm:ss")
         selected_features = self.selected_features + self.cat_features
+        # Compute percentage difference between y_pred and y_test
+        ape = np.abs((y_pred - y_test) / y_test) * 100
         df = pd.DataFrame(
             {
                 "Experiment_ID": np.full(shp, experiment_id),
                 "Date": np.full(shp, self.today),
                 "Time": np.full(shp, now),
                 "Country": np.full(shp, self.country),
                 "Crop": np.full(shp, self.crop),
@@ -374,14 +376,15 @@
                 "Model": np.full(shp, self.model_name),
                 "Region_ID": df_region["Region_ID"].values,
                 "Region": df_region["Region"].values,
                 "Harvest Year": df_region["Harvest Year"].values,
                 "Area (ha)": df_region["Area (ha)"].values,
                 f"Observed {self.target}": np.around(y_test, 3).ravel(),
                 f"Predicted {self.target}": np.around(y_pred, 3).ravel(),
+                f"APE": np.around(ape, 3).ravel(),
             }
         )
 
         if self.median_yield_as_feature:
             # Add median yield to dataframe
             df.loc[:, f"Median {self.target}"] = np.around(
                 df_region[f"Median {self.target}"].values, 3
@@ -716,15 +719,15 @@
 
         mask = self.df_results["Stage_ID"].isin(_stages)
         df = self.df_results[mask]
 
         """ Convert this dataframe into an ML ready format and save to disk """
         df = self.create_ml_dataframe(df)
         dir_output = (
-            self.dir_analysis / self.country / self.crop / str(self.forecast_season)
+            self.dir_analysis / self.country / self.crop / self.model_name / str(self.forecast_season)
         )
         os.makedirs(dir_output, exist_ok=True)
         df.to_csv(
             dir_output / f"{self.country}_{self.crop}_{self.forecast_season}.csv",
             index=False,
         )
 
@@ -764,24 +767,24 @@
         dict_kwargs["forecast_season"] = self.forecast_season
         dict_kwargs["method"] = self.method
         dict_kwargs["national_correlation"] = self.national_correlation
         dict_kwargs["groupby"] = self.correlation_plot_groupby
         dict_kwargs["dg_country"] = self.dg_country
         dict_kwargs["combined_dict"] = self.combined_dict
 
+        if self.spatial_autocorrelation:
+           sa.compute_spatial_autocorrelation(self.df_results, **dict_kwargs)
+
         if self.correlation_plots:
             self.logger.info(f"Correlation plot for {self.country} {self.crop}")
             (
                 dict_selected_features,
                 dict_best_cei,
             ) = correlations.all_correlated_feature_by_time(df, **dict_kwargs)
 
-        if self.spatial_autocorrelation:
-           sa.compute_spatial_autocorrelation(self.df_results, **dict_kwargs)
-
         """ Separate into train and test datasets based on forecast_season """
         mask = df["Harvest Year"] == self.forecast_season
         self.df_train = df[~mask]
         self.df_test = df[mask]
 
         # Drop rows with missing values for self.target_col in df_train
         self.df_train = self.df_train.dropna(subset=[self.target])
```

### Comparing `geocif-0.1.30/geocif/indices_runner.py` & `geocif-0.1.31/geocif/indices_runner.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/logger.py` & `geocif-0.1.31/geocif/logger.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/correlations.py` & `geocif-0.1.31/geocif/ml/correlations.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/embedding.py` & `geocif-0.1.31/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/feature_engineering.py` & `geocif-0.1.31/geocif/ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/feature_selection.py` & `geocif-0.1.31/geocif/ml/feature_selection.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/outliers.py` & `geocif-0.1.31/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/outlook.py` & `geocif-0.1.31/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/output.py` & `geocif-0.1.31/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/spatial_autocorrelation.py` & `geocif-0.1.31/geocif/ml/spatial_autocorrelation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import warnings
+
+from tqdm import tqdm
+import matplotlib.pyplot as plt
 import pandas as pd
 from pysal.lib import weights
-from pysal.explore import esda
-import matplotlib.pyplot as plt
+
+warnings.filterwarnings("ignore")
 
 
 def validate_inputs(df_results, required_columns):
     """
 
     Args:
         df_results:
@@ -36,106 +40,123 @@
     dg_country = dg_country.drop_duplicates(subset="Country Region")
     dg_country = dg_country.dropna(subset=["Country Region", "Region_ID", "geometry"])
 
     df["Country Region"] = (df["Country"] + " " + df["Region"]).str.lower()
     dg_country["Country Region"] = dg_country["Country Region"].str.lower()
     dg_country = dg_country[dg_country["Country Region"].isin(df["Country Region"])]
 
+    dg_country.reset_index(drop=True, inplace=True)
+
     merged_df = dg_country.merge(df, on="Country Region", how="inner")
 
-    return merged_df, dg_country
+    return merged_df
 
 
-def create_base_weights(dg_country):
+def create_base_weights(merged_df):
     """
 
     Args:
-        dg_country:
+        merged_df:
 
     Returns:
 
     """
-    dg_subset = dg_country[["Country Region", "geometry"]].drop_duplicates()
+    dg = merged_df[["Country Region", "geometry"]].drop_duplicates()
 
     try:
-        w_base = weights.Queen.from_dataframe(dg_subset)
+        w_base = weights.Queen.from_dataframe(dg)
     except Exception as e:
         raise RuntimeError(f"Failed to create spatial weights: {e}")
 
     no_neighbors = [
         index for index, neighbors in w_base.neighbors.items() if len(neighbors) == 0
     ]
     if no_neighbors:
-        print(f"Removing {len(no_neighbors)} polygons with 0 neighbors")
-        dg_country = dg_country.drop(index=no_neighbors).reset_index(drop=True)
-        w_base = weights.Queen.from_dataframe(
-            dg_country[["Country Region", "geometry"]]
-        )
+        dg = dg.drop(index=no_neighbors[0]).reset_index(drop=True)
+        w_base = weights.Queen.from_dataframe(dg[["Country Region", "geometry"]])
 
-    return w_base, dg_country
+    return w_base, dg
 
 
 def create_weights_for_year(dg_country, regions_with_data):
     """
 
     Args:
         dg_country:
         regions_with_data:
 
     Returns:
 
     """
-    dg_subset = dg_country[dg_country["Country Region"].isin(regions_with_data)]
+    dg = dg_country[dg_country["Country Region"].isin(regions_with_data)]
+    dg = dg.reset_index(drop=True)
+
+    wt = weights.Queen.from_dataframe(dg)
 
-    wt = weights.Queen.from_dataframe(dg_subset)
+    no_neighbors = [
+        index for index, neighbors in wt.neighbors.items() if len(neighbors) == 0
+    ]
+    if no_neighbors:
+        dg = dg.drop(index=no_neighbors[0]).reset_index(drop=True)
+        wt = weights.Queen.from_dataframe(dg[["Country Region", "geometry"]])
 
-    return wt
+    return wt, dg
 
 
-def compute_morans_i(merged_df, dg_country):
+def compute_morans_i(merged_df):
     """
 
     Args:
         merged_df:
         dg_country:
 
     Returns:
 
     """
+    from pysal.explore import esda
+
+    # Drop any regions with missing data
+    merged_df = merged_df.dropna(subset=["Yield (tn per ha)"])
+
     years = merged_df["Harvest Year"].unique()
     results = {"Harvest Year": [], "Moran's I": [], "p-value": [], "Significant": []}
 
-    for year in years:
+    for year in tqdm(years, desc="Compute Moran's I"):
         year_data = merged_df[merged_df["Harvest Year"] == year]
         regions_with_data = year_data["Country Region"].unique()
         year_data = year_data[year_data["Country Region"].isin(regions_with_data)]
 
-        y = year_data[["Region", "Yield (tn per ha)"]].drop_duplicates()
+        y = year_data[["Country Region", "Region", "Yield (tn per ha)"]].drop_duplicates()
+        dg_country = year_data[["Country Region", "geometry"]].drop_duplicates()
 
         if len(y) > 1:
-            w = create_weights_for_year(dg_country, regions_with_data)
+            w, x = create_weights_for_year(dg_country, regions_with_data)
+            y = y[y["Country Region"].isin(x["Country Region"])]
 
             try:
                 mi = esda.Moran(y["Yield (tn per ha)"].values, w, permutations=999)
             except:
                 breakpoint()
             results["Harvest Year"].append(year)
-            results["Moran's I"].append(mi.I)
+            try:
+                results["Moran's I"].append(mi.I)
+            except:
+                breakpoint()
             results["p-value"].append(mi.p_sim)
             results["Significant"].append(mi.p_sim < 0.1)
         else:
             results["Harvest Year"].append(year)
             results["Moran's I"].append(None)
             results["p-value"].append(None)
             results["Significant"].append(False)
 
     return pd.DataFrame(results)
 
 
-def plot_moransi_time_series(results_df, country, crop, dir_output):
+def plot_morans_i_time_series(results_df, country, crop, dir_output):
     """
 
     Args:
         results_df:
         country:
         crop:
         dir_output:
@@ -190,16 +211,14 @@
         "Crop",
         "Region",
         "Harvest Year",
         "Yield (tn per ha)",
     ]
     validate_inputs(df_results, required_columns)
 
-    merged_df, dg_country = preprocess_data(df_results, dg_country)
+    merged_df = preprocess_data(df_results, dg_country)
     if merged_df.empty:
         raise ValueError("No valid data available after preprocessing")
 
-    w_base, dg_country = create_base_weights(dg_country)
-
-    results_df = compute_morans_i(merged_df, dg_country)
+    results_df = compute_morans_i(merged_df)
 
-    plot_moransi_time_series(results_df, country, crop, dir_output)
+    plot_morans_i_time_series(results_df, country, crop, dir_output)
```

### Comparing `geocif-0.1.30/geocif/ml/stages.py` & `geocif-0.1.31/geocif/ml/stages.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/stats.py` & `geocif-0.1.31/geocif/ml/stats.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/trainers.py` & `geocif-0.1.31/geocif/ml/trainers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/trend.py` & `geocif-0.1.31/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/ml/xai.py` & `geocif-0.1.31/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/playground/misc.py` & `geocif-0.1.31/geocif/playground/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/utils.py` & `geocif-0.1.31/geocif/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif/viz/plot.py` & `geocif-0.1.31/geocif/viz/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/geocif.egg-info/PKG-INFO` & `geocif-0.1.31/geocif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.30
+Version: 0.1.31
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.30/geocif.egg-info/SOURCES.txt` & `geocif-0.1.31/geocif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.30/setup.py` & `geocif-0.1.31/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="geocif",
     name="geocif",
     packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ritviksahajpal.github.io/yield_forecasting/",
-    version="0.1.30",
+    version="0.1.31",
     zip_safe=False,
 )
```

