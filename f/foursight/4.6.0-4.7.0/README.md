# Comparing `tmp/foursight-4.6.0.tar.gz` & `tmp/foursight-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-4.6.0.tar", max compression
+gzip compressed data, was "foursight-4.7.0.tar", max compression
```

## Comparing `foursight-4.6.0.tar` & `foursight-4.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.6.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.6.0/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.6.0/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.6.0/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.6.0/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.6.0/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    65198 2024-04-25 19:24:12.957388 foursight-4.6.0/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.6.0/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.6.0/chalicelib_fourfront/checks/check_utils.py
--rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.6.0/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.6.0/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.6.0/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.6.0/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.6.0/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      558 2024-04-25 19:24:12.958156 foursight-4.6.0/chalicelib_fourfront/checks/helpers/es_utils.py
--rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.6.0/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95977 2024-03-13 13:41:24.369808 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17738 2024-04-11 16:56:14.128461 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.6.0/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.6.0/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45228 2024-04-25 19:24:12.959767 foursight-4.6.0/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.6.0/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    45350 2024-04-11 16:56:14.129826 foursight-4.6.0/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   141107 2024-04-25 19:24:12.962591 foursight-4.6.0/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.6.0/chalicelib_fourfront/gitinfo.json
--rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.6.0/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.6.0/chalicelib_fourfront/scripts/local_check_execution.py
--rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.6.0/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1610 2024-04-25 19:24:12.966149 foursight-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.7.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.7.0/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.7.0/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.7.0/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.7.0/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.7.0/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    65198 2024-04-25 19:24:12.957388 foursight-4.7.0/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.7.0/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.7.0/chalicelib_fourfront/checks/check_utils.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.7.0/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.7.0/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.7.0/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.7.0/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.7.0/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      558 2024-04-25 19:24:12.958156 foursight-4.7.0/chalicelib_fourfront/checks/helpers/es_utils.py
+-rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.7.0/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    97040 2024-05-28 18:10:53.231905 foursight-4.7.0/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17790 2024-05-28 18:10:53.232643 foursight-4.7.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.7.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.7.0/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.7.0/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45228 2024-04-25 19:24:12.959767 foursight-4.7.0/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.7.0/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    45350 2024-04-11 16:56:14.129826 foursight-4.7.0/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   141107 2024-04-25 19:24:12.962591 foursight-4.7.0/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.7.0/chalicelib_fourfront/gitinfo.json
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.7.0/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.7.0/chalicelib_fourfront/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.7.0/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1610 2024-05-28 18:10:53.233373 foursight-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.7.0/PKG-INFO
```

### Comparing `foursight-4.6.0/LICENSE.txt` & `foursight-4.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/app_utils.py` & `foursight-4.7.0/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/check_schedules.py` & `foursight-4.7.0/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/check_setup.json` & `foursight-4.7.0/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/audit_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/badge_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/check_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/es_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/header_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/helpers/es_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/helpers/es_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     },
     "fastqc": {
         "run_time": 50,
         "accepted_versions": ["v1", "v2"]
     },
     "bwa-mem": {
         "run_time": 50,
-        "accepted_versions": ["0.2.6"]
+        "accepted_versions": ["0.2.6", "0.3.0"]
     },
     "pairsqc-single": {
         "run_time": 100,
         "accepted_versions": ["0.2.5", "0.2.6"]
     },
     "hi-c-processing-bam": {
         "run_time": 200,
-        "accepted_versions": ["0.2.6"]
+        "accepted_versions": ["0.2.6", "0.3.0"]
     },
     "hi-c-processing-pairs": {
         "run_time": 200,
-        "accepted_versions": ["0.2.6", "0.2.7"]
+        "accepted_versions": ["0.3.0"]
     },
     "hi-c-processing-pairs-nore": {
         "run_time": 200,
         "accepted_versions": ["0.2.6"]
     },
     "hi-c-processing-pairs-nonorm": {
         "run_time": 200,
@@ -155,35 +155,35 @@
     }
 }
 
 
 # accepted versions for completed pipelines
 accepted_versions = {
     # OFFICIAL
-    'in situ Hi-C':  ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'in situ Hi-C':  ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # OFFICIAL
-    'Dilution Hi-C': ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'Dilution Hi-C': ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # OFFICIAL
-    'TCC':           ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'TCC':           ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # OFFICIAL  # NO-RE
-    'DNase Hi-C':    ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'DNase Hi-C':    ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # OFFICIAL  # NO-NORM
-    'Capture Hi-C':  ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'Capture Hi-C':  ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # OFFICIAL  # NO-RE
-    'Micro-C':       ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'Micro-C':       ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # Preliminary - Released to network  # NO-RE NO-NORM
-    'ChIA-PET':      ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'ChIA-PET':      ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # Preliminary - Released to network  # NO-RE NO-NORM
-    'in situ ChIA-PET': ["HiC_Pipeline_0.2.7"],
+    'in situ ChIA-PET': ["HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # Preliminary - Released to network  # NO-RE NO-NORM
-    'TrAC-loop':     ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'TrAC-loop':     ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # Preliminary - Released to network  # NO-NORM
-    'PLAC-seq':      ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7"],
+    'PLAC-seq':      ["HiC_Pipeline_0.2.6", "HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # Preliminary - Released to network  # NO-NORM
-    'HiChIP': ["HiC_Pipeline_0.2.7"],
+    'HiChIP': ["HiC_Pipeline_0.2.7", "HiC_Pipeline_0.3.0"],
     # bwa mem # handled manually for now
     'MARGI':         ['MARGI_Pipeline_1.1.1_dcic_4'],
     # Preliminary -  Don't release - (Released to network is pending approval from Belmont lab)
     'TSA-seq':       ['RepliSeq_Pipeline_v13.1_step1',
                       'RepliSeq_Pipeline_v14_step1',
                       'RepliSeq_Pipeline_v16_step1',
                       'RepliSeq_Pipeline_v16.1_step1'],
@@ -1406,22 +1406,31 @@
                 If True:
                    If set/exp is released/to project processing results go to other_processed_files field
                    If set/exp is in other status, processing results go to processed_files field
     pc_append: (bool) If True and move_to_pc is True - append outfiles to existing processed files
             This is relevant for pipelines that produce files to be added to datasets upon which a pipeline (eg. Hi-C)
             has already been run - eg. Compartment Caller or Insulation Score/Boundaries
     """
-    titles = {"hic": "HiC Processing Pipeline - Preliminary Files",
+    titles = {"hic": "HiC Processing Pipeline - v0.3.0",
               "repliseq": "Repli-Seq Pipeline - Preliminary Files",
               'chip': "ENCODE ChIP-Seq Pipeline - Preliminary Files",
               'atac': "ENCODE ATAC-Seq Pipeline - Preliminary Files",
               'margi': "iMARGI Processing Pipeline - Preliminary Files",
               'rnaseq': "ENCODE RNA-Seq Pipeline - Preliminary Files",
               'insulation_scores_and_boundaries': "Insulation scores and boundaries calls - Preliminary Files",
               'compartments': "Compartments Signals - Preliminary Files"}
+
+    descriptions = {'hic': ("These are files generated using the updated Hi-C processing pipeline. "
+            "They should be largely similar to those available in the Processed Files tab, which were generated "
+            "with the previous version of the standard pipeline.  One potential difference of note is that the "
+            "version of cooler used to generate the mcool file has a bug fix to prevent a pixel duplication "
+            "issue which is observed in some files generated by the previous version of the pipeline.  Another "
+            "notable difference is that a filter is applied to remove reads with MAPQ scores below 30 prior "
+            "to mcool file generation.")}
+
     """move files to other processed_files field."""
     if not patch_data.get('patch_opf'):
         return ['no content in patch_opf, skipping']
     if not patch_data.get('add_tag'):
         return ['no tag info, skipping']
     pc_set_title = titles[pipeline_type]
     log = []
@@ -1480,14 +1489,18 @@
                 patch_val = ff_utils.get_metadata(acc, key=auth, add_on='frame=raw').get('other_processed_files', [])
             else:
                 patch_val = []
 
             new_data = {'title': pc_set_title,
                         'type': 'preliminary',
                         'files': list_pc}
+
+            if pipeline_type in descriptions:
+                new_data["description"] = descriptions[pipeline_type]
+
             patch_val.append(new_data)
             patch_body = {'other_processed_files': patch_val}
             ff_utils.patch_metadata(patch_body, obj_id=acc, key=auth)
     # add the tag
     set_acc = patch_data['add_tag'][0]
     new_tag = patch_data['add_tag'][1]
     existing_tags = ff_utils.get_metadata(set_acc, auth).get('completed_processes', [])
```

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,42 +54,43 @@
     {
         'app_name': 'pairsqc-single',
         'workflow_uuid': 'b8c533e0-f8c0-4510-b4a1-ac35158e27c3',
         "config": {"instance_type": 't3.small'}
     },
     {
         'app_name': 'bwa-mem',
-        'workflow_uuid': '3feedadc-50f9-4bb4-919b-09a8b731d0cc',
+        'workflow_uuid': '60952f14-693a-434b-9cb2-face065620f6',
         'parameters': {"nThreads": 16},
         'custom_pf_fields': {
             'out_bam': {
                 'genome_assembly': genome,
                 'file_type': 'intermediate file',
                 'description': int_n}
         }
     },
     {
         'app_name': 'hi-c-processing-bam',
-        'workflow_uuid': '023bfb3e-9a8b-42b9-a9d4-216079526f68',
+        'workflow_uuid': '6b2f1481-163e-4099-ae9b-ee49587107d3',
         'parameters': {"nthreads_merge": 16, "nthreads_parse_sort": 16},
         'custom_pf_fields': {
             'annotated_bam': {
                 'genome_assembly': genome,
                 'file_type': 'alignments',
                 'description': out_n},
             'filtered_pairs': {
                 'genome_assembly': genome,
                 'file_type': 'contact list-replicate',
                 'description': out_n}
         }
     },
     {
         'app_name': 'hi-c-processing-pairs',
-        'workflow_uuid': '4dn-dcic-lab:wf-hi-c-processing-pairs-0.2.7',
-        'parameters': {"nthreads": 4,
+        'workflow_uuid': '4dn-dcic-lab:wf-hi-c-processing-pairs-0.3.0',
+        'config': {"instance_type": 'r5a.2xlarge'},
+        'parameters': {"nthreads": 8,
                        "maxmem": "32g",
                        "max_split_cooler": 10,
                        "no_balance": False
                        },
         'custom_pf_fields': {
             'hic': {
                 'genome_assembly': genome,
```

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-4.7.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/system_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-4.7.0/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/chalicelib_fourfront/package.py` & `foursight-4.7.0/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-4.6.0/pyproject.toml` & `foursight-4.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight"
-version = "4.6.0"
+version = "4.7.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
```

### Comparing `foursight-4.6.0/PKG-INFO` & `foursight-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 4.6.0
+Version: 4.7.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

