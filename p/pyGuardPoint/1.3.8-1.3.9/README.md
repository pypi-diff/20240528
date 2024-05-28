# Comparing `tmp/pyGuardPoint-1.3.8.tar.gz` & `tmp/pyguardpoint-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-1.3.8.tar", last modified: Fri Nov 24 13:02:10 2023, max compression
+gzip compressed data, was "pyguardpoint-1.3.9.tar", last modified: Tue May 28 15:02:25 2024, max compression
```

## Comparing `pyGuardPoint-1.3.8.tar` & `pyguardpoint-1.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-11-24 13:02:10.226607 pyGuardPoint-1.3.8/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0     6252 2023-11-24 13:02:10.226607 pyGuardPoint-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-1.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-11-24 13:02:10.202608 pyGuardPoint-1.3.8/pyGuardPoint/
--rw-rw-rw-   0        0        0     8851 2023-11-05 09:13:32.000000 pyGuardPoint-1.3.8/pyGuardPoint/CustomWebsocketTransport.py
--rw-rw-rw-   0        0        0      347 2023-11-06 12:09:16.000000 pyGuardPoint-1.3.8/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11788 2023-10-10 09:50:05.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1376 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     7017 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     2496 2023-10-19 10:27:29.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_controllers.py
--rw-rw-rw-   0        0        0     1338 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1914 2023-10-18 12:02:05.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_diagnostic.py
--rw-rw-rw-   0        0        0     3964 2023-11-06 11:57:57.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_ouputs.py
--rw-rw-rw-   0        0        0     1363 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2359 2023-10-18 11:52:44.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_readers.py
--rw-rw-rw-   0        0        0     2832 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1561 2023-09-13 16:34:08.000000 pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-1.3.8/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1612 2023-11-05 12:58:49.000000 pyGuardPoint-1.3.8/pyGuardPoint/_str_match_algo.py
-drwxrwxrwx   0        0        0        0 2023-11-24 13:02:10.224652 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/
--rw-rw-rw-   0        0        0        0 2023-11-16 11:53:30.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/__init__.py
--rw-rw-rw-   0        0        0     1301 2023-11-16 11:02:01.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11934 2023-11-20 12:14:25.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1391 2023-11-16 11:06:50.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     7093 2023-11-16 11:06:50.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
--rw-rw-rw-   0        0        0     2597 2023-11-24 13:01:26.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
--rw-rw-rw-   0        0        0     1353 2023-11-16 11:16:06.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1927 2023-11-16 11:16:06.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
--rw-rw-rw-   0        0        0     3968 2023-11-16 11:37:00.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
--rw-rw-rw-   0        0        0     1378 2023-11-16 11:16:06.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2386 2023-11-16 11:16:06.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
--rw-rw-rw-   0        0        0     2832 2023-11-16 12:10:19.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1561 2023-11-16 12:10:19.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0    13143 2023-11-23 16:26:27.000000 pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
--rw-rw-rw-   0        0        0     5111 2023-11-08 14:21:12.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4839 2023-11-23 16:26:27.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_asyncio.py
--rw-rw-rw-   0        0        0    11578 2023-11-08 14:15:50.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    21613 2023-10-19 10:17:43.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0      105 2023-08-04 12:11:20.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     4071 2023-11-06 11:15:54.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_threaded.py
--rw-rw-rw-   0        0        0     4364 2023-11-05 12:58:49.000000 pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-11-24 13:02:10.225633 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-11-24 13:02:10.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-11-24 13:02:10.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-24 13:02:10.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2023-11-24 13:02:10.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-24 13:02:10.000000 pyGuardPoint-1.3.8/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-24 13:02:10.226607 pyGuardPoint-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-11-24 13:01:26.000000 pyGuardPoint-1.3.8/setup.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.141089 pyguardpoint-1.3.9/
+-rw-r--r--   0 johnowen   (501) staff       (20)    11357 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/LICENSE.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)     8038 2024-05-28 15:02:25.140885 pyguardpoint-1.3.9/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)     7658 2024-05-28 14:59:56.000000 pyguardpoint-1.3.9/README.rst
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.137862 pyguardpoint-1.3.9/pyGuardPoint/
+-rw-r--r--   0 johnowen   (501) staff       (20)     8613 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/CustomWebsocketTransport.py
+-rw-r--r--   0 johnowen   (501) staff       (20)      342 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1251 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11501 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1340 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     6824 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2429 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1302 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1860 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3857 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1328 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2292 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5432 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_odata_filter.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1566 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_str_match_algo.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.140480 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/
+-rw-r--r--   0 johnowen   (501) staff       (20)        0 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1266 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11647 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1355 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     6900 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2527 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1317 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1873 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3862 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1343 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2319 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    12795 2024-05-28 14:49:38.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4984 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4733 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11293 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_connection.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    20954 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_dataclasses.py
+-rw-r--r--   0 johnowen   (501) staff       (20)       97 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_error.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3982 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_threaded.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4245 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_utils.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.140677 pyguardpoint-1.3.9/pyGuardPoint.egg-info/
+-rw-r--r--   0 johnowen   (501) staff       (20)     8038 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)     1863 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/SOURCES.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/dependency_links.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/not-zip-safe
+-rw-r--r--   0 johnowen   (501) staff       (20)       56 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/requires.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       13 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/top_level.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       38 2024-05-28 15:02:25.141128 pyguardpoint-1.3.9/setup.cfg
+-rw-r--r--   0 johnowen   (501) staff       (20)      610 2024-05-28 14:36:57.000000 pyguardpoint-1.3.9/setup.py
```

### Comparing `pyGuardPoint-1.3.8/LICENSE.txt` & `pyguardpoint-1.3.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `pyGuardPoint-1.3.8/PKG-INFO` & `pyguardpoint-1.3.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,189 @@
-Metadata-Version: 2.1
-Name: pyGuardPoint
-Version: 1.3.8
-Summary: Python wrapper for GuardPoint 10 Access Control System
-Author: John Owen
-Maintainer-email: sales@sensoraccess.co.uk
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: validators
-Requires-Dist: fuzzywuzzy
-Requires-Dist: cryptography
-Requires-Dist: pysignalr
-Requires-Dist: websockets
-
-pyGuardPoint
-===============
-
-pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
-
-pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
-GuardPoint 10 controls and monitors doors,lifts,readers etc. pyGuardPoint currently focuses more on the management of Cardholders over the monitoring and setup of the physical infrastructure.
-
-At the time of writing the current version of GuardPoint 10 is Version 1.90.3.
-Learn more about the GuardPoint 10 ACS here https://www.sensoraccess.co.uk/guardpoint10/
-
-pyGuardPoint is not compatible with the legacy ACS GuardPoint Pro.
-
-What is it good for?
-------------------
-Rapid development of applications and scripts using the GuardPoint ACS.
-pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
-The Python object Cardholder represents a user/person on the system.
-Modify your Cardholder's attributes and update them with just a couple of lines of code.
-
-Examples
-------------------
-Firstly you will always need to import the module:
-
-    from pyGuardPoint import GuardPoint, Cardholder, Card
-
-It is recommended to use a mutually authenticated secure connection to the GuardPoint server in production environments.
-
-To establish a secure connection with a PKCS#12(*.p12) credential file:
-
-    gp = GuardPoint(host="https://sensoraccess.duckdns.org", pwd="admin",
-                        p12_file="MobileGuardDefault.p12",
-                        p12_pwd="test")
-
-To retrieve a list of cardholders:
-
-    gp = GuardPoint(host="10.0.0.1", pwd="password")
-    cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
-    for cardholder in cardholders:
-        print(cardholder.lastName)
-
-To create a new cardholder:
-
-    gp = GuardPoint(host="10.0.0.1", pwd="password")
-    cardholder_pd = CardholderPersonalDetail(email="jeff.buckley@test.com")
-    cardholder = Cardholder(firstName="Jeff", lastName="Buckley",
-                            cardholderPersonalDetail=cardholder_pd)
-    cardholder = gp.new_card_holder(cardholder)
-
-To create a card for the cardholder - A card can represent an assortment of Identity tokens(magnetic-card, smartcard, QRCode , vehicle number plate etc) - as long as it contains a unique card-code:
-
-    from pyGuardPoint import GuardPoint, Card
-
-    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
-
-    cardholders = gp.get_card_holders(firstName="Jeff", lastName="Buckley")
-    if len(cardholders) < 1:
-        exit()
-
-    card = Card(cardType="Magnetic", cardCode="1A1B1123")
-    cardholders[0].cards.append(card)
-    if gp.update_card_holder(cardholders[0]):
-        updated_cardholder = gp.get_card_holder(uid=cardholders[0].uid)
-        print(f"Cardholder {updated_cardholder.firstName} {updated_cardholder.lastName} Updated")
-        print(f"\tEmail: {updated_cardholder.cardholderPersonalDetail.email}")
-        print(f"\tCards: {updated_cardholder.cards}")
-
-The get_card_holders method can be used with a whole host of flags for filtering:
-
-    cardholders = gp.get_card_holders(search_terms="Frank Smith Countermac",
-                                          cardholder_type_name='Visitor',
-                                          filter_expired=True,
-                                          select_ignore_list=['cardholderCustomizedField',
-                                                              'cardholderPersonalDetail',
-                                                              'securityGroup',
-                                                              'cards',
-                                                              'photo'],
-                                          select_include_list=['uid', 'lastName', 'firstName', 'lastPassDate',
-                                                               'insideArea', 'fromDateTime'],
-                                          sort_algorithm=SortAlgorithm.FUZZY_MATCH,
-                                          threshold=10)
-
-The class Cardholder has a couple of convenience functions:
-
-    cardholder.dict(non_empty_only=True)) # Convert to python dictionary
-    cardholder.pretty_print()   # Print nicely in the terminal window
-
-To get a list of areas/zones, and count the number of cardholders in each:
-
-    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
-
-    areas = gp.get_areas()
-
-    areas = gp.get_areas()
-    for area in areas:
-        cardholder_count = gp.get_card_holders(count=True, areas=area)
-        print(f"Cardholders in {area.name} = {str(cardholder_count)}")
-
-To get a list of security groups:
-
-    sec_groups = gp.get_security_groups()
-    for sec_group in sec_groups:
-        print(sec_group)
-
-Scheduling the membership of an Access Group to a Cardholder:
-
-    # Get a cardholder
-    cardholder = gp.get_card_holder(card_code='1B1A1B1C')
-
-    # Add and associate schedule access group to cardholder
-    fromDateValid = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
-    toDateValid = (datetime.now() + timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M:%SZ')
-    sm = ScheduledMag(scheduledSecurityGroupUID=sec_groups[0].uid,
-                      cardholderUID=cardholder.uid,
-                      fromDateValid=fromDateValid,
-                      toDateValid=toDateValid)
-    gp.add_scheduled_mag(sm)
-
-    scheduled_mags = gp.get_scheduled_mags()
-    for scheduled_mag in scheduled_mags:
-        print(scheduled_mag)
-
-More
-------------------
-
-The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
+Metadata-Version: 2.1
+Name: pyGuardPoint
+Version: 1.3.9
+Summary: Python wrapper for GuardPoint 10 Access Control System
+Author: John Owen
+Maintainer-email: sales@sensoraccess.co.uk
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: validators
+Requires-Dist: fuzzywuzzy
+Requires-Dist: cryptography
+Requires-Dist: pysignalr
+Requires-Dist: websockets
+
+pyGuardPoint
+===============
+
+pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
+
+pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
+GuardPoint 10 controls and monitors doors,lifts,readers etc. pyGuardPoint currently focuses more on the management of Cardholders over the monitoring and setup of the physical infrastructure.
+
+At the time of writing the current version of GuardPoint 10 is Version 1.90.3.
+Learn more about the GuardPoint 10 ACS here https://www.sensoraccess.co.uk/guardpoint10/
+
+pyGuardPoint is not compatible with the legacy ACS GuardPoint Pro.
+
+What is it good for?
+------------------
+Rapid development of applications and scripts using the GuardPoint ACS.
+pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
+The Python object Cardholder represents a user/person on the system.
+Modify your Cardholder's attributes and update them with just a couple of lines of code.
+
+Examples
+------------------
+Firstly you will always need to import the module:
+
+    from pyGuardPoint import GuardPoint, Cardholder, Card
+
+It is recommended to use a mutually authenticated secure connection to the GuardPoint server in production environments.
+
+To establish a secure connection with a PKCS#12(*.p12) credential file:
+
+    gp = GuardPoint(host="https://sensoraccess.duckdns.org", pwd="admin",
+                        p12_file="MobileGuardDefault.p12",
+                        p12_pwd="test")
+
+pyGuardPoint also has built-in support for asynchronous connections, under-the-hood it uses the Python module aiohttp.
+The example below demonstrates settings up a AsyncIO connection:
+
+    from pyGuardPoint import GuardPointAsyncIO
+    gp = GuardPointAsyncIO(host="https://sensoraccess.duckdns.org", pwd="admin",
+                        p12_file="MobileGuardDefault.p12",
+                        p12_pwd="test")
+
+To retrieve a list of cardholders:
+
+    gp = GuardPoint(host="10.0.0.1", pwd="password")
+    cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
+    for cardholder in cardholders:
+        print(cardholder.lastName)
+
+To create a new cardholder:
+
+    gp = GuardPoint(host="10.0.0.1", pwd="password")
+    cardholder_pd = CardholderPersonalDetail(email="jeff.buckley@test.com")
+    cardholder = Cardholder(firstName="Jeff", lastName="Buckley",
+                            cardholderPersonalDetail=cardholder_pd)
+    cardholder = gp.new_card_holder(cardholder)
+
+To create a card for the cardholder - A card can represent an assortment of Identity tokens(magnetic-card, smartcard, QRCode , vehicle number plate etc) - as long as it contains a unique card-code:
+
+    from pyGuardPoint import GuardPoint, Card
+
+    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
+
+    cardholders = gp.get_card_holders(firstName="Jeff", lastName="Buckley")
+    if len(cardholders) < 1:
+        exit()
+
+    card = Card(cardType="Magnetic", cardCode="1A1B1123")
+    cardholders[0].cards.append(card)
+    if gp.update_card_holder(cardholders[0]):
+        updated_cardholder = gp.get_card_holder(uid=cardholders[0].uid)
+        print(f"Cardholder {updated_cardholder.firstName} {updated_cardholder.lastName} Updated")
+        print(f"\tEmail: {updated_cardholder.cardholderPersonalDetail.email}")
+        print(f"\tCards: {updated_cardholder.cards}")
+
+The get_card_holders method can be used with a whole host of flags for filtering:
+
+    cardholders = gp.get_card_holders(search_terms="Frank Smith Countermac",
+                                          cardholder_type_name='Visitor',
+                                          filter_expired=True,
+                                          select_ignore_list=['cardholderCustomizedField',
+                                                              'cardholderPersonalDetail',
+                                                              'securityGroup',
+                                                              'cards',
+                                                              'photo'],
+                                          select_include_list=['uid', 'lastName', 'firstName', 'lastPassDate',
+                                                               'insideArea', 'fromDateTime'],
+                                          sort_algorithm=SortAlgorithm.FUZZY_MATCH,
+                                          threshold=10)
+
+The class Cardholder has a couple of convenience functions:
+
+    cardholder.dict(non_empty_only=True)) # Convert to python dictionary
+    cardholder.pretty_print()   # Print nicely in the terminal window
+
+To get a list of areas/zones, and count the number of cardholders in each:
+
+    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
+
+    areas = gp.get_areas()
+
+    areas = gp.get_areas()
+    for area in areas:
+        cardholder_count = gp.get_card_holders(count=True, areas=area)
+        print(f"Cardholders in {area.name} = {str(cardholder_count)}")
+
+To get a list of security groups:
+
+    sec_groups = gp.get_security_groups()
+    for sec_group in sec_groups:
+        print(sec_group)
+
+Scheduling the membership of an Access Group to a Cardholder:
+
+    # Get a cardholder
+    cardholder = gp.get_card_holder(card_code='1B1A1B1C')
+
+    # Add and associate schedule access group to cardholder
+    fromDateValid = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
+    toDateValid = (datetime.now() + timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M:%SZ')
+    sm = ScheduledMag(scheduledSecurityGroupUID=sec_groups[0].uid,
+                      cardholderUID=cardholder.uid,
+                      fromDateValid=fromDateValid,
+                      toDateValid=toDateValid)
+    gp.add_scheduled_mag(sm)
+
+    scheduled_mags = gp.get_scheduled_mags()
+    for scheduled_mag in scheduled_mags:
+        print(scheduled_mag)
+
+GuardPoint servers can be setup with a Signal-R service enabled.
+Once enabled the server will broadcast events to clients listening to events.
+
+    try:
+        gp = GuardPoint(host=GP_HOST,
+                        username=GP_USER,
+                        pwd=GP_PASS,
+                        p12_file=TLS_P12,
+                        p12_pwd=TLS_P12_PWD)
+
+        signal_client = gp.get_signal_client()
+
+        signal_client.on_open(on_open)
+        signal_client.on_close(on_close)
+        signal_client.on_error(on_error)
+        signal_client.on('AccessEventArrived', on_message)
+        signal_client.on("AlarmEventArrived", on_message)
+        signal_client.on("AuditEventArrived", on_message)
+        signal_client.on("CommEventArrived", on_message)
+        signal_client.on("GeneralEventArrived", on_message)
+        signal_client.on("IOEventArrived", on_message)
+        signal_client.on("StatusUpdate", on_message)
+        signal_client.on("TechnicalEventArrived", on_message)
+
+        async def run_signal_client() -> None:
+            task = asyncio.create_task(signal_client.run(), name = "sigR_task")
+            await task
+
+
+        loop = asyncio.get_event_loop()
+        asyncio.run_coroutine_threadsafe(run_signal_client(), loop)
+
+        gp.start_listening(signal_client)
+
+    except GuardPointError as e:
+        print(f"GuardPointError: {e}")
+    except AuthorizationError as e:
+        print(f"SignalR AuthorizationError")
+    except Exception as e:
+        print(f"Exception: {str(e)}")
+
+More
+------------------
+
+The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
```

