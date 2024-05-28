# Comparing `tmp/nwb4fp-0.6.3.9.tar.gz` & `tmp/nwb4fp-0.6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.3.9.tar", last modified: Fri May 17 14:54:28 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.4.0.tar", last modified: Tue May 28 14:37:20 2024, max compression
```

## Comparing `nwb4fp-0.6.3.9.tar` & `nwb4fp-0.6.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:28.450023 nwb4fp-0.6.3.9/
--rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/LICENSE
--rw-rw-rw-   0        0        0     5732 2024-05-17 14:54:28.442030 nwb4fp-0.6.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     7191 2024-05-17 14:41:57.000000 nwb4fp-0.6.3.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 14:54:28.476026 nwb4fp-0.6.3.9/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-17 14:54:22.000000 nwb4fp-0.6.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:27.928027 nwb4fp-0.6.3.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:27.945026 nwb4fp-0.6.3.9/src/nwb4fp/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:28.071026 nwb4fp-0.6.3.9/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3846 2024-05-16 11:52:07.000000 nwb4fp-0.6.3.9/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:28.179028 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1961 2024-05-17 14:54:06.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17455 2024-05-16 12:39:49.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:28.190042 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:27.947024 nwb4fp-0.6.3.9/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:27.947024 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb_0283.py
--rw-rw-rw-   0        0        0     1135 2024-05-17 14:31:30.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:54:28.050039 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5732 2024-05-17 14:54:27.000000 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-17 14:54:27.000000 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:54:27.000000 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2885 2024-05-17 14:54:27.000000 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 14:54:27.000000 nwb4fp-0.6.3.9/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.571581 nwb4fp-0.6.4.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-28 14:37:20.565579 nwb4fp-0.6.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7191 2024-05-17 14:41:57.000000 nwb4fp-0.6.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:37:20.585581 nwb4fp-0.6.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-28 14:36:22.000000 nwb4fp-0.6.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.165577 nwb4fp-0.6.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.180585 nwb4fp-0.6.4.0/src/nwb4fp/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.288578 nwb4fp-0.6.4.0/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3846 2024-05-16 11:52:07.000000 nwb4fp-0.6.4.0/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.343579 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-05-17 14:54:06.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17455 2024-05-16 12:39:49.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14879 2024-05-28 14:36:04.000000 nwb4fp-0.6.4.0/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.423581 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.185582 nwb4fp-0.6.4.0/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.541577 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb_0283.py
+-rw-rw-rw-   0        0        0     1127 2024-05-17 15:45:56.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1127 2024-05-17 17:22:36.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:37:20.258582 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-28 14:37:19.000000 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2024-05-28 14:37:20.000000 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:37:19.000000 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-28 14:37:19.000000 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 14:37:19.000000 nwb4fp-0.6.4.0/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.3.9/LICENSE` & `nwb4fp-0.6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/PKG-INFO` & `nwb4fp-0.6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.9
+Version: 0.6.4.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.9/README.md` & `nwb4fp-0.6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/setup.py` & `nwb4fp-0.6.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.3.9',
+    version='0.6.4.0',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.4.0/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.4.0/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                             method="auto")
     
     sim = analyzer1.compute("template_similarity", method="cosine_similarity")
     unit_locations = analyzer1.compute(input="unit_locations", method="monopolar_triangulation")
     qm_ext = analyzer1.compute(input={"principal_components": dict(n_components=10, mode="by_channel_local"),
                                 "quality_metrics": dict(skip_pc_metrics=False)})
     qm_data = analyzer1.get_extension("quality_metrics").get_data()
-    keep_mask = (qm_data["presence_ratio"] > 0.9) & (qm_data["isi_violations_ratio"] < 0.2) & (np.float64(qm_data["amplitude_median"]) < np.float64(-40.0)) & (qm_data["d_prime"]>3)& (qm_data["l_ratio"]<0.5)
+    keep_mask = (qm_data["presence_ratio"] > 0.9) & (qm_data["isi_violations_ratio"] < 0.2) & (np.float64(qm_data["amplitude_median"]) < np.float64(-50.0)) & (qm_data["d_prime"]>4)& (qm_data["l_ratio"]<0.05)
     q = sort_merge.get_property('quality')
     b=q
     b[keep_mask] = 'good'
     b[keep_mask==False]='mua'
     unit_ids=sort_merge.unit_ids
     cluster_group = pd.DataFrame(
             {"cluster_id": [i for i in range(len(unit_ids))], "group": b}
@@ -252,22 +252,32 @@
     # sqm.compute_quality_metrics(waveform_extractor=wfm, qm_params=qm_params,sparsity=wf.sparsity, skip_pc_metrics=False)
     # print("completet!!!!automerge & quality_metrix_part")
     path_iron = Path(path + "_manual")
     sex.export_to_phy(analyzer1,
                       output_folder = path_iron,
                       remove_if_exists=True,
                       copy_binary=True)
+    
+    path_iron1 = Path(path + "_4match")
+    sex.export_to_phy(analyzer1,
+                      output_folder = path_iron1,
+                      remove_if_exists=True,
+                      copy_binary=False)
+    
+    cluster_group.to_csv(Path(path_iron1 / r"cluster_group.tsv"), sep="\t", index=False)
     cluster_group.to_csv(Path(path_iron / r"cluster_group.tsv"), sep="\t", index=False)
+
     phy_TRD = Path(path + "_manual_reports")
     sex.export_report(sorting_analyzer = analyzer1, output_folder=phy_TRD, remove_if_exists=True)
     analyzer1.save_as(folder=Path(path + "_manual/waveformsfm"), format="binary_folder")
     #divide_wf(path_iron,sort_merge)
     unit_groups = sort_merge.get_property("group")
     if unit_groups is None:
         unit_groups = np.zeros(len(unit_ids), dtype="int32")
     channel_group = pd.DataFrame({"cluster_id": [i for i in range(len(unit_ids))], "channel_group": unit_groups})
     channel_group.to_csv(path_iron / "cluster_channel_group.tsv", sep="\t", index=False)
+    channel_group.to_csv(path_iron1 / "cluster_channel_group.tsv", sep="\t", index=False)
     print("channel_group")
     print(unit_groups)
     print("completet!!!!_export_to_phy_part")
 if __name__ == "__main__":
     main()
```

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.4.0/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.4.0/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.4.0/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.4.0/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb_0283.py` & `nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb_0283.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 def main():
     import os
     import sys
     base_path = Path("Q:/Sachuriga/Sachuriga_Python")
     base_data_folder = Path("S:/Sachuriga/")
     sex = "F"
-    #animals = ["65091","65165","65283","65409","65410","65588","65935"] 
-    animals = ["65091"] 
+    animals = ["65165","65283","65409","65410","65588","65935"] 
+    #animals = ["65091"] 
     age = "P45+"
     project_name = "CR_CA1"
     species = "Mus musculus"
     vedio_search_directory = base_data_folder/fr"Ephys_Vedio/CR_CA1/"
     path_save = base_data_folder/fr"nwb"
     temp_folder = Path(fr'C:/temp_waveform/{project_name}')
     save_path_test=(r"S:\Sachuriga/Ephys_Recording/4nwb_check.csv")
```

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.4.0/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.4.0/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.9
+Version: 0.6.4.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.4.0/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.9/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.4.0/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

