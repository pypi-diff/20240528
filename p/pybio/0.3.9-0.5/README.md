# Comparing `tmp/pybio-0.3.9.tar.gz` & `tmp/pybio-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybio-0.3.9.tar", last modified: Tue Jun 13 13:30:33 2023, max compression
+gzip compressed data, was "pybio-0.5.tar", last modified: Tue May 28 15:25:16 2024, max compression
```

## Comparing `pybio-0.3.9.tar` & `pybio-0.5.tar`

### file list

```diff
@@ -1,55 +1,37 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.557460 pybio-0.3.9/
--rw-rw-r--   0 rotg     (2023757) games       (20)     9263 2023-06-13 13:30:33.556998 pybio-0.3.9/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     9032 2023-06-05 13:06:07.000000 pybio-0.3.9/README.md
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.391168 pybio-0.3.9/pybio/
--rw-rw-r--   0 rotg     (2023757) games       (20)     7814 2023-05-03 14:56:57.000000 pybio-0.3.9/pybio/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.395238 pybio-0.3.9/pybio/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1482 2023-06-13 13:08:38.000000 pybio-0.3.9/pybio/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.396576 pybio-0.3.9/pybio/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    27779 2023-05-11 11:48:32.000000 pybio-0.3.9/pybio/core/genomes.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.449869 pybio-0.3.9/pybio/data/
--rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bam.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bedgraph.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Bedgraph2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Fasta.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Fastq.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gene.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/GeneFeature.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gff3.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Gtf.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Sequence.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Sissrs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/TabReader.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/Wig.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/data/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.450514 pybio-0.3.9/pybio/expression/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/expression/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.482763 pybio-0.3.9/pybio/map/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/STAR.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/bowtie.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/nano.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/map/sege.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.503612 pybio-0.3.9/pybio/maths/
--rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/pstat.py
--rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/maths/stats.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.512562 pybio-0.3.9/pybio/path/
--rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/path/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     9888 2023-06-13 12:59:21.000000 pybio-0.3.9/pybio/pybio
--rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.9/pybio/pybio.config.example
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.513209 pybio-0.3.9/pybio/sequence/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/sequence/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.535570 pybio-0.3.9/pybio/utils/
--rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.9/pybio/utils/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-13 13:30:19.000000 pybio-0.3.9/pybio/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-13 13:30:33.394517 pybio-0.3.9/pybio.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     9263 2023-06-13 13:30:33.392073 pybio-0.3.9/pybio.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-06-13 13:30:33.392434 pybio-0.3.9/pybio.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-13 13:30:33.392862 pybio-0.3.9/pybio.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.9/pybio.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-06-13 13:30:33.394022 pybio-0.3.9/pybio.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-13 13:30:33.394661 pybio-0.3.9/pybio.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-13 13:30:33.557567 pybio-0.3.9/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.9/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2452 2024-05-28 15:25:16.277919 pybio-0.5/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2117 2024-05-28 15:24:16.000000 pybio-0.5/README.md
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     9003 2024-04-25 07:11:04.000000 pybio-0.5/pybio/__init__.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/config/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1519 2024-04-25 07:11:04.000000 pybio-0.5/pybio/config/__init__.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/core/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       98 2024-04-25 07:11:04.000000 pybio-0.5/pybio/core/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    30052 2024-05-28 15:00:11.000000 pybio-0.5/pybio/core/genomes.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/data/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    16345 2024-04-25 07:11:04.000000 pybio-0.5/pybio/data/Bedgraph.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1912 2024-04-25 07:11:04.000000 pybio-0.5/pybio/data/Fasta.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1244 2024-04-25 07:11:04.000000 pybio-0.5/pybio/data/Fastq.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1849 2024-04-25 07:11:04.000000 pybio-0.5/pybio/data/__init__.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/maths/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      974 2024-04-25 07:11:04.000000 pybio-0.5/pybio/maths/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    37335 2024-04-25 07:11:04.000000 pybio-0.5/pybio/maths/pstat.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)   151400 2024-04-25 07:11:04.000000 pybio-0.5/pybio/maths/stats.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/path/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      347 2024-04-25 07:11:04.000000 pybio-0.5/pybio/path/__init__.py
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)    11346 2024-04-25 07:11:04.000000 pybio-0.5/pybio/pybio
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      134 2024-05-28 15:19:59.000000 pybio-0.5/pybio/pybio.config.example
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/sequence/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     5566 2024-04-25 07:11:04.000000 pybio-0.5/pybio/sequence/__init__.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio/utils/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    10199 2024-04-25 07:11:04.000000 pybio-0.5/pybio/utils/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        4 2024-05-28 15:05:23.000000 pybio-0.5/pybio/version
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-28 15:25:16.277919 pybio-0.5/pybio.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2452 2024-05-28 15:25:16.000000 pybio-0.5/pybio.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      557 2024-05-28 15:25:16.000000 pybio-0.5/pybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-05-28 15:25:16.000000 pybio-0.5/pybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-05-28 15:20:35.000000 pybio-0.5/pybio.egg-info/not-zip-safe
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       32 2024-05-28 15:25:16.000000 pybio-0.5/pybio.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        6 2024-05-28 15:25:16.000000 pybio-0.5/pybio.egg-info/top_level.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-05-28 15:25:16.277919 pybio-0.5/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      949 2024-04-25 07:11:04.000000 pybio-0.5/setup.py
```

### Comparing `pybio-0.3.9/pybio/__init__.py` & `pybio-0.5/pybio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 Github: https://github.com/grexor/pybio
 """
 
 import os
 import json
 import pybio.path
 import pybio.data
-import pybio.map
 import pybio.utils
-import pybio.expression
 import pybio.maths
 import pybio.config
 import pybio.sequence
 import pybio.core
 
 pybio_path = os.path.abspath(__file__)
 pybio_folder = os.path.dirname(pybio_path)
@@ -25,15 +23,15 @@
 
 # initialize path module
 pybio.config.init()
 pybio.path.init()
 pybio.core.genomes.init()
 
 def genome_download(species, genome_version, args):
-    print(f"[pybio genome_download] species {species} and version {genome_version}")
+    print(f"pybio | genome | download species {species} and version {genome_version}")
     genomes_ready_fname = os.path.join(pybio.config.genomes_folder, "genomes_ready.json")
     if os.path.exists(genomes_ready_fname):
         genomes_ready = json.load(open(genomes_ready_fname, "rt"))
     else:
         genomes_ready = {}
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("assembly", False)
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("annotation", False)
@@ -41,15 +39,15 @@
     if not genomes_ready.get(species, {}).get(genome_version, {}).get("assembly", False) or not os.path.exists(assembly_folder):
         return_code = pybio.core.genomes.download_assembly(species, genome_version)
         if return_code==0:
             genomes_ready[species][genome_version]["assembly"] = True
         else:
             genomes_ready[species][genome_version]["assembly"] = False
     else:
-        print(f"[pybio genome] FASTA ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}")
+        print(f"pybio | genome | FASTA ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}")
 
     annotation_folder = os.path.join(pybio.config.genomes_folder, f"{species}.annotation.{genome_version}")
     if not genomes_ready.get(species, {}).get(genome_version, {}).get("annotation", False) or not os.path.exists(annotation_folder):
         return_code = pybio.core.genomes.download_annotation(species, genome_version)
         if return_code==0:
             return_code = pybio.core.genomes.prepare(species, genome_version)
         if return_code==0:
@@ -58,37 +56,37 @@
             genomes_ready[species][genome_version]["annotation"] = False
     else:
         print(f"[pybio genome] genome annotation at {pybio.config.genomes_folder}/{species}.annotation.{genome_version}")
 
     json.dump(genomes_ready, open(genomes_ready_fname, "wt"))
 
 def genome_import(species, genome_version, args):
-    print(f"[pybio genome] species {species} and version {genome_version}")
+    print(f"pybio | genome | species {species} and version {genome_version}")
     genomes_ready_fname = os.path.join(pybio.config.genomes_folder, "genomes_ready.json")
     if os.path.exists(genomes_ready_fname):
         genomes_ready = json.load(open(genomes_ready_fname, "rt"))
     else:
         genomes_ready = {}
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("assembly", False)
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("annotation", False)
     assembly_folder = os.path.join(pybio.config.genomes_folder, f"{species}.assembly.{genome_version}")
     if not genomes_ready.get(species, {}).get(genome_version, {}).get("assembly", False) or not os.path.exists(assembly_folder):
         fasta_fname = args.fasta
-        print(f"[pybio genome] importing {fasta_fname} to {assembly_folder}/{species}.fasta")
+        print(f"pybio | genome | importing {fasta_fname} to {assembly_folder}/{species}.fasta")
         if fasta_fname.endswith(".gz"):
             os.system(f"mkdir {assembly_folder}; cp {fasta_fname} {assembly_folder}/{species}.fasta.gz; gunzip -f {assembly_folder}/{species}.fasta.gz")
         else:
             os.system(f"mkdir {assembly_folder}; cp {fasta_fname} {assembly_folder}/{species}.fasta")
         return_code = os.system("python3 -c \"import pybio; pybio.data.Fasta('{assembly_folder}/{species}.fasta').split()\"".format(assembly_folder=assembly_folder, species=species))
         if return_code==0:
             genomes_ready[species][genome_version]["assembly"] = True
         else:
             genomes_ready[species][genome_version]["assembly"] = False
     else:
-        print(f"[pybio genome] FASTA ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}")
+        print(f"pybio | genome | FASTA ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}")
     json.dump(genomes_ready, open(genomes_ready_fname, "wt"))
 
     annotation_folder = os.path.join(pybio.config.genomes_folder, f"{species}.annotation.{genome_version}")
     if not genomes_ready.get(species, {}).get(genome_version, {}).get("annotation", False) or not os.path.exists(annotation_folder):
         gtf_fname = args.gtf
         print(f"[pybio genome] importing {gtf_fname} to {annotation_folder}/{species}.gtf.gz")
         if gtf_fname.endswith(".gz"):
@@ -99,15 +97,15 @@
         if return_code==0:
             genomes_ready[species][genome_version]["annotation"] = True
         else:
             genomes_ready[species][genome_version]["annotation"] = False
             genomes_ready[species][genome_version]["STAR"] = False
             genomes_ready[species][genome_version]["salmon"] = False
     else:
-        print(f"[pybio genome] genome annotation at {pybio.config.genomes_folder}/{species}.annotation.{genome_version}")
+        print(f"pybio | genome | annotation at {pybio.config.genomes_folder}/{species}.annotation.{genome_version}")
     json.dump(genomes_ready, open(genomes_ready_fname, "wt"))
 
 def genome_prepare(species, genome_version, args):
     genomes_ready_fname = os.path.join(pybio.config.genomes_folder, "genomes_ready.json")
     if os.path.exists(genomes_ready_fname):
         genomes_ready = json.load(open(genomes_ready_fname, "rt"))
     else:
@@ -119,21 +117,51 @@
         if not genomes_ready.get(species, {}).get(genome_version, {}).get("STAR", False) or not os.path.exists(star_folder):
             return_code = pybio.core.genomes.star_index(species, genome_version, threads=args.threads)
             if return_code==0:
                 genomes_ready[species][genome_version]["STAR"] = True
             else:
                 genomes_ready[species][genome_version]["STAR"] = False
         else:
-            print(f"[pybio genome] STAR index ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}.star")
+            print(f"pybio | genome | STAR index ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}.star")
 
     if pybio.utils.is_tool("salmon") and not args.nosalmon:
         salmon_folder = os.path.join(pybio.config.genomes_folder, f"{species}.transcripts.{genome_version}.salmon")
         if not genomes_ready.get(species, {}).get(genome_version, {}).get("salmon", False) or not os.path.exists(salmon_folder):
             return_code = pybio.core.genomes.salmon_index(species, genome_version)
             if return_code==0:
                 genomes_ready[species][genome_version]["salmon"] = True
             else:
                 genomes_ready[species][genome_version]["salmon"] = False
         else:
-            print(f"[pybio genome] salmon index ready at {pybio.config.genomes_folder}/{species}.transcripts.{genome_version}.salmon")
+            print(f"pybio | genome | salmon index ready at {pybio.config.genomes_folder}/{species}.transcripts.{genome_version}.salmon")
 
     json.dump(genomes_ready, open(genomes_ready_fname, "wt"))
+
+def gff4jbrowse(fname_input, fname_output):
+    print(f"pybio | gff3 for JBrowse2 | {fname_input} {fname_output}")
+    fin = gzip.open(fname_input) if fname_input.endswith(".gz") else open(fname_input)
+    fout = gzip.open(fname_output, "wt") if fname_input.endswith(".gz") else open(fname_output, "wt")
+    r = fin.readline()
+    while r:
+        r = r.replace("\r", "").replace("\n", "").split("\t")
+        if len(r)>2:
+            if r[2]!="gene":
+                atts = r[-1]
+                atts = atts.split(";")
+                new_atts = []
+                gene_id = None
+                for att in atts:
+                    if att.find("Parent=gene:")!=-1:
+                        gene_id = att.split("Parent=gene:")[1]
+                    elif att.startswith("Name="):
+                        if gene_id!=None:
+                            new_atts.append(f"{att},{gene_id}")
+                        else:
+                            new_atts.append(att)
+                    else:
+                        new_atts.append(att)
+                new_atts = ";".join(new_atts)
+                r[-1] = new_atts
+                fout.write("\t".join(r)+"\n")
+        r = fin.readline()
+    fin.close()
+    fout.close()
```

### Comparing `pybio-0.3.9/pybio/config/__init__.py` & `pybio-0.5/pybio/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     config_lines = open(config_file).readlines()
     new_config = []
     for cline in config_lines:
         if cline.startswith("#"):
             continue
         k, v = cline.split("=")
         if k=="genomes_folder" and genomes_folder!=None:
-            v = genomes_folder
+            v = os.path.abspath(os.path.expanduser(genomes_folder))
         v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
         v = os.path.expanduser(v)
         if k.find("folder")!=-1:
             if not v.startswith("/"):
                 v = "\"" + os.path.join(pybio_folder, eval(v)) + "\""
         setattr(config_module, k, v)
         new_config.append((k, str(v)))
```

### Comparing `pybio-0.3.9/pybio/core/genomes.py` & `pybio-0.5/pybio/core/genomes.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import itertools
 import copy
 import gzip
 import psutil
 import pickle
 import math
 import requests
+import sys
+requests.packages.urllib3.disable_warnings()
 
 process = psutil.Process(os.getpid())
 
 providers_ftp = {}
 providers_ftp["ensembl"] = "https://ftp.ensembl.org/pub"
 providers_ftp["ensemblgenomes"] = "https://ftp.ensemblgenomes.ebi.ac.uk/pub"
 
@@ -51,14 +53,15 @@
     self.transcript_id = transcript_id
     self.gene = genes_db[gene_id]
     self.start = int(start)-1
     self.stop = int(stop)-1
     self.utr3 = None
     self.utr5 = None
     self.exons = set()
+    self.exons_list = [] # list of exons, (start, stop), sorted in 5->3 reading direction, start<=stop
     self.gene.transcripts.add(self)
 
 class Exon:
 
   def __init__(self, exon_id, transcript_id, start, stop):
     self.exon_id = exon_id
     self.transcript = transcripts_db.get(transcript_id, None)
@@ -109,29 +112,36 @@
     if len(gtf_files)==0:
         gtf_files = glob.glob(os.path.join(annotation_folder, "*.gtf"))
     gtf_fname = gtf_files[0]
     if gtf_fname.endswith(".gz"):
         f = gzip.open(gtf_fname, "rt")
     else:
         f = open(gtf_fname, "rt")
+    print(f"[pybio] reading {gtf_fname}")
     clines = 0
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         if r[0].startswith("#"):
             r = f.readline()
             continue
         data = dict(zip(gtf_fields, r))
         atts = {}
         temp = data["atts"].split("; ")
         for el in temp:
             el1, el2 = el.split(" ")[0], " ".join(el.split(" ")[1:])
             atts[el1] = el2[1:-1]
         if data["feature"] == "gene":
-            gene = Gene(atts["gene_id"], atts.get("gene_name", ""), data["chr"], data["strand"], data["start"], data["stop"], atts)
+            gene_id = atts["gene_id"]
+            gene_name = atts.get("gene_name", "")
+            if gene_name=="":
+                gene_name = atts.get("gene", "")
+                if gene_name=="":
+                    gene_name = gene_id
+            gene = Gene(gene_id, gene_name, data["chr"], data["strand"], data["start"], data["stop"], atts)
             genes_db[atts["gene_id"]] = gene
             chr_list.add(data["chr"])
             gene_bins = set()
             gene_start = int(data["start"])-1
             gene_stop = int(data["stop"])-1
             bin_min = math.floor(gene_start/gene_bin_size)
             bin_max = math.floor(gene_stop/gene_bin_size)
@@ -141,32 +151,53 @@
                 gene_bins_db.setdefault(data["chr"], {}).setdefault(gene_bin, set()).add(atts["gene_id"])
         if data["feature"] == "transcript":
             transcript = Transcript(atts["transcript_id"], atts["gene_id"], data["start"], data["stop"])
             transcripts_db[atts["transcript_id"]] = transcript
         if data["feature"] == "exon":
             if atts.get("exon_id", None)==None:
                 atts["exon_id"] = f"exon_{data['start']}_{data['stop']}"
+            # note: some annotations don't have "transcript" records, just "transcript_id" in their "exon" records
+            if transcripts_db.get(atts["transcript_id"], None)==None:
+                transcript = Transcript(atts["transcript_id"], atts["gene_id"], data["start"], data["stop"])
+                transcripts_db[atts["transcript_id"]] = transcript
+            # we also need to update the transcript start/stop if its already there
+            else:
+                transcript = transcripts_db[atts["transcript_id"]]
+                transcript.start = min(int(data["start"])-1, transcript.start)
+                transcript.stop = max(int(data["stop"])-1, transcript.stop)
+                transcripts_db[atts["transcript_id"]] = transcript
             exon = Exon(atts["exon_id"], atts["transcript_id"], data["start"], data["stop"])
             exons_db[atts["exon_id"]] = exon
         if data["feature"] == "three_prime_utr":
             utr3 = Utr3(atts["transcript_id"], data["start"], data["stop"])
         if data["feature"] == "five_prime_utr":
             utr5 = Utr5(atts["transcript_id"], data["start"], data["stop"])
         r = f.readline()
         clines += 1
         if clines%100000==0:
-            print("%.2f M lines parsed, RAM GB used: %.3f" % (clines/1000000.0, process.memory_info().rss/1000000000))
+            print("pybio | {species} {genome_version} | %.2f M lines parsed, RAM GB used: %.3f" % (clines/1000000.0, process.memory_info().rss/1000000000))
     f.close()
     pickle.dump(gene_bins_db, open(os.path.join(annotation_folder, "gene_bins_db.pickle"), "wb"))
 
     print("#exons = ", len(exons_db.keys()))
     print("#transcripts = ", len(transcripts_db.keys()))
     print("#genes = ", len(genes_db.keys()))
     print("chromosome list = ", "; ".join(list(chr_list)))
 
+    # sort exons
+    print("pybio: sorting exons of transcripts to be given in 5'->3' order")
+    for gene_id, gene in genes_db.items():
+        for transcript in gene.transcripts:
+            exons_list = [(exon.start, exon.stop) for exon in transcript.exons]
+            if gene.strand=="+":
+                exons_list.sort(key = lambda x: x[0])
+            else:
+                exons_list.sort(key = lambda x: x[1], reverse=True)
+            transcript.exons_list = exons_list
+
     pickle.dump(exons_db, open(os.path.join(annotation_folder, "exons_db.pickle"), "wb"))
     pickle.dump(transcripts_db, open(os.path.join(annotation_folder, "transcripts_db.pickle"), "wb"))
     pickle.dump(genes_db, open(os.path.join(annotation_folder, "genes_db.pickle"), "wb"))
     return 0
 
 def seq_direct(species, chr, strand, start, stop, flank="N", genome_version=None):
     """
