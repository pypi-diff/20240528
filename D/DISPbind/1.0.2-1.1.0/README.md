# Comparing `tmp/DISPbind-1.0.2.tar.gz` & `tmp/dispbind-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DISPbind-1.0.2.tar", last modified: Wed Dec 14 01:28:35 2022, max compression
+gzip compressed data, was "dispbind-1.1.0.tar", last modified: Mon May 27 12:55:47 2024, max compression
```

## Comparing `DISPbind-1.0.2.tar` & `dispbind-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 rd494      (501) staff       (20)        0 2022-12-14 01:28:35.480570 DISPbind-1.0.2/
-drwxr-xr-x   0 rd494      (501) staff       (20)        0 2022-12-14 01:28:35.475957 DISPbind-1.0.2/DISPbind.egg-info/
--rw-r--r--   0 rd494      (501) staff       (20)      545 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/PKG-INFO
--rw-r--r--   0 rd494      (501) staff       (20)      397 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/SOURCES.txt
--rw-r--r--   0 rd494      (501) staff       (20)        1 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/dependency_links.txt
--rw-r--r--   0 rd494      (501) staff       (20)       52 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/entry_points.txt
--rw-r--r--   0 rd494      (501) staff       (20)      135 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/requires.txt
--rw-r--r--   0 rd494      (501) staff       (20)        9 2022-12-14 01:28:35.000000 DISPbind-1.0.2/DISPbind.egg-info/top_level.txt
--rw-r--r--   0 rd494      (501) staff       (20)     1122 2022-11-16 18:41:35.000000 DISPbind-1.0.2/LICENSE.txt
--rw-r--r--   0 rd494      (501) staff       (20)      545 2022-12-14 01:28:35.480307 DISPbind-1.0.2/PKG-INFO
--rw-r--r--   0 rd494      (501) staff       (20)     4444 2022-12-14 01:27:35.000000 DISPbind-1.0.2/README.md
-drwxr-xr-x   0 rd494      (501) staff       (20)        0 2022-12-14 01:28:35.479847 DISPbind-1.0.2/dispbind/
--rw-r--r--   0 rd494      (501) staff       (20)     1440 2022-12-13 18:11:18.000000 DISPbind-1.0.2/dispbind/DISPbind.py
--rw-r--r--   0 rd494      (501) staff       (20)        0 2022-11-16 18:41:35.000000 DISPbind-1.0.2/dispbind/__init__.py
--rw-r--r--   0 rd494      (501) staff       (20)     6733 2022-12-14 01:23:33.000000 DISPbind-1.0.2/dispbind/align.py
--rw-r--r--   0 rd494      (501) staff       (20)     4817 2022-12-14 01:10:44.000000 DISPbind-1.0.2/dispbind/bam2bw.py
--rw-r--r--   0 rd494      (501) staff       (20)     1069 2022-11-16 18:41:35.000000 DISPbind-1.0.2/dispbind/helper.py
--rw-r--r--   0 rd494      (501) staff       (20)     4781 2022-12-13 18:12:35.000000 DISPbind-1.0.2/dispbind/island.py
--rw-r--r--   0 rd494      (501) staff       (20)       36 2022-11-16 18:41:35.000000 DISPbind-1.0.2/dispbind/main.py
--rw-r--r--   0 rd494      (501) staff       (20)     1295 2022-12-14 01:04:47.000000 DISPbind-1.0.2/dispbind/signal.py
--rw-r--r--   0 rd494      (501) staff       (20)       22 2022-11-28 01:51:49.000000 DISPbind-1.0.2/dispbind/version.py
--rw-r--r--   0 rd494      (501) staff       (20)       38 2022-12-14 01:28:35.480665 DISPbind-1.0.2/setup.cfg
--rw-r--r--   0 rd494      (501) staff       (20)     1191 2022-11-30 16:29:12.000000 DISPbind-1.0.2/setup.py
+drwxr-xr-x   0 dongrui1  (3446) slst-dongrui1  (3079)        0 2024-05-27 12:55:48.000000 dispbind-1.1.0/
+drwxr-xr-x   0 dongrui1  (3446) slst-dongrui1  (3079)        0 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)      834 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/PKG-INFO
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)      397 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/SOURCES.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)        1 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/dependency_links.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)       52 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/entry_points.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)      139 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/requires.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)        9 2024-05-27 12:55:48.000000 dispbind-1.1.0/DISPbind.egg-info/top_level.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     1122 2024-04-17 07:04:24.000000 dispbind-1.1.0/LICENSE.txt
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)      834 2024-05-27 12:55:48.000000 dispbind-1.1.0/PKG-INFO
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     4460 2024-04-17 07:04:24.000000 dispbind-1.1.0/README.md
+drwxr-xr-x   0 dongrui1  (3446) slst-dongrui1  (3079)        0 2024-05-27 12:55:48.000000 dispbind-1.1.0/dispbind/
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     1440 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/DISPbind.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)        0 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/__init__.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     5922 2024-05-27 09:13:10.000000 dispbind-1.1.0/dispbind/align.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     5283 2024-05-21 11:48:40.000000 dispbind-1.1.0/dispbind/bam2bw.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     1069 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/helper.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     4781 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/island.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)       36 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/main.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     1295 2024-04-17 07:04:24.000000 dispbind-1.1.0/dispbind/signal.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)       22 2024-05-21 07:47:01.000000 dispbind-1.1.0/dispbind/version.py
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)       38 2024-05-27 12:55:48.000000 dispbind-1.1.0/setup.cfg
+-rw-r--r--   0 dongrui1  (3446) slst-dongrui1  (3079)     1195 2024-05-27 12:55:41.000000 dispbind-1.1.0/setup.py
```

### Comparing `DISPbind-1.0.2/LICENSE.txt` & `dispbind-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DISPbind-1.0.2/README.md` & `dispbind-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -105,11 +105,11 @@
 | Signal      | Sum of DisP signal in merged region|
 | Rank        | Rank of DisP signal                |
 | Island      | Label Island or not Island         |
 
 
 ## Citation
 
