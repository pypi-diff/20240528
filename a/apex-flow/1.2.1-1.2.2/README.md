# Comparing `tmp/apex_flow-1.2.1.tar.gz` & `tmp/apex_flow-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apex_flow-1.2.1.tar", last modified: Thu May  9 04:21:31 2024, max compression
+gzip compressed data, was "apex_flow-1.2.2.tar", last modified: Tue May 28 05:59:45 2024, max compression
```

## Comparing `apex_flow-1.2.1.tar` & `apex_flow-1.2.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.970988 apex_flow-1.2.1/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.1/LICENSE
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-09 04:21:31.970086 apex_flow-1.2.1/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-09 04:19:27.000000 apex_flow-1.2.1/README.md
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.914918 apex_flow-1.2.1/apex/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-05-09 04:20:18.000000 apex_flow-1.2.1/apex/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/__main__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.1/apex/archive.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10465 2024-04-24 07:51:37.000000 apex_flow-1.2.1/apex/config.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.920537 apex_flow-1.2.1/apex/core/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/__init__.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.932403 apex_flow-1.2.1/apex/core/calculator/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-04-11 09:05:32.000000 apex_flow-1.2.1/apex/core/calculator/ABACUS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/Lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/Task.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.1/apex/core/calculator/VASP.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/calculator.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.946681 apex_flow-1.2.1/apex/core/calculator/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/calculator/lib/abacus_scf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.1/apex/core/calculator/lib/abacus_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/lib/lammps_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/lib/vasp_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-05-08 08:06:39.000000 apex_flow-1.2.1/apex/core/common_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/common_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/gen_confs.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.953144 apex_flow-1.2.1/apex/core/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/crys.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/dispatcher.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/lmp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/mfp_eosfit.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/pwscf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/siesta.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/slab_orientation.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/trans_tools.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/util.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/mpdb.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.957188 apex_flow-1.2.1/apex/core/property/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10390 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/EOS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    11811 2024-04-24 15:53:23.000000 apex_flow-1.2.1/apex/core/property/Elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    27104 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    24024 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    26343 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/property/Property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10716 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9520 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/property/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/reproduce.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/structure.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.958840 apex_flow-1.2.1/apex/database/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/DatabaseFactory.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/DynamoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/MongoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/StorageBase.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-04-24 08:51:43.000000 apex_flow-1.2.1/apex/flow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.1/apex/main.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.959615 apex_flow-1.2.1/apex/op/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/op/RunLAMMPS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/op/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/op/property_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/op/relaxation_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2622 2024-04-26 16:57:00.000000 apex_flow-1.2.1/apex/report.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.961653 apex_flow-1.2.1/apex/reporter/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13972 2024-05-09 04:16:06.000000 apex_flow-1.2.1/apex/reporter/DashReportApp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/reporter/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/reporter/property_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/reporter/relaxation_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/step.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/submit.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.962479 apex_flow-1.2.1/apex/superop/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/RelaxationFlow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/SimplePropertySteps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.1/apex/utils.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.969684 apex_flow-1.2.1/apex_flow.egg-info/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/entry_points.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/requires.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/top_level.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-09 04:21:31.971043 apex_flow-1.2.1/setup.cfg
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-05-09 04:20:18.000000 apex_flow-1.2.1/setup.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.969367 apex_flow-1.2.1/tests/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/context.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus_property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_eos.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_make_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_mpdb.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_equi_std.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_kspacing.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240867 apex_flow-1.2.2/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.2/LICENSE
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 05:59:45.240630 apex_flow-1.2.2/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-28 05:52:49.000000 apex_flow-1.2.2/README.md
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.223174 apex_flow-1.2.2/apex/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/__main__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.2/apex/archive.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10491 2024-05-09 10:37:35.000000 apex_flow-1.2.2/apex/config.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.225057 apex_flow-1.2.2/apex/core/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/__init__.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.226440 apex_flow-1.2.2/apex/core/calculator/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/ABACUS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/Lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/Task.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.2/apex/core/calculator/VASP.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/calculator.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.227877 apex_flow-1.2.2/apex/core/calculator/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/calculator/lib/abacus_scf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.2/apex/core/calculator/lib/abacus_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/lib/lammps_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/lib/vasp_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/common_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/common_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/gen_confs.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.230570 apex_flow-1.2.2/apex/core/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/crys.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/dispatcher.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/lmp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/mfp_eosfit.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/pwscf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/siesta.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/slab_orientation.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/trans_tools.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/util.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/mpdb.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.233090 apex_flow-1.2.2/apex/core/property/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10388 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/EOS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    11809 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    27102 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/Gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    26217 2024-05-28 05:54:53.000000 apex_flow-1.2.2/apex/core/property/Interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    26341 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/Phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/property/Property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10603 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9518 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/property/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/reproduce.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/structure.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.233960 apex_flow-1.2.2/apex/database/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/DatabaseFactory.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/DynamoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/MongoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/StorageBase.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-05-16 05:37:47.000000 apex_flow-1.2.2/apex/flow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.2/apex/main.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.234627 apex_flow-1.2.2/apex/op/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/op/RunLAMMPS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/op/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/op/property_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/op/relaxation_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2702 2024-05-09 12:22:10.000000 apex_flow-1.2.2/apex/report.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.235565 apex_flow-1.2.2/apex/reporter/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13857 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/reporter/DashReportApp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/reporter/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/reporter/property_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/reporter/relaxation_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/step.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/submit.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.236119 apex_flow-1.2.2/apex/superop/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/superop/RelaxationFlow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/superop/SimplePropertySteps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/superop/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.2/apex/utils.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240319 apex_flow-1.2.2/apex_flow.egg-info/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/entry_points.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/requires.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/top_level.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-28 05:59:45.240906 apex_flow-1.2.2/setup.cfg
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-05-28 05:52:49.000000 apex_flow-1.2.2/setup.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240126 apex_flow-1.2.2/tests/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/context.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus_property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_eos.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_make_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_mpdb.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_equi_std.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_kspacing.py
```

### Comparing `apex_flow-1.2.1/LICENSE` & `apex_flow-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/PKG-INFO` & `apex_flow-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.1/README.md` & `apex_flow-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/__init__.py` & `apex_flow-1.2.2/apex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 LOCAL_PATH = os.getcwd()
 
 
 def header():
     header_str = ""
     header_str += "---------------------------------------------------------------\n"
     header_str += "░░░░░░█▐▓▓░████▄▄▄█▀▄▓▓▓▌█░░░░░░░░░░█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█░░░░░\n"
