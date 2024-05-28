# Comparing `tmp/SigProfilerAssignment-0.1.5.tar.gz` & `tmp/SigProfilerAssignment-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SigProfilerAssignment-0.1.5.tar", last modified: Fri May 17 16:50:43 2024, max compression
+gzip compressed data, was "SigProfilerAssignment-0.1.6.tar", last modified: Tue May 28 21:48:42 2024, max compression
```

## Comparing `SigProfilerAssignment-0.1.5.tar` & `SigProfilerAssignment-0.1.6.tar`

### file list

```diff
@@ -1,203 +1,208 @@
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.367061 SigProfilerAssignment-0.1.5/
--rw-r--r--   0 mbarnes    (501) staff       (20)     1342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/LICENSE.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)      719 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/MANIFEST.in
--rw-r--r--   0 mbarnes    (501) staff       (20)    12314 2024-05-17 16:50:43.366582 SigProfilerAssignment-0.1.5/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)    11968 2024-05-17 16:50:32.000000 SigProfilerAssignment-0.1.5/README.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.189056 SigProfilerAssignment-0.1.5/SigProfilerAssignment/
--rw-r--r--   0 mbarnes    (501) staff       (20)     4610 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/Analyzer.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.233077 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/
--rw-r--r--   0 mbarnes    (501) staff       (20)    32944 2024-04-02 19:14:48.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    17348 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16417 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16601 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16771 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16851 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    17285 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    17349 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.239880 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/
--rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
--rw-r--r--   0 mbarnes    (501) staff       (20)      165 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.246055 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/
--rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   267633 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
--rw-r--r--   0 mbarnes    (501) staff       (20)       50 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/__init__.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.434103 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
--rw-r--r--   0 mbarnes    (501) staff       (20)      803 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CNV_features.tsv
--rw-r--r--   0 mbarnes    (501) staff       (20)    15995 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CNV_signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CN_classes_dictionary.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   128402 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.172188 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.579978 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
--rw-r--r--   0 mbarnes    (501) staff       (20)    14328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39321 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    36586 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53285 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   137506 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138652 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   109467 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   148966 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    18940 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17759 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17844 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29808 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   151235 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153270 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    13831 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    18328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    22118 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    96398 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166615 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17757 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17857 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    28686 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)   128501 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129752 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.753527 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39244 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39286 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53205 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53265 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138534 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138665 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150027 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150132 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17825 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17827 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153188 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153263 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31738 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178722 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166497 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     4375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17829 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129685 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129793 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.901440 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39299 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53208 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53279 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138625 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138642 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150107 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150127 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17819 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153243 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33977 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31764 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178725 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166529 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17818 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129718 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129754 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.081125 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39310 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53293 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138548 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138590 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150036 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150053 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153159 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153192 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    34014 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31766 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178728 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166558 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129655 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129717 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.260570 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39230 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39249 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53187 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138524 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138634 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150001 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150098 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153225 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33996 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31745 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178687 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166478 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17840 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129663 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129739 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   380152 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
--rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Samples.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/csvexample.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     8338 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
--rw-r--r--   0 mbarnes    (501) staff       (20)    16970 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    57422 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.173888 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.282010 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/cnv_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)   381521 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.306213 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)     2375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     5496 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     6019 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     6848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1864 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    12790 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     3937 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     2085 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     2359 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1163 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:43.365629 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    63797 2024-05-17 16:50:32.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/decompose_subroutines.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    40644 2024-04-02 19:15:45.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/decomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    36157 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/single_sample.py
--rw-r--r--   0 mbarnes    (501) staff       (20)      207 2024-05-17 16:50:41.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment/version.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-17 16:50:42.193386 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/
--rw-r--r--   0 mbarnes    (501) staff       (20)    12314 2024-05-17 16:50:41.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)    13436 2024-05-17 16:50:42.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/SOURCES.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-05-17 16:50:41.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/dependency_links.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-01-24 20:17:52.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/not-zip-safe
--rw-r--r--   0 mbarnes    (501) staff       (20)      253 2024-05-17 16:50:41.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/requires.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       22 2024-05-17 16:50:41.000000 SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/top_level.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       38 2024-05-17 16:50:43.367188 SigProfilerAssignment-0.1.5/setup.cfg
--rw-r--r--   0 mbarnes    (501) staff       (20)     1626 2024-05-17 16:50:32.000000 SigProfilerAssignment-0.1.5/setup.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.476198 SigProfilerAssignment-0.1.6/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/LICENSE.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)      763 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/MANIFEST.in
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12499 2024-05-28 21:48:42.475247 SigProfilerAssignment-0.1.6/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12153 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/README.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.591948 SigProfilerAssignment-0.1.6/SigProfilerAssignment/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4730 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/Analyzer.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.607181 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6148 2024-05-28 04:03:07.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/.DS_Store
+-rw-r--r--   0 mbarnes    (501) staff       (20)    34335 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17348 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16417 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16601 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16771 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16851 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17285 2024-05-28 09:31:01.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17349 2024-05-27 02:28:53.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.612818 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
+-rw-r--r--   0 mbarnes    (501) staff       (20)      165 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.615528 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   267633 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1102 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/SigProfilerAssignment_CLI.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)       50 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/__init__.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.617147 SigProfilerAssignment-0.1.6/SigProfilerAssignment/controllers/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     8152 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/controllers/cli_controller.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.748964 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
+-rw-r--r--   0 mbarnes    (501) staff       (20)      803 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CNV_features.tsv
+-rw-r--r--   0 mbarnes    (501) staff       (20)    15995 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CNV_signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CN_classes_dictionary.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   128402 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.582467 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.855998 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39321 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)    36586 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53285 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   137506 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138652 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   109467 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   148966 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    18940 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17759 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17844 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29808 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   151235 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153270 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13831 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    18328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    22118 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    96398 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166615 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17757 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17857 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    28686 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)   128501 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129752 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.993437 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39244 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39286 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53205 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53265 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138534 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138665 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150027 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150132 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17825 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17827 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153188 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153263 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31738 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178722 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166497 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17829 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129685 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129793 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.161120 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39299 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53208 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53279 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138625 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138642 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150107 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150127 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17819 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153243 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33977 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31764 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178725 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166529 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17818 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129718 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129754 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.287947 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39310 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53293 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138548 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138590 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150036 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150053 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153159 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153192 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    34014 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31766 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178728 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166558 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129655 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129717 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.391068 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39230 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39249 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53187 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138524 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138634 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150001 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150098 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153225 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33996 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31745 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178687 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166478 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17840 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129663 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129739 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   380152 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
+-rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Samples.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/csvexample.csv
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     8338 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16970 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)    57422 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.584249 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.410165 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/cnv_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   381521 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.430727 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     5496 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6019 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1864 2024-05-27 02:28:53.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12790 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3937 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2085 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2359 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1163 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:42.473962 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    64110 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/decompose_subroutines.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    42090 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/decomposition.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    36157 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/single_sample.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)      182 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment/version.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-05-28 21:48:41.598104 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12499 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13638 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)      104 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/entry_points.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-05-27 02:54:04.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/not-zip-safe
+-rw-r--r--   0 mbarnes    (501) staff       (20)      253 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/requires.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       22 2024-05-28 21:48:41.000000 SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/top_level.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       38 2024-05-28 21:48:42.476444 SigProfilerAssignment-0.1.6/setup.cfg
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1766 2024-05-28 21:48:23.000000 SigProfilerAssignment-0.1.6/setup.py
```

### Comparing `SigProfilerAssignment-0.1.5/LICENSE.txt` & `SigProfilerAssignment-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/MANIFEST.in` & `SigProfilerAssignment-0.1.6/MANIFEST.in`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 include README.md
+include SigProfilerAssignment/controllers/*
 include SigProfilerAssignment/data/*
 include SigProfilerAssignment/data/Reference_Signatures/GRCh37/*
 include SigProfilerAssignment/data/Reference_Signatures/GRCh38/*
 include SigProfilerAssignment/data/Reference_Signatures/mm9/*
 include SigProfilerAssignment/data/Reference_Signatures/mm10/*
 include SigProfilerAssignment/data/Reference_Signatures/rn6/*
 include SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/*
```

