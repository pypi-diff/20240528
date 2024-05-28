# Comparing `tmp/gpe_lib-0.0.2-py3-none-any.whl.zip` & `tmp/gpe_lib-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3401 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     2721 b- defN 24-May-28 13:35 gpe_lib/__init__.py
+Zip file size: 3408 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     2758 b- defN 24-May-28 13:42 gpe_lib/__init__.py
 -rw-rw-rw-  2.0 fat      116 b- defN 24-May-28 11:08 gpe_lib/imports.py
 -rw-rw-rw-  2.0 fat      342 b- defN 24-May-28 12:01 gpe_lib/notebook/__init__.py
 -rw-rw-rw-  2.0 fat      661 b- defN 24-May-28 12:00 gpe_lib/notebook/colab.py
 -rw-rw-rw-  2.0 fat      395 b- defN 24-May-28 12:00 gpe_lib/notebook/jupyter.py
--rw-rw-rw-  2.0 fat      133 b- defN 24-May-28 13:38 gpe_lib-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 13:38 gpe_lib-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 24-May-28 13:38 gpe_lib-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      695 b- defN 24-May-28 13:38 gpe_lib-0.0.2.dist-info/RECORD
-9 files, 5180 bytes uncompressed, 2205 bytes compressed:  57.4%
+-rw-rw-rw-  2.0 fat      133 b- defN 24-May-28 13:42 gpe_lib-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 13:42 gpe_lib-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 24-May-28 13:42 gpe_lib-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      695 b- defN 24-May-28 13:42 gpe_lib-0.0.3.dist-info/RECORD
+9 files, 5217 bytes uncompressed, 2212 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gpe_lib/notebook/colab.py
 Comment: 
 
 Filename: gpe_lib/notebook/jupyter.py
 Comment: 
 
-Filename: gpe_lib-0.0.2.dist-info/METADATA
+Filename: gpe_lib-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: gpe_lib-0.0.2.dist-info/WHEEL
+Filename: gpe_lib-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: gpe_lib-0.0.2.dist-info/top_level.txt
+Filename: gpe_lib-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gpe_lib-0.0.2.dist-info/RECORD
+Filename: gpe_lib-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpe_lib/__init__.py

```diff
@@ -1,18 +1,18 @@
 # gpe_lib/__init__.py
 # --- IMPORTS ---------------------------------------------------------------
 from . import notebook
-import os, requests, matplotlib, matplotlib.font_manager
+import os, requests, matplotlib, matplotlib.font_manager, matplotlib.colors
 
 # --- DECLARATIONS ----------------------------------------------------------
 NIDEC = True
 
 colors_dict = {"ngreen":"#009B49", "ngrey":'#666666', "nblack":"#000000", "egreen":"#008691","yellow":"#BEBE00","blue":"#59B2D8","red":"#FF0000"}
 colors = list(colors_dict.values())
-nidec_cmap = LinearSegmentedColormap.from_list("nidec", [np.array([0.243,0.243,0.243])+np.array([-0.243,0.757,0.234])*i/255 for i in range(256)])
+nidec_cmap = matplotlib.colors.LinearSegmentedColormap.from_list("nidec", [np.array([0.243,0.243,0.243])+np.array([-0.243,0.757,0.234])*i/255 for i in range(256)])
 
 # --- FUNCTIONS -------------------------------------------------------------
 def set_nidec_color_cycle():
     import matplotlib.pyplot as plt
     plt.rcParams["axes.prop_cycle"] = plt.cycler(color=colors_list)
 
 def __use_font(family,fonts):
```

## Comparing `gpe_lib-0.0.2.dist-info/RECORD` & `gpe_lib-0.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gpe_lib/__init__.py,sha256=BG2PQQT03baHPs0PL3KMnN8JI2PNqQ_Jv5OGyCdftJ8,2721
+gpe_lib/__init__.py,sha256=ObcUMUGTNM10TvpIn5ZhQp1vrOJWU4mhS2GU5yaWOI8,2758
 gpe_lib/imports.py,sha256=0sgUi2xhQgPdoGfRahl_wZ3pKMuw-4hw9dDbLDiSr10,116
 gpe_lib/notebook/__init__.py,sha256=9e4B-k_4zKHyRKoaC9n7fT6mL5oa68k6Huw98puMV8E,342
 gpe_lib/notebook/colab.py,sha256=m6lrLGAhtb9Q3s4N3Wa6-JF3CchkCbuQ_FQWzzNAC2M,661
 gpe_lib/notebook/jupyter.py,sha256=8qxY_CJlxaXsRGZcyHZmJk3paktRM9Urz67RRhSr_dA,395
-gpe_lib-0.0.2.dist-info/METADATA,sha256=9Yfaao-PF7S_hAgZxyBG0rsLSHJUcjW_CsZ4_rQs1ME,133
-gpe_lib-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gpe_lib-0.0.2.dist-info/top_level.txt,sha256=5skBuTtZQFyRnJy6zYefBDKPbjEN5n7p0WfsouOBM9k,25
-gpe_lib-0.0.2.dist-info/RECORD,,
+gpe_lib-0.0.3.dist-info/METADATA,sha256=EU7GX0TMWLrBCJ-RTiP772F7p-cLpr3eNMRzTG5Yrxc,133
+gpe_lib-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gpe_lib-0.0.3.dist-info/top_level.txt,sha256=5skBuTtZQFyRnJy6zYefBDKPbjEN5n7p0WfsouOBM9k,25
+gpe_lib-0.0.3.dist-info/RECORD,,
```

