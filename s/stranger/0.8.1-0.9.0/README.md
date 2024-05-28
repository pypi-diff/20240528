# Comparing `tmp/stranger-0.8.1.tar.gz` & `tmp/stranger-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stranger-0.8.1.tar", last modified: Wed Jan 26 16:03:44 2022, max compression
+gzip compressed data, was "dist/stranger-0.9.0.tar", last modified: Tue May 28 07:57:23 2024, max compression
```

## Comparing `stranger-0.8.1.tar` & `stranger-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/
--rw-r--r--   0 dannil     (501) staff       (20)    12162 2022-01-26 16:03:44.000000 stranger-0.8.1/PKG-INFO
--rw-r--r--   0 dannil     (501) staff       (20)     1054 2021-06-07 13:19:33.000000 stranger-0.8.1/LICENSE
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/
--rw-r--r--   0 dannil     (501) staff       (20)    12162 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/PKG-INFO
--rw-r--r--   0 dannil     (501) staff       (20)      698 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/SOURCES.txt
--rw-r--r--   0 dannil     (501) staff       (20)       61 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/entry_points.txt
--rw-r--r--   0 dannil     (501) staff       (20)       52 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/requires.txt
--rw-r--r--   0 dannil     (501) staff       (20)        9 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/top_level.txt
--rw-r--r--   0 dannil     (501) staff       (20)        1 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger.egg-info/dependency_links.txt
--rw-r--r--   0 dannil     (501) staff       (20)     2285 2022-01-26 16:00:28.000000 stranger-0.8.1/CHANGELOG.md
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/tests/
--rw-r--r--   0 dannil     (501) staff       (20)     2025 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/test_utils.py
--rw-r--r--   0 dannil     (501) staff       (20)      334 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/conftest.py
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/tests/cli/
--rw-r--r--   0 dannil     (501) staff       (20)      497 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/cli/test_cli.py
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/tests/fixtures/
--rw-r--r--   0 dannil     (501) staff       (20)     6337 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf
--rw-r--r--   0 dannil     (501) staff       (20)     1695 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf.gz.tbi
--rw-r--r--   0 dannil     (501) staff       (20)     1631 2021-06-07 13:19:33.000000 stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf.gz
--rw-r--r--   0 dannil     (501) staff       (20)      454 2021-06-07 13:19:33.000000 stranger-0.8.1/MANIFEST.in
--rw-r--r--   0 dannil     (501) staff       (20)     9999 2021-06-07 13:19:33.000000 stranger-0.8.1/README.md
--rwxr-xr-x   0 dannil     (501) staff       (20)     4524 2021-06-07 13:19:33.000000 stranger-0.8.1/setup.py
--rw-r--r--   0 dannil     (501) staff       (20)       38 2022-01-26 16:03:44.000000 stranger-0.8.1/setup.cfg
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger/
-drwxr-xr-x   0 dannil     (501) staff       (20)        0 2022-01-26 16:03:44.000000 stranger-0.8.1/stranger/resources/
--rw-r--r--   0 dannil     (501) staff       (20)      367 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/resources/__init__.py
--rw-r--r--   0 dannil     (501) staff       (20)      954 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/resources/repeatexpansionsloci.tsv
--rwxr-xr-x   0 dannil     (501) staff       (20)    30099 2022-01-26 16:00:28.000000 stranger-0.8.1/stranger/resources/variant_catalog_grch37.json
--rw-r--r--   0 dannil     (501) staff       (20)      287 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/constants.py
--rw-r--r--   0 dannil     (501) staff       (20)        0 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/__init__.py
--rw-r--r--   0 dannil     (501) staff       (20)       22 2022-01-26 16:00:28.000000 stranger-0.8.1/stranger/__version__.py
--rw-r--r--   0 dannil     (501) staff       (20)      604 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/vcf_utils.py
--rw-r--r--   0 dannil     (501) staff       (20)     5843 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/cli.py
--rw-r--r--   0 dannil     (501) staff       (20)     7632 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/utils.py
--rwxr-xr-x   0 dannil     (501) staff       (20)      402 2021-06-07 13:19:33.000000 stranger-0.8.1/stranger/__main__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/
+-rw-r--r--   0 dannil     (501) staff       (20)    13262 2024-05-28 07:57:23.000000 stranger-0.9.0/PKG-INFO
+-rw-r--r--   0 dannil     (501) staff       (20)     1054 2018-11-29 09:04:39.000000 stranger-0.9.0/LICENSE
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/
+-rw-r--r--   0 dannil     (501) staff       (20)    13262 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/PKG-INFO
+-rw-r--r--   0 dannil     (501) staff       (20)      698 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/SOURCES.txt
+-rw-r--r--   0 dannil     (501) staff       (20)       61 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/entry_points.txt
+-rw-r--r--   0 dannil     (501) staff       (20)       52 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/requires.txt
+-rw-r--r--   0 dannil     (501) staff       (20)        9 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/top_level.txt
+-rw-r--r--   0 dannil     (501) staff       (20)        1 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger.egg-info/dependency_links.txt
+-rw-r--r--   0 dannil     (501) staff       (20)     2629 2024-05-21 12:01:23.000000 stranger-0.9.0/CHANGELOG.md
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/tests/
+-rw-r--r--   0 dannil     (501) staff       (20)     2025 2018-12-17 10:25:09.000000 stranger-0.9.0/tests/test_utils.py
+-rw-r--r--   0 dannil     (501) staff       (20)      334 2019-12-04 10:29:12.000000 stranger-0.9.0/tests/conftest.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/tests/cli/
+-rw-r--r--   0 dannil     (501) staff       (20)      497 2019-04-11 14:10:05.000000 stranger-0.9.0/tests/cli/test_cli.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/tests/fixtures/
+-rw-r--r--   0 dannil     (501) staff       (20)     6337 2018-11-29 09:04:39.000000 stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf
+-rw-r--r--   0 dannil     (501) staff       (20)     1695 2018-11-29 09:04:39.000000 stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)     1631 2018-11-29 09:04:39.000000 stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      454 2019-12-03 18:12:25.000000 stranger-0.9.0/MANIFEST.in
+-rw-r--r--   0 dannil     (501) staff       (20)    11067 2024-05-21 12:42:00.000000 stranger-0.9.0/README.md
+-rwxr-xr-x   0 dannil     (501) staff       (20)     4524 2019-04-11 14:10:05.000000 stranger-0.9.0/setup.py
+-rw-r--r--   0 dannil     (501) staff       (20)       38 2024-05-28 07:57:23.000000 stranger-0.9.0/setup.cfg
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2024-05-28 07:57:23.000000 stranger-0.9.0/stranger/resources/
+-rw-r--r--   0 dannil     (501) staff       (20)      367 2019-05-16 08:53:03.000000 stranger-0.9.0/stranger/resources/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      954 2020-10-23 15:43:23.000000 stranger-0.9.0/stranger/resources/repeatexpansionsloci.tsv
+-rwxr-xr-x   0 dannil     (501) staff       (20)    29394 2024-05-21 11:58:22.000000 stranger-0.9.0/stranger/resources/variant_catalog_grch37.json
+-rw-r--r--   0 dannil     (501) staff       (20)      474 2024-04-15 11:13:17.000000 stranger-0.9.0/stranger/constants.py
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2018-11-29 09:04:39.000000 stranger-0.9.0/stranger/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)       22 2024-05-21 12:01:55.000000 stranger-0.9.0/stranger/__version__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      604 2018-11-29 09:04:39.000000 stranger-0.9.0/stranger/vcf_utils.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6992 2024-04-15 11:13:17.000000 stranger-0.9.0/stranger/cli.py
+-rw-r--r--   0 dannil     (501) staff       (20)    14702 2024-05-21 11:58:22.000000 stranger-0.9.0/stranger/utils.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)      402 2018-11-29 09:04:39.000000 stranger-0.9.0/stranger/__main__.py
```

### Comparing `stranger-0.8.1/PKG-INFO` & `stranger-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: stranger
-Version: 0.8.1
+Version: 0.9.0
 Summary: Annotate VCF files with str variants
 Home-page: https://github.com/moonso/stranger
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Description: 
         # Stranger [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url] [![PyPI Version][pypi-img]][pypi-url][![DOI][doi-image]][doi-url]
         