### Comparing `SigProfilerAssignment-0.1.5/PKG-INFO` & `SigProfilerAssignment-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -75,14 +75,15 @@
 | signature_database | String | Path to the input set of known mutational signatures (only in case that COSMIC reference signatures are not used), a tab delimited file that contains the signature matrix where the rows are mutation types and columns are signature IDs. |
 | exclude_signature_subgroups | List | Removes the signatures corresponding to specific subtypes to improve refitting (only available when using default COSMIC reference signatures). The usage is explained below. The default value is None, which corresponds to use all COSMIC signatures. |
 | export_probabilities | Boolean | Defines if the probability matrix per mutational context for all samples is created. The default value is True. |
 | export_probabilities_per_mutation | Boolean | Defines if the probability matrices per mutation for all samples are created. Only available when `input_type` is "vcf". The default value is False. |
 | make_plots | Boolean | Toggle on and off for making and saving plots. The default value is True. |
 | sample_reconstruction_plots | String | Select the output format for sample reconstruction plots. Valid inputs are {'pdf', 'png', 'both', None}. The default value is None. |
 | verbose | Boolean | Prints detailed statements. The default value is False. |
+| volume | String | Path to SigProfilerAssignment volumes. Used for Docker/Singularity. Environmental variable "SIGPROFILERASSIGNMENT_VOLUME" takes precedence. Default value is None. |
 
 
 
 ### <a name="subgroups"></a> Signature Subgroups
 
 When using COSMIC reference signatures, some subgroups of signatures can be removed to improve the refitting analysis. To use this feature, the `exclude_signature_subgroups` parameter should be added, following the sintax below:
```

### Comparing `SigProfilerAssignment-0.1.5/README.md` & `SigProfilerAssignment-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 | signature_database | String | Path to the input set of known mutational signatures (only in case that COSMIC reference signatures are not used), a tab delimited file that contains the signature matrix where the rows are mutation types and columns are signature IDs. |
 | exclude_signature_subgroups | List | Removes the signatures corresponding to specific subtypes to improve refitting (only available when using default COSMIC reference signatures). The usage is explained below. The default value is None, which corresponds to use all COSMIC signatures. |
 | export_probabilities | Boolean | Defines if the probability matrix per mutational context for all samples is created. The default value is True. |
 | export_probabilities_per_mutation | Boolean | Defines if the probability matrices per mutation for all samples are created. Only available when `input_type` is "vcf". The default value is False. |
 | make_plots | Boolean | Toggle on and off for making and saving plots. The default value is True. |
 | sample_reconstruction_plots | String | Select the output format for sample reconstruction plots. Valid inputs are {'pdf', 'png', 'both', None}. The default value is None. |
 | verbose | Boolean | Prints detailed statements. The default value is False. |
+| volume | String | Path to SigProfilerAssignment volumes. Used for Docker/Singularity. Environmental variable "SIGPROFILERASSIGNMENT_VOLUME" takes precedence. Default value is None. |
 
 
 
 ### <a name="subgroups"></a> Signature Subgroups
 
 When using COSMIC reference signatures, some subgroups of signatures can be removed to improve the refitting analysis. To use this feature, the `exclude_signature_subgroups` parameter should be added, following the sintax below:
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/Analyzer.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/Analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     new_signature_thresh_hold=0.8,
     exclude_signature_subgroups=None,
     exome=False,
     input_type="matrix",
     context_type="96",
     export_probabilities=True,
     export_probabilities_per_mutation=False,
