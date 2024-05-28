# Comparing `tmp/apex_flow-1.2.2.tar.gz` & `tmp/apex_flow-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apex_flow-1.2.2.tar", last modified: Tue May 28 05:59:45 2024, max compression
+gzip compressed data, was "apex_flow-1.2.3.tar", last modified: Tue May 28 06:41:32 2024, max compression
```

## Comparing `apex_flow-1.2.2.tar` & `apex_flow-1.2.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240867 apex_flow-1.2.2/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.2/LICENSE
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 05:59:45.240630 apex_flow-1.2.2/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-28 05:52:49.000000 apex_flow-1.2.2/README.md
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.223174 apex_flow-1.2.2/apex/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/__main__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.2/apex/archive.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10491 2024-05-09 10:37:35.000000 apex_flow-1.2.2/apex/config.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.225057 apex_flow-1.2.2/apex/core/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/__init__.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.226440 apex_flow-1.2.2/apex/core/calculator/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/ABACUS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/Lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/Task.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.2/apex/core/calculator/VASP.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/calculator.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.227877 apex_flow-1.2.2/apex/core/calculator/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/calculator/lib/abacus_scf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.2/apex/core/calculator/lib/abacus_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/calculator/lib/lammps_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/calculator/lib/vasp_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/common_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/common_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/gen_confs.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.230570 apex_flow-1.2.2/apex/core/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/crys.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/dispatcher.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/lmp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/mfp_eosfit.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/pwscf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/siesta.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/slab_orientation.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/trans_tools.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/lib/util.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/lib/utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/mpdb.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.233090 apex_flow-1.2.2/apex/core/property/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10388 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/EOS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    11809 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    27102 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/Gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    26217 2024-05-28 05:54:53.000000 apex_flow-1.2.2/apex/core/property/Interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    26341 2024-05-27 08:00:15.000000 apex_flow-1.2.2/apex/core/property/Phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/property/Property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10603 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9518 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/core/property/Vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/property/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/core/reproduce.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/core/structure.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.233960 apex_flow-1.2.2/apex/database/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/DatabaseFactory.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/DynamoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/MongoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/StorageBase.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/database/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-05-16 05:37:47.000000 apex_flow-1.2.2/apex/flow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.2/apex/main.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.234627 apex_flow-1.2.2/apex/op/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/op/RunLAMMPS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/op/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/op/property_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/op/relaxation_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2702 2024-05-09 12:22:10.000000 apex_flow-1.2.2/apex/report.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.235565 apex_flow-1.2.2/apex/reporter/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13857 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/reporter/DashReportApp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/reporter/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/reporter/property_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/reporter/relaxation_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.2/apex/step.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/submit.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.236119 apex_flow-1.2.2/apex/superop/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/superop/RelaxationFlow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-05-28 05:52:49.000000 apex_flow-1.2.2/apex/superop/SimplePropertySteps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/apex/superop/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.2/apex/utils.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240319 apex_flow-1.2.2/apex_flow.egg-info/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/entry_points.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/requires.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-28 05:59:45.000000 apex_flow-1.2.2/apex_flow.egg-info/top_level.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-28 05:59:45.240906 apex_flow-1.2.2/setup.cfg
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-05-28 05:52:49.000000 apex_flow-1.2.2/setup.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 05:59:45.240126 apex_flow-1.2.2/tests/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/context.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_abacus_property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_eos.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_make_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_mpdb.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_equi_std.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.2/tests/test_vasp_kspacing.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.419785 apex_flow-1.2.3/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.3/LICENSE
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 06:41:32.419422 apex_flow-1.2.3/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-28 05:52:49.000000 apex_flow-1.2.3/README.md
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.367219 apex_flow-1.2.3/apex/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-05-28 06:34:09.000000 apex_flow-1.2.3/apex/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/__main__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.3/apex/archive.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10491 2024-05-09 10:37:35.000000 apex_flow-1.2.3/apex/config.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.369530 apex_flow-1.2.3/apex/core/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/__init__.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.371655 apex_flow-1.2.3/apex/core/calculator/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/calculator/ABACUS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/calculator/Lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/calculator/Task.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.3/apex/core/calculator/VASP.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/calculator/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/calculator/calculator.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.374071 apex_flow-1.2.3/apex/core/calculator/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/calculator/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/calculator/lib/abacus_scf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.3/apex/core/calculator/lib/abacus_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/calculator/lib/lammps_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/calculator/lib/vasp_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/common_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/common_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/gen_confs.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.377827 apex_flow-1.2.3/apex/core/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/lib/crys.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/lib/dispatcher.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/lmp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/mfp_eosfit.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/pwscf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/siesta.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/slab_orientation.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/trans_tools.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/lib/util.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/lib/utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/mpdb.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.385475 apex_flow-1.2.3/apex/core/property/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10388 2024-05-27 08:00:15.000000 apex_flow-1.2.3/apex/core/property/EOS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    11809 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/property/Elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    27102 2024-05-27 08:00:15.000000 apex_flow-1.2.3/apex/core/property/Gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    25843 2024-05-28 06:31:24.000000 apex_flow-1.2.3/apex/core/property/Interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    26341 2024-05-27 08:00:15.000000 apex_flow-1.2.3/apex/core/property/Phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/property/Property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10603 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/property/Surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9518 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/core/property/Vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/property/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/core/reproduce.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/core/structure.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.394815 apex_flow-1.2.3/apex/database/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/database/DatabaseFactory.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/database/DynamoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/database/MongoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/database/StorageBase.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/database/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-05-16 05:37:47.000000 apex_flow-1.2.3/apex/flow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.3/apex/main.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.399965 apex_flow-1.2.3/apex/op/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/op/RunLAMMPS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/op/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/op/property_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/op/relaxation_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2702 2024-05-09 12:22:10.000000 apex_flow-1.2.3/apex/report.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.407406 apex_flow-1.2.3/apex/reporter/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13857 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/reporter/DashReportApp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/reporter/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/reporter/property_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/reporter/relaxation_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.3/apex/step.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/submit.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.412626 apex_flow-1.2.3/apex/superop/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/superop/RelaxationFlow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-05-28 05:52:49.000000 apex_flow-1.2.3/apex/superop/SimplePropertySteps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/apex/superop/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.3/apex/utils.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.418929 apex_flow-1.2.3/apex_flow.egg-info/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/entry_points.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/requires.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-28 06:41:32.000000 apex_flow-1.2.3/apex_flow.egg-info/top_level.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-28 06:41:32.419846 apex_flow-1.2.3/setup.cfg
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-05-28 06:34:09.000000 apex_flow-1.2.3/setup.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-28 06:41:32.418600 apex_flow-1.2.3/tests/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/context.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_abacus.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_abacus_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_abacus_property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_eos.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-05-28 06:32:03.000000 apex_flow-1.2.3/tests/test_interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_make_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_mpdb.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_vasp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_vasp_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_vasp_equi_std.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.3/tests/test_vasp_kspacing.py
```

### Comparing `apex_flow-1.2.2/LICENSE` & `apex_flow-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/PKG-INFO` & `apex_flow-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.2/README.md` & `apex_flow-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/__init__.py` & `apex_flow-1.2.3/apex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-__version__ = '1.2.2'
+__version__ = '1.2.3'
 LOCAL_PATH = os.getcwd()
 
 
 def header():
     header_str = ""
     header_str += "---------------------------------------------------------------\n"
     header_str += "░░░░░░█▐▓▓░████▄▄▄█▀▄▓▓▓▌█░░░░░░░░░░█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█░░░░░\n"
