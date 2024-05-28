# Comparing `tmp/neurocaps-0.9.3.post1.tar.gz` & `tmp/neurocaps-0.9.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.3.post1.tar", last modified: Mon May 27 18:21:17 2024, max compression
+gzip compressed data, was "neurocaps-0.9.3.post2.tar", last modified: Tue May 28 03:30:46 2024, max compression
```

## Comparing `neurocaps-0.9.3.post1.tar` & `neurocaps-0.9.3.post2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post1/LICENSE.md
--rw-rw-rw-   0        0        0    16793 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/PKG-INFO
--rw-rw-rw-   0        0        0    15451 2024-05-27 18:12:44.000000 neurocaps-0.9.3.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.457019 neurocaps-0.9.3.post1/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.498387 neurocaps-0.9.3.post1/neurocaps/_utils/
--rw-rw-rw-   0        0        0      363 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.500653 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.514479 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-05-27 16:10:31.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-27 16:51:23.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.523140 neurocaps-0.9.3.post1/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    72960 2024-05-27 18:18:07.000000 neurocaps-0.9.3.post1/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4791 2024-05-27 17:56:51.000000 neurocaps-0.9.3.post1/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1626 2024-05-27 17:56:39.000000 neurocaps-0.9.3.post1/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.523140 neurocaps-0.9.3.post1/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    33356 2024-05-27 18:03:42.000000 neurocaps-0.9.3.post1/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    16793 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1512 2024-05-27 16:09:22.000000 neurocaps-0.9.3.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.537372 neurocaps-0.9.3.post1/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post1/tests/test_CAP.py
--rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-27 17:22:37.000000 neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post1/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.3.post1/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.269032 neurocaps-0.9.3.post2/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post2/LICENSE.md
+-rw-rw-rw-   0        0        0    16831 2024-05-28 03:30:46.266911 neurocaps-0.9.3.post2/PKG-INFO
+-rw-rw-rw-   0        0        0    15453 2024-05-28 03:26:11.000000 neurocaps-0.9.3.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.213698 neurocaps-0.9.3.post2/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.236092 neurocaps-0.9.3.post2/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.241101 neurocaps-0.9.3.post2/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.249553 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.254408 neurocaps-0.9.3.post2/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    72959 2024-05-28 03:26:54.000000 neurocaps-0.9.3.post2/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.256289 neurocaps-0.9.3.post2/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33356 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.265913 neurocaps-0.9.3.post2/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    16831 2024-05-28 03:30:46.000000 neurocaps-0.9.3.post2/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-28 03:30:46.000000 neurocaps-0.9.3.post2/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 03:30:46.000000 neurocaps-0.9.3.post2/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-28 03:30:46.000000 neurocaps-0.9.3.post2/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 03:30:46.000000 neurocaps-0.9.3.post2/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1552 2024-05-28 03:27:11.000000 neurocaps-0.9.3.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 03:30:46.269032 neurocaps-0.9.3.post2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 03:30:46.264911 neurocaps-0.9.3.post2/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post2/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     4687 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-27 23:20:35.000000 neurocaps-0.9.3.post2/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post2/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.3.post2/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.3.post1/LICENSE.md` & `neurocaps-0.9.3.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/PKG-INFO` & `neurocaps-0.9.3.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.3.post1
+Version: 0.9.3.post2
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -23,14 +23,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
 Requires-Dist: nibabel
 Requires-Dist: nilearn!=0.10.3,>=0.10.1
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: surfplot
 Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package designed to perform Co-activation Patterns (CAPs) analyses. It utilizes k-means clustering to group timepoints (TRs) into brain states, applicable to both resting-state and task-based fMRI data. The package is compatible with data preprocessed using **fMRIPrep** and assumes your directory is BIDS-compliant, containing a derivatives folder with a pipeline folder (such as fMRIPrep) that holds the preprocessed BOLD data.
 