+    volume=None,
 ):
     decomp.spa_analyze(
         samples=samples,
         output=output,
         signatures=signatures,
         signature_database=signature_database,
         nnls_add_penalty=nnls_add_penalty,
@@ -45,14 +46,15 @@
         new_signature_thresh_hold=new_signature_thresh_hold,
         exclude_signature_subgroups=exclude_signature_subgroups,
         exome=exome,
         input_type=input_type,
         context_type=context_type,
         export_probabilities=export_probabilities,
         export_probabilities_per_mutation=export_probabilities_per_mutation,
+        volume=volume,
     )
 
 
 def denovo_fit(
     samples,
     output,
     signatures=None,
@@ -69,14 +71,15 @@
     devopts=None,
     new_signature_thresh_hold=0.8,
     exome=False,
     input_type="matrix",
     context_type="96",
     export_probabilities=True,
     export_probabilities_per_mutation=False,
+    volume=None,
 ):
     decomp.spa_analyze(
         samples=samples,
         output=output,
         signatures=signatures,
         signature_database=signature_database,
         nnls_add_penalty=nnls_add_penalty,
@@ -94,14 +97,15 @@
         cosmic_fit_option=False,
         devopts=devopts,
         exome=exome,
         input_type=input_type,
         context_type=context_type,
         export_probabilities=export_probabilities,
         export_probabilities_per_mutation=export_probabilities_per_mutation,
+        volume=volume,
     )
 
 
 def cosmic_fit(
     samples,
     output,
     signatures=None,
@@ -119,14 +123,15 @@
     exclude_signature_subgroups=None,
     exome=False,
     input_type="matrix",
     context_type="96",
     export_probabilities=True,
     export_probabilities_per_mutation=False,
     sample_reconstruction_plots=False,
+    volume=None,
 ):
     decomp.spa_analyze(
         samples=samples,
         output=output,
         signatures=signatures,
         signature_database=signature_database,
         nnls_add_penalty=nnls_add_penalty,
@@ -145,8 +150,9 @@
         exclude_signature_subgroups=exclude_signature_subgroups,
         exome=exome,
         input_type=input_type,
         context_type=context_type,
         export_probabilities=export_probabilities,
         export_probabilities_per_mutation=export_probabilities_per_mutation,
         sample_reconstruction_plots=sample_reconstruction_plots,
+        volume=volume,
     )
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 """
 
 import os
 import pandas as pd
 import numpy as np
 import scipy.stats
 import sigProfilerPlotting as sigPlt
-import shutil
 import SigProfilerAssignment
 import SigProfilerAssignment.DecompositionPlots
 from SigProfilerAssignment.DecompositionPlots import SigProfilerPlottingMatrix as mPlt
 from SigProfilerAssignment.DecompositionPlots import (
     PlotDecomposition_SBS96 as spd_96,
     PlotDecomposition_SBS288 as spd_288,
     PlotDecomposition_SBS1536 as spd_1536,
@@ -67,33 +66,32 @@
     "2976",
     "32",
 ]
 DECOMPOSITION_PATH = SigProfilerAssignment.DecompositionPlots.__path__[0]
 REFSIG_PATH = os.path.join(
     SigProfilerAssignment.__path__[0], "data/Reference_Signatures"
 )
-TEMPLATE_PATH = os.path.join(DECOMPOSITION_PATH, "CosmicTemplates")
-
-# Remove templates so that they can be rebuilt
-def remove_cosmic_templates():
-    if not os.path.exists(TEMPLATE_PATH):
-        print("No files are installed at: ", TEMPLATE_PATH)
-    try:
-        shutil.rmtree(TEMPLATE_PATH)
-    except OSError as e:
-        print("Error: %s : %s" % (TEMPLATE_PATH, e.strerror))
+cosmic_template_path = os.path.join(DECOMPOSITION_PATH, "CosmicTemplates")
 
 
 # Create a set of serialized JSON reference signature plots for fast loading
 def install_cosmic_plots(
-    context_type="96", genome_build="GRCh37", cosmic_version="3.4", exome=False
+    context_type="96",
+    genome_build="GRCh37",
+    cosmic_version="3.4",
+    exome=False,
+    volume=None,
 ):
+    global cosmic_template_path
+    # Check if the volume is provided and set the template path
+    if volume is not None:
+        cosmic_template_path = os.path.join(volume, "CosmicTemplates")
 
-    if not os.path.exists(TEMPLATE_PATH):
-        os.mkdir(TEMPLATE_PATH)
+    if not os.path.exists(cosmic_template_path):
+        os.mkdir(cosmic_template_path)
 
     # determine if context is from SBS, ID, DBS, CNV or SV
     context_type_str = ""
     if context_type in SBS_CONTEXTS:
         context_type_str = "SBS"
         # the mtype of the cosmic reference signatures to be plotted
         cosmic_mtype = "96"
@@ -156,29 +154,29 @@
     if context_type in SV_CONTEXTS:
         cosmic_file_name = "COSMIC_v" + str(cosmic_version) + "_SV_GRCh38.txt"
         json_file_name = "COSMIC_v" + str(cosmic_version) + "_SV_GRCh38.json"
         genome_build = "GRCh38"
         exome_str = ""
 
     # Load cosmic plots if they exist
-    filename = os.path.join(TEMPLATE_PATH, json_file_name)
+    filename = os.path.join(cosmic_template_path, json_file_name)
     if os.path.exists(filename):
         cosmic_buff_bytes = json.load(open(filename))
         cosmic_buff_plots = {}
         # Read from JSON, decode, and convert to bytesIO
         for tmp_plots in cosmic_buff_bytes.keys():
             cosmic_buff_plots[tmp_plots] = io.BytesIO(
                 base64.b64decode(cosmic_buff_bytes[tmp_plots])
             )
         return cosmic_buff_plots
 
     # Generate cosmic plots if they were not found
     else:
         cosmic_file_path = os.path.join(REFSIG_PATH, genome_build, cosmic_file_name)
-        json_file_path = os.path.join(TEMPLATE_PATH, json_file_name)
+        json_file_path = os.path.join(cosmic_template_path, json_file_name)
         print(
             "Generating plots for",
             "COSMIC_v"
             + str(cosmic_version)
             + "_"
             + context_type_str
             + "_"
@@ -191,33 +189,36 @@
             cosmic_buff_plots = sigPlt.plotSBS(
                 cosmic_file_path,
                 "buffer",
                 "buffer",
                 cosmic_mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
         elif context_type_str == "DBS":
             cosmic_mtx = pd.read_csv(cosmic_file_path, sep="\t")
             cosmic_buff_plots = sigPlt.plotDBS(
                 cosmic_mtx,
                 "buffer",
                 "buffer",
                 cosmic_mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
         elif context_type_str == "ID":
             cosmic_buff_plots = sigPlt.plotID(
                 cosmic_file_path,
                 "buffer",
                 "buffer",
                 cosmic_mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
         elif context_type_str == "CNV":
             cosmic_buff_plots = sigPlt.plotCNV(
                 cosmic_file_path,
                 "buffer",
                 "buffer",
                 percentage=True,
@@ -339,93 +340,103 @@
         }
     )
     similarities_dataframe = similarities_dataframe.set_index("Sample Names")
 
     return similarities_dataframe
 
 
-def genSBS_pngs(denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp=False):
+def genSBS_pngs(
+    denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp=False, volume=None
+):
     denovo_plots = dict()
     basis_plots = dict()
     if mtype == "1536" or mtype == "288":
+        # this is a special case and we do not support volume here
         denovo_plots = mPlt.plotSBS(
             denovo_mtx, output_path, project, mtype, percentage=True
         )
         if basis_mtx is not None:
             basis_plots = sigPlt.plotSBS(
                 basis_mtx,
                 output_path,
                 project,
                 "96",
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
     elif mtype == "96":
         denovo_plots = sigPlt.plotSBS(
             denovo_mtx,
             output_path,
             project,
             mtype,
             percentage=(not ss_decomp),
             savefig_format="PIL_Image",
+            volume=volume,
         )
         if basis_mtx is not None:
             basis_plots = sigPlt.plotSBS(
                 basis_mtx,
                 output_path,
                 project,
                 mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
     return denovo_plots, basis_plots
 
 
-def genDBS_pngs(denovo_mtx, basis_mtx, output_path, project, mtype):
+def genDBS_pngs(denovo_mtx, basis_mtx, output_path, project, mtype, volume=None):
     denovo_plots = dict()
     basis_plots = dict()
     denovo_plots = sigPlt.plotDBS(
         denovo_mtx,
         output_path,
         project,
         mtype,
         percentage=True,
         savefig_format="PIL_Image",
+        volume=volume,
     )
     if basis_mtx is not None:
         basis_plots = sigPlt.plotDBS(
             basis_mtx,
             output_path,
             project,
             mtype,
             percentage=True,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     return denovo_plots, basis_plots
 
 
-def genID_pngs(denovo_mtx, basis_mtx, output_path, project, mtype):
+def genID_pngs(denovo_mtx, basis_mtx, output_path, project, mtype, volume=None):
     denovo_plots = dict()
     basis_plots = dict()
     denovo_plots = sigPlt.plotID(
         denovo_mtx,
         output_path,
         project,
         mtype,
         percentage=True,
         savefig_format="PIL_Image",
+        volume=volume,
     )
     if basis_mtx is not None:
         basis_plots = sigPlt.plotID(
             basis_mtx,
             output_path,
             project,
             mtype,
             percentage=True,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     return denovo_plots, basis_plots
 
 
 def genCNV_pngs(denovo_mtx, basis_mtx, output_path, project, mtype):
     denovo_plots = dict()
     basis_plots = dict()
@@ -473,35 +484,37 @@
             aggregate=False,
             savefig_format="PIL_Image",
         )
     return denovo_plots, basis_plots
 
 
 # signames, weights
-def gen_sub_plots(denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp):
+def gen_sub_plots(
+    denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp, volume=None
+):
 
     # Make output directory
     if not os.path.exists(output_path):
         os.makedirs(output_path)
 
     if mtype in SBS_CONTEXTS:
         denovo_plots, basis_plots = genSBS_pngs(
-            denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp
+            denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp, volume=volume
         )
         return denovo_plots, basis_plots
 
     elif mtype in DBS_CONTEXTS:
         denovo_plots, basis_plots = genDBS_pngs(
-            denovo_mtx, basis_mtx, output_path, project, mtype
+            denovo_mtx, basis_mtx, output_path, project, mtype, volume=volume
         )
         return denovo_plots, basis_plots
 
     elif mtype in ID_CONTEXTS:
         denovo_plots, basis_plots = genID_pngs(
-            denovo_mtx, basis_mtx, output_path, project, mtype
+            denovo_mtx, basis_mtx, output_path, project, mtype, volume=volume
         )
         return denovo_plots, basis_plots
 
     elif mtype in CNV_CONTEXTS:
         denovo_plots, basis_plots = genCNV_pngs(
             denovo_mtx, basis_mtx, output_path, project, mtype
         )
@@ -514,15 +527,22 @@
 
     else:
         print("ERROR: mtype is " + mtype + " and is not yet supported.")
 
 
 # generate the plot for the reconstruction
 def gen_reconstructed_png_percent(
-    denovo_name, basis_mtx, basis_names, weights, output_path, project, mtype
+    denovo_name,
+    basis_mtx,
+    basis_names,
+    weights,
+    output_path,
+    project,
+    mtype,
+    volume=None,
 ):
     reconstruction_plot = dict()
     mut_col = basis_mtx.iloc[:, 0]
 
     recon_plot = basis_mtx[basis_names[0]] * float(weights[0].strip("%")) / 100
 
     for i in range(1, len(weights)):
@@ -537,41 +557,45 @@
             reconstruction_plot = sigPlt.plotSBS(
                 reconstruction_mtx,
                 output_path,
                 "reconstruction_" + project,
                 "96",
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
         else:
             reconstruction_plot = sigPlt.plotSBS(
                 reconstruction_mtx,
                 output_path,
                 "reconstruction_" + project,
                 mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
     elif mtype in DBS_CONTEXTS:
         reconstruction_plot = sigPlt.plotDBS(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             mtype,
             percentage=True,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     elif mtype in ID_CONTEXTS:
         reconstruction_plot = sigPlt.plotID(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             mtype,
             percentage=True,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     elif mtype in CNV_CONTEXTS:
         reconstruction_plot = sigPlt.plotCNV(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             percentage=True,
@@ -600,14 +624,15 @@
     denovo_name,
     basis_mtx,
     basis_names,
     weights,
     output_path,
     project,
     mtype,
+    volume=None,
 ):
     sample_tmb = denovo_mtx[denovo_name].sum()
     reconstruction_plot = dict()
     mut_col = basis_mtx.iloc[:, 0]
 
     recon_plot = (
         basis_mtx[basis_names[0]] * float(weights[0].strip("%")) / 100 * sample_tmb
@@ -627,41 +652,45 @@
         if mtype == "1536" or mtype == "288":
             reconstruction_plot = sigPlt.plotSBS(
                 reconstruction_mtx,
                 output_path,
                 "reconstruction_" + project,
                 "96",
                 percentage=False,
+                volume=volume,
             )
         else:
             reconstruction_plot = sigPlt.plotSBS(
                 reconstruction_mtx,
                 output_path,
                 "reconstruction_" + project,
                 mtype,
                 percentage=False,
                 savefig_format="PIL_Image",
+                volume=volume,
             )
     elif mtype in DBS_CONTEXTS:
         reconstruction_plot = sigPlt.plotDBS(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             mtype,
             percentage=False,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     elif mtype in ID_CONTEXTS:
         reconstruction_plot = sigPlt.plotID(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             mtype,
             percentage=False,
             savefig_format="PIL_Image",
+            volume=volume,
         )
     elif mtype in CNV_CONTEXTS:
         reconstruction_plot = sigPlt.plotCNV(
             reconstruction_mtx,
             output_path,
             "reconstruction_" + project,
             percentage=True,
@@ -696,15 +725,14 @@
     basis_plots_dict,
     reconstruction_plot_dict,
     reconstruction=False,
     statistics=None,
     cosmic_version=None,
     custom_text=None,
 ):
-
     """
     Generate the correct plot based on mtype.
 
     Parameters:
     ----------
     denovo_name: 				(String) 			Name of denovo signature
     basis_names: 				(List of Strings) 	Names of basis signatures