```

### Comparing `apex_flow-1.2.2/apex/archive.py` & `apex_flow-1.2.3/apex/archive.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/config.py` & `apex_flow-1.2.3/apex/config.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/ABACUS.py` & `apex_flow-1.2.3/apex/core/calculator/ABACUS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/Lammps.py` & `apex_flow-1.2.3/apex/core/calculator/Lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/Task.py` & `apex_flow-1.2.3/apex/core/calculator/Task.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/VASP.py` & `apex_flow-1.2.3/apex/core/calculator/VASP.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/calculator.py` & `apex_flow-1.2.3/apex/core/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/lib/abacus_scf.py` & `apex_flow-1.2.3/apex/core/calculator/lib/abacus_scf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/lib/abacus_utils.py` & `apex_flow-1.2.3/apex/core/calculator/lib/abacus_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/lib/lammps_utils.py` & `apex_flow-1.2.3/apex/core/calculator/lib/lammps_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/calculator/lib/vasp_utils.py` & `apex_flow-1.2.3/apex/core/calculator/lib/vasp_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/common_equi.py` & `apex_flow-1.2.3/apex/core/common_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/common_prop.py` & `apex_flow-1.2.3/apex/core/common_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/gen_confs.py` & `apex_flow-1.2.3/apex/core/gen_confs.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/crys.py` & `apex_flow-1.2.3/apex/core/lib/crys.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/dispatcher.py` & `apex_flow-1.2.3/apex/core/lib/dispatcher.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/lmp.py` & `apex_flow-1.2.3/apex/core/lib/lmp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/mfp_eosfit.py` & `apex_flow-1.2.3/apex/core/lib/mfp_eosfit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/pwscf.py` & `apex_flow-1.2.3/apex/core/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/siesta.py` & `apex_flow-1.2.3/apex/core/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/slab_orientation.py` & `apex_flow-1.2.3/apex/core/lib/slab_orientation.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/trans_tools.py` & `apex_flow-1.2.3/apex/core/lib/trans_tools.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/util.py` & `apex_flow-1.2.3/apex/core/lib/util.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/lib/utils.py` & `apex_flow-1.2.3/apex/core/lib/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/mpdb.py` & `apex_flow-1.2.3/apex/core/mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/EOS.py` & `apex_flow-1.2.3/apex/core/property/EOS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Elastic.py` & `apex_flow-1.2.3/apex/core/property/Elastic.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Gamma.py` & `apex_flow-1.2.3/apex/core/property/Gamma.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Interstitial.py` & `apex_flow-1.2.3/apex/core/property/Interstitial.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,30 +439,18 @@
                 )
             with open("POSCAR", "w+") as fout:
                 for ii in new_pos_line:
                     print(ii, file=fout)
             logging.info(f"gen {type_str}")
             os.chdir(cwd)
 