@@ -234,15 +265,15 @@
     motifs = []
     z = itertools.product("ATCG", repeat=motif_size)
     for el in z:
         motifs.append("".join(el))
     return motifs
 
 def url_exists(path):
-    r = requests.head(path)
+    r = requests.head(path, verify=False)
     return r.status_code == requests.codes.ok
 
 def download_assembly(species, genome_version):
     if genome_version==None:
         return False
     species_capital = species.capitalize()
     assembly = species_db[species]["assembly"]
@@ -263,15 +294,15 @@
         fasta_url = f"{ftp_address}/release-{ensembl_version}/fasta/{species}/dna/{species_capital}.{assembly}.dna.nonchromosomal.fa.gz"
     print(fasta_url)
     script = """
 cd {gdir}
 rm {species}.assembly.{genome_version}/* >/dev/null 2>&1
 mkdir {species}.assembly.{genome_version} >/dev/null 2>&1
 cd {species}.assembly.{genome_version}
-wget {fasta_url} -O {species}.fasta.gz
+wget {fasta_url} -O {species}.fasta.gz --no-check-certificate
 gunzip -f {species}.fasta.gz
 python3 -c "import pybio; pybio.data.Fasta('{species}.fasta').split()"
 """
 
     # download FASTA and split
     print(f"[pybio.core.genomes] download FASTA for {species}.{genome_version}")
     command = script.format(gdir=pybio.config.genomes_folder, fasta_url=fasta_url, species=species, species_capital=species_capital, assembly=assembly, genome_version=genome_version, ensembl_version=ensembl_version)