@@ -713,14 +741,17 @@
     project: 					(String) 			Project name appended to file names
     mtype: 						(String) 			The context 'mtype_options' has valid values
     denovo_plots_dict			(Dictionary)		Signatures are keys, ByteIO plots are values
     basis_plots_dict			(Dictionary)		Signatures are keys, ByteIO plots are values
     reconstruction_plot_dict	(Dictionary)		Signatures are keys, ByteIO plots are values
     reconstruction: 			(Boolean) 			True to generate plot w/ reconstruction
     statistics: 				(Pandas Dataframe) 	Output from calculate_similarities()
+    cosmic_version: 			(String) 			Version of COSMIC signatures
+    custom_text: 				(String) 			Custom text to display on plot
+    volume: 					(String) 			Path to volume where intermediary files are stored
     """
 
     if mtype == "6":
         print("Need to add support for SBS6 Decomposition")
     elif mtype == "24":
         print("Need to add support for SBS24 Decomposition")
     elif mtype == "96":
@@ -861,14 +892,15 @@
     output_path,
     project,
     mtype,
     cosmic_version="3.4",
     genome_build="GRCh37",
     exome=False,
     custom_text=None,
+    volume=None,
 ):
     """
     Generates a decomposition plot of the denovo_mtx using the basis_mtx.
 
     Parameters:
     ----------
 