-Yu-Hang Xing\*, Rui Dong\*, Lukuo Lee, Shruthi Rengarajan, Nicolò Riggi, Gaylor Boulay and Miguel N. Rivera#. **DisP-seq reveals the genome-wide functional organization of DNA-associated disordered proteins** *Under review*
+Yu-Hang Xing\*, Rui Dong\*, Lukuo Lee, Shruthi Rengarajan, Nicolò Riggi, Gaylor Boulay and Miguel N. Rivera#. **DisP-seq reveals the genome-wide functional organization of DNA-associated disordered proteins**, 2023, ***Nature Biotechnol***
 
 ## License
 Copyright (C) 2022 Rivera Lab. See [LICENSE](about/license.md) for license rights and limitations (MIT).
```

### Comparing `DISPbind-1.0.2/dispbind/DISPbind.py` & `dispbind-1.1.0/dispbind/DISPbind.py`

 * *Files identical despite different names*

### Comparing `DISPbind-1.0.2/dispbind/align.py` & `dispbind-1.1.0/dispbind/align.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 #@logger
 def align(options):
     # check index files
     if not options['--index']:
         sys.exit('Alignment requires BWA index files!')
     if not options['--fastq1'] or not options['--fastq2']:
         sys.exit('Alignment requires paired-end fastq files!')