```

### Comparing `apex_flow-1.2.1/apex/archive.py` & `apex_flow-1.2.2/apex/archive.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/config.py` & `apex_flow-1.2.2/apex/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         for kk in bohrium_config_data.keys():
             bohrium.config[kk] = bohrium_config_data[kk]
 
     def get_executor(
             self,
             dispatcher_config: dict
     ) -> DispatcherExecutor:
-        if not (self.context_type or self.machine):
+        if not (self.context_type or self.machine or self.dispatcher_config):
             executor = None
         else:
             # get arguments for instantiation of the DispatcherExecutor
             sig = inspect.signature(DispatcherExecutor.__init__)
             # pop out 'self'
             defined_parameters = list(sig.parameters.keys())
             defined_parameters.pop(0)
```

### Comparing `apex_flow-1.2.1/apex/core/calculator/ABACUS.py` & `apex_flow-1.2.2/apex/core/calculator/ABACUS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/Lammps.py` & `apex_flow-1.2.2/apex/core/calculator/Lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/Task.py` & `apex_flow-1.2.2/apex/core/calculator/Task.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/VASP.py` & `apex_flow-1.2.2/apex/core/calculator/VASP.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/calculator.py` & `apex_flow-1.2.2/apex/core/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/lib/abacus_scf.py` & `apex_flow-1.2.2/apex/core/calculator/lib/abacus_scf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/lib/abacus_utils.py` & `apex_flow-1.2.2/apex/core/calculator/lib/abacus_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/lib/lammps_utils.py` & `apex_flow-1.2.2/apex/core/calculator/lib/lammps_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/calculator/lib/vasp_utils.py` & `apex_flow-1.2.2/apex/core/calculator/lib/vasp_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/common_equi.py` & `apex_flow-1.2.2/apex/core/common_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/common_prop.py` & `apex_flow-1.2.2/apex/core/common_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/gen_confs.py` & `apex_flow-1.2.2/apex/core/gen_confs.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/crys.py` & `apex_flow-1.2.2/apex/core/lib/crys.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/dispatcher.py` & `apex_flow-1.2.2/apex/core/lib/dispatcher.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/lmp.py` & `apex_flow-1.2.2/apex/core/lib/lmp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/mfp_eosfit.py` & `apex_flow-1.2.2/apex/core/lib/mfp_eosfit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/pwscf.py` & `apex_flow-1.2.2/apex/core/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/siesta.py` & `apex_flow-1.2.2/apex/core/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/slab_orientation.py` & `apex_flow-1.2.2/apex/core/lib/slab_orientation.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/trans_tools.py` & `apex_flow-1.2.2/apex/core/lib/trans_tools.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/util.py` & `apex_flow-1.2.2/apex/core/lib/util.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/lib/utils.py` & `apex_flow-1.2.2/apex/core/lib/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/mpdb.py` & `apex_flow-1.2.2/apex/core/mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/property/EOS.py` & `apex_flow-1.2.2/apex/core/property/EOS.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             self.init_from_suffix = parameter["init_from_suffix"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
```

### Comparing `apex_flow-1.2.1/apex/core/property/Elastic.py` & `apex_flow-1.2.2/apex/core/property/Elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         # self.reprod = parameter['reproduce']
         self.parameter = parameter
         self.inter_param = inter_param or {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
```

### Comparing `apex_flow-1.2.1/apex/core/property/Gamma.py` & `apex_flow-1.2.2/apex/core/property/Gamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
         if "start_confs_path" in self.parameter and os.path.exists(
                 self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
```

### Comparing `apex_flow-1.2.1/apex/core/property/Interstitial.py` & `apex_flow-1.2.2/apex/core/property/Interstitial.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,42 @@
 import re
 import shutil
 
 import numpy as np
 from monty.serialization import dumpfn, loadfn
 from pymatgen.analysis.defects.generators import VoronoiInterstitialGenerator
 from pymatgen.analysis.defects.core import Interstitial as pmgInterstitial
-from pymatgen.core.structure import Structure
+from pymatgen.core.structure import Structure, Lattice
 from pymatgen.core.sites import PeriodicSite
+from pymatgen.core.tensors import Tensor
+from pymatgen.core.operations import SymmOp
 
 from apex.core.calculator.lib import abacus_utils
 from apex.core.calculator.lib import lammps_utils
 from apex.core.property.Property import Property
 from apex.core.refine import make_refine
 from apex.core.reproduce import make_repro, post_repro
 from apex.core.structure import StructureInfo
 from dflow.python import upload_packages
 
 upload_packages.append(__file__)
 
 PREDEFINED_LIST = ['bcc', 'fcc', 'hcp']
+TOL = 1e-5
 
 class Interstitial(Property):
     def __init__(self, parameter, inter_param=None):
         parameter["reproduce"] = parameter.get("reproduce", False)
         self.reprod = parameter["reproduce"]
         if not self.reprod:
             if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
                 default_supercell = [1, 1, 1]
                 parameter["supercell"] = parameter.get("supercell", default_supercell)
                 self.supercell = parameter["supercell"]
-                self.insert_ele = parameter["insert_ele"]
+                self.insert_ele = parameter.get("insert_ele", None)
                 parameter["lattice_type"] = parameter.get("lattice_type", None)
                 self.lattice_type = parameter["lattice_type"]
                 parameter["voronoi_param"] = parameter.get("voronoi_param", {})
                 self.voronoi_param = parameter["voronoi_param"]
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
             default_cal_setting = {
                 "relax_pos": True,
@@ -60,15 +63,15 @@
         self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         self.path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
                 self.parameter["start_confs_path"]
         ):
@@ -153,41 +156,67 @@
                 if not os.path.exists(equi_contcar):
                     raise RuntimeError("please do relaxation first")
 
                 if self.inter_param["type"] == "abacus":
                     ss = abacus_utils.stru2Structure(equi_contcar)
                 else:
                     ss = Structure.from_file(equi_contcar)
-
+                rot = Tensor.get_ieee_rotation(ss)
+                op = SymmOp.from_rotation_and_translation(rot)
+                ss.apply_operation(op)
                 # get structure type
                 os.chdir(self.path_to_work)
                 # convert site element into same type for a pseudo-structure just for simple lattice type judgment
                 same_type_ss = ss.copy()
                 species_mapping = {str(specie): "Ni" for specie in same_type_ss.composition.elements}
                 same_type_ss.replace_species(species_mapping)
                 st = StructureInfo(same_type_ss, symprec=0.1, angle_tolerance=5)
                 # indication of structure type
                 self.structure_type = st.lattice_structure
                 # get conventional standard structure to ss
                 orig_st = StructureInfo(ss, symprec=0.1, angle_tolerance=5)
                 conv_ss = orig_st.conventional_structure
                 conv_ss.to("POSCAR", "POSCAR")
+                conv_ss.to("POSCAR_conv", "POSCAR")
                 ss = conv_ss
                 if self.lattice_type:
                     logging.info(msg=f'Adopt user indicated lattice type: {self.lattice_type}')
                     self.structure_type = self.lattice_type
                 os.chdir(cwd)
 
                 # gen defects
                 dss = []
                 self.insert_element_task = os.path.join(self.path_to_work, "element.out")
                 if os.path.isfile(self.insert_element_task):
                     os.remove(self.insert_element_task)
+                if not self.insert_ele:
+                    self.insert_ele = [str(ii) for ii in set(ss.composition.elements)]
                 for ii in self.insert_ele:
                     if self.structure_type in PREDEFINED_LIST:
+                        # rotate and translate hcp structure to specific orientation for interstitial generation
+                        if self.structure_type == 'hcp':
+                            theta = -2 * np.pi / 3
+                            rot_m = np.array([
+                                [np.cos(theta), -np.sin(theta), 0],
+                                [np.sin(theta), np.cos(theta), 0],
+                                [0, 0, 1]
+                            ])
+                            op = SymmOp.from_rotation_and_translation(rotation_matrix=rot_m)
+                            ss.apply_operation(op)
+                            new_lattice = Lattice([
+                                ss.lattice.matrix[0] * -1, ss.lattice.matrix[1] * -1, ss.lattice.matrix[2]
+                            ])
+                            new_frac_coords = ss.frac_coords.copy()
+                            if not ((new_frac_coords[0][0] < 0.5 and new_frac_coords[0][2] < 0.5)\
+                                    or (new_frac_coords[0][0] > 0.5 and new_frac_coords[0][2] > 0.5)):
+                                new_frac_coords[0][2] = ss.frac_coords[1][2]
+                                new_frac_coords[1][2] = ss.frac_coords[0][2]
+                            new_ss = Structure(new_lattice, ss.species, new_frac_coords, coords_are_cartesian=False)
+                            ss = new_ss
+                            ss.to(os.path.join(self.path_to_work, 'POSCAR_conv'), 'POSCAR')
                         # produce a pseudo interstitial structure for later modification
                         vds = [pmgInterstitial(ss, PeriodicSite(ii, [0.12, 0.13, 0.14], ss.lattice))]
                     else:
                         pre_vds = VoronoiInterstitialGenerator(**self.voronoi_param)
                         vds = pre_vds.generate(ss, [ii])
                     for jj in vds:
                         temp = jj.get_supercell_structure(
@@ -249,45 +278,45 @@
                 os.chdir(self.path_to_work)
 
                 # create pre-defined special SIA structure for bcc fcc and hcp
                 if self.structure_type in PREDEFINED_LIST:
                     if not os.path.isfile("task.000000/POSCAR"):
                         raise RuntimeError("need task.000000 structure as reference")
 
-                    with open('POSCAR', "r") as fin:
+
+                    with open('POSCAR_conv', "r") as fin:
                         fin.readline()
                         scale = float(fin.readline().split()[0])
                         self.latt_param = float(fin.readline().split()[0])
                         self.latt_param *= scale
 
                     with open("task.000000/POSCAR", "r") as fin:
                         self.pos_line = fin.read().split("\n")
 
                     for idx, ii in enumerate(self.pos_line):
                         ss = ii.split()
                         if len(ss) > 3:
                             if (
-                                    abs(0.12 / self.supercell[0] - float(ss[0])) < 1e-5
-                                    and abs(0.13 / self.supercell[1] - float(ss[1])) < 1e-5
-                                    and abs(0.14 / self.supercell[2] - float(ss[2])) < 1e-5
+                                    abs(0.12 / self.supercell[0] - float(ss[0])) < TOL
+                                    and abs(0.13 / self.supercell[1] - float(ss[1])) < TOL
+                                    and abs(0.14 / self.supercell[2] - float(ss[2])) < TOL
                             ):
                                 chl = idx
-                    # pseudo-task only run original POSCAR to save calculation resources
-                    shutil.copyfile("POSCAR", "task.000000/POSCAR")
+                    shutil.rmtree("task.000000")
 
                     os.chdir(cwd)
                     # specify interstitial structures
                     if self.structure_type == 'bcc':
                         for idx, ii in enumerate(self.pos_line):
                             ss = ii.split()
                             if len(ss) > 3:
                                 if (
-                                        abs(0.5 / self.supercell[0] - float(ss[0])) < 1e-5
-                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < 1e-5
-                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < 1e-5
+                                        abs(0.5 / self.supercell[0] - float(ss[0])) < TOL
+                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < TOL
+                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < TOL
                                 ):
                                     center = idx
                         bcc_interstital_dict = {
                             'tetrahedral': {chl: [0.25, 0.5, 0]},
                             'octahedral': {chl: [0.5, 0.5, 0]},
                             'crowdion': {chl: [0.25, 0.25, 0]},
                             '<111>dumbbell': {chl: [1 / 3, 1 / 3, 1 / 3],
@@ -300,24 +329,24 @@
                         total_task = self.__gen_tasks(bcc_interstital_dict)
 
                     elif self.structure_type == 'fcc':
                         for idx, ii in enumerate(self.pos_line):
                             ss = ii.split()
                             if len(ss) > 3:
                                 if (
-                                        abs(1 / self.supercell[0] - float(ss[0])) < 1e-5
-                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < 1e-5
-                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < 1e-5
+                                        abs(1 / self.supercell[0] - float(ss[0])) < TOL
+                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < TOL
+                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < TOL
                                 ):
                                     face = idx
 
                                 if (
-                                        abs(1 / self.supercell[0] - float(ss[0])) < 1e-5
-                                        and abs(1 / self.supercell[1] - float(ss[1])) < 1e-5
-                                        and abs(1 / self.supercell[2] - float(ss[2])) < 1e-5
+                                        abs(1 / self.supercell[0] - float(ss[0])) < TOL
+                                        and abs(1 / self.supercell[1] - float(ss[1])) < TOL
+                                        and abs(1 / self.supercell[2] - float(ss[2])) < TOL
                                 ):
                                     corner = idx
 
                         fcc_interstital_dict = {
                             'tetrahedral': {chl: [0.75, 0.25, 0.25]},
                             'octahedral': {chl: [1, 0, 0.5]},
                             'crowdion': {chl: [1, 0.25, 0.25]},
@@ -345,17 +374,17 @@
                         total_task = self.__gen_tasks(fcc_interstital_dict)
 
                     elif self.structure_type == 'hcp':
                         for idx, ii in enumerate(self.pos_line):
                             ss = ii.split()
                             if len(ss) > 3:
                                 if (
-                                        abs(1/3 / self.supercell[0] - float(ss[0])) < 1e-5
-                                        and abs(2/3 / self.supercell[1] - float(ss[1])) < 1e-5
-                                        and abs(0.25 / self.supercell[2] - float(ss[2])) < 1e-5
+                                        abs(1/3 / self.supercell[0] - float(ss[0])) < TOL
+                                        and abs(2/3 / self.supercell[1] - float(ss[1])) < TOL
+                                        and abs(0.25 / self.supercell[2] - float(ss[2])) < TOL
                                 ):
                                     center = idx
                         hcp_interstital_dict = {
                             'O': {chl: [0, 0, 0.5]},
                             'BO': {chl: [0, 0, 0.25]},
                             'C': {chl: [0.5, 0.5, 0.5]},
                             'BC': {chl: [5/6, 2/3, 0.25]},
@@ -383,15 +412,15 @@
         os.chdir(cwd)
         return self.task_list
 
     def __gen_tasks(self, interstitial_dict):
         cwd = os.getcwd()
         for ii, (type_str, adjust_dict) in enumerate(interstitial_dict.items()):
             output_task = os.path.join(
-                self.path_to_work, "task.%06d" % (len(self.dss) + ii)
+                self.path_to_work, "task.%06d" % (len(self.dss) + ii - 1)
             )
             os.makedirs(output_task, exist_ok=True)
             os.chdir(output_task)
             self.task_list.append(output_task)
             # adjust atom positions in POSCAR
             with open(self.insert_element_task, "a+") as fout:
                 print(self.insert_ele[0], file=fout)
@@ -414,14 +443,27 @@
             logging.info(f"gen {type_str}")
             os.chdir(cwd)
 
         total_task = len(self.dss) + len(interstitial_dict)
 
         return total_task
 
+    def _rotate_hcp(self, poscar):
+        ss = Structure.from_file(poscar)
+        theta = np.pi / 3
+        rot_m = np.array([
+            [np.cos(theta), -np.sin(theta), 0],
+            [np.sin(theta), np.cos(theta), 0],
+            [0, 0, 1]
+        ])
+        op = SymmOp.from_rotation_and_translation(rot_m)
+        ss.apply_operation(op)
+        ss.to(poscar, "POSCAR")
+
+
     def post_process(self, task_list):
         if True:
             fin1 = open(os.path.join(task_list[0], "..", "element.out"), "r")
             for ii in task_list:
                 conf = os.path.join(ii, "conf.lmp")
                 inter = os.path.join(ii, "inter.json")
                 insert_ele = fin1.readline().split()[0]
```

### Comparing `apex_flow-1.2.1/apex/core/property/Phonon.py` & `apex_flow-1.2.2/apex/core/property/Phonon.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param is not None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
```

### Comparing `apex_flow-1.2.1/apex/core/property/Property.py` & `apex_flow-1.2.2/apex/core/property/Property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/property/Surface.py` & `apex_flow-1.2.2/apex/core/property/Surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
@@ -170,19 +170,15 @@
                         "conf.lmp",
                         "in.lammps",
                         "STRU",
                     ]:
                         if os.path.exists(jj):
                             os.remove(jj)
                     task_list.append(output_task)
-                    logging.info(
-                        "# %03d generate " % ii,
-                        output_task,
-                        " \t %d atoms" % len(all_slabs[ii].sites),
-                    )
+                    logging.info(f"{ii} generate {output_task} {len(all_slabs[ii].sites)} atoms")
                     # make confs
                     all_slabs[ii].to("POSCAR.tmp", "POSCAR")
                     vasp_utils.regulate_poscar("POSCAR.tmp", "POSCAR")
                     vasp_utils.sort_poscar("POSCAR", "POSCAR", ptypes)
                     vasp_utils.perturb_xz("POSCAR", "POSCAR", self.pert_xz)
                     if self.inter_param["type"] == "abacus":
                         abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
```

### Comparing `apex_flow-1.2.1/apex/core/property/Vacancy.py` & `apex_flow-1.2.2/apex/core/property/Vacancy.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            logging.warning("%s already exists" % path_to_work)
+            logging.debug("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
```

### Comparing `apex_flow-1.2.1/apex/core/refine.py` & `apex_flow-1.2.2/apex/core/refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/reproduce.py` & `apex_flow-1.2.2/apex/core/reproduce.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/core/structure.py` & `apex_flow-1.2.2/apex/core/structure.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/database/DynamoDB.py` & `apex_flow-1.2.2/apex/database/DynamoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/database/MongoDB.py` & `apex_flow-1.2.2/apex/database/MongoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/database/StorageBase.py` & `apex_flow-1.2.2/apex/database/StorageBase.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/flow.py` & `apex_flow-1.2.2/apex/flow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/main.py` & `apex_flow-1.2.2/apex/main.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/op/RunLAMMPS.py` & `apex_flow-1.2.2/apex/op/RunLAMMPS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/op/property_ops.py` & `apex_flow-1.2.2/apex/op/property_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/op/relaxation_ops.py` & `apex_flow-1.2.2/apex/op/relaxation_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/report.py` & `apex_flow-1.2.2/apex/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from apex.config import Config
 from apex.utils import load_config_file, is_json_file, simplify_paths
 from apex.reporter.DashReportApp import DashReportApp
 
 
 def tag_dataset(orig_dataset: dict) -> dict:
     orig_work_path_list = [k for k in orig_dataset.keys()]
-    simplified_path_dict = simplify_paths(orig_work_path_list)
-    simplified_dataset = {simplified_path_dict[k]: v for k, v in orig_dataset.items()}
+    try:
+        simplified_path_dict = simplify_paths(orig_work_path_list)
+        simplified_dataset = {simplified_path_dict[k]: v for k, v in orig_dataset.items()}
+    except KeyError:
+        simplified_dataset = orig_dataset
     # replace data id with tag specified in the dataset if exists
     tagged_dataset = {}
     for k, v in simplified_dataset.items():
         if tag := v.pop('tag', None):
             tagged_dataset[tag] = v
         else:
             tagged_dataset[k] = v
```

### Comparing `apex_flow-1.2.1/apex/reporter/DashReportApp.py` & `apex_flow-1.2.2/apex/reporter/DashReportApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from .relaxation_report import RelaxationReport
 from .property_report import *
 
 
 NO_GRAPH_LIST = ['relaxation']
 UI_FRONTSIZE = 18
 PLOT_FRONTSIZE = 18
-LINE_SIZE = 2
-MARKER_SIZE = 6
+LINE_SIZE = 3
+MARKER_SIZE = 8
 REF_LINE_SIZE = 4
 REF_MARKER_SIZE = 9
 
 
 def return_prop_class(prop_type: str):
     if prop_type == 'eos':
         return EOSReport
@@ -63,16 +63,16 @@
     return datasets
 
 
 class DashReportApp:
     def __init__(self, datasets):
         dbc_css = "https://cdn.jsdelivr.net/gh/AnnMarieW/dash-bootstrap-templates/dbc.min.css"
         self.datasets = datasets
-        self.all_dimensions = set()
-        self.all_datasets = set()
+        self.all_confs = set()
+        self.all_props = set()
         self.app = dash.Dash(
             __name__,
             suppress_callback_exceptions=True,
             external_stylesheets=[dbc.themes.MATERIA, dbc_css]
         )
         #load_figure_template("materia")
         self.app.layout = self.generate_layout()
@@ -118,51 +118,51 @@
         ]
         while True:
             for color in colors:
                 yield color
 
     def generate_layout(self):
         for w in self.datasets.values():
-            self.all_dimensions.update(w.keys())
-            for dimension in w.values():
-                self.all_datasets.update(dimension.keys())
+            self.all_confs.update(w.keys())
+            for conf in w.values():
+                self.all_props.update(conf.keys())
 
         # find the first default combination of configuration and property exist
-        default_dimension = None
-        default_dataset = None
+        default_conf = None
+        default_prop = None
         for w_key, w in self.datasets.items():
             if not w:
                 continue
             for d_key, d in w.items():
                 if d:
-                    default_dimension = d_key
-                    default_dataset = next(iter(d.keys()))
+                    default_conf = d_key
+                    default_prop = next(iter(d.keys()))
                     break
-            if default_dataset:
+            if default_prop:
                 break
 
         radio_inline = False
-        if len(self.all_dimensions) > 10:
+        if len(self.all_confs) > 10:
             radio_inline = True
         layout = html.Div(
             [
                 html.H1("APEX Results Visualization Report", style={'textAlign': 'center'}),
                 html.Label('Configuration:', style={'font-weight': 'bold', "fontSize": UI_FRONTSIZE}),
                 dcc.RadioItems(
                     id='confs-radio',
-                    options=[{'label': name, 'value': name} for name in self.all_dimensions],
-                    value=default_dimension, inline=radio_inline,
+                    options=[{'label': name, 'value': name} for name in self.all_confs],
+                    value=default_conf, inline=radio_inline,
                     style={"fontSize": UI_FRONTSIZE}
                 ),
                 html.Br(),
                 html.Label('Property:', style={'font-weight': 'bold', "fontSize": UI_FRONTSIZE}),
                 dcc.Dropdown(
                     id='props-dropdown',
-                    options=[{'label': name, 'value': name} for name in self.all_datasets],
-                    value=default_dataset,
+                    options=[{'label': name, 'value': name} for name in self.all_props],
+                    value=default_prop,
                     style={"fontSize": UI_FRONTSIZE}
                 ),
                 html.Br(),
                 dcc.Graph(id='graph', style={'display': 'block', "fontSize": UI_FRONTSIZE},
                           className='graph-container'),
                 html.Div(id='table')
             ],
@@ -170,48 +170,48 @@
         )
         return layout
 
     def update_graph_visibility(self, selected_prop, selected_confs):
         prop_type = return_prop_type(selected_prop)
         valid_count = 0
         if prop_type not in NO_GRAPH_LIST:
-            for w_dimension, dataset in self.datasets.items():
+            for w_conf, dataset in self.datasets.items():
                 try:
                     _ = dataset[selected_confs][selected_prop]
                 except KeyError:
                     pass
                 else:
                     valid_count += 1
         if prop_type in NO_GRAPH_LIST or valid_count == 0:
             return {'display': 'none'}
         else:
             return {'display': 'block'}
 
     def update_dropdown_options(self, selected_confs):
-        all_datasets = set()
+        all_props = set()
         for w in self.datasets.values():
             if selected_confs in w:
-                all_datasets.update(w[selected_confs].keys())
+                all_props.update(w[selected_confs].keys())
 
-        return [{'label': name, 'value': name} for name in all_datasets]
+        return [{'label': name, 'value': name} for name in all_props]
 
     def update_graph(self, selected_prop, selected_confs):
         fig = go.Figure()
         prop_type = return_prop_type(selected_prop)
         color_generator = self.plotly_color_cycle()
         if prop_type not in NO_GRAPH_LIST:
-            for w_dimension, dataset in self.datasets.items():
+            for w_conf, dataset in self.datasets.items():
                 try:
                     data = dataset[selected_confs][selected_prop]['result']
                 except KeyError:
                     pass
                 else:
                     propCls = return_prop_class(prop_type)
-                    # trace_name = f"{w_dimension} - {selected_confs} - {selected_prop}"
-                    trace_name = w_dimension
+                    # trace_name = f"{w_conf} - {selected_confs} - {selected_prop}"
+                    trace_name = w_conf
                     traces, layout = propCls.plotly_graph(
                         data, trace_name,
                         color=next(color_generator)
                     )
                     # set color and width of reference lines
                     if prop_type != 'vacancy':
                         for trace in iter(traces):
@@ -282,33 +282,33 @@
         return fig
 
     def update_table(self, selected_prop, selected_confs):
         table_index = 0
         tables = []
         prop_type = return_prop_type(selected_prop)
         if prop_type == 'relaxation':
-            for w_dimension, dataset in self.datasets.items():
-                table_title = html.H3(f"{w_dimension} - {selected_prop}")
+            for w_conf, dataset in self.datasets.items():
+                table_title = html.H3(f"{w_conf} - {selected_prop}")
                 clip_id = f"clip-{table_index}"
                 clipboard = dcc.Clipboard(id=clip_id, style={"fontSize": UI_FRONTSIZE})
                 table = RelaxationReport.dash_table(dataset)
                 table.id = f"table-{table_index}"
                 tables.append(html.Div([table_title, clipboard, table],
                                        style={'width': '100%', 'display': 'inline-block'}))
                 table_index += 1
         else:
-            for w_dimension, dataset in self.datasets.items():
+            for w_conf, dataset in self.datasets.items():
                 try:
                     data = dataset[selected_confs][selected_prop]['result']
                 except KeyError:
                     pass
                 else:
                     propCls = return_prop_class(prop_type)
                     table_title = html.H3(
-                        f"{w_dimension} - {selected_confs} - {selected_prop}",
+                        f"{w_conf} - {selected_confs} - {selected_prop}",
                         style={"fontSize": UI_FRONTSIZE}
                     )
                     table, df = propCls.dash_table(data)
                     table.id = f"table-{table_index}"
                     # add strips to table
                     table.style_data_conditional = [
                         {'if': {'row_index': 'odd'},
```

### Comparing `apex_flow-1.2.1/apex/reporter/property_report.py` & `apex_flow-1.2.2/apex/reporter/property_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/reporter/relaxation_report.py` & `apex_flow-1.2.2/apex/reporter/relaxation_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/step.py` & `apex_flow-1.2.2/apex/step.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/submit.py` & `apex_flow-1.2.2/apex/submit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/superop/RelaxationFlow.py` & `apex_flow-1.2.2/apex/superop/RelaxationFlow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/superop/SimplePropertySteps.py` & `apex_flow-1.2.2/apex/superop/SimplePropertySteps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex/utils.py` & `apex_flow-1.2.2/apex/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/apex_flow.egg-info/PKG-INFO` & `apex_flow-1.2.2/apex_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.1/apex_flow.egg-info/SOURCES.txt` & `apex_flow-1.2.2/apex_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/setup.py` & `apex_flow-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apex-flow",
-    version="1.2.1",
+    version="1.2.2",
     author="Zhuoyuan Li, Tongqi Wen",
     author_email="zhuoyli@outlook.com",
     description="Alloy Properties EXplorer using simulations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/APEX.git",
     packages=setuptools.find_packages(),
```

### Comparing `apex_flow-1.2.1/tests/context.py` & `apex_flow-1.2.2/tests/context.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_abacus.py` & `apex_flow-1.2.2/tests/test_abacus.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_abacus_equi.py` & `apex_flow-1.2.2/tests/test_abacus_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_abacus_property.py` & `apex_flow-1.2.2/tests/test_abacus_property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_elastic.py` & `apex_flow-1.2.2/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_eos.py` & `apex_flow-1.2.2/tests/test_eos.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_gamma.py` & `apex_flow-1.2.2/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_interstitial.py` & `apex_flow-1.2.2/tests/test_interstitial.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_lammps.py` & `apex_flow-1.2.2/tests/test_lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_make_prop.py` & `apex_flow-1.2.2/tests/test_make_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_mpdb.py` & `apex_flow-1.2.2/tests/test_mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_ops.py` & `apex_flow-1.2.2/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_phonon.py` & `apex_flow-1.2.2/tests/test_phonon.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_refine.py` & `apex_flow-1.2.2/tests/test_refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_surface.py` & `apex_flow-1.2.2/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_vacancy.py` & `apex_flow-1.2.2/tests/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_vasp.py` & `apex_flow-1.2.2/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_vasp_equi.py` & `apex_flow-1.2.2/tests/test_vasp_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_vasp_equi_std.py` & `apex_flow-1.2.2/tests/test_vasp_equi_std.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.1/tests/test_vasp_kspacing.py` & `apex_flow-1.2.2/tests/test_vasp_kspacing.py`

 * *Files identical despite different names*