-        total_task = len(self.dss) + len(interstitial_dict)
+        total_task = len(self.dss) + len(interstitial_dict) - 1
 
         return total_task
 
-    def _rotate_hcp(self, poscar):
-        ss = Structure.from_file(poscar)
-        theta = np.pi / 3
-        rot_m = np.array([
-            [np.cos(theta), -np.sin(theta), 0],
-            [np.sin(theta), np.cos(theta), 0],
-            [0, 0, 1]
-        ])
-        op = SymmOp.from_rotation_and_translation(rot_m)
-        ss.apply_operation(op)
-        ss.to(poscar, "POSCAR")
-
 
     def post_process(self, task_list):
         if True:
             fin1 = open(os.path.join(task_list[0], "..", "element.out"), "r")
             for ii in task_list:
                 conf = os.path.join(ii, "conf.lmp")
                 inter = os.path.join(ii, "inter.json")
```

### Comparing `apex_flow-1.2.2/apex/core/property/Phonon.py` & `apex_flow-1.2.3/apex/core/property/Phonon.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Property.py` & `apex_flow-1.2.3/apex/core/property/Property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Surface.py` & `apex_flow-1.2.3/apex/core/property/Surface.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/property/Vacancy.py` & `apex_flow-1.2.3/apex/core/property/Vacancy.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/refine.py` & `apex_flow-1.2.3/apex/core/refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/reproduce.py` & `apex_flow-1.2.3/apex/core/reproduce.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/core/structure.py` & `apex_flow-1.2.3/apex/core/structure.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/database/DynamoDB.py` & `apex_flow-1.2.3/apex/database/DynamoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/database/MongoDB.py` & `apex_flow-1.2.3/apex/database/MongoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/database/StorageBase.py` & `apex_flow-1.2.3/apex/database/StorageBase.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/flow.py` & `apex_flow-1.2.3/apex/flow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/main.py` & `apex_flow-1.2.3/apex/main.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/op/RunLAMMPS.py` & `apex_flow-1.2.3/apex/op/RunLAMMPS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/op/property_ops.py` & `apex_flow-1.2.3/apex/op/property_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/op/relaxation_ops.py` & `apex_flow-1.2.3/apex/op/relaxation_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/report.py` & `apex_flow-1.2.3/apex/report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/reporter/DashReportApp.py` & `apex_flow-1.2.3/apex/reporter/DashReportApp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/reporter/property_report.py` & `apex_flow-1.2.3/apex/reporter/property_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/reporter/relaxation_report.py` & `apex_flow-1.2.3/apex/reporter/relaxation_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/step.py` & `apex_flow-1.2.3/apex/step.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/submit.py` & `apex_flow-1.2.3/apex/submit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/superop/RelaxationFlow.py` & `apex_flow-1.2.3/apex/superop/RelaxationFlow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/superop/SimplePropertySteps.py` & `apex_flow-1.2.3/apex/superop/SimplePropertySteps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex/utils.py` & `apex_flow-1.2.3/apex/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/apex_flow.egg-info/PKG-INFO` & `apex_flow-1.2.3/apex_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.2/apex_flow.egg-info/SOURCES.txt` & `apex_flow-1.2.3/apex_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/setup.py` & `apex_flow-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apex-flow",
-    version="1.2.2",
+    version="1.2.3",
     author="Zhuoyuan Li, Tongqi Wen",
     author_email="zhuoyli@outlook.com",
     description="Alloy Properties EXplorer using simulations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/APEX.git",
     packages=setuptools.find_packages(),