@@ -227,15 +228,15 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
 - Only including session 002 data.
 - Adding a dataset_description.json file to the fmriprep folder.
 - Excluding the nii.gz file in the root BIDS folder.
```

### Comparing `neurocaps-0.9.3.post1/README.md` & `neurocaps-0.9.3.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
 - Only including session 002 data.
 - Adding a dataset_description.json file to the fmriprep folder.
 - Excluding the nii.gz file in the root BIDS folder.
```

### Comparing `neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.3.post2/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.3.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/analysis/cap.py` & `neurocaps-0.9.3.post2/neurocaps/analysis/cap.py`

 * *Files 0% similar despite different names*

```diff
@@ -795,19 +795,19 @@
                 # Initialize variable
                 persistence_dict = {}
                 uninterrupted_volumes = []
                 count = 0
 
                 # Iterate through caps
                 for target in cap_numbers:
-                    # Iterate through each element and count uniterrupted volumes that equal target
+                    # Iterate through each element and count uninterrupted volumes that equal target
                     for index in range(0,len(predicted_subject_timeseries[subj_id][curr_run])):
                         if predicted_subject_timeseries[subj_id][curr_run][index] == target:
                             count +=1
-                        # Store count in list if interuptted and not zero an
+                        # Store count in list if interrupted and not zero 
                         else:
                             if count != 0:
                                 uninterrupted_volumes.append(count)
                             # Reset counter 
                             count = 0
                     # In the event, a participant only occupies one CAP and to ensure final counts are added
                     if count > 0:
```

### Comparing `neurocaps-0.9.3.post1/neurocaps/analysis/merge.py` & `neurocaps-0.9.3.post2/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/analysis/standardize.py` & `neurocaps-0.9.3.post2/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.3.post2/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.3.post2/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.3.post1
+Version: 0.9.3.post2
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -23,14 +23,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
 Requires-Dist: nibabel
 Requires-Dist: nilearn!=0.10.3,>=0.10.1
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: surfplot
 Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package designed to perform Co-activation Patterns (CAPs) analyses. It utilizes k-means clustering to group timepoints (TRs) into brain states, applicable to both resting-state and task-based fMRI data. The package is compatible with data preprocessed using **fMRIPrep** and assumes your directory is BIDS-compliant, containing a derivatives folder with a pipeline folder (such as fMRIPrep) that holds the preprocessed BOLD data.
 
@@ -227,15 +228,15 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
 - Only including session 002 data.
 - Adding a dataset_description.json file to the fmriprep folder.
 - Excluding the nii.gz file in the root BIDS folder.
```

### Comparing `neurocaps-0.9.3.post1/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.3.post2/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/pyproject.toml` & `neurocaps-0.9.3.post2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
 00000080: 7273 696f 6e20 3d20 2230 2e39 2e33 2e70  rsion = "0.9.3.p