@@ -891,36 +923,55 @@
 
     mtype: String. The context of the data. Valid values include: "96", "1536","78", and "83".
 
     cosmic_version: String. The version of signatures being used.
 
     custom_text: String. A custom message displayed on decomposition plot.
 
+    exome: Boolean. True if using exome COSMIC signatures, and False if not.
+
+    volume: String. The path to the volume where the cosmic templates are stored and where intermediate files are saved.
+
     Returns:
     -------
     None.
     """
+
     # Create the denovo plots and load basis plots
     denovo_plots_dict, basis_plots_dict = gen_sub_plots(
-        denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp=False
+        denovo_mtx,
+        basis_mtx,
+        output_path,
+        project,
+        mtype,
+        ss_decomp=False,
+        volume=volume,
     )
     reconstructed_mtx, reconstruction_plot_dict = gen_reconstructed_png_percent(
-        denovo_name, basis_mtx, basis_names, weights, output_path, project, mtype
+        denovo_name,
+        basis_mtx,
+        basis_names,
+        weights,
+        output_path,
+        project,
+        mtype,
+        volume=volume,
     )
     # Create a subset matrix with the present signatures
     present_sigs = np.array(basis_mtx[basis_names])
     reconstructed_mtx = np.dot(present_sigs, nonzero_exposures)
     # Convert dictionary of bytes to dictionary of images
     denovo_plots_dict = convert_to_imgReaderDict(denovo_plots_dict)
     # Load in the COSMIC plots
     basis_plots_dict = install_cosmic_plots(
         context_type=mtype,
         genome_build=genome_build,
         cosmic_version=cosmic_version,
         exome=exome,
+        volume=volume,
     )
     basis_plots_dict = {key: basis_plots_dict[key] for key in basis_names}
     basis_plots_dict = convert_to_imgReaderDict(basis_plots_dict)
     # Generate the reconstruction plot
     reconstruction_plot_dict = convert_to_imgReaderDict(reconstruction_plot_dict)
     # Get the reconstruction statistics
     statistics = calculate_similarities(denovo_mtx, denovo_name, reconstructed_mtx)
@@ -956,14 +1007,15 @@
     output_path,
     project,
     context_type,
     genome_build="GRCh37",
     cosmic_version="3.4",
     custom_text=None,
     exome=False,
+    volume=None,
 ):
     """
     Generates a reconstruction of a sample given a set of signatures.
 
     Parameters:
     ----------
 
