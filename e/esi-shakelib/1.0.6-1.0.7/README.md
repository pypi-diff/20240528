# Comparing `tmp/esi_shakelib-1.0.6.tar.gz` & `tmp/esi_shakelib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_shakelib-1.0.6.tar", last modified: Thu May 16 18:39:27 2024, max compression
+gzip compressed data, was "esi_shakelib-1.0.7.tar", last modified: Tue May 28 17:28:19 2024, max compression
```

## Comparing `esi_shakelib-1.0.6.tar` & `esi_shakelib-1.0.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      517 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1522 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.134951 esi_shakelib-1.0.6/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imt.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/correlation/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/ccf_base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/dummy.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/loth_baker_2013.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/directivity/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/bayless2013.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25636 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/rowshandel2013.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27220 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/ffsimmer.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7274 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/generic_site_amplitication.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmice/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/ak07.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/fm11.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/gmice.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/wald99.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/wgrw12.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10920 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/readme
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3225 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nullgmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    43334 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/multigmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/multiutils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/plotting/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/contour.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/plotrupture.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/sites.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/station.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/src/esi_shakelib/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/containers.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/imt_string.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11907 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6723 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/virtualipe.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3491 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      470 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.085778 esi_shakelib-1.0.7/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-28 17:28:19.085778 esi_shakelib-1.0.7/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      517 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1522 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-28 17:28:19.085778 esi_shakelib-1.0.7/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.065778 esi_shakelib-1.0.7/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.073778 esi_shakelib-1.0.7/src/esi_shakelib/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.073778 esi_shakelib-1.0.7/src/esi_shakelib/conversions/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/convert_imc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/convert_imt.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.073778 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.077777 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.077777 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.077777 esi_shakelib-1.0.7/src/esi_shakelib/correlation/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/correlation/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/correlation/ccf_base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/correlation/dummy.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/correlation/loth_baker_2013.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.077777 esi_shakelib-1.0.7/src/esi_shakelib/directivity/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/directivity/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/directivity/bayless2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25636 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/directivity/rowshandel2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    29046 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/ffsimmer.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7274 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/generic_site_amplitication.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.081778 esi_shakelib-1.0.7/src/esi_shakelib/gmice/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/ak07.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/fm11.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/gmice.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/wald99.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmice/wgrw12.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.081778 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10920 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.081778 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.081778 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_tables/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_tables/readme
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3225 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nullgmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    43334 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/multigmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/multiutils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.081778 esi_shakelib-1.0.7/src/esi_shakelib/plotting/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/plotting/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/plotting/contour.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/plotting/plotrupture.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/sites.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/station.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.085778 esi_shakelib-1.0.7/src/esi_shakelib/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:27:01.000000 esi_shakelib-1.0.7/src/esi_shakelib/utils/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/utils/containers.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/utils/exception.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/utils/imt_string.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11907 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/utils/utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6576 2024-05-28 17:25:24.000000 esi_shakelib-1.0.7/src/esi_shakelib/virtualipe.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-28 17:28:19.085778 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-28 17:28:19.000000 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3491 2024-05-28 17:28:19.000000 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-28 17:28:19.000000 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      470 2024-05-28 17:28:19.000000 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2024-05-28 17:28:19.000000 esi_shakelib-1.0.7/src/esi_shakelib.egg-info/top_level.txt
```

### Comparing `esi_shakelib-1.0.6/LICENSE.md` & `esi_shakelib-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/PKG-INFO` & `esi_shakelib-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.6
+Version: 1.0.7
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `esi_shakelib-1.0.6/README.md` & `esi_shakelib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/pyproject.toml` & `esi_shakelib-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imc.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/convert_imc.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imt.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/convert_imt.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/boore_kishida_2017.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/boore_kishida_2017.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/newmark_hall_1982.py` & `esi_shakelib-1.0.7/src/esi_shakelib/conversions/imt/newmark_hall_1982.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/correlation/ccf_base.py` & `esi_shakelib-1.0.7/src/esi_shakelib/correlation/ccf_base.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/correlation/dummy.py` & `esi_shakelib-1.0.7/src/esi_shakelib/correlation/dummy.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/correlation/loth_baker_2013.py` & `esi_shakelib-1.0.7/src/esi_shakelib/correlation/loth_baker_2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/directivity/bayless2013.py` & `esi_shakelib-1.0.7/src/esi_shakelib/directivity/bayless2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/directivity/rowshandel2013.py` & `esi_shakelib-1.0.7/src/esi_shakelib/directivity/rowshandel2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/ffsimmer.py` & `esi_shakelib-1.0.7/src/esi_shakelib/ffsimmer.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,47 +75,61 @@
 
 class FFSimmer:
     """
     Class to perform monte carlo simulations of finite faults to derive mean ground
     motions
     """
 
-    def __init__(self, origin, rff, measure="median"):
+    def __init__(self, rff, measure="median"):
         """
-        origin: (Origin object)
-            The earthquake origin
-        gmpe: (MultiGMPE object)
-            The MultiGMPE to be used for the simulations
-        rff: (RandomFiniteFault object)
-            An object initialized to a set of random faults
-        nsim: (int)
-            The number of simulations to perform
+        Args:
+            rff (RandomFiniteFault object):
+                An instance of the RandomFiniteFault object.
+            measure (str):
+                Either "mean" or "median" -- the measure of central tendency to report.
         """
         if measure not in ("mean", "median"):
             raise ValueError(f"Unknown measure of central tendency: {measure}")
         self.measure = measure
         warnings.simplefilter("ignore", ConvergenceWarning)
-        self.origin = copy.copy(origin)
         self.rff = rff
+        self.origin = copy.copy(rff.origin)
 
-    def compute_grid(self, grid, gmpes, myimts):
+    def compute_grid(self, grid, gmpe, myimts):
         """
         Args:
-            grid: (Grid2D object)
+            grid (Grid2D object):
                 Basically the vs30grid that we're mapping, used for its dimensions.
                 The site corrections have to be done elsewhere.
-            myimts (list)
+            gmpe (MultiGMPE object):
+                The MultiGMPE to be used for the simulations.
+            myimts (list):
                 List of OQ IMTs to generate grids and transects for
+
+        Returns:
+            dictionary:
+                {
+                    oqimt: {
+                        "mean": 2D Array (the median or mean ground motion values, at
+                            a Vs30 of 760 m/s),
+                        "transect": Array (a transect of the grid at the repis below),
+                        "repi": Array (the Repis corresponding to "transect" above),
+                        oqconst.StdDev.TOTAL: Array,
+                        (if allowed:)
+                        oqconst.StdDev.INTER_EVENT: Array,
+                        oqconst.StdDev.INTRA_EVENT: Array,
+                    },
+                }
         """
         griddict = {}
         hypo = self.origin.getHypo()
         olon = hypo.x
         olat = hypo.y
 
-        sd_types = list(gmpes[myimts[0]].DEFINED_FOR_STANDARD_DEVIATION_TYPES)
+        sd_types = list(gmpe[myimts[0]].DEFINED_FOR_STANDARD_DEVIATION_TYPES)
 
         #
         gd = grid.getGeoDict()
         # Increase the grid resolution if it is greater the 30 arc-seconds
         delta_y = gd.dy
         if delta_y > (30.0 / 3600.0):
             delta_y = delta_y / 2.0
@@ -161,26 +175,26 @@
         sigs = np.empty((nimt, nsim, nx * ny))
         if len(sd_types) > 1:
             taus = np.empty((nimt, nsim, nx * ny))
             phis = np.empty((nimt, nsim, nx * ny))
 
         for idx in range(nsim):
             rupt = self.rff.retrieve_rupt(idx)
-            dist = Distance.fromSites(gmpes[myimts[0]], sites, rupt)
+            dist = Distance.fromSites(gmpe[myimts[0]], sites, rupt)
             dctx = dist.getDistanceContext()
             for k, v in dctx.__dict__.items():
                 if k == "_slots_":
                     continue
                 if not isinstance(dctx.__dict__[k], np.ndarray):
                     continue
                 dctx.__dict__[k] = dctx.__dict__[k].flatten()
-            rctx = rupt.getRuptureContext(gmpes[myimts[0]])
+            rctx = rupt.getRuptureContext(gmpe[myimts[0]])
 
             for iimt, simt in enumerate(myimts):
-                mean, stddevs = gmpes[simt].get_mean_and_stddevs(
+                mean, stddevs = gmpe[simt].get_mean_and_stddevs(
                     sctx, rctx, dctx, simt, sd_types
                 )
                 means[iimt, idx, :] = mean[0]
                 sigs[iimt, idx, :] = stddevs[0][0]
                 if len(sd_types) > 1:
                     taus[iimt, idx, :] = stddevs[1][0]
                     phis[iimt, idx, :] = stddevs[2][0]
@@ -266,26 +280,41 @@
                     grepi, repi, np.flip(mean_phis)
                 )
 
         return griddict
 
     def compute_points(self, sctx, gmpe, myimts, rock_vs30=760.0, soil_vs30=180.0):
         """
+        Compute median (or mean) ground motions for a set of sites defined in "sctx"
+        for the imts in the list "myimts".
+
         Args:
             sctx: (Sites object)
                 A sites context object set up for the points being output
             gmpe: (MultiGMPE object)
                 The gmpe to perform the ground-motion realizations.
             myimts (list)
                 List of OQ IMTs to generate rock and site amplified values for
 
         Returns:
             dictionary:
-                "rock": The sites at a reference rock vs30 of 760 m/s
-                "soil": The sites amplified at their given vs30
+                {
+                    oqimt: {
+                        "site": The sites at their actual Vs30
+                            {
+                                "mean": Array,
+                                oqconst.StdDev.TOTAL: Array,
+                                (if allowed:)
+                                oqconst.StdDev.INTER_EVENT: Array,
+                                oqconst.StdDev.INTRA_EVENT: Array,
+                            }
+                        "rock": The sites at a reference rock vs30 of 760 m/s
+                        "soil": The sites at a reference soil vs30 of 180 m/s
+                    },
+                }
         """
         outdict = {}
 
         sd_types = list(gmpe.DEFINED_FOR_STANDARD_DEVIATION_TYPES)
 
         sctx_rock = copy.deepcopy(sctx)
         sctx_rock.vs30 = np.full_like(sctx.vs30, rock_vs30)
@@ -422,39 +451,47 @@
 
 
 class RandomFiniteFault(object):
     """
     Class to dole out random finite faults efficiently.
     """
 
-    def __init__(self, origin, nsim):
+    def __init__(self, origin, nsim, seed=None):
         """
         Args:
-            origin (Origin objece)
+            origin (Origin object): The origin of the earthquake. Can include
+                attributes "tectonic_region" ("Active", "Stable", "Subduction" are
+                recognized) and "mech" ("ALL", "NM" (normal), "RS" (reverse), "SS"
+                (strike-slip)).
+            nsim (int): The number of simulations to run.
+            seed (int): A seed for the random number generator (for testing only).
         """
         self.origin = origin
         self.nsim = nsim
         self.rupts = []
+        self.rng = np.random.default_rng(seed)
         self.initialize()
 
     def initialize(self):
         """
         Initialize the random arrays
         """
         (mscale, aspect, mindip_deg, maxdip_deg) = get_scaling_params(self.origin)
         _, _, _, _, area_mean, area_std = dimensions_from_magnitude(
             self.origin.mag, mscale, 1, 0
         )
         hypo = self.origin.getHypo()
-        area = 10 ** np.random.normal(np.log10(area_mean[0]), area_std, self.nsim)
+        depth = hypo.z
+        depth = self.rng.uniform(np.clip(depth - 5.0, 0, None), depth + 5, self.nsim)
+        area = 10 ** self.rng.normal(np.log10(area_mean[0]), area_std, self.nsim)
         width = np.sqrt(area / aspect)
         length = aspect * width
-        dx = np.random.uniform(0, length)
-        strike = np.random.uniform(-180, 180, self.nsim)
-        dip = np.radians(np.random.uniform(mindip_deg, maxdip_deg, self.nsim))
+        dx = self.rng.uniform(0, length)
+        strike = self.rng.uniform(-180, 180, self.nsim)
+        dip = np.radians(self.rng.uniform(mindip_deg, maxdip_deg, self.nsim))
         # Need to apply a max to dy that might be less than width based on the
         # eq depth.
         # H = vertical projection of plane
         # sin(dip) = H/W
         # H = W sin(dip)
         height = width * np.sin(dip)
         #  -----
@@ -462,26 +499,25 @@
         #   \  | dz
         # dy \ |
         #     \|
         # sin(dip) = dz / dy
         # top_of_rupture = depth - dz so
         # depth - dz > 0
         # depth > dz
-        dz = np.random.uniform(0, np.minimum(height, hypo.z))
+        dz = self.rng.uniform(0, np.minimum(height, depth))
         dy = dz / np.sin(dip)
         hx = np.array([hypo.x])
         hy = np.array([hypo.y])
-        hz = np.array([hypo.z])
 
         for idx in range(self.nsim):
             self.rupts.append(
                 QuadRupture.fromOrientation(
                     hx,
                     hy,
-                    hz,
+                    np.array([depth[idx]]),
                     [dx[idx]],
                     [dy[idx]],
                     [length[idx]],
                     [width[idx]],
                     [strike[idx]],
                     [np.degrees(dip[idx])],
                     self.origin,
```

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/generic_site_amplitication.py` & `esi_shakelib-1.0.7/src/esi_shakelib/generic_site_amplitication.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmice/ak07.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmice/ak07.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmice/fm11.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmice/fm11.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmice/gmice.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmice/gmice.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmice/wald99.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmice/wald99.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmice/wgrw12.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmice/wgrw12.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt` & `esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat` & `esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nullgmpe.py` & `esi_shakelib-1.0.7/src/esi_shakelib/gmpe/nullgmpe.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/multigmpe.py` & `esi_shakelib-1.0.7/src/esi_shakelib/multigmpe.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/multiutils.py` & `esi_shakelib-1.0.7/src/esi_shakelib/multiutils.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/plotting/contour.py` & `esi_shakelib-1.0.7/src/esi_shakelib/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/plotting/plotrupture.py` & `esi_shakelib-1.0.7/src/esi_shakelib/plotting/plotrupture.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/sites.py` & `esi_shakelib-1.0.7/src/esi_shakelib/sites.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/station.py` & `esi_shakelib-1.0.7/src/esi_shakelib/station.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/utils/containers.py` & `esi_shakelib-1.0.7/src/esi_shakelib/utils/containers.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/utils/imt_string.py` & `esi_shakelib-1.0.7/src/esi_shakelib/utils/imt_string.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/utils/utils.py` & `esi_shakelib-1.0.7/src/esi_shakelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib/virtualipe.py` & `esi_shakelib-1.0.7/src/esi_shakelib/virtualipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 
 from openquake.hazardlib.gsim.base import GMPE
 from openquake.hazardlib.imt import PGA, PGV, SA, MMI
 from openquake.hazardlib import const
 
 from esi_shakelib.utils.exception import ShakeLibException