### Comparing `pyGuardPoint-1.3.8/README.rst` & `pyguardpoint-1.3.9/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,189 @@
-pyGuardPoint
-===============
-
-pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
-
-pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
-GuardPoint 10 controls and monitors doors,lifts,readers etc. pyGuardPoint currently focuses more on the management of Cardholders over the monitoring and setup of the physical infrastructure.
-
-At the time of writing the current version of GuardPoint 10 is Version 1.90.3.
-Learn more about the GuardPoint 10 ACS here https://www.sensoraccess.co.uk/guardpoint10/
-
-pyGuardPoint is not compatible with the legacy ACS GuardPoint Pro.
-
-What is it good for?
-------------------
-Rapid development of applications and scripts using the GuardPoint ACS.
-pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
-The Python object Cardholder represents a user/person on the system.
-Modify your Cardholder's attributes and update them with just a couple of lines of code.
-
-Examples
-------------------
-Firstly you will always need to import the module:
-
-    from pyGuardPoint import GuardPoint, Cardholder, Card
-
-It is recommended to use a mutually authenticated secure connection to the GuardPoint server in production environments.
-
-To establish a secure connection with a PKCS#12(*.p12) credential file:
-
-    gp = GuardPoint(host="https://sensoraccess.duckdns.org", pwd="admin",
-                        p12_file="MobileGuardDefault.p12",
-                        p12_pwd="test")
-
-To retrieve a list of cardholders:
-
-    gp = GuardPoint(host="10.0.0.1", pwd="password")
-    cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
-    for cardholder in cardholders:
-        print(cardholder.lastName)
-
-To create a new cardholder:
-
-    gp = GuardPoint(host="10.0.0.1", pwd="password")
-    cardholder_pd = CardholderPersonalDetail(email="jeff.buckley@test.com")
-    cardholder = Cardholder(firstName="Jeff", lastName="Buckley",
-                            cardholderPersonalDetail=cardholder_pd)
-    cardholder = gp.new_card_holder(cardholder)
-
-To create a card for the cardholder - A card can represent an assortment of Identity tokens(magnetic-card, smartcard, QRCode , vehicle number plate etc) - as long as it contains a unique card-code:
-
-    from pyGuardPoint import GuardPoint, Card
-
-    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
-
-    cardholders = gp.get_card_holders(firstName="Jeff", lastName="Buckley")
-    if len(cardholders) < 1:
-        exit()
-
-    card = Card(cardType="Magnetic", cardCode="1A1B1123")
-    cardholders[0].cards.append(card)
-    if gp.update_card_holder(cardholders[0]):
-        updated_cardholder = gp.get_card_holder(uid=cardholders[0].uid)
-        print(f"Cardholder {updated_cardholder.firstName} {updated_cardholder.lastName} Updated")
-        print(f"\tEmail: {updated_cardholder.cardholderPersonalDetail.email}")
-        print(f"\tCards: {updated_cardholder.cards}")
-
-The get_card_holders method can be used with a whole host of flags for filtering:
-
-    cardholders = gp.get_card_holders(search_terms="Frank Smith Countermac",
-                                          cardholder_type_name='Visitor',
-                                          filter_expired=True,
-                                          select_ignore_list=['cardholderCustomizedField',
-                                                              'cardholderPersonalDetail',
-                                                              'securityGroup',
-                                                              'cards',
-                                                              'photo'],
-                                          select_include_list=['uid', 'lastName', 'firstName', 'lastPassDate',
-                                                               'insideArea', 'fromDateTime'],
-                                          sort_algorithm=SortAlgorithm.FUZZY_MATCH,
-                                          threshold=10)
-
-The class Cardholder has a couple of convenience functions:
-
-    cardholder.dict(non_empty_only=True)) # Convert to python dictionary
-    cardholder.pretty_print()   # Print nicely in the terminal window
-
-To get a list of areas/zones, and count the number of cardholders in each:
-
-    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
-
-    areas = gp.get_areas()
-
-    areas = gp.get_areas()
-    for area in areas:
-        cardholder_count = gp.get_card_holders(count=True, areas=area)
-        print(f"Cardholders in {area.name} = {str(cardholder_count)}")
-
-To get a list of security groups:
-
-    sec_groups = gp.get_security_groups()
-    for sec_group in sec_groups:
-        print(sec_group)
-
-Scheduling the membership of an Access Group to a Cardholder:
-
-    # Get a cardholder
-    cardholder = gp.get_card_holder(card_code='1B1A1B1C')
-
-    # Add and associate schedule access group to cardholder
-    fromDateValid = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
-    toDateValid = (datetime.now() + timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M:%SZ')
-    sm = ScheduledMag(scheduledSecurityGroupUID=sec_groups[0].uid,
-                      cardholderUID=cardholder.uid,
-                      fromDateValid=fromDateValid,
-                      toDateValid=toDateValid)
-    gp.add_scheduled_mag(sm)
-
-    scheduled_mags = gp.get_scheduled_mags()
-    for scheduled_mag in scheduled_mags:
-        print(scheduled_mag)
-
-More
-------------------
-
-The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
+Metadata-Version: 2.1
+Name: pyGuardPoint
+Version: 1.3.9
+Summary: Python wrapper for GuardPoint 10 Access Control System
+Author: John Owen
+Maintainer-email: sales@sensoraccess.co.uk
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: validators
+Requires-Dist: fuzzywuzzy
+Requires-Dist: cryptography
+Requires-Dist: pysignalr
+Requires-Dist: websockets
+
+pyGuardPoint
+===============
+
+pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
+
+pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
+GuardPoint 10 controls and monitors doors,lifts,readers etc. pyGuardPoint currently focuses more on the management of Cardholders over the monitoring and setup of the physical infrastructure.
+
+At the time of writing the current version of GuardPoint 10 is Version 1.90.3.
+Learn more about the GuardPoint 10 ACS here https://www.sensoraccess.co.uk/guardpoint10/
+
+pyGuardPoint is not compatible with the legacy ACS GuardPoint Pro.
+
+What is it good for?
+------------------
+Rapid development of applications and scripts using the GuardPoint ACS.
+pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
+The Python object Cardholder represents a user/person on the system.
+Modify your Cardholder's attributes and update them with just a couple of lines of code.
+
+Examples
+------------------
+Firstly you will always need to import the module:
+
+    from pyGuardPoint import GuardPoint, Cardholder, Card
+
+It is recommended to use a mutually authenticated secure connection to the GuardPoint server in production environments.
+
+To establish a secure connection with a PKCS#12(*.p12) credential file:
+
+    gp = GuardPoint(host="https://sensoraccess.duckdns.org", pwd="admin",
+                        p12_file="MobileGuardDefault.p12",
+                        p12_pwd="test")
+
+pyGuardPoint also has built-in support for asynchronous connections, under-the-hood it uses the Python module aiohttp.
+The example below demonstrates settings up a AsyncIO connection:
+
+    from pyGuardPoint import GuardPointAsyncIO
+    gp = GuardPointAsyncIO(host="https://sensoraccess.duckdns.org", pwd="admin",
+                        p12_file="MobileGuardDefault.p12",
+                        p12_pwd="test")
+
+To retrieve a list of cardholders:
+
+    gp = GuardPoint(host="10.0.0.1", pwd="password")
+    cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
+    for cardholder in cardholders:
+        print(cardholder.lastName)
+
+To create a new cardholder:
+
+    gp = GuardPoint(host="10.0.0.1", pwd="password")
+    cardholder_pd = CardholderPersonalDetail(email="jeff.buckley@test.com")
+    cardholder = Cardholder(firstName="Jeff", lastName="Buckley",
+                            cardholderPersonalDetail=cardholder_pd)
+    cardholder = gp.new_card_holder(cardholder)
+
+To create a card for the cardholder - A card can represent an assortment of Identity tokens(magnetic-card, smartcard, QRCode , vehicle number plate etc) - as long as it contains a unique card-code:
+
+    from pyGuardPoint import GuardPoint, Card
+
+    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
+
+    cardholders = gp.get_card_holders(firstName="Jeff", lastName="Buckley")
+    if len(cardholders) < 1:
+        exit()
+
+    card = Card(cardType="Magnetic", cardCode="1A1B1123")
+    cardholders[0].cards.append(card)
+    if gp.update_card_holder(cardholders[0]):
+        updated_cardholder = gp.get_card_holder(uid=cardholders[0].uid)
+        print(f"Cardholder {updated_cardholder.firstName} {updated_cardholder.lastName} Updated")
+        print(f"\tEmail: {updated_cardholder.cardholderPersonalDetail.email}")
+        print(f"\tCards: {updated_cardholder.cards}")
+
+The get_card_holders method can be used with a whole host of flags for filtering:
+
+    cardholders = gp.get_card_holders(search_terms="Frank Smith Countermac",
+                                          cardholder_type_name='Visitor',
+                                          filter_expired=True,
+                                          select_ignore_list=['cardholderCustomizedField',
+                                                              'cardholderPersonalDetail',
+                                                              'securityGroup',
+                                                              'cards',
+                                                              'photo'],
+                                          select_include_list=['uid', 'lastName', 'firstName', 'lastPassDate',
+                                                               'insideArea', 'fromDateTime'],
+                                          sort_algorithm=SortAlgorithm.FUZZY_MATCH,
+                                          threshold=10)
+
+The class Cardholder has a couple of convenience functions:
+
+    cardholder.dict(non_empty_only=True)) # Convert to python dictionary
+    cardholder.pretty_print()   # Print nicely in the terminal window
+
+To get a list of areas/zones, and count the number of cardholders in each:
+
+    gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
+
+    areas = gp.get_areas()
+
+    areas = gp.get_areas()
+    for area in areas:
+        cardholder_count = gp.get_card_holders(count=True, areas=area)
+        print(f"Cardholders in {area.name} = {str(cardholder_count)}")
+
+To get a list of security groups:
+
+    sec_groups = gp.get_security_groups()
+    for sec_group in sec_groups:
+        print(sec_group)
+
+Scheduling the membership of an Access Group to a Cardholder:
+
+    # Get a cardholder
+    cardholder = gp.get_card_holder(card_code='1B1A1B1C')
+
+    # Add and associate schedule access group to cardholder
+    fromDateValid = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
+    toDateValid = (datetime.now() + timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M:%SZ')
+    sm = ScheduledMag(scheduledSecurityGroupUID=sec_groups[0].uid,
+                      cardholderUID=cardholder.uid,
+                      fromDateValid=fromDateValid,
+                      toDateValid=toDateValid)
+    gp.add_scheduled_mag(sm)
+
+    scheduled_mags = gp.get_scheduled_mags()
+    for scheduled_mag in scheduled_mags:
+        print(scheduled_mag)
+
+GuardPoint servers can be setup with a Signal-R service enabled.
+Once enabled the server will broadcast events to clients listening to events.
+
+    try:
+        gp = GuardPoint(host=GP_HOST,
+                        username=GP_USER,
+                        pwd=GP_PASS,
+                        p12_file=TLS_P12,
+                        p12_pwd=TLS_P12_PWD)
+
+        signal_client = gp.get_signal_client()
+
+        signal_client.on_open(on_open)
+        signal_client.on_close(on_close)
+        signal_client.on_error(on_error)
+        signal_client.on('AccessEventArrived', on_message)
+        signal_client.on("AlarmEventArrived", on_message)
+        signal_client.on("AuditEventArrived", on_message)
+        signal_client.on("CommEventArrived", on_message)
+        signal_client.on("GeneralEventArrived", on_message)
+        signal_client.on("IOEventArrived", on_message)
+        signal_client.on("StatusUpdate", on_message)
+        signal_client.on("TechnicalEventArrived", on_message)
+
+        async def run_signal_client() -> None:
+            task = asyncio.create_task(signal_client.run(), name = "sigR_task")
+            await task
+
+
+        loop = asyncio.get_event_loop()
+        asyncio.run_coroutine_threadsafe(run_signal_client(), loop)
+
+        gp.start_listening(signal_client)
+
+    except GuardPointError as e:
+        print(f"GuardPointError: {e}")
+    except AuthorizationError as e:
+        print(f"SignalR AuthorizationError")
+    except Exception as e:
+        print(f"Exception: {str(e)}")
+
+More
+------------------
+
+The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/CustomWebsocketTransport.py` & `pyguardpoint-1.3.9/pyGuardPoint/CustomWebsocketTransport.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-import asyncio
-import logging
-import ssl
-from contextlib import suppress
-from http import HTTPStatus
-from typing import Awaitable
-from typing import Callable
-from typing import Dict
-from typing import Optional
-from typing import Union
-
-from aiohttp import ClientSession, TCPConnector
-from aiohttp import ClientTimeout
-from aiohttp import ServerConnectionError
-from websockets.client import WebSocketClientProtocol
-from websockets.client import connect
-from websockets.connection import State
-from websockets.exceptions import ConnectionClosed
-
-import pysignalr.exceptions as exceptions
-from pysignalr import NegotiationTimeout
-from pysignalr.messages import CompletionMessage
-from pysignalr.messages import Message
-from pysignalr.messages import PingMessage
-from pysignalr.protocol.abstract import Protocol
-from pysignalr.transport.abstract import ConnectionState
-from pysignalr.transport.abstract import Transport
-from pysignalr.utils import get_connection_url
-from pysignalr.utils import get_negotiate_url
-from pysignalr.utils import replace_scheme
-
-DEFAULT_MAX_SIZE = 2 ** 20  # 1 MB
-DEFAULT_PING_INTERVAL = 10
-DEFAULT_CONNECTION_TIMEOUT = 10
-
-_logger = logging.getLogger('pysignalr.transport')
-_logger.setLevel(logging.DEBUG)
-
-
-class CustomWebsocketTransport(Transport):
-    reconnect = True
-
-    def __init__(
-            self,
-            url: str,
-            ssl_context: ssl.SSLContext,
-            protocol: Protocol,
-            callback: Callable[[Message], Awaitable[None]],
-            headers: Optional[Dict[str, str]] = None,
-            skip_negotiation: bool = False,
-            ping_interval: int = DEFAULT_PING_INTERVAL,
-            connection_timeout: int = DEFAULT_CONNECTION_TIMEOUT,
-            max_size: Optional[int] = DEFAULT_MAX_SIZE,
-    ):
-        super().__init__()
-        self._url = url
-        self._ssl_context = ssl_context
-        self._protocol = protocol
-        self._callback = callback
-        self._headers = headers or {}
-        self._skip_negotiation = skip_negotiation
-        self._ping_interval = ping_interval
-        self._connection_timeout = connection_timeout
-        self._max_size = max_size
-
-        self._state = ConnectionState.disconnected
-        self._connected = asyncio.Event()
-        self._ws: Optional[WebSocketClientProtocol] = None
-        self._open_callback: Optional[Callable[[], Awaitable[None]]] = None
-        self._close_callback: Optional[Callable[[], Awaitable[None]]] = None
-
-    async def close(self) -> None:
-        self.reconnect = False
-        if self._ws:
-            try:
-                await self._ws.close()
-            except Exception:
-                pass
-
-    def on_open(self, callback: Callable[[], Awaitable[None]]) -> None:
-        self._open_callback = callback
-
-    def on_close(self, callback: Callable[[], Awaitable[None]]) -> None:
-        self._close_callback = callback
-
-    def on_error(self, callback: Callable[[CompletionMessage], Awaitable[None]]) -> None:
-        self._error_callback = callback
-
-    async def run(self) -> None:
-        self.reconnect = True
-        while True:
-            if not self.reconnect:
-                return
-            with suppress(NegotiationTimeout):
-                await self._loop()
-            await self._set_state(ConnectionState.disconnected)
-
-
-    async def send(self, message: Message) -> None:
-        conn = await self._get_connection()
-        await conn.send(self._protocol.encode(message))
-
-    async def _loop(self) -> None:
-        await self._set_state(ConnectionState.connecting)
-
-        if not self._skip_negotiation:
-            try:
-                await self._negotiate()
-            except ServerConnectionError as e:
-                raise NegotiationTimeout from e
-
-        self.connection_loop = connect(
-            self._url,
-            extra_headers=self._headers,
-            ping_interval=self._ping_interval,
-            open_timeout=self._connection_timeout,
-            max_size=self._max_size,
-            logger=_logger,
-            ssl=self._ssl_context
-        )
-
-        async for conn in self.connection_loop:
-            try:
-                await self._handshake(conn)
-                self._ws = conn
-                await self._set_state(ConnectionState.connected)
-                await asyncio.gather(
-                    self._process(conn),
-                    self._keepalive(conn),
-                )
-
-            except ConnectionClosed as e:
-                _logger.warning('Connection closed: %s', e)
-                self._ws = None
-                if self.reconnect:
-                    await self._set_state(ConnectionState.reconnecting)
-                else:
-                    await self._set_state(ConnectionState.disconnected)
-
-    async def _set_state(self, state: ConnectionState) -> None:
-        if state == self._state:
-            return
-
-        _logger.info('State change: %s -> %s', self._state.name, state.name)
-
-        if state == ConnectionState.connecting:
-            if self._state != ConnectionState.disconnected:
-                raise RuntimeError('Cannot connect while not disconnected')
-
-            self._connected.clear()
-
-        elif state == ConnectionState.connected:
-            if self._state not in (ConnectionState.connecting, ConnectionState.reconnecting):
-                raise RuntimeError('Cannot connect while not connecting or reconnecting')
-
-            self._connected.set()
-
-            if self._open_callback:
-                await self._open_callback()
-
-        elif state in (ConnectionState.reconnecting, ConnectionState.disconnected):
-            self._connected.clear()
-
-            if self._close_callback:
-                await self._close_callback()
-
-        else:
-            raise NotImplementedError
-
-        self._state = state
-
-    async def _get_connection(self) -> WebSocketClientProtocol:
-        await self._connected.wait()
-        if not self._ws or self._ws.state != State.OPEN:
-            raise RuntimeError('Connection is closed')
-        return self._ws
-
-    async def _process(self, conn: WebSocketClientProtocol) -> None:
-        while True:
-            raw_message = await conn.recv()
-            await self._on_raw_message(raw_message)
-
-    async def _keepalive(self, conn: WebSocketClientProtocol) -> None:
-        while True:
-            await asyncio.sleep(10)
-            await conn.send(self._protocol.encode(PingMessage()))
-
-    async def _handshake(self, conn: WebSocketClientProtocol) -> None:
-        _logger.info('Sending handshake to server')
-        our_handshake = self._protocol.handshake_message()
-        await conn.send(self._protocol.encode(our_handshake))
-
-        _logger.info('Awaiting handshake from server')
-        raw_message = await conn.recv()
-        handshake, messages = self._protocol.decode_handshake(raw_message)
-        if handshake.error:
-            raise ValueError(f'Handshake error: {handshake.error}')
-        for message in messages:
-            await self._on_message(message)
-
-    async def _negotiate(self) -> None:
-        negotiate_url = get_negotiate_url(self._url)
-        _logger.info('Performing negotiation, URL: `%s`', negotiate_url)
-
-        conn = TCPConnector(ssl_context=self._ssl_context)
-        session = ClientSession(
-            timeout=ClientTimeout(connect=self._connection_timeout),
-            connector=conn)
-
-        async with session:
-            async with session.post(negotiate_url, headers=self._headers) as response:
-                if response.status == HTTPStatus.OK:
-                    data = await response.json()
-                elif response.status == HTTPStatus.UNAUTHORIZED:
-                    raise exceptions.AuthorizationError
-                else:
-                    raise exceptions.ConnectionError(response.status)
-
-        connection_id = data.get('connectionId')
-        url = data.get('url')
-        access_token = data.get('accessToken')
-
-        if connection_id:
-            _logger.info('Negotiation completed')
-            self._url = get_connection_url(self._url, connection_id)
-        elif url and access_token:
-            _logger.info('Negotiation completed (Azure)')
-            self._url = replace_scheme(url, ws=True)
-            self._headers['Authorization'] = f'Bearer {access_token}'
-        else:
-            raise exceptions.ServerError(str(data))
-
-    async def _on_raw_message(self, raw_message: Union[str, bytes]) -> None:
-        for message in self._protocol.decode(raw_message):
-            await self._on_message(message)
-
-    async def _on_message(self, message: Message) -> None:
-        await self._callback(message)
+import asyncio
+import logging
+import ssl
+from contextlib import suppress
+from http import HTTPStatus
+from typing import Awaitable
+from typing import Callable
+from typing import Dict
+from typing import Optional
+from typing import Union
+
+from aiohttp import ClientSession, TCPConnector
+from aiohttp import ClientTimeout
+from aiohttp import ServerConnectionError
+from websockets.client import WebSocketClientProtocol
+from websockets.client import connect
+from websockets.connection import State
+from websockets.exceptions import ConnectionClosed
+
+import pysignalr.exceptions as exceptions
+from pysignalr import NegotiationTimeout
+from pysignalr.messages import CompletionMessage
+from pysignalr.messages import Message
+from pysignalr.messages import PingMessage
+from pysignalr.protocol.abstract import Protocol
+from pysignalr.transport.abstract import ConnectionState
+from pysignalr.transport.abstract import Transport
+from pysignalr.utils import get_connection_url
+from pysignalr.utils import get_negotiate_url
+from pysignalr.utils import replace_scheme
+
+DEFAULT_MAX_SIZE = 2 ** 20  # 1 MB
+DEFAULT_PING_INTERVAL = 10
+DEFAULT_CONNECTION_TIMEOUT = 10
+
+_logger = logging.getLogger('pysignalr.transport')
+_logger.setLevel(logging.DEBUG)
+
+
+class CustomWebsocketTransport(Transport):
+    reconnect = True
+
+    def __init__(
+            self,
+            url: str,
+            ssl_context: ssl.SSLContext,
+            protocol: Protocol,
+            callback: Callable[[Message], Awaitable[None]],
+            headers: Optional[Dict[str, str]] = None,
+            skip_negotiation: bool = False,
+            ping_interval: int = DEFAULT_PING_INTERVAL,
+            connection_timeout: int = DEFAULT_CONNECTION_TIMEOUT,
+            max_size: Optional[int] = DEFAULT_MAX_SIZE,
+    ):
+        super().__init__()
+        self._url = url
+        self._ssl_context = ssl_context
+        self._protocol = protocol
+        self._callback = callback
+        self._headers = headers or {}
+        self._skip_negotiation = skip_negotiation
+        self._ping_interval = ping_interval
+        self._connection_timeout = connection_timeout
+        self._max_size = max_size
+
+        self._state = ConnectionState.disconnected
+        self._connected = asyncio.Event()
+        self._ws: Optional[WebSocketClientProtocol] = None
+        self._open_callback: Optional[Callable[[], Awaitable[None]]] = None
+        self._close_callback: Optional[Callable[[], Awaitable[None]]] = None
+
+    async def close(self) -> None:
+        self.reconnect = False
+        if self._ws:
+            try:
+                await self._ws.close()
+            except Exception:
+                pass
+
+    def on_open(self, callback: Callable[[], Awaitable[None]]) -> None:
+        self._open_callback = callback
+
+    def on_close(self, callback: Callable[[], Awaitable[None]]) -> None:
+        self._close_callback = callback
+
+    def on_error(self, callback: Callable[[CompletionMessage], Awaitable[None]]) -> None:
+        self._error_callback = callback
+
+    async def run(self) -> None:
+        self.reconnect = True
+        while True:
+            if not self.reconnect:
+                return
+            with suppress(NegotiationTimeout):
+                await self._loop()
+            await self._set_state(ConnectionState.disconnected)
+
+
+    async def send(self, message: Message) -> None:
+        conn = await self._get_connection()
+        await conn.send(self._protocol.encode(message))
+
+    async def _loop(self) -> None:
+        await self._set_state(ConnectionState.connecting)
+
+        if not self._skip_negotiation:
+            try:
+                await self._negotiate()
+            except ServerConnectionError as e:
+                raise NegotiationTimeout from e
+
+        self.connection_loop = connect(
+            self._url,
+            extra_headers=self._headers,
+            ping_interval=self._ping_interval,
+            open_timeout=self._connection_timeout,
+            max_size=self._max_size,
+            logger=_logger,
+            ssl=self._ssl_context
+        )
+
+        async for conn in self.connection_loop:
+            try:
+                await self._handshake(conn)
+                self._ws = conn
+                await self._set_state(ConnectionState.connected)
+                await asyncio.gather(
+                    self._process(conn),
+                    self._keepalive(conn),
+                )
+
+            except ConnectionClosed as e:
+                _logger.warning('Connection closed: %s', e)
+                self._ws = None
+                if self.reconnect:
+                    await self._set_state(ConnectionState.reconnecting)
+                else:
+                    await self._set_state(ConnectionState.disconnected)
+
+    async def _set_state(self, state: ConnectionState) -> None:
+        if state == self._state:
+            return
+
+        _logger.info('State change: %s -> %s', self._state.name, state.name)
+
+        if state == ConnectionState.connecting:
+            if self._state != ConnectionState.disconnected:
+                raise RuntimeError('Cannot connect while not disconnected')
+
+            self._connected.clear()
+
+        elif state == ConnectionState.connected:
+            if self._state not in (ConnectionState.connecting, ConnectionState.reconnecting):
+                raise RuntimeError('Cannot connect while not connecting or reconnecting')
+
+            self._connected.set()
+
+            if self._open_callback:
+                await self._open_callback()
+
+        elif state in (ConnectionState.reconnecting, ConnectionState.disconnected):
+            self._connected.clear()
+
+            if self._close_callback:
+                await self._close_callback()
+
+        else:
+            raise NotImplementedError
+
+        self._state = state
+
+    async def _get_connection(self) -> WebSocketClientProtocol:
+        await self._connected.wait()
+        if not self._ws or self._ws.state != State.OPEN:
+            raise RuntimeError('Connection is closed')
+        return self._ws
+
+    async def _process(self, conn: WebSocketClientProtocol) -> None:
+        while True:
+            raw_message = await conn.recv()
+            await self._on_raw_message(raw_message)
+
+    async def _keepalive(self, conn: WebSocketClientProtocol) -> None:
+        while True:
+            await asyncio.sleep(10)
+            await conn.send(self._protocol.encode(PingMessage()))
+
+    async def _handshake(self, conn: WebSocketClientProtocol) -> None:
+        _logger.info('Sending handshake to server')
+        our_handshake = self._protocol.handshake_message()
+        await conn.send(self._protocol.encode(our_handshake))
+
+        _logger.info('Awaiting handshake from server')
+        raw_message = await conn.recv()
+        handshake, messages = self._protocol.decode_handshake(raw_message)
+        if handshake.error:
+            raise ValueError(f'Handshake error: {handshake.error}')
+        for message in messages:
+            await self._on_message(message)
+
+    async def _negotiate(self) -> None:
+        negotiate_url = get_negotiate_url(self._url)
+        _logger.info('Performing negotiation, URL: `%s`', negotiate_url)
+
+        conn = TCPConnector(ssl_context=self._ssl_context)
+        session = ClientSession(
+            timeout=ClientTimeout(connect=self._connection_timeout),
+            connector=conn)
+
+        async with session:
+            async with session.post(negotiate_url, headers=self._headers) as response:
+                if response.status == HTTPStatus.OK:
+                    data = await response.json()
+                elif response.status == HTTPStatus.UNAUTHORIZED:
+                    raise exceptions.AuthorizationError
+                else:
+                    raise exceptions.ConnectionError(response.status)
+
+        connection_id = data.get('connectionId')
+        url = data.get('url')
+        access_token = data.get('accessToken')
+
+        if connection_id:
+            _logger.info('Negotiation completed')
+            self._url = get_connection_url(self._url, connection_id)
+        elif url and access_token:
+            _logger.info('Negotiation completed (Azure)')
+            self._url = replace_scheme(url, ws=True)
+            self._headers['Authorization'] = f'Bearer {access_token}'
+        else:
+            raise exceptions.ServerError(str(data))
+
+    async def _on_raw_message(self, raw_message: Union[str, bytes]) -> None:
+        for message in self._protocol.decode(raw_message):
+            await self._on_message(message)
+
+    async def _on_message(self, message: Message) -> None:
+        await self._callback(message)
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_areas.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import Area
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class AreasAPI:
-    def get_areas(self):
-        url = "/odata/API_Areas"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        areas = []
-        for x in json_body['value']:
-            areas.append(Area(x))
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import Area
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class AreasAPI:
+    async def get_areas(self):
+        url = "/odata/API_Areas"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        areas = []
+        for x in json_body['value']:
+            areas.append(Area(x))
         return areas
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cardholders.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholders.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-from datetime import datetime
-
-import validators
-from ._odata_filter import _compose_filter, _compose_select, _compose_expand
-from ._str_match_algo import fuzzy_match
-from .guardpoint_dataclasses import Cardholder, SortAlgorithm, Area
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from .guardpoint_utils import GuardPointResponse
-
-
-class CardholdersAPI:
-
-    def delete_card_holder(self, cardholder: Cardholder):
-        if not validators.uuid(cardholder.uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-
-        url = self.baseurl + "/odata/API_Cardholders"
-        url_query_params = "(" + cardholder.uid + ")"
-
-        code, json_body = self.gp_json_query("DELETE", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
-
-    def update_card_holder_area(self, cardholder_uid: str, area: Area):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        if not validators.uuid(area.uid):
-            raise ValueError(f'Malformed Area UID {area.uid}')
-
-        cardholder = Cardholder()
-        cardholder.uid = cardholder_uid
-        cardholder.insideAreaUID = area.uid
-
-        return self.update_card_holder(cardholder)
-
-    def update_card_holder(self, cardholder: Cardholder):
-        if not validators.uuid(cardholder.uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-
-        if cardholder.cardholderCustomizedField:
-            if len(cardholder.cardholderCustomizedField.changed_attributes) > 0:
-                self.update_custom_fields(cardholder.uid, cardholder.cardholderCustomizedField)
-
-        if cardholder.cardholderPersonalDetail:
-            if len(cardholder.cardholderPersonalDetail.changed_attributes) > 0:
-                self.update_personal_details(cardholder.uid, cardholder.cardholderPersonalDetail)
-
-        if cardholder.cards:
-            if isinstance(cardholder.cards, list):
-                for card in cardholder.cards:
-                    if len(card.changed_attributes) > 0:
-                        if validators.uuid(card.uid):
-                            self.update_card(card)
-                        else:
-                            card.cardholderUID = cardholder.uid
-                            self.new_card(card)
-
-        ch = cardholder.dict(editable_only=True, changed_only=True)
-
-        if len(ch) < 1:  # Nothing to update
-            return True
-
-        url = "/odata/API_Cardholders"
-        url_query_params = f"({cardholder.uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
-
-    def new_card_holder(self, cardholder: Cardholder, changed_only=False):
-
-        # url = "/odata/API_Cardholders/CreateFullCardholder"
-        url = "/odata/API_Cardholders"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            'IgnoreNonEditable': ''
-        }
-
-        if changed_only:
-            ch = cardholder.dict(editable_only=True, changed_only=True, non_empty_only=True)
-        else:
-            ch = cardholder.dict(editable_only=True, non_empty_only=True)
-
-
-        # When using CreateFullCardholder
-        # body = {'cardholder': ch}
-        # print(json.dumps(body))
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=ch)
-        # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code == 201:  # HTTP CREATED
-            new_cardholder = Cardholder(json_body)
-            if cardholder.cardholderPersonalDetail:
-                self.update_personal_details(cardholder_uid=new_cardholder.uid,
-                                             personal_details=cardholder.cardholderPersonalDetail)
-            if cardholder.cardholderCustomizedField:
-                self.update_custom_fields(cardholder_uid=new_cardholder.uid,
-                                          customFields=cardholder.cardholderCustomizedField)
-            if cardholder.cards:
-                if isinstance(cardholder.cards, list):
-                    for card in cardholder.cards:
-                        if validators.uuid(card.uid):
-                            self.update_card(card)
-                        else:
-                            card.cardholderUID = new_cardholder.uid
-                            self.new_card(card)
-
-            return self._get_card_holder(new_cardholder.uid)
-
-        elif code == 422:  # unprocessable Entity
-            if "errorMessages" in json_body:
-                raise GuardPointError(
-                    f'{json_body["errorMessages"][0]["message"]}-{json_body["errorMessages"][0]["other"]}')
-        else:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-    def get_card_holder(self,
-                        uid: str = None,
-                        card_code: str = None):
-        if card_code:
-            # Part of the Cards_API
-            return self.get_cardholder_by_card_code(card_code)
-        else:
-            return self._get_card_holder(uid)
-
-    def get_card_holder_photo(self, uid):
-        if not validators.uuid(uid):
-            raise ValueError(f'Malformed UID {uid}')
-
-        url = "/odata/API_Cardholders"
-        url_query_params = "(" + uid + ")?$select=photo"
-
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Photo Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return json_body['value'][0]['photo']
-
-    def _get_card_holder(self, uid):
-        if not validators.uuid(uid):
-            raise ValueError(f'Malformed UID {uid}')
-
-        url = "/odata/API_Cardholders"
-        url_query_params = "(" + uid + ")?" \
-                                       "$expand=" \
-                                       "cardholderType," \
-                                       "cards," \
-                                       "cardholderCustomizedField," \
-                                       "cardholderPersonalDetail," \
-                                       "securityGroup," \
-                                       "insideArea"
-
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code == 404:  # Not Found
-            return None
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return Cardholder(json_body['value'][0])
-
-    def get_card_holders(self, offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None,
-                         filter_expired: bool = False, cardholder_type_name: str = None,
-                         sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75,
-                         count: bool = False, earliest_last_pass: datetime = None,
-                         select_ignore_list: list = None, select_include_list: list = None,
-                         **cardholder_kwargs):
-
-        if offset is None:
-            offset = 0
-
-        # Filter arguments which have to exact match
-        match_args = dict()
-        for k, v in cardholder_kwargs.items():
-            if hasattr(Cardholder, k):
-                match_args[k] = v
-
-        url = "/odata/API_Cardholders"
-
-        filter_str = _compose_filter(search_words=search_terms,
-                                     areas=areas,
-                                     filter_expired=filter_expired,
-                                     cardholder_type_name=cardholder_type_name,
-                                     earliest_last_pass=earliest_last_pass,
-                                     exact_match=match_args)
-
-        select_str = _compose_select(select_ignore_list, select_include_list)
-
-        expand_str = _compose_expand(select_ignore_list, select_include_list)
-
-        url_query_params = ("?" + select_str + expand_str + filter_str)
-
-        if count:
-            url_query_params += "$count=true&$top=0"
-        else:
-            url_query_params += "$orderby=fromDateValid%20desc&"
-            url_query_params += "$top=" + str(limit) + "&$skip=" + str(offset)
-
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholders Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if count:
-            return json_body['@odata.count']
-
-        cardholders = []
-        for x in json_body['value']:
-            cardholders.append(Cardholder(x))
-
-        if sort_algorithm == SortAlgorithm.FUZZY_MATCH:
-            cardholders = fuzzy_match(search_words=search_terms, cardholders=cardholders, threshold=threshold)
-
-        return cardholders
+from datetime import datetime
+
+import validators
+from ._odata_filter import _compose_filter, _compose_select, _compose_expand
+from ._str_match_algo import fuzzy_match
+from .guardpoint_dataclasses import Cardholder, SortAlgorithm, Area
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from .guardpoint_utils import GuardPointResponse
+
+
+class CardholdersAPI:
+
+    def delete_card_holder(self, cardholder: Cardholder):
+        if not validators.uuid(cardholder.uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+
+        url = self.baseurl + "/odata/API_Cardholders"
+        url_query_params = "(" + cardholder.uid + ")"
+
+        code, json_body = self.gp_json_query("DELETE", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        if json_body:
+            GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
+
+    def update_card_holder_area(self, cardholder_uid: str, area: Area):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        if not validators.uuid(area.uid):
+            raise ValueError(f'Malformed Area UID {area.uid}')
+
+        cardholder = Cardholder()
+        cardholder.uid = cardholder_uid
+        cardholder.insideAreaUID = area.uid
+
+        return self.update_card_holder(cardholder)
+
+    def update_card_holder(self, cardholder: Cardholder):
+        if not validators.uuid(cardholder.uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+
+        if cardholder.cardholderCustomizedField:
+            if len(cardholder.cardholderCustomizedField.changed_attributes) > 0:
+                self.update_custom_fields(cardholder.uid, cardholder.cardholderCustomizedField)
+
+        if cardholder.cardholderPersonalDetail:
+            if len(cardholder.cardholderPersonalDetail.changed_attributes) > 0:
+                self.update_personal_details(cardholder.uid, cardholder.cardholderPersonalDetail)
+
+        if cardholder.cards:
+            if isinstance(cardholder.cards, list):
+                for card in cardholder.cards:
+                    if len(card.changed_attributes) > 0:
+                        if validators.uuid(card.uid):
+                            self.update_card(card)
+                        else:
+                            card.cardholderUID = cardholder.uid
+                            self.new_card(card)
+
+        ch = cardholder.dict(editable_only=True, changed_only=True)
+
+        if len(ch) < 1:  # Nothing to update
+            return True
+
+        url = "/odata/API_Cardholders"
+        url_query_params = f"({cardholder.uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
+
+    def new_card_holder(self, cardholder: Cardholder, changed_only=False):
+
+        # url = "/odata/API_Cardholders/CreateFullCardholder"
+        url = "/odata/API_Cardholders"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            'IgnoreNonEditable': ''
+        }
+
+        if changed_only:
+            ch = cardholder.dict(editable_only=True, changed_only=True, non_empty_only=True)
+        else:
+            ch = cardholder.dict(editable_only=True, non_empty_only=True)
+
+
+        # When using CreateFullCardholder
+        # body = {'cardholder': ch}
+        # print(json.dumps(body))
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=ch)
+        # Check response body is formatted correctly
+        if json_body:
+            GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code == 201:  # HTTP CREATED
+            new_cardholder = Cardholder(json_body)
+            if cardholder.cardholderPersonalDetail:
+                self.update_personal_details(cardholder_uid=new_cardholder.uid,
+                                             personal_details=cardholder.cardholderPersonalDetail)
+            if cardholder.cardholderCustomizedField:
+                self.update_custom_fields(cardholder_uid=new_cardholder.uid,
+                                          customFields=cardholder.cardholderCustomizedField)
+            if cardholder.cards:
+                if isinstance(cardholder.cards, list):
+                    for card in cardholder.cards:
+                        if validators.uuid(card.uid):
+                            self.update_card(card)
+                        else:
+                            card.cardholderUID = new_cardholder.uid
+                            self.new_card(card)
+
+            return self._get_card_holder(new_cardholder.uid)
+
+        elif code == 422:  # unprocessable Entity
+            if "errorMessages" in json_body:
+                raise GuardPointError(
+                    f'{json_body["errorMessages"][0]["message"]}-{json_body["errorMessages"][0]["other"]}')
+        else:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+    def get_card_holder(self,
+                        uid: str = None,
+                        card_code: str = None):
+        if card_code:
+            # Part of the Cards_API
+            return self.get_cardholder_by_card_code(card_code)
+        else:
+            return self._get_card_holder(uid)
+
+    def get_card_holder_photo(self, uid):
+        if not validators.uuid(uid):
+            raise ValueError(f'Malformed UID {uid}')
+
+        url = "/odata/API_Cardholders"
+        url_query_params = "(" + uid + ")?$select=photo"
+
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Photo Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return json_body['value'][0]['photo']
+
+    def _get_card_holder(self, uid):
+        if not validators.uuid(uid):
+            raise ValueError(f'Malformed UID {uid}')
+
+        url = "/odata/API_Cardholders"
+        url_query_params = "(" + uid + ")?" \
+                                       "$expand=" \
+                                       "cardholderType," \
+                                       "cards," \
+                                       "cardholderCustomizedField," \
+                                       "cardholderPersonalDetail," \
+                                       "securityGroup," \
+                                       "insideArea"
+
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code == 404:  # Not Found
+            return None
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return Cardholder(json_body['value'][0])
+
+    def get_card_holders(self, offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None,
+                         filter_expired: bool = False, cardholder_type_name: str = None,
+                         sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75,
+                         count: bool = False, earliest_last_pass: datetime = None,
+                         select_ignore_list: list = None, select_include_list: list = None,
+                         **cardholder_kwargs):
+
+        if offset is None:
+            offset = 0
+
+        # Filter arguments which have to exact match
+        match_args = dict()
+        for k, v in cardholder_kwargs.items():
+            if hasattr(Cardholder, k):
+                match_args[k] = v
+
+        url = "/odata/API_Cardholders"
+
+        filter_str = _compose_filter(search_words=search_terms,
+                                     areas=areas,
+                                     filter_expired=filter_expired,
+                                     cardholder_type_name=cardholder_type_name,
+                                     earliest_last_pass=earliest_last_pass,
+                                     exact_match=match_args)
+
+        select_str = _compose_select(select_ignore_list, select_include_list)
+
+        expand_str = _compose_expand(select_ignore_list, select_include_list)
+
+        url_query_params = ("?" + select_str + expand_str + filter_str)
+
+        if count:
+            url_query_params += "$count=true&$top=0"
+        else:
+            url_query_params += "$orderby=fromDateValid%20desc&"
+            url_query_params += "$top=" + str(limit) + "&$skip=" + str(offset)
+
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholders Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if count:
+            return json_body['@odata.count']
+
+        cardholders = []
+        for x in json_body['value']:
+            cardholders.append(Cardholder(x))
+
+        if sort_algorithm == SortAlgorithm.FUZZY_MATCH:
+            cardholders = fuzzy_match(search_words=search_terms, cardholders=cardholders, threshold=threshold)
+
+        return cardholders
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import CardholderType
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class CardholderTypesAPI:
-    def get_cardholder_types(self):
-        url = "/odata/API_CardholderTypes"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"CardholderType Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        cardholder_types = []
-        for x in json_body['value']:
-            cardholder_types.append(CardholderType(x))
-        return cardholder_types
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import CardholderType
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class CardholderTypesAPI:
+    def get_cardholder_types(self):
+        url = "/odata/API_CardholderTypes"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"CardholderType Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        cardholder_types = []
+        for x in json_body['value']:
+            cardholder_types.append(CardholderType(x))
+        return cardholder_types
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_cards.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from ._odata_filter import _compose_filter
-from .guardpoint_dataclasses import Card, Cardholder
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class CardsAPI:
-    def get_cards(self, count=False, **card_kwargs):
-        # Filter arguments which have to exact match
-        match_args = dict()
-        for k, v in card_kwargs.items():
-            if hasattr(Card, k):
-                match_args[k] = v
-
-        url = "/odata/API_Cards"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        if count:
-            url_query_params = "?$count=true&$top=0"
-        else:
-            filter_str = _compose_filter(exact_match=match_args)
-            url_query_params = ("?" + filter_str)
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        if count:
-            return json_body['@odata.count']
-
-        cards = []
-        for x in json_body['value']:
-            cards.append(Card(x))
-        return cards
-
-    def delete_card(self, card: Card):
-        if not validators.uuid(card.uid):
-            raise ValueError(f'Malformed Card UID {card.uid}')
-
-        url = "/odata/API_Cards"
-        url_query_params = "(" + card.uid + ")"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = self.gp_json_query("DELETE", headers=headers, url=(url + url_query_params))
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Card Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
-
-    def update_card(self, card: Card):
-        if not validators.uuid(card.uid):
-            raise ValueError(f'Malformed Card UID {card.uid}')
-
-        url = "/odata/API_Cards"
-        url_query_params = f"({card.uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        ch = card.dict(changed_only=True)
-
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            else:
-                raise GuardPointError(f"No body - ({code})")
-
-        return True
-
-    def new_card(self, card: Card):
-        url = "/odata/API_Cards"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-        body = card.dict(editable_only=True)
-
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code == 201:  # HTTP CREATED
-            return Card(json_body)
-        else:
-            if "errorMessages" in json_body:
-                raise GuardPointError(json_body["errorMessages"][0]["other"])
-            elif "message" in json_body:
-                raise GuardPointError(json_body['message'])
-            else:
-                raise GuardPointError(str(code))
-
-    def get_card(self, card_uid: str):
-        url = "/odata/API_Cards"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        url_query_params = f"({card_uid})"
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-            else:
-                raise GuardPointError(str(code))
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-
-        return Card(json_body['value'])
-
-    def get_cardholder_by_card_code(self, card_code):
-        url = "/odata/API_Cards"
-        filter_str = f"?$filter=cardcode%20eq%20'{card_code}'%20and%20status%20eq%20'Used'%20&"
-        url_query_params = f"{filter_str}" \
-                           f"$expand=cardholder(" \
-                           "$expand=securityGroup($select=name)," \
-                           "cardholderType($select=typeName)," \
-                           "cards," \
-                           "cardholderPersonalDetail," \
-                           "cardholderCustomizedField," \
-                           "securityGroup," \
-                           "insideArea)" \
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        card_holders = []
-        for x in json_body['value']:
-            if 'cardholder' in x:
-                card_holders.append(Cardholder(x['cardholder']))
-
-        if len(card_holders) > 0:
-            return card_holders[0]
-        else:
-            raise GuardPointError("No Cardholder Found")
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from .._odata_filter import _compose_filter
+from ..guardpoint_dataclasses import Card, Cardholder
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class CardsAPI:
+    async def get_cards(self, count=False, **card_kwargs):
+        # Filter arguments which have to exact match
+        match_args = dict()
+        for k, v in card_kwargs.items():
+            if hasattr(Card, k):
+                match_args[k] = v
+
+        url = "/odata/API_Cards"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        if count:
+            url_query_params = "?$count=true&$top=0"
+        else:
+            filter_str = _compose_filter(exact_match=match_args)
+            url_query_params = ("?" + filter_str)
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url+url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        if count:
+            return json_body['@odata.count']
+
+        cards = []
+        for x in json_body['value']:
+            cards.append(Card(x))
+        return cards
+
+    async def delete_card(self, card: Card):
+        if not validators.uuid(card.uid):
+            raise ValueError(f'Malformed Card UID {card.uid}')
+
+        url = "/odata/API_Cards"
+        url_query_params = "(" + card.uid + ")"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = await self.gp_json_query("DELETE", headers=headers, url=(url + url_query_params))
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Card Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
+
+    async def update_card(self, card: Card):
+        if not validators.uuid(card.uid):
+            raise ValueError(f'Malformed Card UID {card.uid}')
+
+        url = "/odata/API_Cards"
+        url_query_params = f"({card.uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        ch = card.dict(changed_only=True)
+
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
+
+        return True
+
+    async def new_card(self, card: Card):
+        url = "/odata/API_Cards"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+        body = card.dict(editable_only=True)
+
+        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code == 201:  # HTTP CREATED
+            return Card(json_body)
+        else:
+            if "errorMessages" in json_body:
+                raise GuardPointError(json_body["errorMessages"][0]["other"])
+            elif "message" in json_body:
+                raise GuardPointError(json_body['message'])
+            else:
+                raise GuardPointError(str(code))
+
+    async def get_card(self, card_uid: str):
+        url = "/odata/API_Cards"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        url_query_params = f"({card_uid})"
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    raise GuardPointError(json_body['error'])
+            else:
+                raise GuardPointError(str(code))
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+
+        return Card(json_body['value'])
+
+    async def get_cardholder_by_card_code(self, card_code):
+        url = "/odata/API_Cards"
+        filter_str = f"?$filter=cardcode%20eq%20'{card_code}'%20and%20status%20eq%20'Used'%20&"
+        url_query_params = f"{filter_str}" \
+                           f"$expand=cardholder(" \
+                           "$expand=securityGroup($select=name)," \
+                           "cardholderType($select=typeName)," \
+                           "cards," \
+                           "cardholderPersonalDetail," \
+                           "cardholderCustomizedField," \
+                           "securityGroup," \
+                           "insideArea)" \
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    raise GuardPointError(json_body['error'])
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        card_holders = []
+        for x in json_body['value']:
+            if 'cardholder' in x:
+                card_holders.append(Cardholder(x['cardholder']))
+
+        if len(card_holders) > 0:
+            return card_holders[0]
+        else:
+            raise GuardPointError("No Cardholder Found")
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_controllers.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_controllers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import Controller
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class ControllersAPI:
-    def get_controllers(self, ):
-        url = "/odata/API_Controllers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        controllers = []
-        for x in json_body['value']:
-            controllers.append(Controller(x))
-        return controllers
-
-    def get_controller(self, controller_uid: str):
-        if not validators.uuid(controller_uid):
-            raise ValueError(f"Malformed controller_uid: {controller_uid}")
-
-        url = "/odata/API_Controllers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        url_query_params = f"({controller_uid})"
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-            else:
-                raise GuardPointError(str(code))
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if len(json_body) < 1:
-            return None
-        else:
+import validators
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import Controller
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ControllersAPI:
+    def get_controllers(self, ):
+        url = "/odata/API_Controllers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        controllers = []
+        for x in json_body['value']:
+            controllers.append(Controller(x))
+        return controllers
+
+    def get_controller(self, controller_uid: str):
+        if not validators.uuid(controller_uid):
+            raise ValueError(f"Malformed controller_uid: {controller_uid}")
+
+        url = "/odata/API_Controllers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        url_query_params = f"({controller_uid})"
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    raise GuardPointError(json_body['error'])
+            else:
+                raise GuardPointError(str(code))
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if len(json_body) < 1:
+            return None
+        else:
             return Controller(json_body['value'][0])
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_customizedfields.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from .guardpoint_dataclasses import CardholderCustomizedField
-
-
-class CustomizedFieldsAPI:
-
-    def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        url = "/odata/API_CardholderCustomizedFields"
-        url_query_params = f"({cardholder_uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        ch = customFields.dict(changed_only=True)
-
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
+import validators
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from .guardpoint_dataclasses import CardholderCustomizedField
+
+
+class CustomizedFieldsAPI:
+
+    def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        url = "/odata/API_CardholderCustomizedFields"
+        url_query_params = f"({cardholder_uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        ch = customFields.dict(changed_only=True)
+
+        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_diagnostic.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_diagnostic.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import validators
-from pyGuardPoint.guardpoint_utils import GuardPointResponse
-
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class DiagnosticAPI:
-    '''
-    {
-        "controllersUIDs" :[
-            "B3C0976A-3F8C-4B52-AE65-CB6F88FFD813"
-        ],
-        "command": "7901000000000A28"
-    }
-    '''
-    def simulate_access_event(self, controller_uid: str, reader_num: int, card_code: str):
-        if not validators.uuid(controller_uid):
-            raise ValueError(f"Malformed controller_uid: {controller_uid}")
-        if len(card_code) < 8:
-            raise ValueError(f"card_code too short (8 character minimum): {card_code}")
-        if reader_num > 255:
-            raise ValueError(f"Reader num too great (Max 255) {reader_num}")
-
-        url = "/api/Diagnostic"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        controllers_uids = []
-        controllers_uids.append(controller_uid)
-        body = dict()
-        body['controllersUIDs'] = controllers_uids
-        body['command'] = "79{0:0>2X}{1:0>12s}".format(reader_num, card_code)
-
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'success' in json_body:
-            if json_body['success']:
-                return True
-
-        return False
+import validators
+from pyGuardPoint.guardpoint_utils import GuardPointResponse
+
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class DiagnosticAPI:
+    '''
+    {
+        "controllersUIDs" :[
+            "B3C0976A-3F8C-4B52-AE65-CB6F88FFD813"
+        ],
+        "command": "7901000000000A28"
+    }
+    '''
+    def simulate_access_event(self, controller_uid: str, reader_num: int, card_code: str):
+        if not validators.uuid(controller_uid):
+            raise ValueError(f"Malformed controller_uid: {controller_uid}")
+        if len(card_code) < 8:
+            raise ValueError(f"card_code too short (8 character minimum): {card_code}")
+        if reader_num > 255:
+            raise ValueError(f"Reader num too great (Max 255) {reader_num}")
+
+        url = "/api/Diagnostic"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        controllers_uids = []
+        controllers_uids.append(controller_uid)
+        body = dict()
+        body['controllersUIDs'] = controllers_uids
+        body['command'] = "79{0:0>2X}{1:0>12s}".format(reader_num, card_code)
+
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'success' in json_body:
+            if json_body['success']:
+                return True
+
+        return False
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_ouputs.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_ouputs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import validators
-
-from .guardpoint_dataclasses import Relay
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class OutputsAPI:
-
-    def get_relay(self, relay_uid):
-        url = self.baseurl + "/odata/API_Outputs"
-        url_query_params = f"({relay_uid})"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                return None
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        return Relay(json_body['value'][0])
-
-
-    def get_relays(self):
-        url = self.baseurl + "/odata/API_Outputs"
-
-        code, json_body = self.gp_json_query("GET", url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"No Outputs Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        # Compose list of security groups
-        relays = []
-        for entry in json_body['value']:
-            if isinstance(entry, dict):
-                relay = Relay(entry)
-                relays.append(relay)
-        return relays
-
-    def activate_relay(self, relay: Relay, period: int = 0):
-        return self.activate_relay_by_uid(relay.uid, period)
-
-    def activate_relay_by_uid(self, relay_uid: str, period: int = 0):
-
-        url = self.baseurl + "/odata/API_Outputs/Activate"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        if not validators.uuid(relay_uid):
-            raise ValueError("Malformed Relay UID")
-
-        body = dict()
-        body["uids"] = [relay_uid]
-        body["period"] = period
-
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-            if isinstance(json_body, dict):
-                if len(json_body) == 1:
-                    r_uid = list(json_body.keys())[0]
-                    if validators.uuid(r_uid):
-                        if 'item1' in json_body[r_uid]:
-                            error_msg = GuardPointResponse.extract_error_msg(json_body[r_uid]['item1'])
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Relay Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
+import validators
+
+from .guardpoint_dataclasses import Relay
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class OutputsAPI:
+
+    def get_relay(self, relay_uid):
+        url = self.baseurl + "/odata/API_Outputs"
+        url_query_params = f"({relay_uid})"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                return None
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        return Relay(json_body['value'][0])
+
+
+    def get_relays(self):
+        url = self.baseurl + "/odata/API_Outputs"
+
+        code, json_body = self.gp_json_query("GET", url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"No Outputs Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        # Compose list of security groups
+        relays = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                relay = Relay(entry)
+                relays.append(relay)
+        return relays
+
+    def activate_relay(self, relay: Relay, period: int = 0):
+        return self.activate_relay_by_uid(relay.uid, period)
+
+    def activate_relay_by_uid(self, relay_uid: str, period: int = 0):
+
+        url = self.baseurl + "/odata/API_Outputs/Activate"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        if not validators.uuid(relay_uid):
+            raise ValueError("Malformed Relay UID")
+
+        body = dict()
+        body["uids"] = [relay_uid]
+        body["period"] = period
+
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+            if isinstance(json_body, dict):
+                if len(json_body) == 1:
+                    r_uid = list(json_body.keys())[0]
+                    if validators.uuid(r_uid):
+                        if 'item1' in json_body[r_uid]:
+                            error_msg = GuardPointResponse.extract_error_msg(json_body[r_uid]['item1'])
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Relay Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_personaldetails.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from .guardpoint_dataclasses import CardholderPersonalDetail
-
-
-class PersonalDetailsAPI:
-
-    def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        url = "/odata/API_CardholderPersonalDetails"
-        url_query_params = f"({cardholder_uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        ch = personal_details.dict(editable_only=True, changed_only=True)
-
-        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
+import validators
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from .guardpoint_dataclasses import CardholderPersonalDetail
+
+
+class PersonalDetailsAPI:
+
+    def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        url = "/odata/API_CardholderPersonalDetails"
+        url_query_params = f"({cardholder_uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        ch = personal_details.dict(editable_only=True, changed_only=True)
+
+        code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
         return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_readers.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_readers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import Reader
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class ReadersAPI:
-    def get_readers(self, ):
-        url = "/odata/API_Readers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        readers = []
-        for x in json_body['value']:
-            readers.append(Reader(x))
-        return readers
-
-    def get_reader(self, reader_uid: str):
-        if not validators.uuid(reader_uid):
-            raise ValueError(f"Malformed reader_uid: {reader_uid}")
-
-        url = "/odata/API_Readers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        url_query_params = f"({reader_uid})"
-
-        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-            else:
-                raise GuardPointError(str(code))
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-
-        return Reader(json_body['value'])
-
+import validators
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import Reader
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ReadersAPI:
+    def get_readers(self, ):
+        url = "/odata/API_Readers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        readers = []
+        for x in json_body['value']:
+            readers.append(Reader(x))
+        return readers
+
+    def get_reader(self, reader_uid: str):
+        if not validators.uuid(reader_uid):
+            raise ValueError(f"Malformed reader_uid: {reader_uid}")
+
+        url = "/odata/API_Readers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        url_query_params = f"({reader_uid})"
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    raise GuardPointError(json_body['error'])
+            else:
+                raise GuardPointError(str(code))
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+
+        return Reader(json_body['value'])
+
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import validators
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import ScheduledMag, Cardholder
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class ScheduledMagsAPI:
-
-    def get_scheduled_mags(self, cardholder: Cardholder = None):
-        url = self.baseurl + "/odata/API_ScheduledMags"
-        if cardholder:
-            if not validators.uuid(cardholder.uid):
-                raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-            url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
-        else:
-            url_query_params = ""
-
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"MAG Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        # Compose list of security groups
-        scheduled_mags = []
-        for entry in json_body['value']:
-            if isinstance(entry, dict):
-                sm = ScheduledMag(entry)
-                scheduled_mags.append(sm)
-        return scheduled_mags
-
-    def add_scheduled_mag(self, scheduled_mag: ScheduledMag):
-        url = self.baseurl + "/odata/API_ScheduledMags"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-        body = scheduled_mag.dict(editable_only=True)
-
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code == 201:  # HTTP CREATED
-            return json_body['uid']
-        else:
-            if 'value' in json_body:
-                if isinstance(json_body['value'], list):
-                    json_body = json_body['value'][0]
-            else:
-                error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-                if code == 401:
-                    raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-                elif code == 404:  # Not Found
-                    raise GuardPointError(f"Cardholder Not Found")
-                else:
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import ScheduledMag, Cardholder
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ScheduledMagsAPI:
+
+    async def get_scheduled_mags(self, cardholder: Cardholder = None):
+        url = "/odata/API_ScheduledMags"
+        if cardholder:
+            if not validators.uuid(cardholder.uid):
+                raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+            url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
+        else:
+            url_query_params = ""
+
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"MAG Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        # Compose list of security groups
+        scheduled_mags = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                sm = ScheduledMag(entry)
+                scheduled_mags.append(sm)
+        return scheduled_mags
+
+    def add_scheduled_mag(self, scheduled_mag: ScheduledMag):
+        url = self.baseurl + "/odata/API_ScheduledMags"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+        body = scheduled_mag.dict(editable_only=True)
+
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code == 201:  # HTTP CREATED
+            return json_body['uid']
+        else:
+            if 'value' in json_body:
+                if isinstance(json_body['value'], list):
+                    json_body = json_body['value'][0]
+            else:
+                error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+                if code == 401:
+                    raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+                elif code == 404:  # Not Found
+                    raise GuardPointError(f"Cardholder Not Found")
+                else:
                     raise GuardPointError(f"{error_msg}")
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_guardpoint_securitygroups.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from .guardpoint_utils import GuardPointResponse
-from .guardpoint_dataclasses import SecurityGroup
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class SecurityGroupsAPI:
-    def get_security_groups(self):
-        url = self.baseurl + "/odata/api_SecurityGroups"
-        # url_query_params = "?$select=uid,name&$filter=name%20ne%20'Anytime%20Anywhere'"
-        url_query_params = ""
-        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Security Group Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        # Compose list of security groups
-        security_groups = []
-        for entry in json_body['value']:
-            if isinstance(entry, dict):
-                sg = SecurityGroup(entry)
-                security_groups.append(sg)
-        return security_groups
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import SecurityGroup
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class SecurityGroupsAPI:
+    def get_security_groups(self):
+        url = self.baseurl + "/odata/api_SecurityGroups"
+        # url_query_params = "?$select=uid,name&$filter=name%20ne%20'Anytime%20Anywhere'"
+        url_query_params = ""
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Security Group Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        # Compose list of security groups
+        security_groups = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                sg = SecurityGroup(entry)
+                security_groups.append(sg)
+        return security_groups
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/_str_match_algo.py` & `pyguardpoint-1.3.9/pyGuardPoint/_str_match_algo.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import json
-from fuzzywuzzy import process
-from fuzzywuzzy import fuzz
-
-def fuzzy_match(search_words: str, cardholders: list, threshold: int = 75):
-    if not search_words:
-        return cardholders
-
-    cardholder_patterns = []
-    for cardholder in cardholders:
-        cardholder_patterns.append(cardholder.to_search_pattern())
-
-    match_ratios = process.extract(search_words, cardholder_patterns, scorer=fuzz.token_sort_ratio)
-
-    sorted_cardholders = []
-    for match in match_ratios:
-        if match[1] >= threshold:
-            pos = cardholder_patterns.index(match[0])
-            sorted_cardholders.append(cardholders[pos])
-
-    return sorted_cardholders
-
-
-if __name__ == "__main__":
-    from pyGuardPoint_Build.pyGuardPoint import Cardholder
-
-    EXPORT_FILENAME = '../../cardholder_export.json'
-    with open(EXPORT_FILENAME) as f:
-        entries = json.load(f)
-    count = len(entries)
-    print(f"Importing {str(count)} entries from {EXPORT_FILENAME}.")
-
-    cardholders = []
-    for entry in entries:
-        cardholders.append(Cardholder(entry))
-
-    search_pattern = "john owen"
-    print("Search Pattern:" + search_pattern)
-    sorted_cardholders = fuzzy_match(search_pattern, cardholders, 50)
-
-    print(f"Got {len(sorted_cardholders)} matches")
-    print(f"Best Match: {sorted_cardholders[0].firstName} {sorted_cardholders[0].lastName}")
-    print(f"Second Best Match: {sorted_cardholders[1].firstName} {sorted_cardholders[1].lastName}")
-    # pos = cardholder_patterns.index(match_ratios[0][0])
-
-    # print(cardholders[pos].pretty_print())
+import json
+from fuzzywuzzy import process
+from fuzzywuzzy import fuzz
+
+def fuzzy_match(search_words: str, cardholders: list, threshold: int = 75):
+    if not search_words:
+        return cardholders
+
+    cardholder_patterns = []
+    for cardholder in cardholders:
+        cardholder_patterns.append(cardholder.to_search_pattern())
+
+    match_ratios = process.extract(search_words, cardholder_patterns, scorer=fuzz.token_sort_ratio)
+
+    sorted_cardholders = []
+    for match in match_ratios:
+        if match[1] >= threshold:
+            pos = cardholder_patterns.index(match[0])
+            sorted_cardholders.append(cardholders[pos])
+
+    return sorted_cardholders
+
+
+if __name__ == "__main__":
+    from pyGuardPoint_Build.pyGuardPoint import Cardholder
+
+    EXPORT_FILENAME = '../../cardholder_export.json'
+    with open(EXPORT_FILENAME) as f:
+        entries = json.load(f)
+    count = len(entries)
+    print(f"Importing {str(count)} entries from {EXPORT_FILENAME}.")
+
+    cardholders = []
+    for entry in entries:
+        cardholders.append(Cardholder(entry))
+
+    search_pattern = "john owen"
+    print("Search Pattern:" + search_pattern)
+    sorted_cardholders = fuzzy_match(search_pattern, cardholders, 50)
+
+    print(f"Got {len(sorted_cardholders)} matches")
+    print(f"Best Match: {sorted_cardholders[0].firstName} {sorted_cardholders[0].lastName}")
+    print(f"Second Best Match: {sorted_cardholders[1].firstName} {sorted_cardholders[1].lastName}")
+    # pos = cardholder_patterns.index(match_ratios[0][0])
+
+    # print(cardholders[pos].pretty_print())
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_areas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import Area
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class AreasAPI:
-    async def get_areas(self):
-        url = "/odata/API_Areas"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        areas = []
-        for x in json_body['value']:
-            areas.append(Area(x))
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import Area
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class AreasAPI:
+    def get_areas(self):
+        url = "/odata/API_Areas"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        areas = []
+        for x in json_body['value']:
+            areas.append(Area(x))
         return areas
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-from datetime import datetime
-
-import validators
-from .._odata_filter import _compose_filter, _compose_select, _compose_expand
-from .._str_match_algo import fuzzy_match
-from ..guardpoint_dataclasses import Cardholder, SortAlgorithm, Area
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-from ..guardpoint_utils import GuardPointResponse
-
-
-class CardholdersAPI:
-
-    async def delete_card_holder(self, cardholder: Cardholder):
-        if not validators.uuid(cardholder.uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-
-        url = "/odata/API_Cardholders"
-        url_query_params = "(" + cardholder.uid + ")"
-
-        code, json_body = await self.gp_json_query("DELETE", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
-
-    async def update_card_holder_area(self, cardholder_uid: str, area: Area):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        if not validators.uuid(area.uid):
-            raise ValueError(f'Malformed Area UID {area.uid}')
-
-        cardholder = Cardholder()
-        cardholder.uid = cardholder_uid
-        cardholder.insideAreaUID = area.uid
-
-        return await self.update_card_holder(cardholder)
-
-    async def update_card_holder(self, cardholder: Cardholder):
-        if not validators.uuid(cardholder.uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-
-        if cardholder.cardholderCustomizedField:
-            if len(cardholder.cardholderCustomizedField.changed_attributes) > 0:
-                await self.update_custom_fields(cardholder.uid, cardholder.cardholderCustomizedField)
-
-        if cardholder.cardholderPersonalDetail:
-            if len(cardholder.cardholderPersonalDetail.changed_attributes) > 0:
-                await self.update_personal_details(cardholder.uid, cardholder.cardholderPersonalDetail)
-
-        if cardholder.cards:
-            if isinstance(cardholder.cards, list):
-                for card in cardholder.cards:
-                    if len(card.changed_attributes) > 0:
-                        if validators.uuid(card.uid):
-                            await self.update_card(card)
-                        else:
-                            card.cardholderUID = cardholder.uid
-                            await self.new_card(card)
-
-        ch = cardholder.dict(editable_only=True, changed_only=True)
-
-        if len(ch) < 1:  # Nothing to update
-            return True
-
-        url = "/odata/API_Cardholders"
-        url_query_params = f"({cardholder.uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
-
-    async def new_card_holder(self, cardholder: Cardholder, changed_only=False):
-
-        # url = "/odata/API_Cardholders/CreateFullCardholder"
-        url = "/odata/API_Cardholders"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            'IgnoreNonEditable': ''
-        }
-
-        if changed_only:
-            ch = cardholder.dict(editable_only=True, changed_only=True, non_empty_only=True)
-        else:
-            ch = cardholder.dict(editable_only=True, non_empty_only=True)
-
-
-        # When using CreateFullCardholder
-        # body = {'cardholder': ch}
-        # print(json.dumps(body))
-        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=ch)
-        # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code == 201:  # HTTP CREATED
-            new_cardholder = Cardholder(json_body)
-            if cardholder.cardholderPersonalDetail:
-                await self.update_personal_details(cardholder_uid=new_cardholder.uid,
-                                             personal_details=cardholder.cardholderPersonalDetail)
-            if cardholder.cardholderCustomizedField:
-                await self.update_custom_fields(cardholder_uid=new_cardholder.uid,
-                                          customFields=cardholder.cardholderCustomizedField)
-            if cardholder.cards:
-                if isinstance(cardholder.cards, list):
-                    for card in cardholder.cards:
-                        if validators.uuid(card.uid):
-                            await self.update_card(card)
-                        else:
-                            card.cardholderUID = new_cardholder.uid
-                            await self.new_card(card)
-
-            return await self._get_card_holder(new_cardholder.uid)
-
-        elif code == 422:  # unprocessable Entity
-            if "errorMessages" in json_body:
-                raise GuardPointError(
-                    f'{json_body["errorMessages"][0]["message"]}-{json_body["errorMessages"][0]["other"]}')
-        else:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-    async def get_card_holder(self,
-                        uid: str = None,
-                        card_code: str = None):
-        if card_code:
-            # Part of the Cards_API
-            return await self.get_cardholder_by_card_code(card_code)
-        else:
-            return await self._get_card_holder(uid)
-
-    async def get_card_holder_photo(self, uid):
-        if not validators.uuid(uid):
-            raise ValueError(f'Malformed UID {uid}')
-
-        url = "/odata/API_Cardholders"
-        url_query_params = "(" + uid + ")?$select=photo"
-
-        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Photo Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return json_body['value'][0]['photo']
-
-    async def _get_card_holder(self, uid):
-        if not validators.uuid(uid):
-            raise ValueError(f'Malformed UID {uid}')
-
-        url = "/odata/API_Cardholders"
-        url_query_params = "(" + uid + ")?" \
-                                       "$expand=" \
-                                       "cardholderType," \
-                                       "cards," \
-                                       "cardholderCustomizedField," \
-                                       "cardholderPersonalDetail," \
-                                       "securityGroup," \
-                                       "insideArea"
-
-        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code == 404:  # Not Found
-            return None
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return Cardholder(json_body['value'][0])
-
-    async def get_card_holders(self, offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None,
-                         filter_expired: bool = False, cardholder_type_name: str = None,
-                         sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75,
-                         count: bool = False, earliest_last_pass: datetime = None,
-                         select_ignore_list: list = None, select_include_list: list = None,
-                         **cardholder_kwargs):
-
-        if offset is None:
-            offset = 0
-
-        # Filter arguments which have to exact match
-        match_args = dict()
-        for k, v in cardholder_kwargs.items():
-            if hasattr(Cardholder, k):
-                match_args[k] = v
-
-        url = "/odata/API_Cardholders"
-
-        filter_str = _compose_filter(search_words=search_terms,
-                                     areas=areas,
-                                     filter_expired=filter_expired,
-                                     cardholder_type_name=cardholder_type_name,
-                                     earliest_last_pass=earliest_last_pass,
-                                     exact_match=match_args)
-
-        select_str = _compose_select(select_ignore_list, select_include_list)
-
-        expand_str = _compose_expand(select_ignore_list, select_include_list)
-
-        url_query_params = ("?" + select_str + expand_str + filter_str)
-
-        if count:
-            url_query_params += "$count=true&$top=0"
-        else:
-            url_query_params += "$orderby=fromDateValid%20desc&"
-            url_query_params += "$top=" + str(limit) + "&$skip=" + str(offset)
-
-        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
-        # Check response body is formatted correctly
-        # if json_body:
-        #    GuardPointResponse.check_odata_body_structure(json_body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholders Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if count:
-            return json_body['@odata.count']
-
-        cardholders = []
-        for x in json_body['value']:
-            cardholders.append(Cardholder(x))
-
-        if sort_algorithm == SortAlgorithm.FUZZY_MATCH:
-            cardholders = fuzzy_match(search_words=search_terms, cardholders=cardholders, threshold=threshold)
-
-        return cardholders
+from datetime import datetime
+
+import validators
+from .._odata_filter import _compose_filter, _compose_select, _compose_expand
+from .._str_match_algo import fuzzy_match
+from ..guardpoint_dataclasses import Cardholder, SortAlgorithm, Area
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_utils import GuardPointResponse
+
+
+class CardholdersAPI:
+
+    async def delete_card_holder(self, cardholder: Cardholder):
+        if not validators.uuid(cardholder.uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+
+        url = "/odata/API_Cardholders"
+        url_query_params = "(" + cardholder.uid + ")"
+
+        code, json_body = await self.gp_json_query("DELETE", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        if json_body:
+            GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
+
+    async def update_card_holder_area(self, cardholder_uid: str, area: Area):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        if not validators.uuid(area.uid):
+            raise ValueError(f'Malformed Area UID {area.uid}')
+
+        cardholder = Cardholder()
+        cardholder.uid = cardholder_uid
+        cardholder.insideAreaUID = area.uid
+
+        return await self.update_card_holder(cardholder)
+
+    async def update_card_holder(self, cardholder: Cardholder):
+        if not validators.uuid(cardholder.uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+
+        if cardholder.cardholderCustomizedField:
+            if len(cardholder.cardholderCustomizedField.changed_attributes) > 0:
+                await self.update_custom_fields(cardholder.uid, cardholder.cardholderCustomizedField)
+
+        if cardholder.cardholderPersonalDetail:
+            if len(cardholder.cardholderPersonalDetail.changed_attributes) > 0:
+                await self.update_personal_details(cardholder.uid, cardholder.cardholderPersonalDetail)
+
+        if cardholder.cards:
+            if isinstance(cardholder.cards, list):
+                for card in cardholder.cards:
+                    if len(card.changed_attributes) > 0:
+                        if validators.uuid(card.uid):
+                            await self.update_card(card)
+                        else:
+                            card.cardholderUID = cardholder.uid
+                            await self.new_card(card)
+
+        ch = cardholder.dict(editable_only=True, changed_only=True)
+
+        if len(ch) < 1:  # Nothing to update
+            return True
+
+        url = "/odata/API_Cardholders"
+        url_query_params = f"({cardholder.uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
+
+    async def new_card_holder(self, cardholder: Cardholder, changed_only=False):
+
+        # url = "/odata/API_Cardholders/CreateFullCardholder"
+        url = "/odata/API_Cardholders"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            'IgnoreNonEditable': ''
+        }
+
+        if changed_only:
+            ch = cardholder.dict(editable_only=True, changed_only=True, non_empty_only=True)
+        else:
+            ch = cardholder.dict(editable_only=True, non_empty_only=True)
+
+
+        # When using CreateFullCardholder
+        # body = {'cardholder': ch}
+        # print(json.dumps(body))
+        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=ch)
+        # Check response body is formatted correctly
+        if json_body:
+            GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code == 201:  # HTTP CREATED
+            new_cardholder = Cardholder(json_body)
+            if cardholder.cardholderPersonalDetail:
+                await self.update_personal_details(cardholder_uid=new_cardholder.uid,
+                                             personal_details=cardholder.cardholderPersonalDetail)
+            if cardholder.cardholderCustomizedField:
+                await self.update_custom_fields(cardholder_uid=new_cardholder.uid,
+                                          customFields=cardholder.cardholderCustomizedField)
+            if cardholder.cards:
+                if isinstance(cardholder.cards, list):
+                    for card in cardholder.cards:
+                        if validators.uuid(card.uid):
+                            await self.update_card(card)
+                        else:
+                            card.cardholderUID = new_cardholder.uid
+                            await self.new_card(card)
+
+            return await self._get_card_holder(new_cardholder.uid)
+
+        elif code == 422:  # unprocessable Entity
+            if "errorMessages" in json_body:
+                raise GuardPointError(
+                    f'{json_body["errorMessages"][0]["message"]}-{json_body["errorMessages"][0]["other"]}')
+        else:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+    async def get_card_holder(self,
+                        uid: str = None,
+                        card_code: str = None):
+        if card_code:
+            # Part of the Cards_API
+            return await self.get_cardholder_by_card_code(card_code)
+        else:
+            return await self._get_card_holder(uid)
+
+    async def get_card_holder_photo(self, uid):
+        if not validators.uuid(uid):
+            raise ValueError(f'Malformed UID {uid}')
+
+        url = "/odata/API_Cardholders"
+        url_query_params = "(" + uid + ")?$select=photo"
+
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Photo Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return json_body['value'][0]['photo']
+
+    async def _get_card_holder(self, uid):
+        if not validators.uuid(uid):
+            raise ValueError(f'Malformed UID {uid}')
+
+        url = "/odata/API_Cardholders"
+        url_query_params = "(" + uid + ")?" \
+                                       "$expand=" \
+                                       "cardholderType," \
+                                       "cards," \
+                                       "cardholderCustomizedField," \
+                                       "cardholderPersonalDetail," \
+                                       "securityGroup," \
+                                       "insideArea"
+
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code == 404:  # Not Found
+            return None
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return Cardholder(json_body['value'][0])
+
+    async def get_card_holders(self, offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None,
+                         filter_expired: bool = False, cardholder_type_name: str = None,
+                         sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75,
+                         count: bool = False, earliest_last_pass: datetime = None,
+                         select_ignore_list: list = None, select_include_list: list = None,
+                         **cardholder_kwargs):
+
+        if offset is None:
+            offset = 0
+
+        # Filter arguments which have to exact match
+        match_args = dict()
+        for k, v in cardholder_kwargs.items():
+            if hasattr(Cardholder, k):
+                match_args[k] = v
+
+        url = "/odata/API_Cardholders"
+
+        filter_str = _compose_filter(search_words=search_terms,
+                                     areas=areas,
+                                     filter_expired=filter_expired,
+                                     cardholder_type_name=cardholder_type_name,
+                                     earliest_last_pass=earliest_last_pass,
+                                     exact_match=match_args)
+
+        select_str = _compose_select(select_ignore_list, select_include_list)
+
+        expand_str = _compose_expand(select_ignore_list, select_include_list)
+
+        url_query_params = ("?" + select_str + expand_str + filter_str)
+
+        if count:
+            url_query_params += "$count=true&$top=0"
+        else:
+            url_query_params += "$orderby=fromDateValid%20desc&"
+            url_query_params += "$top=" + str(limit) + "&$skip=" + str(offset)
+
+        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
+        # Check response body is formatted correctly
+        # if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholders Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if count:
+            return json_body['@odata.count']
+
+        cardholders = []
+        for x in json_body['value']:
+            cardholders.append(Cardholder(x))
+
+        if sort_algorithm == SortAlgorithm.FUZZY_MATCH:
+            cardholders = fuzzy_match(search_words=search_terms, cardholders=cardholders, threshold=threshold)
+
+        return cardholders
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import CardholderType
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class CardholderTypesAPI:
-    async def get_cardholder_types(self):
-        url = "/odata/API_CardholderTypes"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"CardholderType Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        cardholder_types = []
-        for x in json_body['value']:
-            cardholder_types.append(CardholderType(x))
-        return cardholder_types
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import CardholderType
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class CardholderTypesAPI:
+    async def get_cardholder_types(self):
+        url = "/odata/API_CardholderTypes"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"CardholderType Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        cardholder_types = []
+        for x in json_body['value']:
+            cardholder_types.append(CardholderType(x))
+        return cardholder_types
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import validators
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import Controller
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class ControllersAPI:
-    async def get_controllers(self):
-        url = "/odata/API_Controllers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                return None
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        controllers = []
-        for x in json_body['value']:
-            controllers.append(Controller(x))
-        return controllers
-
-    async def get_controller(self, controller_uid: str):
-        if not validators.uuid(controller_uid):
-            raise ValueError(f"Malformed controller_uid: {controller_uid}")
-
-        url = "/odata/API_Controllers"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        url_query_params = f"({controller_uid})"
-
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                return None
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if len(json_body) < 1:
-            return None
-        else:
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import Controller
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ControllersAPI:
+    async def get_controllers(self):
+        url = "/odata/API_Controllers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                return None
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        controllers = []
+        for x in json_body['value']:
+            controllers.append(Controller(x))
+        return controllers
+
+    async def get_controller(self, controller_uid: str):
+        if not validators.uuid(controller_uid):
+            raise ValueError(f"Malformed controller_uid: {controller_uid}")
+
+        url = "/odata/API_Controllers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        url_query_params = f"({controller_uid})"
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                return None
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if len(json_body) < 1:
+            return None
+        else:
             return Controller(json_body['value'][0])
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import validators
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-from ..guardpoint_dataclasses import CardholderCustomizedField
-
-
-class CustomizedFieldsAPI:
-
-    async def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        url = "/odata/API_CardholderCustomizedFields"
-        url_query_params = f"({cardholder_uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        ch = customFields.dict(changed_only=True)
-
-        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_dataclasses import CardholderCustomizedField
+
+
+class CustomizedFieldsAPI:
+
+    async def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        url = "/odata/API_CardholderCustomizedFields"
+        url_query_params = f"({cardholder_uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        ch = customFields.dict(changed_only=True)
+
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-import validators
-from pyGuardPoint.guardpoint_utils import GuardPointResponse
-
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class DiagnosticAPI:
-    '''
-    {
-        "controllersUIDs" :[
-            "B3C0976A-3F8C-4B52-AE65-CB6F88FFD813"
-        ],
-        "command": "7901000000000A28"
-    }
-    '''
-    async def simulate_access_event(self, controller_uid: str, reader_num: int, card_code: str):
-        if not validators.uuid(controller_uid):
-            raise ValueError(f"Malformed controller_uid: {controller_uid}")
-        if len(card_code) < 8:
-            raise ValueError(f"card_code too short (8 character minimum): {card_code}")
-        if reader_num > 255:
-            raise ValueError(f"Reader num too great (Max 255) {reader_num}")
-
-        url = "/api/Diagnostic"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
-        }
-
-        controllers_uids = []
-        controllers_uids.append(controller_uid)
-        body = dict()
-        body['controllersUIDs'] = controllers_uids
-        body['command'] = "79{0:0>2X}{1:0>12s}".format(reader_num, card_code)
-
-        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'success' in json_body:
-            if json_body['success']:
-                return True
-
-        return False
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_dataclasses import Reader
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ReadersAPI:
+    async def get_readers(self, ):
+        url = "/odata/API_Readers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json'
+        }
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        readers = []
+        for x in json_body['value']:
+            readers.append(Reader(x))
+        return readers
+
+    async def get_reader(self, reader_uid: str):
+        if not validators.uuid(reader_uid):
+            raise ValueError(f"Malformed reader_uid: {reader_uid}")
+
+        url = "/odata/API_Readers"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        url_query_params = f"({reader_uid})"
+
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    raise GuardPointError(json_body['error'])
+            else:
+                raise GuardPointError(str(code))
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+
+        return Reader(json_body['value'])
+
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import validators
-
-from ..guardpoint_dataclasses import Relay
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-class OutputsAPI:
-
-    async def get_relay(self, relay_uid):
-        url = "/odata/API_Outputs"
-        url_query_params = f"({relay_uid})"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                return None
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        return Relay(json_body['value'][0])
-
-
-    async def get_relays(self):
-        url = "/odata/API_Outputs"
-
-        code, json_body = await self.gp_json_query("GET", url=url)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"No Outputs Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        # Compose list of security groups
-        relays = []
-        for entry in json_body['value']:
-            if isinstance(entry, dict):
-                relay = Relay(entry)
-                relays.append(relay)
-        return relays
-
-    async def activate_relay(self, relay: Relay, period: int = 0):
-        return await self.activate_relay_by_uid(relay.uid, period)
-
-    async def activate_relay_by_uid(self, relay_uid: str, period: int = 0):
-
-        url = "/odata/API_Outputs/Activate"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-
-        if not validators.uuid(relay_uid):
-            raise ValueError("Malformed Relay UID")
-
-        body = dict()
-        body["uids"] = [relay_uid]
-        body["period"] = period
-
-        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-            if isinstance(json_body, dict):
-                if len(json_body) == 1:
-                    r_uid = list(json_body.keys())[0]
-                    if validators.uuid(r_uid):
-                        if 'item1' in json_body[r_uid]:
-                            error_msg = GuardPointResponse.extract_error_msg(json_body[r_uid]['item1'])
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Relay Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        return True
+import validators
+
+from ..guardpoint_dataclasses import Relay
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+class OutputsAPI:
+
+    async def get_relay(self, relay_uid):
+        url = "/odata/API_Outputs"
+        url_query_params = f"({relay_uid})"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+        code, json_body = await self.gp_json_query("GET", headers=headers, url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                return None
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        return Relay(json_body['value'][0])
+
+
+    async def get_relays(self):
+        url = "/odata/API_Outputs"
+
+        code, json_body = await self.gp_json_query("GET", url=url)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"No Outputs Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        # Compose list of security groups
+        relays = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                relay = Relay(entry)
+                relays.append(relay)
+        return relays
+
+    async def activate_relay(self, relay: Relay, period: int = 0):
+        return await self.activate_relay_by_uid(relay.uid, period)
+
+    async def activate_relay_by_uid(self, relay_uid: str, period: int = 0):
+
+        url = "/odata/API_Outputs/Activate"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+
+        if not validators.uuid(relay_uid):
+            raise ValueError("Malformed Relay UID")
+
+        body = dict()
+        body["uids"] = [relay_uid]
+        body["period"] = period
+
+        code, json_body = await self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+            if isinstance(json_body, dict):
+                if len(json_body) == 1:
+                    r_uid = list(json_body.keys())[0]
+                    if validators.uuid(r_uid):
+                        if 'item1' in json_body[r_uid]:
+                            error_msg = GuardPointResponse.extract_error_msg(json_body[r_uid]['item1'])
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Relay Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py` & `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import validators
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-from ..guardpoint_dataclasses import CardholderPersonalDetail
-
-
-class PersonalDetailsAPI:
-
-    async def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
-        if not validators.uuid(cardholder_uid):
-            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
-
-        url = "/odata/API_CardholderPersonalDetails"
-        url_query_params = f"({cardholder_uid})"
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-            # 'IgnoreNonEditable': ''
-        }
-
-        ch = personal_details.dict(editable_only=True, changed_only=True)
-
-        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-
-        if code != 204:  # HTTP NO_CONTENT
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"Cardholder Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
+import validators
+from ..guardpoint_utils import GuardPointResponse
+from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ..guardpoint_dataclasses import CardholderPersonalDetail
+
+
+class PersonalDetailsAPI:
+
+    async def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
+        if not validators.uuid(cardholder_uid):
+            raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
+
+        url = "/odata/API_CardholderPersonalDetails"
+        url_query_params = f"({cardholder_uid})"
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            # 'IgnoreNonEditable': ''
+        }
+
+        ch = personal_details.dict(editable_only=True, changed_only=True)
+
+        code, json_body = await self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
+
+        if code != 204:  # HTTP NO_CONTENT
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"Cardholder Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
         return True
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py` & `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import validators
-from ..guardpoint_utils import GuardPointResponse
-from ..guardpoint_dataclasses import ScheduledMag, Cardholder
-from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
-
-
-class ScheduledMagsAPI:
-
-    async def get_scheduled_mags(self, cardholder: Cardholder = None):
-        url = "/odata/API_ScheduledMags"
-        if cardholder:
-            if not validators.uuid(cardholder.uid):
-                raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
-            url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
-        else:
-            url_query_params = ""
-
-        code, json_body = await self.gp_json_query("GET", url=(url + url_query_params))
-
-        if code != 200:
-            error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            elif code == 404:  # Not Found
-                raise GuardPointError(f"MAG Not Found")
-            else:
-                raise GuardPointError(f"{error_msg}")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'value' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-        if not isinstance(json_body['value'], list):
-            raise GuardPointError("Badly formatted response.")
-
-        # Compose list of security groups
-        scheduled_mags = []
-        for entry in json_body['value']:
-            if isinstance(entry, dict):
-                sm = ScheduledMag(entry)
-                scheduled_mags.append(sm)
-        return scheduled_mags
-
-    def add_scheduled_mag(self, scheduled_mag: ScheduledMag):
-        url = self.baseurl + "/odata/API_ScheduledMags"
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json',
-        }
-        body = scheduled_mag.dict(editable_only=True)
-
-        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
-
-        if code == 201:  # HTTP CREATED
-            return json_body['uid']
-        else:
-            if 'value' in json_body:
-                if isinstance(json_body['value'], list):
-                    json_body = json_body['value'][0]
-            else:
-                error_msg = GuardPointResponse.extract_error_msg(json_body)
-
-                if code == 401:
-                    raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-                elif code == 404:  # Not Found
-                    raise GuardPointError(f"Cardholder Not Found")
-                else:
+import validators
+from .guardpoint_utils import GuardPointResponse
+from .guardpoint_dataclasses import ScheduledMag, Cardholder
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+
+
+class ScheduledMagsAPI:
+
+    def get_scheduled_mags(self, cardholder: Cardholder = None):
+        url = self.baseurl + "/odata/API_ScheduledMags"
+        if cardholder:
+            if not validators.uuid(cardholder.uid):
+                raise ValueError(f'Malformed Cardholder UID {cardholder.uid}')
+            url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
+        else:
+            url_query_params = ""
+
+        code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
+
+        if code != 200:
+            error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            elif code == 404:  # Not Found
+                raise GuardPointError(f"MAG Not Found")
+            else:
+                raise GuardPointError(f"{error_msg}")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'value' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+        if not isinstance(json_body['value'], list):
+            raise GuardPointError("Badly formatted response.")
+
+        # Compose list of security groups
+        scheduled_mags = []
+        for entry in json_body['value']:
+            if isinstance(entry, dict):
+                sm = ScheduledMag(entry)
+                scheduled_mags.append(sm)
+        return scheduled_mags
+
+    def add_scheduled_mag(self, scheduled_mag: ScheduledMag):
+        url = self.baseurl + "/odata/API_ScheduledMags"
+        headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+        }
+        body = scheduled_mag.dict(editable_only=True)
+
+        code, json_body = self.gp_json_query("POST", headers=headers, url=url, json_body=body)
+
+        if code == 201:  # HTTP CREATED
+            return json_body['uid']
+        else:
+            if 'value' in json_body:
+                if isinstance(json_body['value'], list):
+                    json_body = json_body['value'][0]
+            else:
+                error_msg = GuardPointResponse.extract_error_msg(json_body)
+
+                if code == 401:
+                    raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+                elif code == 404:  # Not Found
+                    raise GuardPointError(f"Cardholder Not Found")
+                else:
                     raise GuardPointError(f"{error_msg}")
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/guardpoint.py` & `pyguardpoint-1.3.9/pyGuardPoint/guardpoint.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import asyncio
-import logging
-
-from pysignalr.client import SignalRClient
-
-from .CustomWebsocketTransport import CustomWebsocketTransport, DEFAULT_PING_INTERVAL, DEFAULT_CONNECTION_TIMEOUT, \
-    DEFAULT_MAX_SIZE
-from ._guardpoint_cardholdertypes import CardholderTypesAPI
-from ._guardpoint_controllers import ControllersAPI
-from ._guardpoint_diagnostic import DiagnosticAPI
-from ._guardpoint_ouputs import OutputsAPI
-from ._guardpoint_readers import ReadersAPI
-from ._guardpoint_scheduledmags import ScheduledMagsAPI
-from ._guardpoint_customizedfields import CustomizedFieldsAPI
-from ._guardpoint_personaldetails import PersonalDetailsAPI
-from ._guardpoint_securitygroups import SecurityGroupsAPI
-from .guardpoint_connection import GuardPointConnection, GuardPointAuthType
-from ._guardpoint_cards import CardsAPI
-from ._guardpoint_cardholders import CardholdersAPI
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from ._guardpoint_areas import AreasAPI
-from .guardpoint_utils import url_parser, ConvertBase64
-
-log = logging.getLogger(__name__)
-
-
-def stop_listening(client: SignalRClient):
-    async def stop_signal_client() -> None:
-        await client._transport.close()
-
-    asyncio.run(stop_signal_client())
-    '''if not self.task:
-        return
-
-    self.task.cancel()
-    while not self.task.cancelled():
-        sleep(1)'''
-
-
-class GuardPoint(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
-                 CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
-                 OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
-    task = None
-
-    def __init__(self, **kwargs):
-        # Set default values if not present
-        host = kwargs.get('host', "localhost")
-        port = kwargs.get('port', None)
-        url_components = url_parser(host)
-        if url_components['host'] == '':
-            url_components['host'] = url_components['path']
-            url_components['path'] = ''
-        if port:
-            url_components['port'] = port
-        auth = kwargs.get('auth', GuardPointAuthType.BEARER_TOKEN)
-        user = kwargs.get('username', "admin")
-        pwd = kwargs.get('pwd', "admin")
-        key = kwargs.get('key', "00000000-0000-0000-0000-000000000000")
-        token = kwargs.get('token', None)
-        certfile = kwargs.get('cert_file', None)
-        keyfile = kwargs.get('key_file', None)
-        cafile = kwargs.get('ca_file', None)
-        timeout = kwargs.get('timeout', 5)
-        p12_file = kwargs.get('p12_file', None)
-        p12_pwd = kwargs.get('p12_pwd', "")
-        super().__init__(url_components=url_components, auth=auth, user=user, pwd=pwd, key=key, token=token,
-                         cert_file=certfile, key_file=keyfile, ca_file=cafile, timeout=timeout,
-                         p12_file=p12_file, p12_pwd=p12_pwd)
-
-    def get_cardholder_count(self):
-        url = self.baseurl + "/odata/GetCardholdersCount"
-        code, json_body = self.gp_json_query("GET", url=url)
-
-        if code != 200:
-            error_msg = ""
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    error_msg = json_body['error']
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            else:
-                raise GuardPointError(f"No body - ({code})")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'totalItems' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-
-        return int(json_body['totalItems'])
-
-    def get_signal_client(self):
-        client = SignalRClient(self.baseurl + "/Hub/EventsHub")
-        headers = {}
-        if self.authType == GuardPointAuthType.BASIC:
-            auth_str = "Basic " + ConvertBase64.encode(f"{self.user}:{self.key}")
-        else:
-            token = self.get_token()
-            auth_str = f"Bearer {token}"
-        headers['Authorization'] = auth_str
-        client._transport = CustomWebsocketTransport(
-            url=client._url,
-            ssl_context=self.get_ssl_context(),
-            protocol=client._protocol,
-            callback=client._on_message,
-            headers=headers,
-            ping_interval=DEFAULT_PING_INTERVAL,
-            connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
-            max_size=DEFAULT_MAX_SIZE,
-        )
-        return client
-
-    def start_listening(self, client: SignalRClient):
-        async def run_signal_client() -> None:
-            '''group = gp_asyncio.gather(
-                client.run(),
-            )
-            await group'''
-            self.task = asyncio.create_task(client.run(), name = "sigR_task")
-            await self.task
-
-        try:
-            asyncio.run(run_signal_client())
-        except asyncio.CancelledError:
-            print(f"{self.task.get_name()} cancelled")
-
+import asyncio
+import logging
+
+from pysignalr.client import SignalRClient
+
+from .CustomWebsocketTransport import CustomWebsocketTransport, DEFAULT_PING_INTERVAL, DEFAULT_CONNECTION_TIMEOUT, \
+    DEFAULT_MAX_SIZE
+from ._guardpoint_cardholdertypes import CardholderTypesAPI
+from ._guardpoint_controllers import ControllersAPI
+from ._guardpoint_diagnostic import DiagnosticAPI
+from ._guardpoint_ouputs import OutputsAPI
+from ._guardpoint_readers import ReadersAPI
+from ._guardpoint_scheduledmags import ScheduledMagsAPI
+from ._guardpoint_customizedfields import CustomizedFieldsAPI
+from ._guardpoint_personaldetails import PersonalDetailsAPI
+from ._guardpoint_securitygroups import SecurityGroupsAPI
+from .guardpoint_connection import GuardPointConnection, GuardPointAuthType
+from ._guardpoint_cards import CardsAPI
+from ._guardpoint_cardholders import CardholdersAPI
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from ._guardpoint_areas import AreasAPI
+from .guardpoint_utils import url_parser, ConvertBase64
+
+log = logging.getLogger(__name__)
+
+
+def stop_listening(client: SignalRClient):
+    async def stop_signal_client() -> None:
+        await client._transport.close()
+
+    asyncio.run(stop_signal_client())
+    '''if not self.task:
+        return
+
+    self.task.cancel()
+    while not self.task.cancelled():
+        sleep(1)'''
+
+
+class GuardPoint(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
+                 CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
+                 OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
+    task = None
+
+    def __init__(self, **kwargs):
+        # Set default values if not present
+        host = kwargs.get('host', "localhost")
+        port = kwargs.get('port', None)
+        url_components = url_parser(host)
+        if url_components['host'] == '':
+            url_components['host'] = url_components['path']
+            url_components['path'] = ''
+        if port:
+            url_components['port'] = port
+        auth = kwargs.get('auth', GuardPointAuthType.BEARER_TOKEN)
+        user = kwargs.get('username', "admin")
+        pwd = kwargs.get('pwd', "admin")
+        key = kwargs.get('key', "00000000-0000-0000-0000-000000000000")
+        token = kwargs.get('token', None)
+        certfile = kwargs.get('cert_file', None)
+        keyfile = kwargs.get('key_file', None)
+        cafile = kwargs.get('ca_file', None)
+        timeout = kwargs.get('timeout', 5)
+        p12_file = kwargs.get('p12_file', None)
+        p12_pwd = kwargs.get('p12_pwd', "")
+        super().__init__(url_components=url_components, auth=auth, user=user, pwd=pwd, key=key, token=token,
+                         cert_file=certfile, key_file=keyfile, ca_file=cafile, timeout=timeout,
+                         p12_file=p12_file, p12_pwd=p12_pwd)
+
+    def get_cardholder_count(self):
+        url = self.baseurl + "/odata/GetCardholdersCount"
+        code, json_body = self.gp_json_query("GET", url=url)
+
+        if code != 200:
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'totalItems' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+
+        return int(json_body['totalItems'])
+
+    def get_signal_client(self):
+        client = SignalRClient(self.baseurl + "/Hub/EventsHub")
+        headers = {}
+        if self.authType == GuardPointAuthType.BASIC:
+            auth_str = "Basic " + ConvertBase64.encode(f"{self.user}:{self.key}")
+        else:
+            token = self.get_token()
+            auth_str = f"Bearer {token}"
+        headers['Authorization'] = auth_str
+        client._transport = CustomWebsocketTransport(
+            url=client._url,
+            ssl_context=self.get_ssl_context(),
+            protocol=client._protocol,
+            callback=client._on_message,
+            headers=headers,
+            ping_interval=DEFAULT_PING_INTERVAL,
+            connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
+            max_size=DEFAULT_MAX_SIZE,
+        )
+        return client
+
+    def start_listening(self, client: SignalRClient):
+        async def run_signal_client() -> None:
+            '''group = gp_asyncio.gather(
+                client.run(),
+            )
+            await group'''
+            self.task = asyncio.create_task(client.run(), name = "sigR_task")
+            await self.task
+
+        try:
+            asyncio.run(run_signal_client())
+        except asyncio.CancelledError:
+            print(f"{self.task.get_name()} cancelled")
+
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_asyncio.py` & `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_asyncio.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import logging
-
-from pysignalr.client import SignalRClient
-
-from .CustomWebsocketTransport import CustomWebsocketTransport, DEFAULT_PING_INTERVAL, DEFAULT_CONNECTION_TIMEOUT, \
-    DEFAULT_MAX_SIZE
-from .gp_asyncio._async_guardpoint_cardholdertypes import CardholderTypesAPI
-from .gp_asyncio._async_guardpoint_controllers import ControllersAPI
-from .gp_asyncio._async_guardpoint_diagnostic import DiagnosticAPI
-from .gp_asyncio._async_guardpoint_ouputs import OutputsAPI
-from .gp_asyncio._async_guardpoint_readers import ReadersAPI
-from .gp_asyncio._async_guardpoint_scheduledmags import ScheduledMagsAPI
-from .gp_asyncio._async_guardpoint_customizedfields import CustomizedFieldsAPI
-from .gp_asyncio._async_guardpoint_personaldetails import PersonalDetailsAPI
-from .gp_asyncio._async_guardpoint_securitygroups import SecurityGroupsAPI
-from .gp_asyncio._async_guardpoint_cards import CardsAPI
-from .gp_asyncio._async_guardpoint_cardholders import CardholdersAPI
-from .gp_asyncio._async_guardpoint_areas import AreasAPI
-from .gp_asyncio.guardpoint_connection_asyncio import GuardPointConnection, GuardPointAuthType
-
-from .guardpoint_error import GuardPointError, GuardPointUnauthorized
-from .guardpoint_utils import url_parser, ConvertBase64
-
-log = logging.getLogger(__name__)
-
-
-class GuardPointAsyncIO(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
-                        CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
-                        OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
-    task = None
-
-    def __init__(self, **kwargs):
-        # Set default values if not present
-        host = kwargs.get('host', "localhost")
-        port = kwargs.get('port', None)
-        url_components = url_parser(host)
-        if url_components['host'] == '':
-            url_components['host'] = url_components['path']
-            url_components['path'] = ''
-        if port:
-            url_components['port'] = port
-        auth = kwargs.get('auth', GuardPointAuthType.BEARER_TOKEN)
-        user = kwargs.get('username', "admin")
-        pwd = kwargs.get('pwd', "admin")
-        key = kwargs.get('key', "00000000-0000-0000-0000-000000000000")
-        token = kwargs.get('token', None)
-        certfile = kwargs.get('cert_file', None)
-        keyfile = kwargs.get('key_file', None)
-        key_pwd = kwargs.get('key_pwd', "")
-        cafile = kwargs.get('ca_file', None)
-        timeout = kwargs.get('timeout', 5)
-        p12_file = kwargs.get('p12_file', None)
-        p12_pwd = kwargs.get('p12_pwd', "")
-        super().open(url_components=url_components, auth=auth, user=user, pwd=pwd, key=key, token=token,
-                         cert_file=certfile, key_file=keyfile, key_pwd=key_pwd, ca_file=cafile, timeout=timeout,
-                         p12_file=p12_file, p12_pwd=p12_pwd)
-
-    async def get_cardholder_count(self):
-        url = self.baseurl + "/odata/GetCardholdersCount"
-        code, json_body = await self.gp_json_query("GET", url=url)
-
-        if code != 200:
-            error_msg = ""
-            if isinstance(json_body, dict):
-                if 'error' in json_body:
-                    error_msg = json_body['error']
-
-            if code == 401:
-                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
-            else:
-                raise GuardPointError(f"No body - ({code})")
-
-        # Check response body is formatted as expected
-        if not isinstance(json_body, dict):
-            raise GuardPointError("Badly formatted response.")
-        if 'totalItems' not in json_body:
-            raise GuardPointError("Badly formatted response.")
-
-        return int(json_body['totalItems'])
-
-    async def get_signal_client(self):
-        client = SignalRClient(self.baseurl + "/Hub/EventsHub")
-        headers = {}
-        if self.authType == GuardPointAuthType.BASIC:
-            auth_str = "Basic " + ConvertBase64.encode(f"{self.user}:{self.key}")
-        else:
-            token = await self.get_token()
-            auth_str = f"Bearer {token}"
-        headers['Authorization'] = auth_str
-        client._transport = CustomWebsocketTransport(
-            url=client._url,
-            ssl_context=self.get_ssl_context(),
-            protocol=client._protocol,
-            callback=client._on_message,
-            headers=headers,
-            ping_interval=DEFAULT_PING_INTERVAL,
-            connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
-            max_size=DEFAULT_MAX_SIZE,
-        )
-        return client
-
-    async def start_listening(self, client: SignalRClient):
-        return await client.run()
-
-    async def stop_listening(self, client: SignalRClient):
-        return await client._transport.close()
+import logging
+
+from pysignalr.client import SignalRClient
+
+from .CustomWebsocketTransport import CustomWebsocketTransport, DEFAULT_PING_INTERVAL, DEFAULT_CONNECTION_TIMEOUT, \
+    DEFAULT_MAX_SIZE
+from .gp_asyncio._async_guardpoint_cardholdertypes import CardholderTypesAPI
+from .gp_asyncio._async_guardpoint_controllers import ControllersAPI
+from .gp_asyncio._async_guardpoint_diagnostic import DiagnosticAPI
+from .gp_asyncio._async_guardpoint_ouputs import OutputsAPI
+from .gp_asyncio._async_guardpoint_readers import ReadersAPI
+from .gp_asyncio._async_guardpoint_scheduledmags import ScheduledMagsAPI
+from .gp_asyncio._async_guardpoint_customizedfields import CustomizedFieldsAPI
+from .gp_asyncio._async_guardpoint_personaldetails import PersonalDetailsAPI
+from .gp_asyncio._async_guardpoint_securitygroups import SecurityGroupsAPI
+from .gp_asyncio._async_guardpoint_cards import CardsAPI
+from .gp_asyncio._async_guardpoint_cardholders import CardholdersAPI
+from .gp_asyncio._async_guardpoint_areas import AreasAPI
+from .gp_asyncio.guardpoint_connection_asyncio import GuardPointConnection, GuardPointAuthType
+
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
+from .guardpoint_utils import url_parser, ConvertBase64
+
+log = logging.getLogger(__name__)
+
+
+class GuardPointAsyncIO(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
+                        CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
+                        OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
+    task = None
+
+    def __init__(self, **kwargs):
+        # Set default values if not present
+        host = kwargs.get('host', "localhost")
+        port = kwargs.get('port', None)
+        url_components = url_parser(host)
+        if url_components['host'] == '':
+            url_components['host'] = url_components['path']
+            url_components['path'] = ''
+        if port:
+            url_components['port'] = port
+        auth = kwargs.get('auth', GuardPointAuthType.BEARER_TOKEN)
+        user = kwargs.get('username', "admin")
+        pwd = kwargs.get('pwd', "admin")
+        key = kwargs.get('key', "00000000-0000-0000-0000-000000000000")
+        token = kwargs.get('token', None)
+        certfile = kwargs.get('cert_file', None)
+        keyfile = kwargs.get('key_file', None)
+        key_pwd = kwargs.get('key_pwd', "")
+        cafile = kwargs.get('ca_file', None)
+        timeout = kwargs.get('timeout', 5)
+        p12_file = kwargs.get('p12_file', None)
+        p12_pwd = kwargs.get('p12_pwd', "")
+        super().open(url_components=url_components, auth=auth, user=user, pwd=pwd, key=key, token=token,
+                         cert_file=certfile, key_file=keyfile, key_pwd=key_pwd, ca_file=cafile, timeout=timeout,
+                         p12_file=p12_file, p12_pwd=p12_pwd)
+
+    async def get_cardholder_count(self):
+        url = self.baseurl + "/odata/GetCardholdersCount"
+        code, json_body = await self.gp_json_query("GET", url=url)
+
+        if code != 200:
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
+
+        # Check response body is formatted as expected
+        if not isinstance(json_body, dict):
+            raise GuardPointError("Badly formatted response.")
+        if 'totalItems' not in json_body:
+            raise GuardPointError("Badly formatted response.")
+
+        return int(json_body['totalItems'])
+
+    async def get_signal_client(self):
+        client = SignalRClient(self.baseurl + "/Hub/EventsHub")
+        headers = {}
+        if self.authType == GuardPointAuthType.BASIC:
+            auth_str = "Basic " + ConvertBase64.encode(f"{self.user}:{self.key}")
+        else:
+            token = await self.get_token()
+            auth_str = f"Bearer {token}"
+        headers['Authorization'] = auth_str
+        client._transport = CustomWebsocketTransport(
+            url=client._url,
+            ssl_context=self.get_ssl_context(),
+            protocol=client._protocol,
+            callback=client._on_message,
+            headers=headers,
+            ping_interval=DEFAULT_PING_INTERVAL,
+            connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
+            max_size=DEFAULT_MAX_SIZE,
+        )
+        return client
+
+    async def start_listening(self, client: SignalRClient):
+        return await client.run()
+
+    async def stop_listening(self, client: SignalRClient):
+        return await client._transport.close()
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_dataclasses.py` & `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_dataclasses.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,659 +1,659 @@
-import logging
-from collections import defaultdict
-from dataclasses import dataclass, asdict, field
-from enum import Enum
-
-log = logging.getLogger(__name__)
-
-
-class Observable:
-    # A set of all attributes which get changed
-    changed_attributes = set()
-
-    def __init__(self):
-        self.observed = defaultdict(list)
-
-    def __setattr__(self, name, value):
-        super().__setattr__(name, value)
-
-        for observer in self.observed.get(name, []):
-            observer(name)
-
-    def add_observer(self, name):
-        self.observed[name].append(lambda name: self.changed_attributes.add(name))
-
-
-def sanitise_args(obj: Observable, args, kwargs):
-    kwarg_dict = dict()
-    obj.changed_attributes = set()
-
-    for arg in args:
-        if isinstance(arg, dict):
-            kwarg_dict.update(arg)
-
-    for k, v in kwargs.items():
-        if hasattr(type(obj), k):
-            kwarg_dict[k] = v
-            obj.changed_attributes.add(k)
-        else:
-            log.debug(f"{obj.__class__.__name__}.{k} - attribute ignored.")
-            # raise ValueError(f"No such attribute: {k}")
-
-    return kwarg_dict
-
-
-class SortAlgorithm(Enum):
-    SERVER_DEFAULT = 0,
-    FUZZY_MATCH = 1
-
-@dataclass
-class Controller:
-    isActivated: any = None
-    uid: str = ""
-    address: int = 0
-    networkUID: str = ""
-    name: str = ""
-    isPooling: any = None
-    status: str = ""
-    purpose: str = ""
-    isConnected: any = None
-    disconnectTime: str = ""
-    description: any = None
-    script: str = ""
-    firmwareVersion: str = ""
-    hardwareVersion: str = ""
-    apiKey: any = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        controller_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in controller_dict:
-            if isinstance(controller_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, controller_dict[property_name])
-
-    def dict(self):
-        controller_dict = {}
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                controller_dict[k] = v
-            elif isinstance(v, type(None)):
-                controller_dict[k] = None
-            else:
-                controller_dict[k] = str(v)
-
-        return controller_dict
-
-@dataclass
-class Reader:
-    uid: str = ""
-    name: str = ""
-    description: any = None
-    number: int = 0
-    controllerUID: str = ""
-    firstOutputUID: any = None
-    secondOutputUID: any = None
-    weeklyProgramUID: any = None
-    readerFunctionIDs: any = None
-    apiKey: any = None
-    doorAlarmInputUID: str = ""
-    doorControlInput1UID: any = None
-    doorControlInput2UID: any = None
-    doorRemoteInputUID: str = ""
-    motorizedReaderInputUID: any = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        reader_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in reader_dict:
-            if isinstance(reader_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, reader_dict[property_name])
-
-    def dict(self):
-        reader_dict = {}
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                reader_dict[k] = v
-            elif isinstance(v, type(None)):
-                reader_dict[k] = None
-            else:
-                reader_dict[k] = str(v)
-
-        return reader_dict
-
-
-@dataclass
-class Relay(Observable):
-    digitalOutputStatus: str = ""
-    uid: str = ""
-    number: int = 0
-    name: str = ""
-    description: any = None
-    weeklyProgramUID: any = None
-    controllerUID: str = ""
-    liftReaderUID: any = None
-    constantState: str = ""
-    apiKey: any = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        relay_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in relay_dict:
-            if isinstance(relay_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, relay_dict[property_name])
-
-        # Monitor Changes
-        for k, v in asdict(self).items():
-            if isinstance(v, (str, type(None), bool, int)):
-                self.add_observer(k)
-
-    def _remove_non_changed(self, relay_dict: dict):
-        for key, value in list(relay_dict.items()):
-            if key not in self.changed_attributes:
-                relay_dict.pop(key)
-        return relay_dict
-
-    def dict(self, editable_only=False, changed_only=False):
-        relay_dict = {}
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                relay_dict[k] = v
-            elif isinstance(v, type(None)):
-                relay_dict[k] = None
-            else:
-                relay_dict[k] = str(v)
-
-        if editable_only:
-            if 'uid' in relay_dict:
-                relay_dict.pop('uid')
-
-        if changed_only:
-            relay_dict = self._remove_non_changed(relay_dict)
-
-        return relay_dict
-
-
-@dataclass
-class Card(Observable):
-    technologyType: int = 0
-    description: str = ""
-    cardCode: str = ""
-    status: str = "Free"
-    cardholderUID: any = None
-    cardType: str = "Magnetic"
-    readerFunctionUID: any = None
-    uid: str = ""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        card_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in card_dict:
-            if isinstance(card_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, card_dict[property_name])
-
-        # Monitor Changes
-        for k, v in asdict(self).items():
-            if isinstance(v, (str, type(None), bool, int)):
-                self.add_observer(k)
-
-    def _remove_non_changed(self, ch: dict):
-        for key, value in list(ch.items()):
-            if key not in self.changed_attributes:
-                ch.pop(key)
-        return ch
-
-    def dict(self, editable_only=False, changed_only=False):
-        c = {}
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                c[k] = v
-            elif isinstance(v, type(None)):
-                c[k] = None
-            else:
-                c[k] = str(v)
-
-        if editable_only:
-            if 'uid' in c:
-                c.pop('uid')
-            if 'readerFunctionUID' in c:
-                c.pop('readerFunctionUID')
-
-        if changed_only:
-            c = self._remove_non_changed(c)
-
-        return c
-
-
-@dataclass
-class Area:
-    uid: str = ""
-    name: str = ""
-
-    def __init__(self, area_dict: dict):
-        for property_name in area_dict:
-            if isinstance(area_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, area_dict[property_name])
-
-    def dict(self):
-        return {k: str(v) for k, v in asdict(self).items()}
-
-
-@dataclass
-class SecurityGroup:
-    ownerSiteUID: str = ""
-    uid: str = ""
-    name: str = ""
-    apiKey: any = ""
-    description: str = ""
-    isAppliedToVisitor: bool = False
-
-    def __init__(self, security_group_dict: dict):
-        for property_name in security_group_dict:
-            if isinstance(security_group_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, security_group_dict[property_name])
-
-    def dict(self):
-        return {k: str(v) for k, v in asdict(self).items()}
-
-
-@dataclass
-class ScheduledMag(Observable):
-    uid: str = ""
-    securityGroupAPIKey: str = ""
-    scheduledSecurityGroupUID: str = ""
-    cardholderUID: str = ""
-    toDateValid: str = ""
-    fromDateValid: str = ""
-    status: str = ""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        scheduled_mags_dict = sanitise_args(self, args, kwargs)
-
-        # Initialise clss attributes from dictionary
-        for property_name in scheduled_mags_dict:
-            if isinstance(scheduled_mags_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, scheduled_mags_dict[property_name])
-                self.add_observer(property_name)
-
-    def dict(self, editable_only=False):
-        c = {}
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                c[k] = v
-            elif isinstance(v, type(None)):
-                c[k] = None
-            else:
-                c[k] = str(v)
-
-        if editable_only:
-            if 'uid' in c:
-                c.pop('uid')
-            if 'status' in c:
-                c.pop('status')
-
-        return c
-
-
-@dataclass
-class CardholderCustomizedField(Observable):
-    uid: str = ""
-    cF_BoolField_1: bool = False,
-    cF_BoolField_2: bool = False
-    cF_BoolField_3: bool = False
-    cF_BoolField_4: bool = False
-    cF_BoolField_5: bool = False
-    cF_IntField_1: int = 0
-    cF_IntField_2: int = 0
-    cF_IntField_3: int = 0
-    cF_IntField_4: int = 0
-    cF_IntField_5: int = 0
-    cF_DateTimeField_1: any = None
-    cF_DateTimeField_2: any = None
-    cF_DateTimeField_3: any = None
-    cF_DateTimeField_4: any = None
-    cF_DateTimeField_5: any = None
-    cF_StringField_1: str = ""
-    cF_StringField_2: str = ""
-    cF_StringField_3: str = ""
-    cF_StringField_4: str = ""
-    cF_StringField_5: str = ""
-    cF_StringField_6: str = ""
-    cF_StringField_7: str = ""
-    cF_StringField_8: str = ""
-    cF_StringField_9: str = ""
-    cF_StringField_10: str = ""
-    cF_StringField_11: str = ""
-    cF_StringField_12: str = ""
-    cF_StringField_13: str = ""
-    cF_StringField_14: str = ""
-    cF_StringField_15: str = ""
-    cF_StringField_16: str = ""
-    cF_StringField_17: str = ""
-    cF_StringField_18: str = ""
-    cF_StringField_19: str = ""
-    cF_StringField_20: str = ""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        custom_fields_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in custom_fields_dict:
-            if isinstance(custom_fields_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, custom_fields_dict[property_name])
-
-        # Monitor Changes
-        for k, v in asdict(self).items():
-            if isinstance(v, (str, type(None), bool, int)):
-                self.add_observer(k)
-
-    def dict(self, changed_only=False):
-        c = dict()
-        for k, v in asdict(self).items():
-            if isinstance(v, (bool, int)):
-                c[k] = v
-            elif isinstance(v, int):
-                c[k] = v
-            elif isinstance(v, type(None)):
-                c[k] = None
-            else:
-                c[k] = str(v)
-
-        if changed_only:
-            c = self._remove_non_changed(c)
-
-        return c
-
-    def _remove_non_changed(self, ch: dict):
-        for key, value in list(ch.items()):
-            if key not in self.changed_attributes:
-                ch.pop(key)
-        return ch
-
-
-@dataclass
-class CardholderPersonalDetail(Observable):
-    uid: str = ""
-    officePhone: str = ""
-    cityOrDistrict: str = ""
-    streetOrApartment: str = ""
-    postCode: str = ""
-    privatePhoneOrFax: str = ""
-    mobile: str = ""
-    email: str = ""
-    carRegistrationNum: str = ""
-    company: str = ""
-    idFreeText: str = ""
-    idType: str = "IdentityCard"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        person_details_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in person_details_dict:
-            if isinstance(person_details_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, person_details_dict[property_name])
-
-        # Monitor Changes
-        for k, v in asdict(self).items():
-            if isinstance(v, (str, type(None), bool, int)):
-                self.add_observer(k)
-
-    def dict(self, editable_only=False, changed_only=False, non_empty_only=False):
-        ch = dict()
-
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                ch[k] = v
-            elif isinstance(v, type(None)):
-                pass
-                # ch[k] = None
-            elif isinstance(v, str):
-                if non_empty_only:
-                    if len(v) > 0:
-                        ch[k] = str(v)
-                else:
-                    ch[k] = str(v)
-            else:
-                pass
-
-        if changed_only:
-            ch = self._remove_non_changed(ch)
-
-        if editable_only:
-            ch = self._remove_non_editable(ch)
-
-        return ch
-
-    def _remove_non_changed(self, ch: dict):
-        for key, value in list(ch.items()):
-            if key not in self.changed_attributes:
-                ch.pop(key)
-        return ch
-
-    @staticmethod
-    def _remove_non_editable(ch: dict):
-        if 'uid' in ch:
-            ch.pop('uid')
-        return ch
-
-
-@dataclass
-class CardholderType:
-    uid: str = ""
-    typeName: str = ""
-    defaultBPTemplate: str = ""
-
-    def __init__(self, cardholder_type_dict: dict):
-        for property_name in cardholder_type_dict:
-            if isinstance(cardholder_type_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, cardholder_type_dict[property_name])
-
-    def dict(self):
-        return {k: str(v) for k, v in asdict(self).items()}
-
-
-@dataclass
-class Cardholder(Observable):
-    uid: str = ""
-    lastName: str = ""
-    firstName: str = ""
-    cardholderIdNumber: any = None
-    status: any = None
-    fromDateValid: any = None
-    isFromDateActive: any = None
-    toDateValid: any = None
-    isToDateActive: any = None
-    photo: any = None
-    cardholderType: CardholderType = None
-    securityGroup: SecurityGroup = None
-    cardholderPersonalDetail: CardholderPersonalDetail = None
-    cardholderCustomizedField: CardholderCustomizedField = None
-    insideArea: Area = None
-    ownerSiteUID: str = ""
-    securityGroupApiKey: any = None
-    ownerSiteApiKey: any = None
-    accessGroupApiKeys: any = None
-    liftAccessGroupApiKeys: any = None
-    cardholderTypeUID: str = ""
-    departmentUID: any = None
-    description: str = ""
-    grantAccessForSupervisor: any = None
-    isSupervisor: any = None
-    needEscort: any = None
-    personalWeeklyProgramUID: any = None
-    pinCode: str = ""
-    sharedStatus: str = ""
-    securityGroupUID: str = ""
-    accessGroupUIDs: any = None
-    liftAccessGroupUIDs: any = None
-    lastDownloadTime: any = None
-    lastInOutArea: str = ""
-    lastInOutReaderUID: any = None
-    lastInOutDate: any = None
-    lastAreaReaderDate: any = None
-    lastAreaReaderUID: any = None
-    lastPassDate: any = None
-    lastReaderPassUID: any = None
-    insideAreaUID: str = ""
-    cards: list = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        cardholder_dict = sanitise_args(self, args, kwargs)
-
-        for property_name in cardholder_dict:
-            if isinstance(cardholder_dict[property_name], list):
-                if property_name == "cards":
-                    setattr(self, property_name, [])
-                    for card_entry in cardholder_dict[property_name]:
-                        if isinstance(card_entry, Card):
-                            self.cards.append(card_entry)
-                        else:
-                            self.cards.append(Card(card_entry))
-                else:
-                    setattr(self, property_name, cardholder_dict[property_name])
-
-            if property_name == "cardholderPersonalDetail":
-                if isinstance(cardholder_dict[property_name], CardholderPersonalDetail):
-                    self.cardholderPersonalDetail = cardholder_dict[property_name]
-
-            if property_name == "cardholderCustomizedField":
-                if isinstance(cardholder_dict[property_name], CardholderCustomizedField):
-                    self.cardholderCustomizedField = cardholder_dict[property_name]
-
-            if isinstance(cardholder_dict[property_name], dict):
-                if property_name == "insideArea":
-                    self.insideArea = Area(cardholder_dict[property_name])
-                if property_name == "securityGroup":
-                    self.securityGroup = SecurityGroup(cardholder_dict[property_name])
-                if property_name == "cardholderType":
-                    self.cardholderType = CardholderType(cardholder_dict[property_name])
-                if property_name == "cardholderPersonalDetail":
-                    self.cardholderPersonalDetail = CardholderPersonalDetail(cardholder_dict[property_name])
-                if property_name == "cardholderCustomizedField":
-                    self.cardholderCustomizedField = CardholderCustomizedField(cardholder_dict[property_name])
-
-            if isinstance(cardholder_dict[property_name], (str, type(None), bool, int)):
-                setattr(self, property_name, cardholder_dict[property_name])
-
-        # Monitor Changes
-        for k, v in asdict(self).items():
-            if isinstance(v, (str, type(None), bool, int)):
-                self.add_observer(k)
-
-    def to_search_pattern(self):
-        pattern = ""
-        if self.firstName:
-            pattern += self.firstName + " "
-        if self.lastName:
-            pattern += self.lastName + " "
-        if self.cardholderPersonalDetail:
-            if self.cardholderPersonalDetail.company:
-                pattern += self.cardholderPersonalDetail.company + " "
-            if self.cardholderPersonalDetail.email:
-                pattern += self.cardholderPersonalDetail.email
-        return pattern
-
-    def pretty_print(self, obj: object = None):
-        if obj is None:
-            obj = self
-        for attribute_name in obj.__dict__:
-            if attribute_name != 'observed':
-                attribute = getattr(obj, attribute_name)
-                if isinstance(attribute, list):
-                    print(f"{attribute_name}:")
-                    print(f"\t{str(attribute)}")
-                elif hasattr(attribute, '__dict__'):
-                    print(f"{attribute_name}:")
-                    obj.pretty_print(attribute)
-                else:
-                    print(f"\t{attribute_name:<25}" + str(attribute))
-
-    def dict(self, editable_only=False, changed_only=False, non_empty_only=False):
-        ch = dict()
-
-        for k, v in asdict(self).items():
-            if isinstance(v, (list, dict, bool, int)):
-                ch[k] = v
-            elif isinstance(v, type(None)):
-                if not non_empty_only:
-                    ch[k] = None
-            elif isinstance(v, str):
-                if non_empty_only:
-                    if len(v) > 0:
-                        ch[k] = str(v)
-                else:
-                    ch[k] = str(v)
-            else:
-                pass
-
-        if changed_only:
-            ch = self._remove_non_changed(ch)
-
-        if editable_only:
-            ch = self._remove_non_editable(ch)
-
-        return ch
-
-    def _remove_non_changed(self, ch: dict):
-        for key, value in list(ch.items()):
-            if key not in self.changed_attributes:
-                ch.pop(key)
-        return ch
-
-    @staticmethod
-    def _remove_non_editable(ch: dict):
-        if 'uid' in ch:
-            ch.pop('uid')
-        if 'ownerSiteUID' in ch:
-            ch.pop('ownerSiteUID')
-        if 'lastDownloadTime' in ch:
-            ch.pop('lastDownloadTime')
-        if 'lastInOutArea' in ch:
-            ch.pop('lastInOutArea')
-        if 'lastInOutReaderUID' in ch:
-            ch.pop('lastInOutReaderUID')
-        if 'lastInOutDate' in ch:
-            ch.pop('lastInOutDate')
-        if 'lastAreaReaderDate' in ch:
-            ch.pop('lastAreaReaderDate')
-        if 'lastAreaReaderUID' in ch:
-            ch.pop('lastAreaReaderUID')
-        if 'lastPassDate' in ch:
-            ch.pop('lastPassDate')
-        if 'lastReaderPassUID' in ch:
-            ch.pop('lastReaderPassUID')
-        if 'status' in ch:
-            ch.pop('status')
-        if 'insideArea' in ch:
-            ch.pop('insideArea')
-        if 'cardholderPersonalDetail' in ch:
-            ch.pop('cardholderPersonalDetail')
-        if 'cardholderCustomizedField' in ch:
-            ch.pop('cardholderCustomizedField')
-        if 'cardholderType' in ch:
-            ch.pop('cardholderType')
-        if 'securityGroup' in ch:
-            ch.pop('securityGroup')
-        if 'cards' in ch:
-            ch.pop('cards')
-        if 'accessGroupUIDs' in ch:
-            ch.pop('accessGroupUIDs')
-        if 'liftAccessGroupUIDs' in ch:
-            ch.pop('liftAccessGroupUIDs')
-
-        return ch
-
-
-if __name__ == "__main__":
-    cardholdertype = CardholderType(typeName="test")
-    print(cardholdertype.typeName)
-
-    '''securityGroup = SecurityGroup(ownerSiteUID="1234",
-                                  uid="sdfs", name="test", apiKey="None", description="test", isAppliedToVisitor=False)
-    print(securityGroup.name)
-    print(securityGroup.uid)'''
+import logging
+from collections import defaultdict
+from dataclasses import dataclass, asdict, field
+from enum import Enum
+
+log = logging.getLogger(__name__)
+
+
+class Observable:
+    # A set of all attributes which get changed
+    changed_attributes = set()
+
+    def __init__(self):
+        self.observed = defaultdict(list)
+
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+
+        for observer in self.observed.get(name, []):
+            observer(name)
+
+    def add_observer(self, name):
+        self.observed[name].append(lambda name: self.changed_attributes.add(name))
+
+
+def sanitise_args(obj: Observable, args, kwargs):
+    kwarg_dict = dict()
+    obj.changed_attributes = set()
+
+    for arg in args:
+        if isinstance(arg, dict):
+            kwarg_dict.update(arg)
+
+    for k, v in kwargs.items():
+        if hasattr(type(obj), k):
+            kwarg_dict[k] = v
+            obj.changed_attributes.add(k)
+        else:
+            log.debug(f"{obj.__class__.__name__}.{k} - attribute ignored.")
+            # raise ValueError(f"No such attribute: {k}")
+
+    return kwarg_dict
+
+
+class SortAlgorithm(Enum):
+    SERVER_DEFAULT = 0,
+    FUZZY_MATCH = 1
+
+@dataclass
+class Controller:
+    isActivated: any = None
+    uid: str = ""
+    address: int = 0
+    networkUID: str = ""
+    name: str = ""
+    isPooling: any = None
+    status: str = ""
+    purpose: str = ""
+    isConnected: any = None
+    disconnectTime: str = ""
+    description: any = None
+    script: str = ""
+    firmwareVersion: str = ""
+    hardwareVersion: str = ""
+    apiKey: any = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        controller_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in controller_dict:
+            if isinstance(controller_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, controller_dict[property_name])
+
+    def dict(self):
+        controller_dict = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                controller_dict[k] = v
+            elif isinstance(v, type(None)):
+                controller_dict[k] = None
+            else:
+                controller_dict[k] = str(v)
+
+        return controller_dict
+
+@dataclass
+class Reader:
+    uid: str = ""
+    name: str = ""
+    description: any = None
+    number: int = 0
+    controllerUID: str = ""
+    firstOutputUID: any = None
+    secondOutputUID: any = None
+    weeklyProgramUID: any = None
+    readerFunctionIDs: any = None
+    apiKey: any = None
+    doorAlarmInputUID: str = ""
+    doorControlInput1UID: any = None
+    doorControlInput2UID: any = None
+    doorRemoteInputUID: str = ""
+    motorizedReaderInputUID: any = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        reader_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in reader_dict:
+            if isinstance(reader_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, reader_dict[property_name])
+
+    def dict(self):
+        reader_dict = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                reader_dict[k] = v
+            elif isinstance(v, type(None)):
+                reader_dict[k] = None
+            else:
+                reader_dict[k] = str(v)
+
+        return reader_dict
+
+
+@dataclass
+class Relay(Observable):
+    digitalOutputStatus: str = ""
+    uid: str = ""
+    number: int = 0
+    name: str = ""
+    description: any = None
+    weeklyProgramUID: any = None
+    controllerUID: str = ""
+    liftReaderUID: any = None
+    constantState: str = ""
+    apiKey: any = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        relay_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in relay_dict:
+            if isinstance(relay_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, relay_dict[property_name])
+
+        # Monitor Changes
+        for k, v in asdict(self).items():
+            if isinstance(v, (str, type(None), bool, int)):
+                self.add_observer(k)
+
+    def _remove_non_changed(self, relay_dict: dict):
+        for key, value in list(relay_dict.items()):
+            if key not in self.changed_attributes:
+                relay_dict.pop(key)
+        return relay_dict
+
+    def dict(self, editable_only=False, changed_only=False):
+        relay_dict = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                relay_dict[k] = v
+            elif isinstance(v, type(None)):
+                relay_dict[k] = None
+            else:
+                relay_dict[k] = str(v)
+
+        if editable_only:
+            if 'uid' in relay_dict:
+                relay_dict.pop('uid')
+
+        if changed_only:
+            relay_dict = self._remove_non_changed(relay_dict)
+
+        return relay_dict
+
+
+@dataclass
+class Card(Observable):
+    technologyType: int = 0
+    description: str = ""
+    cardCode: str = ""
+    status: str = "Free"
+    cardholderUID: any = None
+    cardType: str = "Magnetic"
+    readerFunctionUID: any = None
+    uid: str = ""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        card_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in card_dict:
+            if isinstance(card_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, card_dict[property_name])
+
+        # Monitor Changes
+        for k, v in asdict(self).items():
+            if isinstance(v, (str, type(None), bool, int)):
+                self.add_observer(k)
+
+    def _remove_non_changed(self, ch: dict):
+        for key, value in list(ch.items()):
+            if key not in self.changed_attributes:
+                ch.pop(key)
+        return ch
+
+    def dict(self, editable_only=False, changed_only=False):
+        c = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                c[k] = v
+            elif isinstance(v, type(None)):
+                c[k] = None
+            else:
+                c[k] = str(v)
+
+        if editable_only:
+            if 'uid' in c:
+                c.pop('uid')
+            if 'readerFunctionUID' in c:
+                c.pop('readerFunctionUID')
+
+        if changed_only:
+            c = self._remove_non_changed(c)
+
+        return c
+
+
+@dataclass
+class Area:
+    uid: str = ""
+    name: str = ""
+
+    def __init__(self, area_dict: dict):
+        for property_name in area_dict:
+            if isinstance(area_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, area_dict[property_name])
+
+    def dict(self):
+        return {k: str(v) for k, v in asdict(self).items()}
+
+
+@dataclass
+class SecurityGroup:
+    ownerSiteUID: str = ""
+    uid: str = ""
+    name: str = ""
+    apiKey: any = ""
+    description: str = ""
+    isAppliedToVisitor: bool = False
+
+    def __init__(self, security_group_dict: dict):
+        for property_name in security_group_dict:
+            if isinstance(security_group_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, security_group_dict[property_name])
+
+    def dict(self):
+        return {k: str(v) for k, v in asdict(self).items()}
+
+
+@dataclass
+class ScheduledMag(Observable):
+    uid: str = ""
+    securityGroupAPIKey: str = ""
+    scheduledSecurityGroupUID: str = ""
+    cardholderUID: str = ""
+    toDateValid: str = ""
+    fromDateValid: str = ""
+    status: str = ""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        scheduled_mags_dict = sanitise_args(self, args, kwargs)
+
+        # Initialise clss attributes from dictionary
+        for property_name in scheduled_mags_dict:
+            if isinstance(scheduled_mags_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, scheduled_mags_dict[property_name])
+                self.add_observer(property_name)
+
+    def dict(self, editable_only=False):
+        c = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                c[k] = v
+            elif isinstance(v, type(None)):
+                c[k] = None
+            else:
+                c[k] = str(v)
+
+        if editable_only:
+            if 'uid' in c:
+                c.pop('uid')
+            if 'status' in c:
+                c.pop('status')
+
+        return c
+
+
+@dataclass
+class CardholderCustomizedField(Observable):
+    uid: str = ""
+    cF_BoolField_1: bool = False,
+    cF_BoolField_2: bool = False
+    cF_BoolField_3: bool = False
+    cF_BoolField_4: bool = False
+    cF_BoolField_5: bool = False
+    cF_IntField_1: int = 0
+    cF_IntField_2: int = 0
+    cF_IntField_3: int = 0
+    cF_IntField_4: int = 0
+    cF_IntField_5: int = 0
+    cF_DateTimeField_1: any = None
+    cF_DateTimeField_2: any = None
+    cF_DateTimeField_3: any = None
+    cF_DateTimeField_4: any = None
+    cF_DateTimeField_5: any = None
+    cF_StringField_1: str = ""
+    cF_StringField_2: str = ""
+    cF_StringField_3: str = ""
+    cF_StringField_4: str = ""
+    cF_StringField_5: str = ""
+    cF_StringField_6: str = ""
+    cF_StringField_7: str = ""
+    cF_StringField_8: str = ""
+    cF_StringField_9: str = ""
+    cF_StringField_10: str = ""
+    cF_StringField_11: str = ""
+    cF_StringField_12: str = ""
+    cF_StringField_13: str = ""
+    cF_StringField_14: str = ""
+    cF_StringField_15: str = ""
+    cF_StringField_16: str = ""
+    cF_StringField_17: str = ""
+    cF_StringField_18: str = ""
+    cF_StringField_19: str = ""
+    cF_StringField_20: str = ""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        custom_fields_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in custom_fields_dict:
+            if isinstance(custom_fields_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, custom_fields_dict[property_name])
+
+        # Monitor Changes
+        for k, v in asdict(self).items():
+            if isinstance(v, (str, type(None), bool, int)):
+                self.add_observer(k)
+
+    def dict(self, changed_only=False):
+        c = dict()
+        for k, v in asdict(self).items():
+            if isinstance(v, (bool, int)):
+                c[k] = v
+            elif isinstance(v, int):
+                c[k] = v
+            elif isinstance(v, type(None)):
+                c[k] = None
+            else:
+                c[k] = str(v)
+
+        if changed_only:
+            c = self._remove_non_changed(c)
+
+        return c
+
+    def _remove_non_changed(self, ch: dict):
+        for key, value in list(ch.items()):
+            if key not in self.changed_attributes:
+                ch.pop(key)
+        return ch
+
+
+@dataclass
+class CardholderPersonalDetail(Observable):
+    uid: str = ""
+    officePhone: str = ""
+    cityOrDistrict: str = ""
+    streetOrApartment: str = ""
+    postCode: str = ""
+    privatePhoneOrFax: str = ""
+    mobile: str = ""
+    email: str = ""
+    carRegistrationNum: str = ""
+    company: str = ""
+    idFreeText: str = ""
+    idType: str = "IdentityCard"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        person_details_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in person_details_dict:
+            if isinstance(person_details_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, person_details_dict[property_name])
+
+        # Monitor Changes
+        for k, v in asdict(self).items():
+            if isinstance(v, (str, type(None), bool, int)):
+                self.add_observer(k)
+
+    def dict(self, editable_only=False, changed_only=False, non_empty_only=False):
+        ch = dict()
+
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                ch[k] = v
+            elif isinstance(v, type(None)):
+                pass
+                # ch[k] = None
+            elif isinstance(v, str):
+                if non_empty_only:
+                    if len(v) > 0:
+                        ch[k] = str(v)
+                else:
+                    ch[k] = str(v)
+            else:
+                pass
+
+        if changed_only:
+            ch = self._remove_non_changed(ch)
+
+        if editable_only:
+            ch = self._remove_non_editable(ch)
+
+        return ch
+
+    def _remove_non_changed(self, ch: dict):
+        for key, value in list(ch.items()):
+            if key not in self.changed_attributes:
+                ch.pop(key)
+        return ch
+
+    @staticmethod
+    def _remove_non_editable(ch: dict):
+        if 'uid' in ch:
+            ch.pop('uid')
+        return ch
+
+
+@dataclass
+class CardholderType:
+    uid: str = ""
+    typeName: str = ""
+    defaultBPTemplate: str = ""
+
+    def __init__(self, cardholder_type_dict: dict):
+        for property_name in cardholder_type_dict:
+            if isinstance(cardholder_type_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, cardholder_type_dict[property_name])
+
+    def dict(self):
+        return {k: str(v) for k, v in asdict(self).items()}
+
+
+@dataclass
+class Cardholder(Observable):
+    uid: str = ""
+    lastName: str = ""
+    firstName: str = ""
+    cardholderIdNumber: any = None
+    status: any = None
+    fromDateValid: any = None
+    isFromDateActive: any = None
+    toDateValid: any = None
+    isToDateActive: any = None
+    photo: any = None
+    cardholderType: CardholderType = None
+    securityGroup: SecurityGroup = None
+    cardholderPersonalDetail: CardholderPersonalDetail = None
+    cardholderCustomizedField: CardholderCustomizedField = None
+    insideArea: Area = None
+    ownerSiteUID: str = ""
+    securityGroupApiKey: any = None
+    ownerSiteApiKey: any = None
+    accessGroupApiKeys: any = None
+    liftAccessGroupApiKeys: any = None
+    cardholderTypeUID: str = ""
+    departmentUID: any = None
+    description: str = ""
+    grantAccessForSupervisor: any = None
+    isSupervisor: any = None
+    needEscort: any = None
+    personalWeeklyProgramUID: any = None
+    pinCode: str = ""
+    sharedStatus: str = ""
+    securityGroupUID: str = ""
+    accessGroupUIDs: any = None
+    liftAccessGroupUIDs: any = None
+    lastDownloadTime: any = None
+    lastInOutArea: str = ""
+    lastInOutReaderUID: any = None
+    lastInOutDate: any = None
+    lastAreaReaderDate: any = None
+    lastAreaReaderUID: any = None
+    lastPassDate: any = None
+    lastReaderPassUID: any = None
+    insideAreaUID: str = ""
+    cards: list = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        cardholder_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in cardholder_dict:
+            if isinstance(cardholder_dict[property_name], list):
+                if property_name == "cards":
+                    setattr(self, property_name, [])
+                    for card_entry in cardholder_dict[property_name]:
+                        if isinstance(card_entry, Card):
+                            self.cards.append(card_entry)
+                        else:
+                            self.cards.append(Card(card_entry))
+                else:
+                    setattr(self, property_name, cardholder_dict[property_name])
+
+            if property_name == "cardholderPersonalDetail":
+                if isinstance(cardholder_dict[property_name], CardholderPersonalDetail):
+                    self.cardholderPersonalDetail = cardholder_dict[property_name]
+
+            if property_name == "cardholderCustomizedField":
+                if isinstance(cardholder_dict[property_name], CardholderCustomizedField):
+                    self.cardholderCustomizedField = cardholder_dict[property_name]
+
+            if isinstance(cardholder_dict[property_name], dict):
+                if property_name == "insideArea":
+                    self.insideArea = Area(cardholder_dict[property_name])
+                if property_name == "securityGroup":
+                    self.securityGroup = SecurityGroup(cardholder_dict[property_name])
+                if property_name == "cardholderType":
+                    self.cardholderType = CardholderType(cardholder_dict[property_name])
+                if property_name == "cardholderPersonalDetail":
+                    self.cardholderPersonalDetail = CardholderPersonalDetail(cardholder_dict[property_name])
+                if property_name == "cardholderCustomizedField":
+                    self.cardholderCustomizedField = CardholderCustomizedField(cardholder_dict[property_name])
+
+            if isinstance(cardholder_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, cardholder_dict[property_name])
+
+        # Monitor Changes
+        for k, v in asdict(self).items():
+            if isinstance(v, (str, type(None), bool, int)):
+                self.add_observer(k)
+
+    def to_search_pattern(self):
+        pattern = ""
+        if self.firstName:
+            pattern += self.firstName + " "
+        if self.lastName:
+            pattern += self.lastName + " "
+        if self.cardholderPersonalDetail:
+            if self.cardholderPersonalDetail.company:
+                pattern += self.cardholderPersonalDetail.company + " "
+            if self.cardholderPersonalDetail.email:
+                pattern += self.cardholderPersonalDetail.email
+        return pattern
+
+    def pretty_print(self, obj: object = None):
+        if obj is None:
+            obj = self
+        for attribute_name in obj.__dict__:
+            if attribute_name != 'observed':
+                attribute = getattr(obj, attribute_name)
+                if isinstance(attribute, list):
+                    print(f"{attribute_name}:")
+                    print(f"\t{str(attribute)}")
+                elif hasattr(attribute, '__dict__'):
+                    print(f"{attribute_name}:")
+                    obj.pretty_print(attribute)
+                else:
+                    print(f"\t{attribute_name:<25}" + str(attribute))
+
+    def dict(self, editable_only=False, changed_only=False, non_empty_only=False):
+        ch = dict()
+
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                ch[k] = v
+            elif isinstance(v, type(None)):
+                if not non_empty_only:
+                    ch[k] = None
+            elif isinstance(v, str):
+                if non_empty_only:
+                    if len(v) > 0:
+                        ch[k] = str(v)
+                else:
+                    ch[k] = str(v)
+            else:
+                pass
+
+        if changed_only:
+            ch = self._remove_non_changed(ch)
+
+        if editable_only:
+            ch = self._remove_non_editable(ch)
+
+        return ch
+
+    def _remove_non_changed(self, ch: dict):
+        for key, value in list(ch.items()):
+            if key not in self.changed_attributes:
+                ch.pop(key)
+        return ch
+
+    @staticmethod
+    def _remove_non_editable(ch: dict):
+        if 'uid' in ch:
+            ch.pop('uid')
+        if 'ownerSiteUID' in ch:
+            ch.pop('ownerSiteUID')
+        if 'lastDownloadTime' in ch:
+            ch.pop('lastDownloadTime')
+        if 'lastInOutArea' in ch:
+            ch.pop('lastInOutArea')
+        if 'lastInOutReaderUID' in ch:
+            ch.pop('lastInOutReaderUID')
+        if 'lastInOutDate' in ch:
+            ch.pop('lastInOutDate')
+        if 'lastAreaReaderDate' in ch:
+            ch.pop('lastAreaReaderDate')
+        if 'lastAreaReaderUID' in ch:
+            ch.pop('lastAreaReaderUID')
+        if 'lastPassDate' in ch:
+            ch.pop('lastPassDate')
+        if 'lastReaderPassUID' in ch:
+            ch.pop('lastReaderPassUID')
+        if 'status' in ch:
+            ch.pop('status')
+        if 'insideArea' in ch:
+            ch.pop('insideArea')
+        if 'cardholderPersonalDetail' in ch:
+            ch.pop('cardholderPersonalDetail')
+        if 'cardholderCustomizedField' in ch:
+            ch.pop('cardholderCustomizedField')
+        if 'cardholderType' in ch:
+            ch.pop('cardholderType')
+        if 'securityGroup' in ch:
+            ch.pop('securityGroup')
+        if 'cards' in ch:
+            ch.pop('cards')
+        if 'accessGroupUIDs' in ch:
+            ch.pop('accessGroupUIDs')
+        if 'liftAccessGroupUIDs' in ch:
+            ch.pop('liftAccessGroupUIDs')
+
+        return ch
+
+
+if __name__ == "__main__":
+    cardholdertype = CardholderType(typeName="test")
+    print(cardholdertype.typeName)
+
+    '''securityGroup = SecurityGroup(ownerSiteUID="1234",
+                                  uid="sdfs", name="test", apiKey="None", description="test", isAppliedToVisitor=False)
+    print(securityGroup.name)
+    print(securityGroup.uid)'''
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_threaded.py` & `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_threaded.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from concurrent.futures import ThreadPoolExecutor
-from .guardpoint import GuardPoint, GuardPointError
-from .guardpoint_dataclasses import SortAlgorithm, Cardholder
-
-
-class GuardPointThreaded:
-
-    def __init__(self, **kwargs):
-        self.gp = GuardPoint(**kwargs)
-        self.executor = ThreadPoolExecutor(max_workers=1)
-
-    def new_card_holder(self, on_finished, cardholder: Cardholder):
-        future = self.executor.submit(self.gp.new_card_holder(), cardholder=cardholder)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def get_card_holder(self, on_finished, uid=None, card_code=None):
-        future = self.executor.submit(self.gp.get_card_holder, uid=uid, card_code=card_code)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def get_card_holders(self, on_finished, offset=0, limit=10, search_terms=None,
-                         cardholder_type_name=None,
-                         areas=None,
-                         filter_expired=False,
-                         sort_algorithm=SortAlgorithm.SERVER_DEFAULT,
-                         threshold=75,
-                         count=False,
-                         earliest_last_pass=None,
-                         select_ignore_list=None,
-                         select_include_list=None,
-                         **cardholder_kwargs):
-
-        future = self.executor.submit(self.gp.get_card_holders, offset=offset, limit=limit, search_terms=search_terms,
-                                      cardholder_type_name=cardholder_type_name, areas=areas,
-                                      filter_expired=filter_expired,
-                                      sort_algorithm=sort_algorithm, threshold=threshold,
-                                      count=count, earliest_last_pass=earliest_last_pass,
-                                      select_ignore_list=select_ignore_list,
-                                      select_include_list=select_include_list,
-                                      **cardholder_kwargs)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def update_cardholder(self, on_finished, cardholder: Cardholder):
-        future = self.executor.submit(self.gp.update_card_holder, cardholder=cardholder)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def delete_cardholder(self, on_finished, cardholder: Cardholder):
-        future = self.executor.submit(self.gp.delete_card_holder, cardholder=cardholder)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def get_cards(self, on_finished):
-        future = self.executor.submit(self.gp.get_cards)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def delete_card(self, on_finished, card):
-        future = self.executor.submit(self.gp.delete_card)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future, card)
-
-    def get_areas(self, on_finished):
-        future = self.executor.submit(self.gp.get_areas)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-    def get_security_groups(self, on_finished):
-        future = self.executor.submit(self.gp.get_security_groups)
-        callback = GPThreadCallBack(on_finished)
-        future.add_done_callback(callback.handle_future)
-
-
-class GPThreadCallBack:
-    on_finished = None
-
-    def __init__(self, on_finished_func):
-        self.on_finished = on_finished_func
-
-    def handle_future(self, future):
-        try:
-            r = future.result()
-            self.on_finished(r)
-        except GuardPointError as e:
-            self.on_finished(e)
-        except Exception as e:
-            self.on_finished(GuardPointError(e))
+from concurrent.futures import ThreadPoolExecutor
+from .guardpoint import GuardPoint, GuardPointError
+from .guardpoint_dataclasses import SortAlgorithm, Cardholder
+
+
+class GuardPointThreaded:
+
+    def __init__(self, **kwargs):
+        self.gp = GuardPoint(**kwargs)
+        self.executor = ThreadPoolExecutor(max_workers=1)
+
+    def new_card_holder(self, on_finished, cardholder: Cardholder):
+        future = self.executor.submit(self.gp.new_card_holder(), cardholder=cardholder)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def get_card_holder(self, on_finished, uid=None, card_code=None):
+        future = self.executor.submit(self.gp.get_card_holder, uid=uid, card_code=card_code)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def get_card_holders(self, on_finished, offset=0, limit=10, search_terms=None,
+                         cardholder_type_name=None,
+                         areas=None,
+                         filter_expired=False,
+                         sort_algorithm=SortAlgorithm.SERVER_DEFAULT,
+                         threshold=75,
+                         count=False,
+                         earliest_last_pass=None,
+                         select_ignore_list=None,
+                         select_include_list=None,
+                         **cardholder_kwargs):
+
+        future = self.executor.submit(self.gp.get_card_holders, offset=offset, limit=limit, search_terms=search_terms,
+                                      cardholder_type_name=cardholder_type_name, areas=areas,
+                                      filter_expired=filter_expired,
+                                      sort_algorithm=sort_algorithm, threshold=threshold,
+                                      count=count, earliest_last_pass=earliest_last_pass,
+                                      select_ignore_list=select_ignore_list,
+                                      select_include_list=select_include_list,
+                                      **cardholder_kwargs)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def update_cardholder(self, on_finished, cardholder: Cardholder):
+        future = self.executor.submit(self.gp.update_card_holder, cardholder=cardholder)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def delete_cardholder(self, on_finished, cardholder: Cardholder):
+        future = self.executor.submit(self.gp.delete_card_holder, cardholder=cardholder)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def get_cards(self, on_finished):
+        future = self.executor.submit(self.gp.get_cards)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def delete_card(self, on_finished, card):
+        future = self.executor.submit(self.gp.delete_card)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future, card)
+
+    def get_areas(self, on_finished):
+        future = self.executor.submit(self.gp.get_areas)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+    def get_security_groups(self, on_finished):
+        future = self.executor.submit(self.gp.get_security_groups)
+        callback = GPThreadCallBack(on_finished)
+        future.add_done_callback(callback.handle_future)
+
+
+class GPThreadCallBack:
+    on_finished = None
+
+    def __init__(self, on_finished_func):
+        self.on_finished = on_finished_func
+
+    def handle_future(self, future):
+        try:
+            r = future.result()
+            self.on_finished(r)
+        except GuardPointError as e:
+            self.on_finished(e)
+        except Exception as e:
+            self.on_finished(GuardPointError(e))
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint/guardpoint_utils.py` & `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import binascii
-import time
-import base64
-from urllib.parse import urlparse
-from .guardpoint_error import GuardPointError
-
-
-def url_parser(url):
-    parts = urlparse(url)
-    directories = parts.path.strip('/').split('/')
-    queries = parts.query.strip('&').split('&')
-    host = parts.netloc.strip(':').split(':')[0]
-
-    elements = {
-        'scheme': parts.scheme,
-        'host': host,
-        'path': parts.path,
-        'params': parts.params,
-        'query': parts.query,
-        'port': parts.port,
-        'fragment': parts.fragment,
-        'directories': directories,
-        'queries': queries,
-    }
-
-    return elements
-
-
-class ConvertBase64:
-
-    @staticmethod
-    def encode(text: str):
-        return base64.b64encode(text.encode('ascii')).decode('ascii')
-
-    @staticmethod
-    def decode(text: str):
-        try:
-            return base64.b64decode(text.encode('ascii')).decode('ascii')
-        except binascii.Error:
-            return base64.b64decode(text.encode('ascii') + b"==").decode('ascii')
-
-
-class GuardPointResponse:
-    @staticmethod
-    def extract_error_msg(response_body):
-        error_msg = ""
-        if isinstance(response_body, dict):
-            if "errorMessages" in response_body:
-                if isinstance(response_body["errorMessages"], list):
-                    if 'message' in response_body["errorMessages"][0] and 'other' in response_body["errorMessages"][0]:
-                        error_msg = f'{response_body["errorMessages"][0]["message"]}-{response_body["errorMessages"][0]["other"]}'
-            if 'message' in response_body:
-                error_msg = response_body['message']
-            if 'error' in response_body:
-                error_msg = response_body['error']
-            if 'errors' in response_body:
-                if isinstance(response_body['errors'], dict):
-                    for key in response_body['errors']:
-                        if isinstance(response_body['errors'][key], list):
-                            error_msg = error_msg + response_body['errors'][key][0] + '\n';
-                        elif isinstance(response_body['errors'][key], str):
-                            error_msg = error_msg + response_body['errors'][key][0] + '\n';
-        return error_msg
-
-    @staticmethod
-    def check_odata_body_structure(response_body):
-        if not isinstance(response_body, dict):
-            raise GuardPointError("Non-JSON Response Body")
-        if '@odata.context' not in response_body:
-            if 'error' in response_body:
-                raise GuardPointError(response_body['error'])
-            else:
-                raise GuardPointError("Non-ODATA Response Body")
-        if not str(response_body['@odata.context']).endswith("$entity"):
-            # Non entities seem to always appear to contain 'value'
-            check = False
-            for item in response_body:
-                if item in ['value', 'errorMessages', 'message', 'error']:
-                    check = True
-            if not check:
-                raise GuardPointError("Response Body does not contain either('value', 'errorMessages', 'message', "
-                                      "'error')")
-
-        return response_body
-
-
-class Stopwatch:
-
-    def __init__(self):
-        self._time = 0
-
-    def start(self):
-        self._time = time.time()
-        return self
-
-    def stop(self):
-        self._time = time.time() - self._time
-
-    def print(self, unit=None, precision=2, show_unit=1):
-        division_table = {'h': 360, 'm': 60, 's': 1, 'ms': 0.001}
-        unit_table = {'ms': "milliseconds", 's': "seconds", 'm': "minutes", 'h': "hours"}
-        if unit not in division_table:
-            for key, val in division_table.items():
-                if self._time >= val:
-                    unit = key
-                    break
-            else:
-                unit = 'ms'
-        unit_text = ""
-        if show_unit == 1:
-            unit_text = " " + unit
-        elif show_unit == 2:
-            unit_text = " " + unit_table[unit]
-        elif show_unit == 3:
-            unit_text = " " + unit_table[unit].capitalize()
-        return f"{(self._time / division_table[unit]):.{precision}f}{unit_text}"
-
-    def __str__(self):
-        return str(self._time)
+import binascii
+import time
+import base64
+from urllib.parse import urlparse
+from .guardpoint_error import GuardPointError
+
+
+def url_parser(url):
+    parts = urlparse(url)
+    directories = parts.path.strip('/').split('/')
+    queries = parts.query.strip('&').split('&')
+    host = parts.netloc.strip(':').split(':')[0]
+
+    elements = {
+        'scheme': parts.scheme,
+        'host': host,
+        'path': parts.path,
+        'params': parts.params,
+        'query': parts.query,
+        'port': parts.port,
+        'fragment': parts.fragment,
+        'directories': directories,
+        'queries': queries,
+    }
+
+    return elements
+
+
+class ConvertBase64:
+
+    @staticmethod
+    def encode(text: str):
+        return base64.b64encode(text.encode('ascii')).decode('ascii')
+
+    @staticmethod
+    def decode(text: str):
+        try:
+            return base64.b64decode(text.encode('ascii')).decode('ascii')
+        except binascii.Error:
+            return base64.b64decode(text.encode('ascii') + b"==").decode('ascii')
+
+
+class GuardPointResponse:
+    @staticmethod
+    def extract_error_msg(response_body):
+        error_msg = ""
+        if isinstance(response_body, dict):
+            if "errorMessages" in response_body:
+                if isinstance(response_body["errorMessages"], list):
+                    if 'message' in response_body["errorMessages"][0] and 'other' in response_body["errorMessages"][0]:
+                        error_msg = f'{response_body["errorMessages"][0]["message"]}-{response_body["errorMessages"][0]["other"]}'
+            if 'message' in response_body:
+                error_msg = response_body['message']
+            if 'error' in response_body:
+                error_msg = response_body['error']
+            if 'errors' in response_body:
+                if isinstance(response_body['errors'], dict):
+                    for key in response_body['errors']:
+                        if isinstance(response_body['errors'][key], list):
+                            error_msg = error_msg + response_body['errors'][key][0] + '\n';
+                        elif isinstance(response_body['errors'][key], str):
+                            error_msg = error_msg + response_body['errors'][key][0] + '\n';
+        return error_msg
+
+    @staticmethod
+    def check_odata_body_structure(response_body):
+        if not isinstance(response_body, dict):
+            raise GuardPointError("Non-JSON Response Body")
+        if '@odata.context' not in response_body:
+            if 'error' in response_body:
+                raise GuardPointError(response_body['error'])
+            else:
+                raise GuardPointError("Non-ODATA Response Body")
+        if not str(response_body['@odata.context']).endswith("$entity"):
+            # Non entities seem to always appear to contain 'value'
+            check = False
+            for item in response_body:
+                if item in ['value', 'errorMessages', 'message', 'error']:
+                    check = True
+            if not check:
+                raise GuardPointError("Response Body does not contain either('value', 'errorMessages', 'message', "
+                                      "'error')")
+
+        return response_body
+
+
+class Stopwatch:
+
+    def __init__(self):
+        self._time = 0
+
+    def start(self):
+        self._time = time.time()
+        return self
+
+    def stop(self):
+        self._time = time.time() - self._time
+
+    def print(self, unit=None, precision=2, show_unit=1):
+        division_table = {'h': 360, 'm': 60, 's': 1, 'ms': 0.001}
+        unit_table = {'ms': "milliseconds", 's': "seconds", 'm': "minutes", 'h': "hours"}
+        if unit not in division_table:
+            for key, val in division_table.items():
+                if self._time >= val:
+                    unit = key
+                    break
+            else:
+                unit = 'ms'
+        unit_text = ""
+        if show_unit == 1:
+            unit_text = " " + unit
+        elif show_unit == 2:
+            unit_text = " " + unit_table[unit]
+        elif show_unit == 3:
+            unit_text = " " + unit_table[unit].capitalize()
+        return f"{(self._time / division_table[unit]):.{precision}f}{unit_text}"
+
+    def __str__(self):
+        return str(self._time)
```

### Comparing `pyGuardPoint-1.3.8/pyGuardPoint.egg-info/SOURCES.txt` & `pyguardpoint-1.3.9/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