@@ -1001,35 +1053,43 @@
     Returns:
     -------
     None.
     """
 
     # Create the denovo plots
     denovo_plots_dict = gen_sub_plots(
-        denovo_mtx, None, output_path, project, context_type, ss_decomp=True
+        denovo_mtx,
+        None,
+        output_path,
+        project,
+        context_type,
+        ss_decomp=True,
+        volume=volume,
     )
     denovo_plots_dict = denovo_plots_dict[0]
     # Load in the COSMIC plots
     basis_plots_dict = install_cosmic_plots(
         context_type=context_type,
         genome_build=genome_build,
         cosmic_version=cosmic_version,
         exome=exome,
+        volume=volume,
     )
 
     # Create reconstructed matrix and plot
     reconstructed_mtx, reconstruction_plot_dict = gen_reconstructed_png_numerical(
         denovo_mtx,
         denovo_name,
         basis_mtx,
         basis_names,
         weights,
         output_path,
         project,
         context_type,
+        volume=volume,
     )
 
     denovo_plots_dict = convert_to_imgReaderDict(denovo_plots_dict)
     # subset basis_plots_dict to only the plots used
     basis_plots_dict = {key: basis_plots_dict[key] for key in basis_names}
     basis_plots_dict = convert_to_imgReaderDict(basis_plots_dict)
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CNV_features.tsv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CNV_features.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CNV_signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CNV_signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/CN_classes_dictionary.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/CN_classes_dictionary.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/Samples.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/Samples.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/csvexample.csv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/csvexample.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/decompose_subroutines.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/decompose_subroutines.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,15 @@
     connected_sigs=True,
     make_decomposition_plots=True,
     originalProcessAvg=None,
     new_signature_thresh_hold=0.8,
     sig_exclusion_list=[],
     exome=False,
     m_for_subgroups="SBS",
+    volume=None,
 ):
     originalProcessAvg = originalProcessAvg.reset_index()
     if not os.path.exists(directory + "/Solution_Stats"):
         os.makedirs(directory + "/Solution_Stats")
     # open the log file for signature decomposition
     lognote = open(
         directory
@@ -607,14 +608,15 @@
                 nonzero_exposures / 5000,
                 directory,
                 "test",
                 mtype_par,
                 cosmic_version=cosmic_version,
                 genome_build=genome_build,
                 exome=exome,
+                volume=volume,
             )
             merger.append(byte_plot)
             with alive_bar(
                 1, ctrl_c=False, bar="blocks", title=f"Decompositon Plot:{denovo_name}"
             ) as bar:
                 bar()
 
@@ -756,14 +758,15 @@
     pcawg_rule=False,
     verbose=False,
     make_plots=True,
     samples="./",
     input_type="matrix",
     denovo_refit_option=True,
     exome=False,
+    volume=None,
 ):
     if processAvg.shape[0] == allgenomes.shape[0] and processAvg.shape[0] != 96:
         collapse_to_SBS96 = False
 
     # Get the type of solution from the last part of the layer_directory name
     solution_type = layer_directory.split("/")[-1]
     solution_prefix = solution_type.split("_")
@@ -1322,28 +1325,30 @@
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 "78",
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "INDEL" or m == "83":
             plot.plotID(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 "94",
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "CNV" or m == "48":
             plot.plotCNV(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
@@ -1376,84 +1381,90 @@
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "96":
             plot.plotSBS(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "288":
             plot.plotSBS(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "384":
             plot.plotSBS(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "1536":
             plot.plotSBS(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         elif m == "4608":
             plot.plotSBS(
                 layer_directory
                 + "/Signatures/"
                 + solution_prefix
                 + "_"
                 + "Signatures.txt",
                 layer_directory + "/Signatures/",
                 solution_prefix,
                 m,
                 True,
                 custom_text_upper=signature_stabilities,
                 custom_text_middle=signature_total_mutations,
+                volume=volume,
             )
         else:
             custom_signatures_plot(processes, layer_directory + "/Signatures")
 
     if export_probabilities == True:
         probability = probabilities(
             processAvg, exposureAvg, index, allsigids, allcolnames
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/decomposition.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,44 @@
 from SigProfilerMatrixGenerator.scripts import CNVMatrixGenerator as scna
 from sigProfilerPlotting import sigProfilerPlotting as sigPlot
 import sigProfilerPlotting
 import os, sys
 from PyPDF2 import PdfMerger
 import fitz
 import time
+from pathlib import Path
+
+
+def get_storage_dir(volume=None):
+    """
+    Get the directory for saving/loading storage files.
+
+    :param volume: Optional; User specified directory for saving/loading storage files. SIGPROFILERASSIGNMENT_VOLUME takes precedence over this parameter.
+    :return: The absolute path to the directory to be used for saving/loading storage files as a string, or None if no directory is specified.
+    """
+    # Environment variable name
+    env_var_name = "SIGPROFILERASSIGNMENT_VOLUME"
+
+    # Check if the environment variable is set
+    env_directory = os.getenv(env_var_name)
+
+    # Determine the directory to use
+    if env_directory:
+        storage_dir = Path(env_directory)
+    elif volume:
+        storage_dir = Path(volume)
+    else:
+        storage_dir = None
+
+    # Create the directory if it is not None and does not exist
+    if storage_dir:
+        storage_dir.mkdir(parents=True, exist_ok=True)
+        return str(storage_dir.resolve())
+
+    return None
 
 
 def convert_PDF_to_PNG(input_file_name, output_directory, page_names):
     pdf_doc = fitz.open(input_file_name)
     zoom = 3
     magnify = fitz.Matrix(zoom, zoom)
 
@@ -100,14 +130,15 @@
             weights,
             output_dir,
             project,
             mtype,
             genome_build=execution_parameters["reference_genome"],
             cosmic_version=str(execution_parameters["cosmic_version"]),
             exome=execution_parameters["exome"],
+            volume=get_storage_dir(execution_parameters["volume"]),
         )
         final_pdf.append(result)
 
     pdf_output_path = os.path.join(
         output_dir, "Reconstructed_Sample_Plots_" + str(mtype) + ".pdf"
     )
     web_png_path = os.path.join(output_dir, "WebPNGs")
@@ -130,14 +161,16 @@
     sysdata.write("INPUT DATA\n")
     sysdata.write("\tinput_type: {}\n".format(execution_parameters["input_type"]))
     sysdata.write("\toutput: {}\n".format(execution_parameters["output"]))
     if isinstance(execution_parameters["samples"], str):
         sysdata.write("\tsamples: {}\n".format(execution_parameters["samples"]))
     else:
         sysdata.write("\tsamples: {}\n".format(type(execution_parameters["samples"])))
+    if execution_parameters["volume"] is not None:
+        sysdata.write("\tvolume: {}\n".format(execution_parameters["volume"]))
     sysdata.write(
         "\treference_genome: {}\n".format(execution_parameters["reference_genome"])
     )
     sysdata.write("\tcontext_types: {}\n".format(execution_parameters["context_type"]))
     sysdata.write("\texome: {}\n".format(execution_parameters["exome"]))
 
     sysdata.write("COSMIC MATCH\n")
@@ -211,14 +244,15 @@
     new_signature_thresh_hold=0.8,
     exclude_signature_subgroups=None,
     exome=False,
     export_probabilities=True,
     export_probabilities_per_mutation=False,
     sample_reconstruction_plots=None,
     make_metadata=True,
+    volume=None,
 ):
     """
     Decomposes the De Novo Signatures into COSMIC Signatures and assigns COSMIC signatures into samples.
 
     Parameters:
 
         signatures: A string. Path to a  tab delimited file that contains the signaure table where the rows are mutation types and colunms are signature IDs.
