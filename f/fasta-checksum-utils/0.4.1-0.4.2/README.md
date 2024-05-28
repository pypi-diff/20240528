# Comparing `tmp/fasta_checksum_utils-0.4.1.tar.gz` & `tmp/fasta_checksum_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasta_checksum_utils-0.4.1.tar", max compression
+gzip compressed data, was "fasta_checksum_utils-0.4.2.tar", max compression
```

## Comparing `fasta_checksum_utils-0.4.1.tar` & `fasta_checksum_utils-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7653 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/LICENSE
--rw-r--r--   0        0        0     3616 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/README.md
--rw-r--r--   0        0        0      336 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/__init__.py
--rw-r--r--   0        0        0      903 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/_contig.py
--rw-r--r--   0        0        0      305 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/_file.py
--rw-r--r--   0        0        0     3103 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/algorithms.py
--rw-r--r--   0        0        0     1502 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/entry.py
--rw-r--r--   0        0        0     7357 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/fasta_checksum_utils/fasta.py
--rw-r--r--   0        0        0      720 2024-02-13 18:28:15.326175 fasta_checksum_utils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 fasta_checksum_utils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     7653 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3613 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/README.md
+-rw-r--r--   0        0        0      336 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/_contig.py
+-rw-r--r--   0        0        0      305 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/_file.py
+-rw-r--r--   0        0        0     3103 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/algorithms.py
+-rw-r--r--   0        0        0     1502 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/entry.py
+-rw-r--r--   0        0        0     7357 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/fasta_checksum_utils/fasta.py
+-rw-r--r--   0        0        0      720 2024-05-28 15:05:53.551553 fasta_checksum_utils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 fasta_checksum_utils-0.4.2/PKG-INFO
```

### Comparing `fasta_checksum_utils-0.4.1/LICENSE` & `fasta_checksum_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fasta_checksum_utils-0.4.1/README.md` & `fasta_checksum_utils-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     all_algorithms = (fc.algorithms.AlgorithmMD5, fc.algorithms.AlgorithmGA4GH)
     
     # calculate multiple checksums for a whole file
     all_checksums: tuple[str, ...] = await fc.checksum_file(file=covid_genome, algorithms=all_algorithms)
     print(all_checksums)
     # prints tuple: ("863ee5dba1da0ca3f87783782284d489", "SQ.mMg8qNej7pU84juQQWobw9JyUy09oYdd")
     
-    # calculate an MD5 and TRUNC512 checksum for a specific contig in a PySAM FASTA file:
+    # calculate an MD5 and GA4GH checksum for a specific contig in a PySAM FASTA file:
     fh = pysam.FastaFile(str(covid_genome))
     try:
         contig_checksums: tuple[str, ...] = await fc.checksum_contig(
             fh=fh, 
             contig_name="NC_045512.2", 
             algorithms=all_algorithms,
         )
```

### Comparing `fasta_checksum_utils-0.4.1/fasta_checksum_utils/_contig.py` & `fasta_checksum_utils-0.4.2/fasta_checksum_utils/_contig.py`

 * *Files identical despite different names*

### Comparing `fasta_checksum_utils-0.4.1/fasta_checksum_utils/algorithms.py` & `fasta_checksum_utils-0.4.2/fasta_checksum_utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `fasta_checksum_utils-0.4.1/fasta_checksum_utils/entry.py` & `fasta_checksum_utils-0.4.2/fasta_checksum_utils/entry.py`

 * *Files identical despite different names*

### Comparing `fasta_checksum_utils-0.4.1/fasta_checksum_utils/fasta.py` & `fasta_checksum_utils-0.4.2/fasta_checksum_utils/fasta.py`

 * *Files identical despite different names*

### Comparing `fasta_checksum_utils-0.4.1/pyproject.toml` & `fasta_checksum_utils-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasta-checksum-utils"
-version = "0.4.1"
+version = "0.4.2"
 description = "Library and command-line utility for checksumming FASTA files and individual contigs."
 authors = ["David Lougheed <david.lougheed@gmail.com>"]
 license = "LGPL-3.0"
 readme = "README.md"
 packages = [{include = "fasta_checksum_utils"}]
 
 [tool.poetry.scripts]
```

### Comparing `fasta_checksum_utils-0.4.1/PKG-INFO` & `fasta_checksum_utils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasta-checksum-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Library and command-line utility for checksumming FASTA files and individual contigs.
 License: LGPL-3.0
 Author: David Lougheed
 Author-email: david.lougheed@gmail.com
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -107,15 +107,15 @@
     all_algorithms = (fc.algorithms.AlgorithmMD5, fc.algorithms.AlgorithmGA4GH)
     
     # calculate multiple checksums for a whole file
     all_checksums: tuple[str, ...] = await fc.checksum_file(file=covid_genome, algorithms=all_algorithms)
     print(all_checksums)
     # prints tuple: ("863ee5dba1da0ca3f87783782284d489", "SQ.mMg8qNej7pU84juQQWobw9JyUy09oYdd")
     
-    # calculate an MD5 and TRUNC512 checksum for a specific contig in a PySAM FASTA file:
+    # calculate an MD5 and GA4GH checksum for a specific contig in a PySAM FASTA file:
     fh = pysam.FastaFile(str(covid_genome))
     try:
         contig_checksums: tuple[str, ...] = await fc.checksum_contig(
             fh=fh, 
             contig_name="NC_045512.2", 
             algorithms=all_algorithms,
         )
```