-        Annotates output files from [ExpansionHunter][hunter] with the pathologic implications of the repeat sizes.
+        Annotates output files from [ExpansionHunter][hunter] and [TRGT][trgt] with the pathologic implications of the repeat sizes.
         
         ## Installation
         
         ```
-        git clone github.com/moonso/stranger
+        git clone github.com/clinical-genomics/stranger
         cd stranger
         pip install --editable .
         ```
         
         ## Usage
         
         ```
-        stranger --help
         Usage: stranger [OPTIONS] VCF
         
           Annotate str variants with str status
         
         Options:
           -f, --repeats-file PATH         Path to a file with repeat definitions. See
-                                          README for explanation  [default: $HOME/stranger
-                                          /stranger/resources/variant_catalog_grch37.json]
-          -i, --family_id TEXT            Family ID used in RankScore output
+                                          README for explanation  [default: $HOME/
+                                          stranger/stranger/resources/vari
+                                          ant_catalog_grch37.json]
+          -i, --family_id TEXT
+          -t, --trgt                      File was produced with TRGT
           --version
           --loglevel [DEBUG|INFO|WARNING|ERROR|CRITICAL]
                                           Set the level of log output.  [default:
                                           INFO]
           --help                          Show this message and exit.
-        
         ```
         
         
         ## Repeat definitions
         
         The repeats are called with Expansion Hunter as mentioned earlier. ExpansionHunter will annotate the number of times that a repeat has been seen in the bam files of each individual and what repeat id the variant has.
         Stranger will annotate the level of pathogenicity for the repeat number. The intervals that comes with the package are manually collected from the literature since there is no single source where this information can be collected.
         
         You can find a repeat definitions json file that comes with Stranger [here](https://github.com/moonso/stranger/blob/master/stranger/resources/variant_catalog_grch37.json). It is based on the ExpansionHunter variant catalog, but extended with a few disease locus relevant keys:
         
-        | Column/Key | Content/Value |
-        | ------- | ------- |
-        | HGNC_ID | HGNC identifier for the repeat or most associated gene. |
-        | HGNC_SYMBOL |HGNC symbol for the repeat or most associated gene. |
-        | REPID | ExpansionHunter repeat ID. |
-        | RU | Basic repeat unit, as seen in ExpansionHunter. Unused. |
-        | DisplayRU | Repeat unit, as clinicians are used to see it. |
-        | Normal_Max | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
-        | Pathologic_Min | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
-        | Disease | Associated disease. |
-        | InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc |
-        | Source | Reference literature resource type, eg GeneReviews or PubMed |
-        | SourceId | PMID or GeneReviews book ID for references|
+        | Column/Key      | Content/Value                                                                                   |
+        |-----------------|-------------------------------------------------------------------------------------------------|
+        | HGNC_ID         | HGNC identifier for the repeat or most associated gene.                                         |
+        | HGNC_SYMBOL     | HGNC symbol for the repeat or most associated gene.                                             |
+        | REPID           | ExpansionHunter repeat ID.                                                                      |
+        | RU              | Basic repeat unit, as seen in ExpansionHunter. Unused.                                          |
+        | DisplayRU       | Repeat unit, as clinicians are used to see it.                                                  |
+        | Normal_Max      | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
+        | Pathologic_Min  | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
+        | Disease         | Associated disease.                                                                             |
+        | InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc                                                        |
+        | Source          | Reference literature resource type, eg GeneReviews or PubMed                                    |
+        | SourceId        | PMID or GeneReviews book ID for references                                                      |
+        | TRID            | Trgt repeat ID if not same as REPID                                                             |
+        | PathologicStruc | Array of index for pathogenic motif                                                             |
+        
         
         Other fields accepted by ExpansionHunter are also encouraged.
         
         For convenience, here is a formated table with some of the current contents:
         
         | HGNCId | LocusId | DisplayRU | InheritanceMode | normal_max | pathologic_min | Disease | SourceDisplay | SourceId |
         | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- |
@@ -159,14 +162,15 @@
         
         ```
         ##INFO=<ID=STR_STATUS,Number=A,Type=String,Description="Repeat expansion status. Alternatives in [normal, pre_mutation, full_mutation]">
         4       3076603 .       C       <STR17>,<STR18> .       PASS    END=3076660;REF=19;RL=57;RU=CAG;VARID=HTT;REPID=HTT;STR_STATUS=normal,normal
         ```
         
         [hunter]: https://github.com/Illumina/ExpansionHunter
+        [trgt]: https://github.com/PacificBiosciences/trgt
         
         [travis-url]: https://travis-ci.com/moonso/stranger
         [travis-image]: https://travis-ci.com/moonso/stranger.svg?branch=master
         [pypi-img]: https://img.shields.io/pypi/v/stranger.svg?style=flat-square
         [pypi-url]: https://pypi.python.org/pypi/stranger/
         [coveralls-url]: https://coveralls.io/github/moonso/stranger
         [coveralls-image]: https://coveralls.io/repos/github/moonso/stranger/badge.svg?branch=master
```

### Comparing `stranger-0.8.1/LICENSE` & `stranger-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/stranger.egg-info/PKG-INFO` & `stranger-0.9.0/stranger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: stranger
-Version: 0.8.1
+Version: 0.9.0
 Summary: Annotate VCF files with str variants
 Home-page: https://github.com/moonso/stranger
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Description: 
         # Stranger [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url] [![PyPI Version][pypi-img]][pypi-url][![DOI][doi-image]][doi-url]
         
-        Annotates output files from [ExpansionHunter][hunter] with the pathologic implications of the repeat sizes.
+        Annotates output files from [ExpansionHunter][hunter] and [TRGT][trgt] with the pathologic implications of the repeat sizes.
         
         ## Installation
         
         ```
-        git clone github.com/moonso/stranger
+        git clone github.com/clinical-genomics/stranger
         cd stranger
         pip install --editable .
         ```
         
         ## Usage
         
         ```
-        stranger --help
         Usage: stranger [OPTIONS] VCF
         
           Annotate str variants with str status
         
         Options:
           -f, --repeats-file PATH         Path to a file with repeat definitions. See
-                                          README for explanation  [default: $HOME/stranger
-                                          /stranger/resources/variant_catalog_grch37.json]
-          -i, --family_id TEXT            Family ID used in RankScore output
+                                          README for explanation  [default: $HOME/
+                                          stranger/stranger/resources/vari
+                                          ant_catalog_grch37.json]
+          -i, --family_id TEXT
+          -t, --trgt                      File was produced with TRGT
           --version
           --loglevel [DEBUG|INFO|WARNING|ERROR|CRITICAL]
                                           Set the level of log output.  [default:
                                           INFO]
           --help                          Show this message and exit.
-        
         ```
         
         
         ## Repeat definitions
         
         The repeats are called with Expansion Hunter as mentioned earlier. ExpansionHunter will annotate the number of times that a repeat has been seen in the bam files of each individual and what repeat id the variant has.
         Stranger will annotate the level of pathogenicity for the repeat number. The intervals that comes with the package are manually collected from the literature since there is no single source where this information can be collected.
         
         You can find a repeat definitions json file that comes with Stranger [here](https://github.com/moonso/stranger/blob/master/stranger/resources/variant_catalog_grch37.json). It is based on the ExpansionHunter variant catalog, but extended with a few disease locus relevant keys:
         
-        | Column/Key | Content/Value |
-        | ------- | ------- |
-        | HGNC_ID | HGNC identifier for the repeat or most associated gene. |
-        | HGNC_SYMBOL |HGNC symbol for the repeat or most associated gene. |
-        | REPID | ExpansionHunter repeat ID. |
-        | RU | Basic repeat unit, as seen in ExpansionHunter. Unused. |
-        | DisplayRU | Repeat unit, as clinicians are used to see it. |
-        | Normal_Max | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
-        | Pathologic_Min | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
-        | Disease | Associated disease. |
-        | InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc |
-        | Source | Reference literature resource type, eg GeneReviews or PubMed |
-        | SourceId | PMID or GeneReviews book ID for references|
+        | Column/Key      | Content/Value                                                                                   |
+        |-----------------|-------------------------------------------------------------------------------------------------|
+        | HGNC_ID         | HGNC identifier for the repeat or most associated gene.                                         |
+        | HGNC_SYMBOL     | HGNC symbol for the repeat or most associated gene.                                             |
+        | REPID           | ExpansionHunter repeat ID.                                                                      |
+        | RU              | Basic repeat unit, as seen in ExpansionHunter. Unused.                                          |
+        | DisplayRU       | Repeat unit, as clinicians are used to see it.                                                  |
+        | Normal_Max      | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
+        | Pathologic_Min  | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
+        | Disease         | Associated disease.                                                                             |
+        | InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc                                                        |
+        | Source          | Reference literature resource type, eg GeneReviews or PubMed                                    |
+        | SourceId        | PMID or GeneReviews book ID for references                                                      |
+        | TRID            | Trgt repeat ID if not same as REPID                                                             |
+        | PathologicStruc | Array of index for pathogenic motif                                                             |
+        
         
         Other fields accepted by ExpansionHunter are also encouraged.
         
         For convenience, here is a formated table with some of the current contents:
         
         | HGNCId | LocusId | DisplayRU | InheritanceMode | normal_max | pathologic_min | Disease | SourceDisplay | SourceId |
         | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- |
@@ -159,14 +162,15 @@
         
         ```
         ##INFO=<ID=STR_STATUS,Number=A,Type=String,Description="Repeat expansion status. Alternatives in [normal, pre_mutation, full_mutation]">
         4       3076603 .       C       <STR17>,<STR18> .       PASS    END=3076660;REF=19;RL=57;RU=CAG;VARID=HTT;REPID=HTT;STR_STATUS=normal,normal
         ```
         
         [hunter]: https://github.com/Illumina/ExpansionHunter
+        [trgt]: https://github.com/PacificBiosciences/trgt
         
         [travis-url]: https://travis-ci.com/moonso/stranger
         [travis-image]: https://travis-ci.com/moonso/stranger.svg?branch=master
         [pypi-img]: https://img.shields.io/pypi/v/stranger.svg?style=flat-square
         [pypi-url]: https://pypi.python.org/pypi/stranger/
         [coveralls-url]: https://coveralls.io/github/moonso/stranger
         [coveralls-image]: https://coveralls.io/repos/github/moonso/stranger/badge.svg?branch=master
```

### Comparing `stranger-0.8.1/stranger.egg-info/SOURCES.txt` & `stranger-0.9.0/stranger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/CHANGELOG.md` & `stranger-0.9.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
-## [x.x.x]
+## [0.9.0]
+- Add Docker image
+- Parse TRGT VCFs - in particular, decompose and parse FORMAT.MC
+- Bring in updated loci references from raredisese reference-files
+- Fix processing TRGT VCFs with missing MC and TRIDs without underscore [#59](https://github.com/Clinical-Genomics/stranger/pull/59)
+- Updates to pathogenic motifs for two loci: RFC1, RAPGEF2
+
 
 ## [0.8.1]
 Fix DAB1 pathologic repeat unit name
 Update POLG coords, quite a bit on hg38
 
 ## [0.8.0]
 Off by one error on PathogenticMin output. All affected have at least been cautioned pre_mutation with proper size.
```

### Comparing `stranger-0.8.1/tests/test_utils.py` & `stranger-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf` & `stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf.gz.tbi` & `stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/tests/fixtures/643594.clinical.str.vcf.gz` & `stranger-0.9.0/tests/fixtures/643594.clinical.str.vcf.gz`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/README.md` & `stranger-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 # Stranger [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url] [![PyPI Version][pypi-img]][pypi-url][![DOI][doi-image]][doi-url]
 
-Annotates output files from [ExpansionHunter][hunter] with the pathologic implications of the repeat sizes.
+Annotates output files from [ExpansionHunter][hunter] and [TRGT][trgt] with the pathologic implications of the repeat sizes.
 
 ## Installation
 
 ```
-git clone github.com/moonso/stranger
+git clone github.com/clinical-genomics/stranger
 cd stranger
 pip install --editable .
 ```
 
 ## Usage
 
 ```
-stranger --help
 Usage: stranger [OPTIONS] VCF
 
   Annotate str variants with str status
 
 Options:
   -f, --repeats-file PATH         Path to a file with repeat definitions. See
-                                  README for explanation  [default: $HOME/stranger
-                                  /stranger/resources/variant_catalog_grch37.json]
-  -i, --family_id TEXT            Family ID used in RankScore output
+                                  README for explanation  [default: $HOME/
+                                  stranger/stranger/resources/vari
+                                  ant_catalog_grch37.json]
+  -i, --family_id TEXT
+  -t, --trgt                      File was produced with TRGT
   --version
   --loglevel [DEBUG|INFO|WARNING|ERROR|CRITICAL]
                                   Set the level of log output.  [default:
                                   INFO]
   --help                          Show this message and exit.
-
 ```
 
 
 ## Repeat definitions
 
 The repeats are called with Expansion Hunter as mentioned earlier. ExpansionHunter will annotate the number of times that a repeat has been seen in the bam files of each individual and what repeat id the variant has.
 Stranger will annotate the level of pathogenicity for the repeat number. The intervals that comes with the package are manually collected from the literature since there is no single source where this information can be collected.
 
 You can find a repeat definitions json file that comes with Stranger [here](https://github.com/moonso/stranger/blob/master/stranger/resources/variant_catalog_grch37.json). It is based on the ExpansionHunter variant catalog, but extended with a few disease locus relevant keys:
 
-| Column/Key | Content/Value |
-| ------- | ------- |
-| HGNC_ID | HGNC identifier for the repeat or most associated gene. |
-| HGNC_SYMBOL |HGNC symbol for the repeat or most associated gene. |
-| REPID | ExpansionHunter repeat ID. |
-| RU | Basic repeat unit, as seen in ExpansionHunter. Unused. |
-| DisplayRU | Repeat unit, as clinicians are used to see it. |
-| Normal_Max | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
-| Pathologic_Min | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
-| Disease | Associated disease. |
-| InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc |
-| Source | Reference literature resource type, eg GeneReviews or PubMed |
-| SourceId | PMID or GeneReviews book ID for references|
+| Column/Key      | Content/Value                                                                                   |
+|-----------------|-------------------------------------------------------------------------------------------------|
+| HGNC_ID         | HGNC identifier for the repeat or most associated gene.                                         |
+| HGNC_SYMBOL     | HGNC symbol for the repeat or most associated gene.                                             |
+| REPID           | ExpansionHunter repeat ID.                                                                      |
+| RU              | Basic repeat unit, as seen in ExpansionHunter. Unused.                                          |
+| DisplayRU       | Repeat unit, as clinicians are used to see it.                                                  |
+| Normal_Max      | (#copies) Longest repeat expected for normal individual; higher are marked pre- or full-mutation |
+| Pathologic_Min  | (#copies) Shortest repeat expected for pathology. This and higher is annotated as full-mutation. |
+| Disease         | Associated disease.                                                                             |
+| InheritanceMode | Mode of inheritance "AR", "AD", "XR" etc                                                        |
+| Source          | Reference literature resource type, eg GeneReviews or PubMed                                    |
+| SourceId        | PMID or GeneReviews book ID for references                                                      |
+| TRID            | Trgt repeat ID if not same as REPID                                                             |
+| PathologicStruc | Array of index for pathogenic motif                                                             |
+
 
 Other fields accepted by ExpansionHunter are also encouraged.
 
 For convenience, here is a formated table with some of the current contents:
 
 | HGNCId | LocusId | DisplayRU | InheritanceMode | normal_max | pathologic_min | Disease | SourceDisplay | SourceId |
 | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- |
@@ -150,14 +153,15 @@
 
 ```
 ##INFO=<ID=STR_STATUS,Number=A,Type=String,Description="Repeat expansion status. Alternatives in [normal, pre_mutation, full_mutation]">
 4       3076603 .       C       <STR17>,<STR18> .       PASS    END=3076660;REF=19;RL=57;RU=CAG;VARID=HTT;REPID=HTT;STR_STATUS=normal,normal
 ```
 
 [hunter]: https://github.com/Illumina/ExpansionHunter
+[trgt]: https://github.com/PacificBiosciences/trgt
 
 [travis-url]: https://travis-ci.com/moonso/stranger
 [travis-image]: https://travis-ci.com/moonso/stranger.svg?branch=master
 [pypi-img]: https://img.shields.io/pypi/v/stranger.svg?style=flat-square
 [pypi-url]: https://pypi.python.org/pypi/stranger/
 [coveralls-url]: https://coveralls.io/github/moonso/stranger
 [coveralls-image]: https://coveralls.io/repos/github/moonso/stranger/badge.svg?branch=master
```

### Comparing `stranger-0.8.1/setup.py` & `stranger-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/stranger/resources/repeatexpansionsloci.tsv` & `stranger-0.9.0/stranger/resources/repeatexpansionsloci.tsv`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/stranger/resources/variant_catalog_grch37.json` & `stranger-0.9.0/stranger/resources/variant_catalog_grch37.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7502842002185489%*

 * *Differences: {'1': "{'LocusStructure': '(CCG)*', 'ReferenceRegion': 'X:147582158-147582203', delete: "*

 * *      "['SweGenMean', 'SweGenStd']}",*

 * * '10': "{'PathologicStruc': [1]}",*

 * * '11': "{'DisplayRU': 'GGGGCC', 'TRID': 'FTDALS1_C9orf72'}",*

 * * '14': "{'NormalMax': 35, 'PathologicMin': 50}",*

 * * '15': "{'PathologicStruc': [0]}",*

 * * '17': "{'PathologicStruc': [1]}",*

 * * '2': "{'NormalMax': 35}",*

 * * '20': "{'PathologicStruc': [0]}",*

 * * '23': "{'ReferenceRegion': '3:138664862-138664904'}",*

 * * '25': "{'ReferenceRegion': '2:176957786-176957831'} […]*

```diff
@@ -1,33 +1,43 @@
 [
     {
+        "Disease": "OPDM",
+        "DisplayRU": "CCG",
+        "HGNCId": 67,
+        "InheritanceMode": "AD",
+        "LocusId": "ABCD3",
+        "LocusStructure": "(CCG)*",
+        "NormalMax": 50,
+        "PathologicMin": 118,
+        "ReferenceRegion": "1:94883978-94884000",
+        "VariantType": "Repeat"
+    },
+    {
         "Disease": "Fraxe",
         "DisplayRU": "CCG",
         "HGNCId": 3776,
         "InheritanceMode": "XR",
         "LocusId": "AFF2",
-        "LocusStructure": "(GCC)*",
+        "LocusStructure": "(CCG)*",
         "NormalMax": 39,
         "PathologicMin": 200,
-        "ReferenceRegion": "X:147582151-147582211",
+        "ReferenceRegion": "X:147582158-147582203",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
-        "SweGenMean": 23.87,
-        "SweGenStd": 7.523,
         "VariantType": "Repeat"
     },
     {
         "Disease": "SBMA",
         "DisplayRU": "CAG",
         "HGNCId": 644,
         "InheritanceMode": "XR",
         "LocusId": "AR",
         "LocusStructure": "(GCA)*",
-        "NormalMax": 34,
+        "NormalMax": 35,
         "PathologicMin": 38,
         "ReferenceRegion": "X:66765158-66765227",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "SweGenMean": 22.94,
         "SweGenStd": 3.366,
@@ -37,46 +47,32 @@
         "Disease": "EIEE",
         "DisplayRU": "GCN",
         "HGNCId": 18060,
         "InheritanceMode": "XR",
         "LocusId": "ARX_EIEE",
         "LocusStructure": "(NGC)*",
         "NormalMax": 16,
-        "PathologicMin": 17,
+        "PathologicMin": 18,
         "ReferenceRegion": "X:25031766-25031814",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
-        "VariantType": "Repeat"
-    },
-    {
-        "Disease": "PRTS",
-        "DisplayRU": "GCN",
-        "HGNCId": 18060,
-        "InheritanceMode": "XR",
-        "LocusId": "ARX_PRTS",
-        "LocusStructure": "(NGC)*",
-        "NormalMax": 12,
-        "PathologicMin": 20,
-        "ReferenceRegion": "X:25031646-25031682",
-        "Source": "GeneReviews",
-        "SourceDisplay": "GeneReviews Internet 2019-11-07",
-        "SourceId": "NBK535148",
+        "TRID": "EIEE1_ARX",
         "VariantType": "Repeat"
     },
     {
         "Disease": "DRPLA",
         "DisplayRU": "CAG",
         "HGNCId": 3033,
         "InheritanceMode": "AD",
         "LocusId": "ATN1",
         "LocusStructure": "(CAG)*",
         "NormalMax": 35,
         "PathologicMin": 48,
-        "ReferenceRegion": "12:7045879-7045936",
+        "ReferenceRegion": "12:7045891-7045936",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "SweGenMean": 17.99,
         "SweGenStd": 3.053,
         "VariantType": "Repeat"
     },
@@ -99,95 +95,89 @@
     },
     {
         "Disease": "SCA1",
         "DisplayRU": "CAG",
         "HGNCId": 10548,
         "InheritanceMode": "AD",
         "LocusId": "ATXN1",
-        "LocusStructure": "(TGC)*",
+        "LocusStructure": "(CTG)*",
         "NormalMax": 35,
-        "PathologicMin": 45,
-        "ReferenceRegion": "6:16327864-16327954",
+        "PathologicMin": 40,
+        "ReferenceRegion": "6:16327866-16327953",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2017-06-22",
         "SourceId": "NBK1184",
         "SweGenMean": 31.17,
         "SweGenStd": 2.022,
         "VariantType": "Repeat"
     },
     {
         "Disease": "SCA2",
         "DisplayRU": "CAG",
         "HGNCId": 10555,
         "InheritanceMode": "AD",
         "LocusId": "ATXN2",
-        "LocusStructure": "(GCT)*",
+        "LocusStructure": "(CTG)*",
         "NormalMax": 31,
-        "PathologicMin": 37,
+        "PathologicMin": 33,
         "ReferenceRegion": "12:112036753-112036822",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-02-14",
         "SourceId": "NBK1275",
         "SweGenMean": 22.11,
         "SweGenStd": 1.353,
         "VariantType": "Repeat"
     },
     {
         "Disease": "MJD",
         "DisplayRU": "CAG",
         "HGNCId": 7106,
         "InheritanceMode": "AD",
         "LocusId": "ATXN3",
-        "LocusStructure": "(GCT)*",
+        "LocusStructure": "(CTG)*",
         "NormalMax": 44,
-        "PathologicMin": 60,
-        "ReferenceRegion": "14:92537353-92537386",
+        "PathologicMin": 56,
+        "ReferenceRegion": "14:92537354-92537384",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "VariantType": "Repeat"
     },
     {
         "Disease": "SCA7",
         "DisplayRU": "CAG",
         "HGNCId": 10560,
         "InheritanceMode": "AD",
         "LocusId": "ATXN7",
-        "LocusStructure": "(GCA)*(GCC)+",
+        "LocusStructure": "(CAG)*",
         "NormalMax": 19,
         "PathologicMin": 36,
-        "PathologicRegion": "3:63898360-63898390",
-        "ReferenceRegion": [
-            "3:63898360-63898390",
-            "3:63898390-63898402"
+        "PathologicRegion": "3:63898361-63898391",
+        "PathologicStruc": [
+            0
         ],
+        "ReferenceRegion": "3:63898361-63898391",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
-        "SweGenMean": 10.31,
-        "SweGenStd": 1.285,
-        "VariantId": [
-            "ATXN7",
-            "ATXN7_GCC"
-        ],
-        "VariantType": [
-            "Repeat",
-            "Repeat"
-        ]
+        "VariantType": "Repeat"
     },
     {
         "Disease": "SCA8",
         "DisplayRU": "CTG",
         "HGNCId": 10561,
         "InheritanceMode": "AD",
         "LocusId": "ATXN8OS",
         "LocusStructure": "(CTA)*(CTG)*",
         "NormalMax": 50,
         "PathologicMin": 80,
         "PathologicRegion": "13:70713515-70713560",
+        "PathologicStruc": [
+            1
+        ],
         "ReferenceRegion": [
             "13:70713485-70713515",
             "13:70713515-70713560"
         ],
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
@@ -200,15 +190,15 @@
         "VariantType": [
             "Repeat",
             "Repeat"
         ]
     },
     {
         "Disease": "FTDALS1",
-        "DisplayRU": "GGCCCC",
+        "DisplayRU": "GGGGCC",
         "HGNCId": 28337,
         "InheritanceMode": "AD",
         "LocusId": "C9ORF72",
         "LocusStructure": "(GGCCCC)*",
         "NormalMax": 25,
         "OfftargetRegions": [
             "1:150552238-150552273",
@@ -244,14 +234,15 @@
         "PathologicMin": 40,
         "ReferenceRegion": "9:27573526-27573544",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "SweGenMean": 4.42,
         "SweGenStd": 3.815,
+        "TRID": "FTDALS1_C9orf72",
         "VariantType": "RareRepeat"
     },
     {
         "Disease": "SCA6",
         "DisplayRU": "CAG",
         "HGNCId": 1388,
         "InheritanceMode": "AD",
@@ -287,16 +278,16 @@
     {
         "Disease": "SCA31",
         "DisplayRU": "TGGAA",
         "HGNCId": 24160,
         "InheritanceMode": "AD",
         "LocusId": "BEAN1",
         "LocusStructure": "(TGGAA)*TAAAATAAAATAAAATAAAATAAAATAAAATAAAATAAAATAAAATAAAA",
-        "NormalMax": 10,
-        "PathologicMin": 40,
+        "NormalMax": 35,
+        "PathologicMin": 50,
         "ReferenceRegion": "16:66524301-66524356",
         "Source": "PubMed",
         "SourceDisplay": "Sato et al AJHG 2009",
         "SourceId": "19878914",
         "VariantType": "Repeat"
     },
     {
@@ -305,14 +296,17 @@
         "HGNCId": 13164,
         "InheritanceMode": "AD",
         "LocusId": "CNBP",
         "LocusStructure": "(CAGG)*(CAGA)*(CA)*",
         "NormalMax": 30,
         "PathologicMin": 75,
         "PathologicRegion": "3:128891419-128891499",
+        "PathologicStruc": [
+            0
+        ],
         "ReferenceRegion": [
             "3:128891419-128891499",
             "3:128891499-128891539",
             "3:128891539-128891575"
         ],
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2020-03-19",
@@ -353,14 +347,17 @@
         "HGNCId": 2661,
         "InheritanceMode": "AD",
         "LocusId": "DAB1",
         "LocusStructure": "(AAAAT)*(GAAAT)*(AAAAT)*",
         "NormalMax": 16,
         "PathologicMin": 31,
         "PathologicRegion": "1:57832725-57832780",
+        "PathologicStruc": [
+            1
+        ],
         "ReferenceRegion": [
             "1:57832715-57832725",
             "1:57832725-57832780",
             "1:57832780-57832790"
         ],
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-05-30",
@@ -416,14 +413,17 @@
         "HGNCId": 18683,
         "InheritanceMode": "AR",
         "LocusId": "EIF4A3",
         "LocusStructure": "(CCTCGCTGCGCCGCTGCCGA)*(CCTCGCTGTGCCGCTGCCGA)*",
         "NormalMax": 9,
         "PathologicMin": 10,
         "PathologicRegion": "17:78120821-78120840",
+        "PathologicStruc": [
+            0
+        ],
         "ReferenceRegion": [
             "17:78120821-78120840",
             "17:78120841-78120938"
         ],
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
@@ -433,14 +433,30 @@
         ],
         "VariantType": [
             "Repeat",
             "Repeat"
         ]
     },
     {
+        "Disease": "SCA27B",
+        "DisplayRU": "GAA",
+        "HGNCId": 3671,
+        "InheritanceMode": "AD",
+        "LocusId": "FGF14",
+        "LocusStructure": "(GAA)*",
+        "NormalMax": 150,
+        "PathologicMin": 250,
+        "ReferenceRegion": "13:102813926-102814076",
+        "Source": "PubMed",
+        "SourceDisplay": "Rafehi et al 2022 AJHG S0002-9297(22)00506-7",
+        "SourceId": "36493768",
+        "VariantId": "FGF14",
+        "VariantType": "Repeat"
+    },
+    {
         "Disease": "FragileX",
         "DisplayRU": "CGG",
         "HGNCId": 3775,
         "InheritanceMode": "XR",
         "LocusId": "FMR1",
         "LocusStructure": "(CGG)*",
         "NormalMax": 55,
@@ -480,15 +496,15 @@
         "DisplayRU": "GCN",
         "HGNCId": 1092,
         "InheritanceMode": "AD",
         "LocusId": "FOXL2",
         "LocusStructure": "(NGC)*",
         "NormalMax": 14,
         "PathologicMin": 15,
-        "ReferenceRegion": "3:138664863-138664904",
+        "ReferenceRegion": "3:138664862-138664904",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "VariantType": "Repeat"
     },
     {
         "Disease": "FRDA",
@@ -515,81 +531,36 @@
         ],
         "VariantType": [
             "Repeat",
             "Repeat"
         ]
     },
     {
-        "Disease": "HFGS",
-        "DisplayRU": "GCN",
-        "HGNCId": 5102,
-        "InheritanceMode": "AD",
-        "LocusId": "HOXA13_I",
-        "LocusStructure": "(NGC)*",
-        "NormalMax": 14,
-        "PathologicMin": 22,
-        "ReferenceRegion": "7:27239544-27239585",
-        "Source": "GeneReviews",
-        "SourceDisplay": "GeneReviews Internet 2019-08-08",
-        "SourceId": "NBK1423",
-        "VariantType": "Repeat"
-    },
-    {
-        "Disease": "HFGS",
-        "DisplayRU": "GCN",
-        "HGNCId": 5102,
-        "InheritanceMode": "AD",
-        "LocusId": "HOXA13_II",
-        "LocusStructure": "(NGC)*",
-        "NormalMax": 12,
-        "PathologicMin": 18,
-        "ReferenceRegion": "7:27239445-27239480",
-        "Source": "GeneReviews",
-        "SourceDisplay": "GeneReviews Internet 2019-08-08",
-        "SourceId": "NBK1423",
-        "VariantType": "Repeat"
-    },
-    {
-        "Disease": "HFGS",
-        "DisplayRU": "GCN",
-        "HGNCId": 5102,
-        "InheritanceMode": "AD",
-        "LocusId": "HOXA13_III",
-        "LocusStructure": "(NGC)*",
-        "NormalMax": 18,
-        "PathologicMin": 24,
-        "ReferenceRegion": "7:27239298-27239351",
-        "Source": "GeneReviews",
-        "SourceDisplay": "GeneReviews Internet 2019-08-08",
-        "SourceId": "NBK1423",
-        "VariantType": "Repeat"
-    },
-    {
         "Disease": "SDTY5",
         "DisplayRU": "GCN",
         "HGNCId": 5136,
         "InheritanceMode": "AD",
         "LocusId": "HOXD13",
         "LocusStructure": "(GCN)*",
         "NormalMax": 15,
         "PathologicMin": 22,
-        "ReferenceRegion": "2:176957787-176957831",
+        "ReferenceRegion": "2:176957786-176957831",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "VariantType": "Repeat"
     },
     {
         "Disease": "Huntington",
         "DisplayRU": "CAG",
         "HGNCId": 4851,
         "InheritanceMode": "AD",
         "LocusId": "HTT",
         "LocusStructure": "(CAG)*CAACAG(CCG)*",
-        "NormalMax": 26,
+        "NormalMax": 34,
         "PathologicMin": 36,
         "PathologicRegion": "4:3076603-3076660",
         "ReferenceRegion": [
             "4:3076603-3076660",
             "4:3076666-3076693"
         ],
         "Source": "GeneReviews",
@@ -643,15 +614,15 @@
         "DisplayRU": "GGC",
         "HGNCId": 1226,
         "InheritanceMode": "AD",
         "LocusId": "GIPC1",
         "LocusStructure": "(CCG)*",
         "NormalMax": 32,
         "PathologicMin": 73,
-        "ReferenceRegion": "19:14606854-14606886",
+        "ReferenceRegion": "19:14606853-14606886",
         "Source": "PubMed",
         "SourceDisplay": "Deng et al 2020 AJHG 106(6) 793-804",
         "SourceId": "32413282",
         "VariantType": "Repeat"
     },
     {
         "Disease": "SCA36",
@@ -659,14 +630,17 @@
         "HGNCId": 15911,
         "InheritanceMode": "AD",
         "LocusId": "NOP56",
         "LocusStructure": "(GGCCTG)*(CGCCTG)*",
         "NormalMax": 14,
         "PathologicMin": 650,
         "PathologicRegion": "20:2633379-2633403",
+        "PathologicStruc": [
+            0
+        ],
         "ReferenceRegion": [
             "20:2633379-2633403",
             "20:2633403-2633421"
         ],
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2014-08-07",
         "SourceId": "NBK231880",
@@ -699,17 +673,17 @@
     {
         "Disease": "CCHS",
         "DisplayRU": "GCN",
         "HGNCId": 9143,
         "InheritanceMode": "AD",
         "LocusId": "PHOX2B",
         "LocusStructure": "(GCN)*",
-        "NormalMax": 20,
+        "NormalMax": 21,
         "PathologicMin": 25,
-        "ReferenceRegion": "4:41747988-41748049",
+        "ReferenceRegion": "4:41747988-41748048",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2014-01-30",
         "SourceId": "NBK1427",
         "SweGenMean": 26.33,
         "SweGenStd": 11.88,
         "VariantType": "Repeat"
     },
@@ -736,14 +710,17 @@
         "HGNCId": 16854,
         "InheritanceMode": "AD",
         "LocusId": "RAPGEF2",
         "LocusStructure": "(TTTTA)*(TTTCA)*(TTTTA)*",
         "NormalMax": 1,
         "PathologicMin": 10,
         "PathologicRegion": "4:160263704-160263708",
+        "PathologicStruc": [
+            1
+        ],
         "ReferenceRegion": [
             "4:160263679-160263703",
             "4:160263704-160263708",
             "4:160263709-160263768"
         ],
         "Source": "PubMed",
         "SourceDisplay": "Ishiura et al (2018) Nature Genetics 50 581-90",
@@ -756,14 +733,61 @@
         "VariantType": [
             "Repeat",
             "Repeat",
             "Repeat"
         ]
     },
     {
+        "Disease": "CANVAS",
+        "DisplayRU": "AARRG",
+        "HGNCId": 9969,
+        "InheritanceMode": "AR",
+        "LocusId": "RFC1",
+        "LocusStructure": "(AARRG)*",
+        "NormalMax": 11,
+        "PathologicMin": 12,
+        "ReferenceRegion": "4:39350044-39350099",
+        "Source": "PubMed",
+        "SourceDisplay": "Cortese et al 2019 Nat Gen",
+        "SourceId": "30926972",
+        "SweGenMean": 26.77,
+        "SweGenStd": 18.68,
+        "VariantType": "Repeat"
+    },
+    {
+        "Disease": "OPDM4",
+        "DisplayRU": "CGG",
+        "HGNCId": 26814,
+        "InheritanceMode": "AD",
+        "LocusId": "RILPL1",
+        "LocusStructure": "(GGC)*",
+        "NormalMax": 16,
+        "PathologicMin": 139,
+        "ReferenceRegion": "12:124018267-124018302",
+        "Source": "PubMed",
+        "SourceDisplay": "Yu et al (2022) AJHG 109(3):533-541",
+        "SourceId": "35148830",
+        "VariantType": "Repeat"
+    },
+    {
+        "Disease": "CCD",
+        "DisplayRU": "GCN",
+        "HGNCId": 10472,
+        "InheritanceMode": "AD",
+        "LocusId": "RUNX2",
+        "LocusStructure": "(GCN)*",
+        "NormalMax": 17,
+        "PathologicMin": 20,
+        "ReferenceRegion": "6:45390487-45390538",
+        "Source": "GeneReviews",
+        "SourceDisplay": "GeneReviews Internet 2019-11-07",
+        "SourceId": "NBK535148",
+        "VariantType": "Repeat"
+    },
+    {
         "Disease": "FAME1",
         "DisplayRU": "TTTCA",
         "HGNCId": 31750,
         "InheritanceMode": "AD",
         "LocusId": "SAMD12",
         "LocusStructure": "(TAAAA)*(TGAAA)*(TAAAA)*",
         "NormalMax": 1,
@@ -785,29 +809,14 @@
         "VariantType": [
             "Repeat",
             "Repeat",
             "Repeat"
         ]
     },
     {
-        "Disease": "CCD",
-        "DisplayRU": "GCN",
-        "HGNCId": 10472,
-        "InheritanceMode": "AD",
-        "LocusId": "RUNX2",
-        "LocusStructure": "(GCN)*",
-        "NormalMax": 17,
-        "PathologicMin": 20,
-        "ReferenceRegion": "6:45390488-45390538",
-        "Source": "GeneReviews",
-        "SourceDisplay": "GeneReviews Internet 2019-11-07",
-        "SourceId": "NBK535148",
-        "VariantType": "Repeat"
-    },
-    {
         "Disease": "MRGH",
         "DisplayRU": "GCN",
         "HGNCId": 11199,
         "InheritanceMode": "XR",
         "LocusId": "SOX3",
         "LocusStructure": "(NGC)*",
         "NormalMax": 15,
@@ -823,15 +832,15 @@
         "DisplayRU": "CAN",
         "HGNCId": 11588,
         "InheritanceMode": "AD",
         "LocusId": "TBP",
         "LocusStructure": "(GCA)*",
         "NormalMax": 40,
         "PathologicMin": 49,
-        "ReferenceRegion": "6:170870994-170871109",
+        "ReferenceRegion": "6:170870995-170871103",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-09-12",
         "SourceId": "NBK1438",
         "SweGenMean": 36.24,
         "SweGenStd": 2.293,
         "VariantType": "Repeat"
     },
@@ -864,14 +873,29 @@
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "SweGenMean": 16.87,
         "SweGenStd": 8.388,
         "VariantType": "Repeat"
     },
     {
+        "Disease": "SCA",
+        "DisplayRU": "CAG",
+        "HGNCId": 23194,
+        "InheritanceMode": "AD",
+        "LocusId": "THAP11",
+        "LocusStructure": "(CAG)*",
+        "NormalMax": 38,
+        "PathologicMin": 45,
+        "ReferenceRegion": "16:67876766-67876853",
+        "Source": "PubMed",
+        "SourceDisplay": "Tan et al (2023) Movement Disorders 38(7):1282-1293",
+        "SourceId": "37148549",
+        "VariantType": "Repeat"
+    },
+    {
         "Disease": "FAME6",
         "DisplayRU": "TTTCA",
         "HGNCId": 11969,
         "InheritanceMode": "AD",
         "LocusId": "TNRC6A",
         "LocusStructure": "(TTTTA)*(TTTCA)*(TTTTA)*",
         "NormalMax": 1,
@@ -898,122 +922,81 @@
     },
     {
         "Disease": "DBQD2",
         "DisplayRU": "GGC",
         "HGNCId": 15516,
         "InheritanceMode": "AR",
         "LocusId": "XYLT1",
-        "LocusStructure": "(GGC)*",
-        "NormalMax": 20,
+        "LocusStructure": "(GCC)*",
+        "NormalMax": 60,
         "PathologicMin": 70,
-        "ReferenceRegion": "16:17564765-17564778",
+        "ReferenceRegion": "16:17564764-17564779",
         "Source": "PubMed",
         "SourceDisplay": "LaCroix et al (2018) AJHG 104(1) 35-44",
         "SourceId": "30554721",
         "VariantType": "Repeat"
     },
     {
         "Disease": "HPE5",
         "DisplayRU": "GCN",
         "HGNCId": 12873,
         "InheritanceMode": "AD",
         "LocusId": "ZIC2",
         "LocusStructure": "(GCN)*",
         "NormalMax": 15,
         "PathologicMin": 25,
-        "ReferenceRegion": "13:100637703-100637747",
+        "ReferenceRegion": "13:100637702-100637747",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "VariantType": "Repeat"
     },
     {
         "Disease": "VACTERLX",
         "DisplayRU": "GCN",
         "HGNCId": 12874,
         "InheritanceMode": "XR",
         "LocusId": "ZIC3",
         "LocusStructure": "(GCN)*",
         "NormalMax": 10,
         "PathologicMin": 12,
-        "ReferenceRegion": "X:136648986-136649015",
+        "ReferenceRegion": "X:136648985-136649015",
         "Source": "GeneReviews",
         "SourceDisplay": "GeneReviews Internet 2019-11-07",
         "SourceId": "NBK535148",
         "VariantType": "Repeat"
     },
     {
-        "Disease": "ALS - susceptibility to",
-        "DisplayRU": "GCG",
-        "HGNCId": 17043,
-        "InheritanceMode": "AD",
-        "LocusId": "NIPA1",
-        "LocusStructure": "(CGC)*",
-        "NormalMax": 8,
-        "PathologicMin": 10000,
-        "ReferenceRegion": "15:23086366-23086390",
-        "Source": "PubMed",
-        "SourceDisplay": "Tazelaar et al (2019) Neurobiol Aging 74 234.e9-234.e15",
-        "SourceId": "30342764",
-        "VariantType": "Repeat"
-    },
-    {
         "Disease": "GDPAG",
         "DisplayRU": "GCA",
         "HGNCId": 4331,
         "InheritanceMode": "AR",
         "LocusId": "GLS",
         "LocusStructure": "(GCA)*",
-        "NormalMax": 20,
+        "NormalMax": 26,
         "PathologicMin": 90,
         "ReferenceRegion": "2:191745598-191745646",
         "Source": "PubMed",
         "SourceDisplay": "van Kuilenburg et al (2019) NEJM 380 1433-1441",
         "SourceId": "30970188",
         "SweGenMean": 12.66,
         "SweGenStd": 4.0,
         "VariantType": "Repeat"
     },
     {
-        "Disease": "CANVAS",
-        "DisplayRU": "AARRG",
-        "HGNCId": 9969,
-        "InheritanceMode": "AR",
-        "LocusId": "RFC1",
-        "LocusStructure": "(AARRG)*",
-        "NormalMax": 11,
-        "PathologicMin": 12,
-        "ReferenceRegion": "4:39350044-39350099",
-        "Source": "PubMed",
-        "SourceDisplay": "Cortese et al 2019 Nat Gen",
-        "SourceId": "30926972",
-        "SweGenMean": 26.77,
-        "SweGenStd": 18.68,
+        "Disease": "SCA4",
+        "DisplayRU": "GGC",
+        "HGNCId": 777,
+        "InheritanceMode": "AD",
+        "LocusId": "ZFHX3",
+        "LocusStructure": "(GCC)*",
+        "NormalMax": 28,
+        "PathologicMin": 42,
+        "ReferenceRegion": "16:72821593-72821656",
+        "Source": "DOI",
+        "SourceDisplay": "Paucar, Nilsson, Engvall et al medRxiv 2023-10-03",
+        "SourceId": "10.1101/2023.10.03.23296230",
+        "SweGenMean": 21,
+        "SweGenStd": 0.8,
         "VariantType": "Repeat"
-    },
-    {
-        "Disease": "-",
-        "DisplayRU": "CTG",
-        "HGNCId": 9179,
-        "InheritanceMode": "-",
-        "LocusId": "POLG",
-        "LocusStructure": "(CTG)*TTG(CTG)*",
-        "NormalMax": 15,
-        "PathologicMin": 10000,
-        "PathologicRegion": "15:89876830-89876859",
-        "ReferenceRegion": [
-            "15:89876821-89876826",
-            "15:89876830-89876859"
-        ],
-        "Source": "Expert",
-        "SourceDisplay": "Research only - contact CMMS KUH regarding findings",
-        "SourceId": "CMMS",
-        "VariantId": [
-            "POLG_I",
-            "POLG_II"
-        ],
-        "VariantType": [
-            "Repeat",
-            "Repeat"
-        ]
     }
 ]
```

### Comparing `stranger-0.8.1/stranger/vcf_utils.py` & `stranger-0.9.0/stranger/vcf_utils.py`

 * *Files identical despite different names*

### Comparing `stranger-0.8.1/stranger/cli.py` & `stranger-0.9.0/stranger/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import click
 import gzip
 
 from pprint import pprint as pp
 from codecs import (open, getreader)
 
 from stranger.resources import repeats_json_path
-from stranger.utils import (parse_repeat_file, get_repeat_info, get_info_dict, get_variant_line)
+from stranger.utils import (decompose_var, get_format_dicts, get_individual_index, get_info_dict, get_repeat_info, get_variant_line, parse_repeat_file, update_decomposed_variant_format_fields)
 from stranger.vcf_utils import print_headers
-from stranger.constants import ANNOTATE_REPEAT_KEYS
+from stranger.constants import ANNOTATE_REPEAT_KEYS, ANNOTATE_REPEAT_KEYS_TRGT
 from stranger.__version__ import __version__
 
 LOG = logging.getLogger(__name__)
 LOG_LEVELS = ['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
@@ -26,20 +26,21 @@
 @click.option('-f', '--repeats-file',
     type = click.Path(exists=True),
     help="Path to a file with repeat definitions. See README for explanation",
     default=repeats_json_path,
     show_default=True,
 )
 @click.option('-i','--family_id', default='1')
+@click.option('-t','--trgt', is_flag=True, help='File was produced with TRGT')
 @click.option('--version', is_flag=True, callback=print_version,
               expose_value=False, is_eager=True)
 @click.option('--loglevel', default='INFO', type=click.Choice(LOG_LEVELS),
               help="Set the level of log output.", show_default=True)
 @click.pass_context
-def cli(context, vcf, family_id, repeats_file, loglevel):
+def cli(context, vcf, family_id, repeats_file, loglevel, trgt):
     """Annotate str variants with str status"""
     coloredlogs.install(level=loglevel)
     LOG.info("Running stranger version %s", __version__)
 
     repeat_information = None
     repeats_file_type = 'tsv'
     if repeats_file.endswith('.json'):
@@ -49,15 +50,15 @@
     with open(repeats_file, 'r') as file_handle:
         repeat_information = parse_repeat_file(file_handle, repeats_file_type)
 
     if not repeat_information:
         LOG.warning("Could not find any repeat info")
         context.abort()
 
-    header_definitions = [
+    header_info_definitions = [
         {
             'id': 'STR_STATUS', 'num': 'A', 'type': 'String',
             'desc': 'Repeat expansion status. Alternatives in [normal, pre_mutation, full_mutation]'
         },
         {
             'id': 'STR_NORMAL_MAX', 'num': '1', 'type': 'Integer',
             'desc': 'Max number of repeats allowed to call as normal'
@@ -105,47 +106,66 @@
         {
             'id': 'Disease', 'num': '1', 'type': 'String',
             'desc': 'Associated disorder'
         },
     ]
 
     stranger_headers = []
-    for hdef in header_definitions:
+    for hdef in header_info_definitions:
         header = '##INFO=<ID={0},Number={1},Type={2},Description="{3}">'.format(
             hdef.get('id'), hdef.get('num'), hdef.get('type'), hdef.get('desc'))
         stranger_headers.append(header)
 
-
     if vcf.endswith('.gz'):
         LOG.info("Vcf is zipped")
         vcf_handle = getreader('utf-8')(gzip.open(vcf), errors='replace')
     else:
         vcf_handle = open(vcf, mode='r', encoding='utf-8', errors='replace')
 
-    LOG.info("Parsing variants from %s", vcf)
     for line in vcf_handle:
         line = line.rstrip()
         if line.startswith('#'):
             if line.startswith('##'):
                 click.echo(line)
                 continue
             # Print the new header lines describing stranger annotation
             for header in stranger_headers:
                 click.echo(header)
             # Print the vcf header line
             header_info = line[1:].split('\t')
             click.echo(line)
             continue
         variant_info = dict(zip(header_info, line.split('\t')))
-        variant_info['alts'] = variant_info['ALT'].split(',')
         variant_info['info_dict'] = get_info_dict(variant_info['INFO'])
-        repeat_data = get_repeat_info(variant_info, repeat_information)
-        if repeat_data:
-            variant_info['info_dict']['STR_STATUS'] = repeat_data['repeat_strings']
-            variant_info['info_dict']['STR_NORMAL_MAX'] = str(repeat_data['lower'])
-            variant_info['info_dict']['STR_PATHOLOGIC_MIN'] = str(repeat_data['upper'])
-            variant_info['info_dict']['RankScore'] = ':'.join([str(family_id), str(repeat_data['rank_score'])])
-            for annotate_repeat_key in ANNOTATE_REPEAT_KEYS:
-                if repeat_data.get(annotate_repeat_key):
-                    variant_info['info_dict'][annotate_repeat_key] = str(repeat_data[annotate_repeat_key])
+        variant_info['alts'] = variant_info['ALT'].split(',')
+
+        variant_infos = [variant_info]
+
+        if trgt:
+            individual_index = get_individual_index(header_info)
+            variant_info['format_dicts'] = get_format_dicts(variant_info['FORMAT'], [variant_info[individual] for individual in header_info[individual_index:]])
+
+            LOG.debug("format %s for inds %s gives dicts %s",variant_info['FORMAT'], [individual for individual in header_info[individual_index:]], variant_info['format_dicts'])
+            if len(variant_info['alts']) > 1:
+                variant_infos = decompose_var(variant_info)
+
+        for variant_info in variant_infos:
+            LOG.debug("decomposed variant info %s", variant_info)
+            update_decomposed_variant_format_fields(variant_info, header_info, individual_index)
+
+            repeat_data = get_repeat_info(variant_info, repeat_information)
+
+            if repeat_data:
+                variant_info['info_dict']['STR_STATUS'] = repeat_data['repeat_strings']
+                variant_info['info_dict']['STR_NORMAL_MAX'] = str(repeat_data['lower'])
+                variant_info['info_dict']['STR_PATHOLOGIC_MIN'] = str(repeat_data['upper'])
+                variant_info['info_dict']['RankScore'] = ':'.join([str(family_id), str(repeat_data['rank_score'])])
+
+                annotate_repeat_keys = ANNOTATE_REPEAT_KEYS
+                if trgt:
+                    annotate_repeat_keys = ANNOTATE_REPEAT_KEYS_TRGT
+                for annotate_repeat_key in annotate_repeat_keys:
+                    if repeat_data.get(annotate_repeat_key):
+                        variant_info['info_dict'][annotate_repeat_key] = str(repeat_data[annotate_repeat_key])
+
+                click.echo(get_variant_line(variant_info, header_info))
 
-        click.echo(get_variant_line(variant_info, header_info))
```