@@ -248,14 +282,17 @@
         >>>signatures = "path/to/dDe_Novo_Solution_Signatures.txt"
         >>>activities="path/to/De_Novo_Solution_Activities.txt"
         >>>samples="path/to/Samples.txt"
         >>>output="name or path/to/output.txt"
         decomp.decompose(signatures, activities, samples, output, genome_build="GRCh37", verbose=False)
 
     """
+
+    volume = get_storage_dir(volume)
+
     if devopts == None:
         layer_directory1 = output + "/De_Novo_Solution"
         layer_directory2 = output + "/Decompose_Solution"
         layer_directory3 = output + "/Assignment_Solution"
     else:
         layer_directory1 = devopts["denovo_outpath"]
         layer_directory2 = devopts["decompose_outpath"]
@@ -276,14 +313,15 @@
             genome_build,
             samples,
             exome=exome,
             bed_file=None,
             chrom_based=False,
             plot=False,
             gs=False,
+            volume=volume,
         )
         genomes = data[vcf_context]
 
     elif input_type.split(":")[0].lower() == "seg":
         cnv_file_type = input_type.split(":")[1].upper()
         context_type = "CNV48"
         genomes = scna.generateCNVMatrix(
@@ -441,14 +479,15 @@
         "nnls_add_penalty": nnls_add_penalty,
         "nnls_remove_penalty": nnls_remove_penalty,
         "initial_remove_penalty": initial_remove_penalty,
         "de_novo_fit_penalty": de_novo_fit_penalty,
         "collapse_to_SBS96": collapse_to_SBS96,
         "export_probabilities": export_probabilities,
         "make_plots": make_plots,
+        "volume": volume,
     }
 
     if make_metadata:
         # create JOB_METADATA_SPA
         sysdata = open(os.path.join(output, "JOB_METADATA_SPA.txt"), "w")
         sysdata.write("THIS FILE CONTAINS THE METADATA ABOUT SYSTEM AND RUNTIME\n\n\n")
         sysdata.write("-------System Info-------\n")
@@ -628,14 +667,15 @@
                 make_plots=make_plots,
                 export_probabilities=export_probabilities,
                 export_probabilities_per_mutation=export_probabilities_per_mutation,
                 samples=samples,
                 input_type=input_type,
                 denovo_refit_option=denovo_refit_option,
                 exome=exome,
+                volume=volume,
             )
 
         else:
             signature_stabilities = devopts["signature_stabilities"]
             signature_total_mutations = devopts["signature_total_mutations"]
             signature_stats = devopts["signature_stats"]
             sequence = devopts["sequence"]
@@ -666,14 +706,15 @@
                 refit_denovo_signatures=True,
                 export_probabilities=export_probabilities,
                 export_probabilities_per_mutation=export_probabilities_per_mutation,
                 samples=samples,
                 input_type=input_type,
                 denovo_refit_option=denovo_refit_option,
                 exome=exome,
+                volume=volume,
             )
 
         if make_metadata:
             with open(os.path.join(output, "JOB_METADATA_SPA.txt"), "a") as sysdata:
                 current_time_end = datetime.datetime.now()
                 sysdata.write(
                     f"\n Finished Denovo fitting! \nExecution time:{str(current_time_end-current_time_start)}\n"
@@ -790,14 +831,15 @@
             remove_penalty=0.01,
             make_decomposition_plots=make_decomposition_plots,
             originalProcessAvg=originalProcessAvg,
             new_signature_thresh_hold=new_signature_thresh_hold,
             sig_exclusion_list=sig_exclusion_list,
             exome=exome,
             m_for_subgroups=m_for_subgroups,
+            volume=volume,
         )
         # final_signatures = sub.signature_decomposition(processAvg, m, layer_directory2, genome_build=genome_build)
         # extract the global signatures and new signatures from the final_signatures dictionary
         globalsigs = final_signatures["globalsigs"]
         globalsigs = np.array(globalsigs)
         newsigs = final_signatures["newsigs"]
         processAvg = np.hstack([globalsigs, newsigs])
@@ -840,14 +882,15 @@
             make_plots=make_plots,
             export_probabilities=export_probabilities,
             export_probabilities_per_mutation=export_probabilities_per_mutation,
             samples=samples,
             input_type=input_type,
             denovo_refit_option=denovo_refit_option,
             exome=exome,
+            volume=volume,
         )
 
         if make_metadata:
             with open(os.path.join(output, "JOB_METADATA_SPA.txt"), "a") as sysdata:
                 current_time_end = datetime.datetime.now()
                 sysdata.write(
                     f"\n Finished Decompose fitting! \nExecution time:{str(current_time_end-current_time_start)}\n"
@@ -1001,14 +1044,15 @@
             make_plots=make_plots,
             export_probabilities=export_probabilities,
             export_probabilities_per_mutation=export_probabilities_per_mutation,
             samples=samples,
             input_type=input_type,
             denovo_refit_option=denovo_refit_option,
             exome=exome,
+            volume=volume,
         )
         if make_metadata:
             with open(os.path.join(output, "JOB_METADATA_SPA.txt"), "a") as sysdata:
                 current_time_end = datetime.datetime.now()
                 sysdata.write(
                     f"\n Finished Cosmic fitting! \nExecution time:{str(current_time_end-current_time_start)}\n"
                 )
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment/single_sample.py` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment/single_sample.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/PKG-INFO` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -75,14 +75,15 @@
 | signature_database | String | Path to the input set of known mutational signatures (only in case that COSMIC reference signatures are not used), a tab delimited file that contains the signature matrix where the rows are mutation types and columns are signature IDs. |
 | exclude_signature_subgroups | List | Removes the signatures corresponding to specific subtypes to improve refitting (only available when using default COSMIC reference signatures). The usage is explained below. The default value is None, which corresponds to use all COSMIC signatures. |
 | export_probabilities | Boolean | Defines if the probability matrix per mutational context for all samples is created. The default value is True. |
 | export_probabilities_per_mutation | Boolean | Defines if the probability matrices per mutation for all samples are created. Only available when `input_type` is "vcf". The default value is False. |
 | make_plots | Boolean | Toggle on and off for making and saving plots. The default value is True. |
 | sample_reconstruction_plots | String | Select the output format for sample reconstruction plots. Valid inputs are {'pdf', 'png', 'both', None}. The default value is None. |
 | verbose | Boolean | Prints detailed statements. The default value is False. |
+| volume | String | Path to SigProfilerAssignment volumes. Used for Docker/Singularity. Environmental variable "SIGPROFILERASSIGNMENT_VOLUME" takes precedence. Default value is None. |
 
 
 
 ### <a name="subgroups"></a> Signature Subgroups
 
 When using COSMIC reference signatures, some subgroups of signatures can be removed to improve the refitting analysis. To use this feature, the `exclude_signature_subgroups` parameter should be added, following the sintax below:
```

### Comparing `SigProfilerAssignment-0.1.5/SigProfilerAssignment.egg-info/SOURCES.txt` & `SigProfilerAssignment-0.1.6/SigProfilerAssignment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 SigProfilerAssignment/Analyzer.py
+SigProfilerAssignment/SigProfilerAssignment_CLI.py
 SigProfilerAssignment/__init__.py
 SigProfilerAssignment/decompose_subroutines.py
 SigProfilerAssignment/decomposition.py
 SigProfilerAssignment/single_sample.py
 SigProfilerAssignment/version.py
 SigProfilerAssignment.egg-info/PKG-INFO
 SigProfilerAssignment.egg-info/SOURCES.txt
 SigProfilerAssignment.egg-info/dependency_links.txt
+SigProfilerAssignment.egg-info/entry_points.txt
 SigProfilerAssignment.egg-info/not-zip-safe
 SigProfilerAssignment.egg-info/requires.txt
 SigProfilerAssignment.egg-info/top_level.txt
+SigProfilerAssignment/DecompositionPlots/.DS_Store
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py
 SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
+SigProfilerAssignment/controllers/cli_controller.py
 SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
 SigProfilerAssignment/data/CNV_features.tsv
 SigProfilerAssignment/data/CNV_signatures.txt
 SigProfilerAssignment/data/CN_classes_dictionary.txt
 SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
 SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
 SigProfilerAssignment/data/Samples.txt
```

### Comparing `SigProfilerAssignment-0.1.5/setup.py` & `SigProfilerAssignment-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import shutil
 import os
 
 # remove the dist folder first if exists
 if os.path.exists("dist"):
     shutil.rmtree("dist")
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 
 
 def write_version_py(filename="SigProfilerAssignment/version.py"):
     # Copied from numpy setup.py
     cnt = """
 # THIS FILE IS GENERATED FROM SigProfilerAssignment SETUP.PY
 short_version = '%(version)s'
 version = '%(version)s'
-Update = 'v0.1.5: Add text for stability and mutation count to the de novo signature plots.'
+Update = 'v0.1.6: Add CLI and volume parameter for template files.'
 
     
     """
     fh = open(filename, "w")
     fh.write(
         cnt
         % {
@@ -58,9 +58,14 @@
     url="https://github.com/AlexandrovLab/SigProfilerAssignment.git",
     author="Raviteja Vangara",
     author_email="rvangara@health.ucsd.edu",
     license="UCSD",
     packages=["SigProfilerAssignment"],
     install_requires=requirements,
     include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "SigProfilerAssignment=SigProfilerAssignment.SigProfilerAssignment_CLI:main_function",
+        ],
+    },
     zip_safe=False,
 )
```