+    if options['--fastq1'] == options['--fastq2']:
+        sys.exit('Check the -a and -b input, they should not be the same file!')
 
     # check output directory
     out_dir = check_outdir(options['--output'])
     bwa_map(out_dir,options['--index'], options['--name'], options['--mquality'], options['--fastq1'], options['--fastq2'], options['--thread'], options['--gsize'])
 
 def check_outdir(out_dir):
     '''
@@ -54,87 +56,72 @@
 
 
 def bwa_map(out_dir, index, name, mquality, fastq1, fastq2, thread, gsize):
     '''
     1. Map reads with BWA
     2. Create BigWig file
     '''
-    # BWA mapping R1
     print('Map reads with BWA...')
-    bwa_cmd1 = 'bwa aln -t '
-    bwa_cmd1 += ' %s %s %s ' % (thread, index, fastq1)
-    bwa_cmd1 += '> %s/%s 2>/dev/null' % (out_dir, name + '.r1.sai')
+    bwa_cmd1 = 'bwa mem -t '
+    bwa_cmd1 += ' %s %s %s %s' % (thread, index, fastq1, fastq2)
+    bwa_cmd1 += '| samtools sort -T %s/%s -o %s/%s 2>/dev/null' % (out_dir, name + '.sort.tmp', out_dir, name + '.raw.bam')
     return_code = os.system(bwa_cmd1) >> 8
     if return_code:
         sys.exit('Error: cannot map reads with BWA!')
-    # BWA mapping R2
-    bwa_cmd2 = 'bwa aln -t '
-    bwa_cmd2 += ' %s %s %s ' % (thread, index, fastq2)
-    bwa_cmd2 += '> %s/%s 2>/dev/null' % (out_dir, name + '.r2.sai')
-    return_code = os.system(bwa_cmd2) >> 8
-    if return_code:
-        sys.exit('Error: cannot map reads with BWA!')
-    # BWA sampe
-    bwa_sampe = 'bwa sampe '
-    bwa_sampe += ' %s %s/%s %s/%s ' % (index, out_dir, name + '.r1.sai', out_dir, name + '.r2.sai')
-    bwa_sampe += ' %s %s > %s/%s 2>/dev/null' % (fastq1, fastq2, out_dir, name + '.sam')
-    return_code = os.system(bwa_sampe) >> 8
-    if return_code:
-        sys.exit('Error: cannot map reads with BWA!')
-    print('BWA mapping finished...')
-    # sam to bam
-    sam2bam = 'samtools view -bS'
-    sam2bam += ' %s/%s > %s/%s ' % (out_dir, name + '.sam', out_dir, name + '.raw.bam')
-    return_code = os.system(sam2bam) >> 8
-    if return_code:
-        sys.exit('Error: cannot convert sam to bam file!')
-    # selece high quality reads
+
     filter_bam = 'samtools view -b -F2308 -q '
     filter_bam += ' %s %s/%s > %s/%s ' % (mquality, out_dir, name + '.raw.bam', out_dir, name + '.bam')
     return_code = os.system(filter_bam) >> 8
     if return_code:
         sys.exit('Error: cannot filter bam file!')
     # sort bam
     sort_bam = 'samtools sort -T '
-    sort_bam += ' %s/%s -o %s/%s %s/%s ' % (out_dir, name + '.sorted', out_dir, name + '.sorted.bam', out_dir, name + '.bam')
+    sort_bam += ' %s/%s -o %s/%s %s/%s ' % (out_dir, name + '.sorted.temp', out_dir, name + '.sorted.bam', out_dir, name + '.bam')
     return_code = os.system(sort_bam) >> 8
     if return_code:
         sys.exit('Error: cannot sort bam file!')
-    # remove duplicate
+   # remove duplicate
     rm_dup = 'samtools rmdup -s '
-    rm_dup += ' %s/%s %s/%s ' % (out_dir, name + '.sorted.bam', out_dir, name + '.sorted.deduped.bam')
+    rm_dup += ' %s/%s %s/%s ' % (out_dir, name + '.sorted.bam', out_dir, name + '.deduped.bam')
     return_code = os.system(rm_dup) >> 8
     if return_code:
         sys.exit('Error: cannot remove dup!')
-    # bam to bedpe and fill gaps
-    bam2bedpe = 'samtools view -b -f2 '
-    bam2bedpe += ' %s/%s | bedtools bamtobed -bedpe 2>/dev/null | cut -f 1,2,6 |sort -k1,1 -k2,2n > %s/%s' % (out_dir, name + '.sorted.deduped.bam', out_dir, name + '.bed')
+    # bam to sortn
+    bamsortn = 'samtools view -f2 -b'
+    bamsortn += ' %s/%s |samtools sort -T %s/%s -n > %s/%s' % (out_dir, name + '.deduped.bam',out_dir, name + '.sort.tmp', out_dir, name + '.sorted_n.bam')
+    return_code = os.system(bamsortn) >> 8
+    if return_code:
+        sys.exit('Error: cannot sorted by name!')
+
+    bam2bedpe = 'bedtools bamtobed -bedpe -i '
+    bam2bedpe += ' %s/%s 2>/dev/null | perl -alne \'print \"$F[0]\\t$F[1]\\t$F[5]\" if $F[5]>$F[1] and $F[0]=~/chr/ and $F[1]>0 and $F[5]>0\' |sort -k1,1 -k2,2n > %s/%s' % (out_dir, name + '.sorted_n.bam', out_dir, name + '.bed')
     return_code = os.system(bam2bedpe) >> 8
     if return_code:
         sys.exit('Error: cannot remove dup!')
 
+
     # create Bigwig file
     if which('bedGraphToBigWig') is not None:
         print('Create BigWig file...')
-        map_bam_fname = '%s/%s' % (out_dir, name + '.sorted.deduped.bam')
+        map_bam_fname = '%s/%s' % (out_dir, name + '.deduped.bam')
         # index bam if not exist
         if not os.path.isfile(map_bam_fname + '.bai'):
             pysam.index(map_bam_fname)
         map_bam = pysam.AlignmentFile(map_bam_fname, 'rb')
         # scale to HPB
         mapped_reads = map_bam.mapped
         s = 10000000.0 / mapped_reads
         map_bed_fname = '%s/%s' % (out_dir, name + '.bed')
         map_bed = pybedtools.BedTool(map_bed_fname)
         bedgraph_fname = '%s/%s' % (out_dir,name + '.bg')
         with open(bedgraph_fname, 'w') as bedgraph_f:
             for line in map_bed.genome_coverage(bg=True,
                                                 g=gsize,
                                                 scale=s, split=True):
-                value = str(int(float(line[3]) + 0.5))
+                value = str(float(line[3]) + 0.5)
                 bedgraph_f.write('\t'.join(line[:3]) + '\t%s\n' % value)
         # sort bedgraph
         sort_bg = 'LC_COLLATE=C sort -k1,1 -k2,2n %s/%s > %s/%s ' % (out_dir,name + '.bg', out_dir,name + '.sorted.bg')
         return_code = os.system(sort_bg) >> 8
         if return_code:
             sys.exit('Error: cannot sort bg!')
         # bg 2 bigwig
@@ -142,15 +129,12 @@
         bigwig_fname = '%s/%s' % (out_dir,name + '.bw')
         return_code = os.system('bedGraphToBigWig %s %s %s' %
                                 (bedgraph_sname, gsize,
                                  bigwig_fname)) >> 8
         if return_code:
             sys.exit('Error: cannot convert bedGraph to BigWig!')
 
-        file2rm = '%s/%s,%s/%s,%s/%s,%s/%s,%s/%s,%s/%s,%s/%s,%s/%s,%s/%s' % (out_dir, name + '.r1.sai', out_dir, name + '.r2.sai', \
-                                                                            out_dir, name + '.sam',out_dir, name + '.bam', \
-                                                                            out_dir, name + '.raw.bam', out_dir, name + '.sorted.bam', \
-                                                                            out_dir, name + '.bg', out_dir, name + '.sorted.bg', out_dir, name + '.bed')
+        file2rm = '%s/%s,%s/%s,%s/%s,%s/%s,%s/%s' % (out_dir, name + '.bam',out_dir, name + '.sorted_n.bam', out_dir, name + '.bg', out_dir, name + '.sorted.bg', out_dir, name + '.bed')
         for f in file2rm.strip().split(","):
                 os.remove(f)
     else:
         print('Could not find bedGraphToBigWig, so skip this step!')
```

### Comparing `DISPbind-1.0.2/dispbind/bam2bw.py` & `dispbind-1.1.0/dispbind/bam2bw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Usage: DISPbind bam2bw [options] -b bam -n NAME -o OUT
+Usage: DISPbind bam2bw [options] -b bam -g genomesize -n NAME -o OUT
 
 Options:
     -h --help                      Show help message.
     -v --version                   Show version.
     -m MQ --mquality=MQUALITY      Mapping quality. [default: 10]
     -g GSIZE --gsize=GSIZE         Genome size file.
     -n NAME --name=NAME            Output file name. [default: bwa_out]
@@ -58,63 +58,68 @@
     filter_bam = 'samtools view -b -F2308 -q '
     filter_bam += ' %s %s > %s/%s ' % (mquality, bam, out_dir, name + '.filter.bam')
     return_code = os.system(filter_bam) >> 8
     if return_code:
         sys.exit('Error: cannot filter bam file!')
     # sort bam
     sort_bam = 'samtools sort -T '
-    sort_bam += ' %s/%s -o %s/%s %s/%s ' % (out_dir, name + '.sorted', out_dir, name + '.sorted.bam', out_dir, name + '.filter.bam')
+    #sort_bam += ' %s/%s -o %s/%s %s/%s ' % (out_dir, name + '.sorted', out_dir, name + '.sorted.bam', out_dir, name + '.bam')
+    sort_bam += ' %s/%s -o %s/%s %s/%s ' % (out_dir, name + '.sorted.temp', out_dir, name + '.sorted.bam', out_dir, name + '.filter.bam')
     return_code = os.system(sort_bam) >> 8
     if return_code:
         sys.exit('Error: cannot sort bam file!')
     # remove duplicate
     rm_dup = 'samtools rmdup -s '
-    rm_dup += ' %s/%s %s/%s ' % (out_dir, name + '.sorted.bam', out_dir, name + '.sorted.deduped.bam')
+    rm_dup += ' %s/%s %s/%s ' % (out_dir, name + '.sorted.bam', out_dir, name + '.deduped.bam')
     return_code = os.system(rm_dup) >> 8
     if return_code:
         sys.exit('Error: cannot remove dup!')
     # bam to bedpe and fill gaps
-    bam2bedpe = 'samtools view -b -f2 '
-    bam2bedpe += ' %s/%s | bedtools bamtobed -bedpe 2>/dev/null | cut -f 1,2,6 |sort -k1,1 -k2,2n > %s/%s' % (out_dir, name + '.sorted.deduped.bam', out_dir, name + '.bed')
+    bam2sortn = 'samtools view -b -f2 '
+    bam2sortn += ' %s/%s | samtools sort -n > %s/%s' % (out_dir, name + '.deduped.bam', out_dir, name + '.sorted_n.bam')
+    return_code = os.system(bam2sortn) >> 8
+    if return_code:
+        sys.exit('Error: cannot sort bam file by name!')
+    bam2bedpe = 'bedtools bamtobed -bedpe -i '
+    bam2bedpe += ' %s/%s 2>/dev/null | perl -alne \'print \"$F[0]\\t$F[1]\\t$F[5]\" if $F[5]>$F[1] and $F[0]=~/chr/ and $F[1]>0 and $F[5]>0\' |sort -k1,1 -k2,2n > %s/%s' % (out_dir, name + '.sorted_n.bam', out_dir, name + '.bed')
     return_code = os.system(bam2bedpe) >> 8
     if return_code:
-        sys.exit('Error: cannot remove dup!')
+        sys.exit('Error: cannot convert bam to bedpe!')
 
     # create Bigwig file
     if which('bedGraphToBigWig') is not None:
         print('Create BigWig file...')
-        map_bam_fname = '%s/%s' % (out_dir, name + '.sorted.deduped.bam')
+        map_bam_fname = '%s/%s' % (out_dir, name + '.deduped.bam')
         # index bam if not exist
         if not os.path.isfile(map_bam_fname + '.bai'):
             pysam.index(map_bam_fname)
         map_bam = pysam.AlignmentFile(map_bam_fname, 'rb')
         # scale to HPB
         mapped_reads = map_bam.mapped
         s = 10000000.0 / mapped_reads
         map_bed_fname = '%s/%s' % (out_dir, name + '.bed')
         map_bed = pybedtools.BedTool(map_bed_fname)
         bedgraph_fname = '%s/%s' % (out_dir,name + '.bg')
         with open(bedgraph_fname, 'w') as bedgraph_f:
             for line in map_bed.genome_coverage(bg=True,
                                                 g=gsize,
                                                 scale=s, split=True):
-                value = str(int(float(line[3]) + 0.5))
+                value = str(float(line[3]) + 0.5)
                 bedgraph_f.write('\t'.join(line[:3]) + '\t%s\n' % value)
         # sort bedgraph
         sort_bg = 'LC_COLLATE=C sort -k1,1 -k2,2n %s/%s > %s/%s ' % (out_dir,name + '.bg', out_dir,name + '.sorted.bg')
         return_code = os.system(sort_bg) >> 8
         if return_code:
             sys.exit('Error: cannot sort bg!')
         # bg 2 bigwig
         bedgraph_sname = '%s/%s' % (out_dir,name + '.sorted.bg')
         bigwig_fname = '%s/%s' % (out_dir,name + '.bw')
         return_code = os.system('bedGraphToBigWig %s %s %s' %
                                 (bedgraph_sname, gsize,
                                  bigwig_fname)) >> 8
         if return_code:
             sys.exit('Error: cannot convert bedGraph to BigWig!')
-        file2rm = '%s/%s,%s/%s,%s/%s,%s/%s,%s/%s' % (out_dir, name + '.filter.bam', out_dir, name + '.sorted.bam', \
-                                                     out_dir, name + '.bg', out_dir, name + '.sorted.bg', out_dir, name + '.bed')
+        file2rm = '%s/%s,%s/%s,%s/%s,%s/%s,%s/%s,%s/%s' % (out_dir, name + '.filter.bam',out_dir, name + '.sorted_n.bam', out_dir, name + '.sorted.bam', out_dir, name + '.bg', out_dir, name + '.sorted.bg', out_dir, name + '.bed')
         for f in file2rm.strip().split(","):
                 os.remove(f)
     else:
         print('Could not find bedGraphToBigWig, so skip this step!')
```

### Comparing `DISPbind-1.0.2/dispbind/helper.py` & `dispbind-1.1.0/dispbind/helper.py`

 * *Files identical despite different names*

### Comparing `DISPbind-1.0.2/dispbind/island.py` & `dispbind-1.1.0/dispbind/island.py`

 * *Files identical despite different names*

### Comparing `DISPbind-1.0.2/dispbind/signal.py` & `dispbind-1.1.0/dispbind/signal.py`

 * *Files identical despite different names*

### Comparing `DISPbind-1.0.2/setup.py` & `dispbind-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,19 +21,19 @@
       keywords='disorder protein',
       packages=find_packages(),
       install_requires=[
           'requests',
           'pysam>=0.8.4',
           'pybedtools>=0.7.5',
           'pandas>=1.0.5',
-          'matplotlib>=3.3.0'
+          'matplotlib>=3.3.0',
           'numpy>=1.10.0',
-          'docopt>=0.6.0'
-          'pyBigWig>=0.3.17'
-          'seaborn>=0.10.0'
+          'docopt>=0.6.0',
+          'pyBigWig>=0.3.17',
+          'seaborn>=0.10.0',
           'scipy',
       ],
       entry_points={
           'console_scripts': [
               'DISPbind=dispbind.DISPbind:main'
           ],
       },
```