@@ -297,15 +328,15 @@
         gff3_url = f"{ftp_address}/release-{ensembl_version}/gff3/{species}/{species_capital}.{assembly}.{ensembl_version}.gff3.gz"
     script = """
 cd {gdir}
 rm {species}.annotation.{genome_version}/* >/dev/null 2>&1
 mkdir {species}.annotation.{genome_version} >/dev/null 2>&1
 cd {species}.annotation.{genome_version}
 # https://www.biostars.org/p/279235/#279238
-wget {gff3_url} -O {species}.gff3.gz
+wget {gff3_url} -O {species}.gff3.gz --no-check-certificate
 """
     # download GFF3
     print(f"[pybio.core.genomes] download annotation GFF3 for {species}.{genome_version}")
     command = script.format(gff3_url=gff3_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
     print(command)
     os.system(command)
 
@@ -316,15 +347,15 @@
         gtf_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.gtf.gz"
 
     script = """
 cd {gdir}
 mkdir {species}.annotation.{genome_version} >/dev/null 2>&1
 cd {species}.annotation.{genome_version}
 # https://www.biostars.org/p/279235/#279238
-wget {gtf_url} -O {species}.gtf.gz
+wget {gtf_url} -O {species}.gtf.gz --no-check-certificate
 """
     # download GTF
     print(f"[pybio.core.genomes] download annotation GTF for {species}.{genome_version}")
     command = script.format(gtf_url=gtf_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
     return os.system(command)
 
 def star_index(species, genome_version, threads=1):
@@ -333,17 +364,16 @@
     ensembl_version = genome_version.replace("ensembl", "")
     ensembl_version = ensembl_version.replace("genomes", "")
     script = """
 cd {gdir}
 rm {species}.assembly.{genome_version}.star/* >/dev/null 2>&1
 mkdir {species}.assembly.{genome_version}.star >/dev/null 2>&1
 cd {species}.assembly.{genome_version}.star
-gunzip ../{species}.annotation.{genome_version}/{species}.gtf.gz
+gunzip -k ../{species}.annotation.{genome_version}/{species}.gtf.gz # -k to keep both .gz and uncompressed GTF, some tools require uncompressed GTF
 STAR --runMode genomeGenerate --genomeSAindexNbases {genomeSAindexNbases} --genomeDir ../{species}.assembly.{genome_version}.star --genomeFastaFiles ../{species}.assembly.{genome_version}/{species}.fasta --runThreadN {threads} --sjdbGTFfile ../{species}.annotation.{genome_version}/{species}.gtf
-gzip -f ../{species}.annotation.{genome_version}/{species}.gtf
 """
     fasta_file = f"{pybio.config.genomes_folder}/{species}.assembly.{genome_version}/{species}.fasta"
     fasta_size = os.path.getsize(fasta_file)
     genomeSAindexNbases = int(min(14, math.log(fasta_size, 2)/2 - 1))
     command = script.format(threads=threads, genomeSAindexNbases=genomeSAindexNbases, gdir=pybio.config.genomes_folder, species=species, species_capital=species_capital, assembly=assembly, ensembl_version=ensembl_version, genome_version=genome_version)
     return os.system(command)
 
@@ -358,72 +388,69 @@
         ftp_address = f"{ftp_address}/{subfolder}"
     
     script = """
 cd {gdir}
 rm {species}.transcripts.{genome_version}/* >/dev/null 2>&1
 mkdir {species}.transcripts.{genome_version} >/dev/null 2>&1
 cd {species}.transcripts.{genome_version}
-wget {ftp_address}/release-{ensembl_version}/fasta/{species}/cdna/{species_capital}.{assembly}.cdna.all.fa.gz -O {species}.transcripts.fasta.gz
+wget {ftp_address}/release-{ensembl_version}/fasta/{species}/cdna/{species_capital}.{assembly}.cdna.all.fa.gz -O {species}.transcripts.fasta.gz --no-check-certificate
 
 cd {gdir}
 salmon index -t {species}.transcripts.{genome_version}/{species}.transcripts.fasta.gz -i {species}.transcripts.{genome_version}.salmon
 """
     command = script.format(ftp_address=ftp_address, gdir=pybio.config.genomes_folder, species=species, species_capital=species_capital, assembly=assembly, ensembl_version=ensembl_version, genome_version=genome_version)
     return os.system(command)
 
 def get_latest_ensembl():
-    import requests, sys
     server = "https://rest.ensembl.org"
     ext = "/info/data/?"
-    r = requests.get(server+ext, headers={ "Content-Type" : "application/json"})
+    r = requests.get(server+ext, headers={ "Content-Type" : "application/json"}, verify=False)
     if not r.ok:
         r.raise_for_status()
         sys.exit()
     decoded = r.json()
     return str(decoded["releases"][0])
 
 def get_latest_ensemblgenomes():
-    import requests, sys   
     server = "https://rest.ensembl.org"
     ext = "/info/eg_version?"
-    r = requests.get(server+ext, headers={ "Content-Type" : "application/json"})
+    r = requests.get(server+ext, headers={ "Content-Type" : "application/json"}, verify=False)
     if not r.ok:
         r.raise_for_status()
         sys.exit()
     decoded = r.json()
     return str(decoded["version"])
 
 def get_genome_info(genome_id): 
   server = "https://rest.ensembl.org"
   ext = f"/info/genomes/{genome_id}?"
-  r = requests.get(server+ext, headers={ "Content-Type" : "application/json"})
+  r = requests.get(server+ext, headers={ "Content-Type" : "application/json"}, verify=False)
   if not r.ok:
       return {}
   decoded = r.json()
   return decoded
 
 def list_species_ensembl(prepared=True):
     from bs4 import BeautifulSoup
-    import requests
     genome_species_fname_finished = os.path.join(pybio.config.genomes_folder, "genome_species.tab.finished")
     os.system(f"rm {genome_species_fname_finished} >/dev/null 2>&1")
     # download prepared file? (do not query Ensembl)
     if prepared:
         if not os.path.exists(pybio.config.genomes_folder):
             os.makedirs(pybio.config.genomes_folder)
         genome_species_online = "https://raw.githubusercontent.com/grexor/pybio/master/ensembl/genome_species.tab"
-        r = requests.get(genome_species_online, allow_redirects=True)
+        r = requests.get(genome_species_online, allow_redirects=True, verify=False)
         open(os.path.join(pybio.config.genomes_folder, "genome_species.tab"), "wb").write(r.content)
     else:
         print("[pybio.core.genomes] Species list from Ensembl; done once and takes ~ 1 minute")
         ensembl_version = get_latest_ensembl()
         ensemblgenomes_version = get_latest_ensemblgenomes()
         species_db = {}
         def listFD(url, ext=''):
-            page = requests.get(url).text
+            page = requests.get(url, verify=False).text
             soup = BeautifulSoup(page, 'html.parser')
             return [node.get('href')[:-1] for node in soup.find_all('a') if node.get('href').endswith(ext)]
         if not os.path.exists(pybio.config.genomes_folder):
             os.makedirs(pybio.config.genomes_folder)
         f = open(os.path.join(pybio.config.genomes_folder, "genome_species.tab"), "wt")
         f.write("species\tassembly\tprovider\tprovider_subfolder\tgenome_version\tdisplay_name\n")
         for species in listFD(f"https://ftp.ensembl.org/pub/release-{ensembl_version}/fasta/", "/")[1:]:
@@ -590,7 +617,20 @@
                 # negative test
                 for pos in range(int(data["stop"]), int(data["stop"])+100):
                     _, _, exons, _, _ = annotate("homo_sapiens", data["chr"], data["strand"], pos)
                     exons = [exon.exon_id for exon in exons]
                     assert(atts["exon_id"] not in exons)
         r = f.readline()
     f.close()
+
+# find genes (gene_id, gene_name) by exact match of a search term
+def find_genes(search):
+    results = set()
+    for gene_id, gene in genes_db.items():
+        if gene.gene_name==search:
+            results.add((0, gene_id, gene.gene_name))
+        elif gene.gene_name.find(search)!=-1:
+            results.add((1, gene_id, gene.gene_name))
+    results = list(results)
+    results.sort()
+    results = [(e1, e2) for (_, e1, e2) in results]
+    return results
```

### Comparing `pybio-0.3.9/pybio/data/Bedgraph.py` & `pybio-0.5/pybio/data/Bedgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import gzip
-import bisect
 import pybio
 import os
 import json
-import pysam
-import numpy as np
 
 def mix_sort(x):
     if isinstance(x, int):
         return "0%d" % x
     else:
         return str(x)
```

### Comparing `pybio-0.3.9/pybio/data/Fasta.py` & `pybio-0.5/pybio/data/Fasta.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/data/Fastq.py` & `pybio-0.5/pybio/data/Fastq.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/maths/__init__.py` & `pybio-0.5/pybio/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/maths/pstat.py` & `pybio-0.5/pybio/maths/pstat.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/maths/stats.py` & `pybio-0.5/pybio/maths/stats.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/pybio` & `pybio-0.5/pybio/pybio`

 * *Files 10% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 parser.add_argument("-version", "--version", help="Print version", action="store_true")
 parser.add_argument("-nostar", "--nostar", help="Do not process genome with STAR (index)", action="store_true")
 parser.add_argument("-nosalmon", "--nosalmon", help="Do not process transcripts with salmon (index)", action="store_true")
 parser.add_argument("-species", "--species", help="Species name, e.g. homo_sapiens")
 parser.add_argument("-genome_version", "--genome_version", help="Version of the genome, e.g. ensembl109; if not provided, the latest Ensembl version is used")
 parser.add_argument("-fasta", "--fasta", help="Process sequences from fasta file")
 parser.add_argument("-gtf", "--gtf", help="GTF file to import")
-parser.add_argument("-threads", "--threads", default="1", help="Number of threads to use (default: 1)")
+parser.add_argument("-threads", "--threads", '-t', '--t', default="1", help="Number of threads to use (default: 1)")
 parser.add_argument("-help", "-h", "--help", action="store_true")
+parser.add_argument("-xs", "--xs", help="Add '--outSAMstrandField intronMotif'", action="store_false")
 args = parser.parse_args()
 
 help_0 = """
 Usage: pybio <command> [options]
 
 Commands:
   -- Genome
-     genome species        Download and prepare latest genome version 
+     genome species        Download and prepare genome
 
   -- Search
      search search_text    Displays all available genomes matching search_text
 
   -- Configuration
      config [folder]       If no folder provided, prompts for location of genomes data folder
-     path species          Prints FASTA and GTF file path for provided species (one per line, two last lines of output)
+     path species          Prints FASTA and GTF file path for provided species (+genome version)
 
 Options:
 
+     -genome_version       Specify genome version (e.g. ensembl110)
      -nostar, -nosalmon    Avoid building STAR and samlmon index for the genome
      -threads n            Number of threads to use (STAR mapping, etc), default: 1
      -fasta fasta_file     Fasta file for custom genome
      -gtf gtf_file         GTF file for custom genome
      -version              Display pybio version
 
 """
@@ -60,14 +62,22 @@
 # single-end sequencing
 $ pybio star homo_sapiens r1.fastq.gz output.bam
 
 # paired-end sequencing
 $ pybio star homo_sapiens r1.fastq.gz r2.fastq.gz output.bam
 """
 
+help_gff4jbrowse = """
+Prepare GFF3 for JBrowse2, without gene records and moving the Parent=gene: to Name property of transcripts
+
+Example:
+
+$ pybio gff3jbrowse2 input.gff output.gff
+"""
+
 help_sam2bam = """
 Convert .sam to .bam file:
 
 Example:
 
 $ pybio sam2bam file1.sam file1.bam
 """
@@ -99,15 +109,15 @@
             potential_hits.append((len(display_name), species_id, display_name))
     potential_hits.sort()
     if len(potential_hits)>0:
         return potential_hits
     return []
 
 def display_potential_hits(potential_hits, search_text):
-    print(f"We found {len(potential_hits)} genome hits for your provided genome species `{search_text}`.\nPlease choose the species genome you would like to download:\n")
+    print(f"We found {len(potential_hits)} genome hits for your provided genome species `{search_text}`.\n")
     for hit in potential_hits:
         print(f"Species = '{hit[1]}', display name = '{hit[2]}'")
     if len(potential_hits)>0:
         print(f"\nFor example, to download the first hit from the list above, you could write:\n")
         print(f"$ pybio genome {potential_hits[0][1]}")
         print()
     sys.exit(1)
@@ -134,69 +144,82 @@
 
     if args.commands[0]=="path":
         if len(args.commands)<2:
             print("Please provide species, e.g.:\n\n$ pybio path homo_sapiens\n")
             sys.exit(0)
         species = args.commands[1]
         species, genome_version, potential_hits = resolve_species_version(species, args)
+        if genome_version==None:
+            print(f"pybio couldn't find any genomes for species '{species}'.\nPlease provide a valid genome species to retrieve paths.")
+            sys.exit(0)
         annotation_folder = os.path.join(pybio.config.genomes_folder, "%s.annotation.%s" % (species, genome_version))
         assembly_folder = os.path.join(pybio.config.genomes_folder, "%s.assembly.%s" % (species, genome_version))
         fasta_file = os.path.join(assembly_folder, f"{species}.fasta")
         gtf_file = os.path.join(annotation_folder, f"{species}.gtf.gz")
         gff3_file = os.path.join(annotation_folder, f"{species}.gff3.gz")
         print(fasta_file)
         print(gtf_file)
         print(gff3_file)
         sys.exit(0)
 
     if args.commands[0] in ["species", "search"]:
         if len(args.commands)>1:
             potential_hits = determine_species(args.commands[1])
             display_potential_hits(potential_hits, args.commands[1])
+        else:
+            print(f"Please provide a search term for the species, otherwise all available Ensembl genome species are stored in the local database at:\n\n{pybio.config.genomes_folder}/genome_species.tab")
 
     if args.commands[0]=="genome":
         if len(args.commands)==1:
             print("All genomes data stored at: " + pybio.config.genomes_folder)
             print(help_genome)
             sys.exit(0)
         species = args.commands[1]
         species, genome_version, potential_hits = resolve_species_version(species, args)
         if len(potential_hits)>1:
             display_potential_hits(potential_hits, species)
         if genome_version==None:
-            print("Unknown genome version, examples: ensembl109 or ensemblgenomes56")
+            print("Please provide a custom or valid Ensembl genome version, examples: custom_genome_v1 / ensembl110 / ensemblgenomes57")
             sys.exit(1)
         if genome_version.find("ensembl")!=-1:
             pybio.genome_download(species, genome_version, args)
             pybio.genome_prepare(species, genome_version, args)
-        elif args.fasta!=None and args.gtf!=None: # provided genome, specified species, fasta, gtf and genome_version, ok
+        elif args.fasta!=None and args.gtf!=None: # user provided genome, species, fasta, gtf, genome_version
             pybio.genome_import(species, genome_version, args)
             pybio.genome_prepare(species, genome_version, args)
         elif (args.fasta==None or args.gtf==None) and (genome_version.find("ensembl")==-1):
             print(f"Could not find a match for the species '{species}'.")
             print("If you would like to import a custom genome from your own FASTA and GTF files,\nan example call would be:\n")
-            print("$ pybio genome custom_species -fasta /path/to/fasta -gtf /path/to/gtf -genome_version genome_v1\n")
-            print("The above imported genome would be reachable under species 'custom_species' and genome_version 'genome_v1'.\n")
+            print("$ pybio genome custom_species -fasta /path/to/fasta -gtf /path/to/gtf -genome_version custom_genome_v1\n")
+            print("The above imported genome would be reachable under species 'custom_species' and genome_version 'custom_genome_v1'.\n")
             print("In case you would like to import an Ensembl ready genome:\n")
-            print("$ pybio genome homo_sapiens ensembl109\n")
-            print("Ommiting the genome version will download the latest Ensembl release.\n")
+            print("$ pybio genome homo_sapiens ensembl110\n")
+            print("Ommiting the genome version will download the latest Ensembl release of the genome.\n")
 
     if args.commands[0]=="config":
         if len(args.commands)>1:
             pybio.config.init(args.commands[1]) # pybio config genome_folder
 
     if args.commands[0]=="sam2bam":
         if len(args.commands) not in [3]:
             print(help_sam2bam)
             sys.exit()
         input_fname = args.commands[1]
         output_fname = args.commands[2]
-        os.system(f"samtools view -F 4 -bS {input_fname} -o {output_fname} # -F 4 means only mapped reads")
-        os.system(f"samtools sort {output_fname} -o {output_fname}")
-        os.system(f"samtools index {output_fname}")
+        os.system(f"samtools view -@ {args.threads} -F 4 -bS {input_fname} -o {output_fname} # -F 4 means only mapped reads")
+        os.system(f"samtools sort {output_fname} -o {output_fname} -@ {args.threads}")
+        os.system(f"samtools index {output_fname} -@ {args.threads}")
+
+    if args.commands[0]=="gff4jbrowse":
+        if len(args.commands) not in [3]:
+            print(help_gff4jbrowse)
+            sys.exit()
+        file1=args.commands[1]
+        file2=args.commands[2]
+        pybio.gff4jbrowse(file1, file2)
 
     if args.commands[0]=="star":
         if len(args.commands) not in [4,5]:
             print(help_star)
             sys.exit()
         
         species = args.commands[1]
@@ -217,18 +240,25 @@
             file2=args.commands[3]
             output = args.commands[4]
 
         # remove .bam if provided
         if output.endswith(".bam"):
             output = output[:-4]
 
+        # --outFilterMultimapNmax 1
+        # --outSAMstrandField intronMotif
+        add_params = []
+        if args.xs:
+            add_params.append("--outSAMstrandField intronMotif")
+        add_params = " ".join(add_params)
         if file2!=None: # paired-end
-            os.system(f"STAR --runThreadN {args.threads} --outFileNamePrefix {output}_ --outFilterMultimapNmax 1 --genomeDir {star_folder} --readFilesIn {file1} {file2} --readFilesCommand zcat")
+            print(f"STAR --runThreadN {args.threads} --outFileNamePrefix {output}_  --genomeDir {star_folder} --readFilesIn {file1} {file2} --readFilesCommand zcat {add_params}")
+            os.system(f"STAR --runThreadN {args.threads} --outFileNamePrefix {output}_  --genomeDir {star_folder} --readFilesIn {file1} {file2} --readFilesCommand zcat {add_params}")
         if file2==None: # single-end
-            os.system(f"STAR --runThreadN {args.threads} --outFileNamePrefix {output}_ --outFilterMultimapNmax 1 --genomeDir {star_folder} --readFilesIn {file1} --readFilesCommand zcat")
+            os.system(f"STAR --runThreadN {args.threads} --outFileNamePrefix {output}_  --genomeDir {star_folder} --readFilesIn {file1} --readFilesCommand zcat {add_params}")
 
-        os.system(f"pybio sam2bam {output}_Aligned.out.sam {output}.bam")
+        os.system(f"pybio sam2bam {output}_Aligned.out.sam {output}.bam -threads {args.threads}")
         os.system(f"mv {output}_Log.final.out {output}.stats.txt")
         os.system(f"mv {output}_Log.out {output}.log.txt")
         os.system(f"mv {output}_Log.progress.out {output}.progress.txt")
         os.system(f"rm {output}_Aligned.out.sam")
-        os.system(f"mv {output}_SJ.out.tab {output}.splice.tab")
+        os.system(f"mv {output}_SJ.out.tab {output}.splice.tab")
```

### Comparing `pybio-0.3.9/pybio/sequence/__init__.py` & `pybio-0.5/pybio/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/pybio/utils/__init__.py` & `pybio-0.5/pybio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.9/setup.py` & `pybio-0.5/setup.py`

 * *Files identical despite different names*