-from esi_shakelib.ffsimmer import FFSimmer
 from esi_shakelib.generic_site_amplitication import GenericSiteAmplification
 from esi_utils_rupture.point_rupture import PointRupture
 
 
 class VirtualIPE(GMPE):
     """
     Implements a virtual IPE that is the combination of a MultiGMPE
@@ -48,34 +47,32 @@
     DEFINED_FOR_TECTONIC_REGION_TYPE = None
     #: Determined by the GMPE selected.
     REQUIRES_RUPTURE_PARAMETERS = None
     #: Determined by the GMPE selected.
     REQUIRES_SITES_PARAMETERS = None
 
     @classmethod
-    def __fromFuncs__(cls, gmpe, gmice, rupture_obj=None, rff=None):
+    def __fromFuncs__(cls, gmpe, gmice, rupture_obj=None):
         """
         Creates a new VirtualIPE object with the specified MultiGMPE and
         GMICE. There is no default constructor, you must use this method.
 
         Args:
             gmpe: An instance of the MultiGMPE object.
             gmice: An instance of a GMICE object.
-            rupture_obj: A rupture object, if not None and a PointRupture, FFSimmer
-                will be used.
+            rupture_obj: A rupture object.
 
         Returns:
             :class:`VirtualIPE`: A new instance of a VirtualIPE object.
 
         """
         self = cls()
         self.gmpe = gmpe
         self.gmice = gmice
         self.rupture_obj = rupture_obj
-        self.rff = rff
 
         if (
             gmpe.ALL_GMPES_HAVE_PGV is True
             and PGV in gmice.DEFINED_FOR_INTENSITY_MEASURE_TYPES
         ):
             self.imt = PGV()
         elif (
```

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib.egg-info/PKG-INFO` & `esi_shakelib-1.0.7/src/esi_shakelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.6
+Version: 1.0.7
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `esi_shakelib-1.0.6/src/esi_shakelib.egg-info/SOURCES.txt` & `esi_shakelib-1.0.7/src/esi_shakelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