-00000090: 6f73 7431 220d 0a61 7574 686f 7273 203d  ost1"..authors =
+00000090: 6f73 7432 220d 0a61 7574 686f 7273 203d  ost2"..authors =
 000000a0: 205b 7b6e 616d 6520 3d20 2244 6f6e 6973   [{name = "Donis
 000000b0: 6861 2053 6d69 7468 222c 2065 6d61 696c  ha Smith", email
 000000c0: 203d 2022 646f 6e69 7368 6173 6d69 7468   = "donishasmith
 000000d0: 406f 7574 6c6f 6f6b 2e63 6f6d 227d 5d0d  @outlook.com"}].
 000000e0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 000000f0: 436f 2d61 6374 6976 6174 696f 6e20 5061  Co-activation Pa
 00000100: 7474 6572 6e73 2028 4341 5073 2920 5079  tterns (CAPs) Py
@@ -73,23 +73,25 @@
 00000480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00000490: 2022 6b6e 6565 6422 2c0d 0a20 2020 2020   "kneed",..     
 000004a0: 2020 2020 2020 2020 2020 2022 6e69 6261             "niba
 000004b0: 6265 6c22 2c0d 0a20 2020 2020 2020 2020  bel",..         
 000004c0: 2020 2020 2020 2022 6e69 6c65 6172 6e3e         "nilearn>
 000004d0: 3d30 2e31 302e 312c 2021 3d30 2e31 302e  =0.10.1, !=0.10.
 000004e0: 3322 2c0d 0a20 2020 2020 2020 2020 2020  3",..           
-000004f0: 2020 2020 2022 7375 7266 706c 6f74 222c       "surfplot",
-00000500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000510: 2020 226e 6575 726f 6d61 7073 222c 0d0a    "neuromaps",..
-00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000530: 2270 7962 6964 733b 2070 6c61 7466 6f72  "pybids; platfor
-00000540: 6d5f 7379 7374 656d 2021 3d20 2757 696e  m_system != 'Win
-00000550: 646f 7773 2722 0d0a 2020 2020 2020 2020  dows'"..        
-00000560: 2020 2020 2020 2020 5d0d 0a0d 0a5b 7072          ]....[pr
-00000570: 6f6a 6563 742e 7572 6c73 5d0d 0a48 6f6d  oject.urls]..Hom
-00000580: 6570 6167 6520 3d20 2268 7474 7073 3a2f  epage = "https:/
-00000590: 2f67 6974 6875 622e 636f 6d2f 646f 6e69  /github.com/doni
-000005a0: 7368 6164 736d 6974 682f 6e65 7572 6f63  shadsmith/neuroc
-000005b0: 6170 7322 2020 0d0a 0d0a 5b74 6f6f 6c2e  aps"  ....[tool.
-000005c0: 6469 7374 7574 696c 732e 6264 6973 745f  distutils.bdist_
-000005d0: 7768 6565 6c5d 0d0a 756e 6976 6572 7361  wheel]..universa
-000005e0: 6c20 3d20 7472 7565                      l = true
+000004f0: 2020 2020 2022 7363 696b 6974 2d6c 6561       "scikit-lea
+00000500: 726e 3e3d 312e 342e 3022 2c0d 0a20 2020  rn>=1.4.0",..   
+00000510: 2020 2020 2020 2020 2020 2020 2022 7375               "su
+00000520: 7266 706c 6f74 222c 0d0a 2020 2020 2020  rfplot",..      
+00000530: 2020 2020 2020 2020 2020 226e 6575 726f            "neuro
+00000540: 6d61 7073 222c 0d0a 2020 2020 2020 2020  maps",..        
+00000550: 2020 2020 2020 2020 2270 7962 6964 733b          "pybids;
+00000560: 2070 6c61 7466 6f72 6d5f 7379 7374 656d   platform_system
+00000570: 2021 3d20 2757 696e 646f 7773 2722 0d0a   != 'Windows'"..
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 5d0d 0a0d 0a5b 7072 6f6a 6563 742e 7572  ]....[project.ur
+000005a0: 6c73 5d0d 0a48 6f6d 6570 6167 6520 3d20  ls]..Homepage = 
+000005b0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000005c0: 636f 6d2f 646f 6e69 7368 6164 736d 6974  com/donishadsmit
+000005d0: 682f 6e65 7572 6f63 6170 7322 2020 0d0a  h/neurocaps"  ..
+000005e0: 0d0a 5b74 6f6f 6c2e 6469 7374 7574 696c  ..[tool.distutil
+000005f0: 732e 6264 6973 745f 7768 6565 6c5d 0d0a  s.bdist_wheel]..
+00000600: 756e 6976 6572 7361 6c20 3d20 7472 7565  universal = true
```

### Comparing `neurocaps-0.9.3.post1/tests/test_CAP.py` & `neurocaps-0.9.3.post2/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.3.post2/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.3.post2/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/tests/test_merge_dicts.py` & `neurocaps-0.9.3.post2/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3.post1/tests/test_standardize.py` & `neurocaps-0.9.3.post2/tests/test_standardize.py`

 * *Files identical despite different names*