```

### Comparing `apex_flow-1.2.2/tests/context.py` & `apex_flow-1.2.3/tests/context.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_abacus.py` & `apex_flow-1.2.3/tests/test_abacus.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_abacus_equi.py` & `apex_flow-1.2.3/tests/test_abacus_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_abacus_property.py` & `apex_flow-1.2.3/tests/test_abacus_property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_elastic.py` & `apex_flow-1.2.3/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_eos.py` & `apex_flow-1.2.3/tests/test_eos.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_gamma.py` & `apex_flow-1.2.3/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_interstitial.py` & `apex_flow-1.2.3/tests/test_interstitial.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 self.interstitial.make_confs(self.target_path, self.equi_path)
         shutil.copy(
             os.path.join(self.source_path, "CONTCAR_V_bcc"),
             os.path.join(self.equi_path, "CONTCAR"),
         )
         task_list = self.interstitial.make_confs(self.target_path, self.equi_path)
         dfm_dirs = glob.glob(os.path.join(self.target_path, "task.00000[1-9]"))
-        self.assertEqual(len(dfm_dirs), 6)
+        self.assertEqual(len(dfm_dirs), 5)
 
         incar0 = Incar.from_file(os.path.join("vasp_input", "INCAR.rlx"))
         incar0["ISIF"] = 3
 
         self.assertEqual(
             os.path.realpath(os.path.join(self.equi_path, "CONTCAR")),
             os.path.realpath(os.path.join(self.target_path, "POSCAR")),
```

### Comparing `apex_flow-1.2.2/tests/test_lammps.py` & `apex_flow-1.2.3/tests/test_lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_make_prop.py` & `apex_flow-1.2.3/tests/test_make_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_mpdb.py` & `apex_flow-1.2.3/tests/test_mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_ops.py` & `apex_flow-1.2.3/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_phonon.py` & `apex_flow-1.2.3/tests/test_phonon.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_refine.py` & `apex_flow-1.2.3/tests/test_refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_surface.py` & `apex_flow-1.2.3/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_vacancy.py` & `apex_flow-1.2.3/tests/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_vasp.py` & `apex_flow-1.2.3/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_vasp_equi.py` & `apex_flow-1.2.3/tests/test_vasp_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_vasp_equi_std.py` & `apex_flow-1.2.3/tests/test_vasp_equi_std.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.2/tests/test_vasp_kspacing.py` & `apex_flow-1.2.3/tests/test_vasp_kspacing.py`

 * *Files identical despite different names*

