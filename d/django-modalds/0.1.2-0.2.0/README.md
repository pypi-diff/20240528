# Comparing `tmp/django_modalds-0.1.2.tar.gz` & `tmp/django_modalds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modalds-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_modalds-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_modalds-0.1.2.tar` & `django_modalds-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     6148 2024-03-20 06:31:46.234580 django_modalds-0.1.2/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.1.2/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-20 06:42:27.733546 django_modalds-0.1.2/.gitignore
--rw-r--r--   0        0        0      561 2024-03-20 06:42:46.246240 django_modalds-0.1.2/.idea/django-modalds.iml
--rw-r--r--   0        0        0      174 2024-03-20 06:42:46.266987 django_modalds-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      419 2024-03-20 06:42:46.257139 django_modalds-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      280 2024-03-20 06:42:46.249379 django_modalds-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-20 06:42:46.269904 django_modalds-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     4075 2024-04-12 07:06:44.870789 django_modalds-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.1.2/LICENSE
--rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.1.2/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.1.2/django_modalds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.1.2/django_modalds/__init__.py
--rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.1.2/django_modalds/admin.py
--rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.1.2/django_modalds/apps.py
--rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.1.2/django_modalds/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.1.2/django_modalds/migrations/__init__.py
--rw-r--r--   0        0        0     5597 2024-03-20 04:58:30.866086 django_modalds-0.1.2/django_modalds/models.py
--rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.1.2/django_modalds/static/popupds/.DS_Store
--rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.1.2/django_modalds/static/popupds/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.1.2/django_modalds/static/popupds/js/jquery.cookie.js
--rw-r--r--   0        0        0     2515 2024-04-12 05:18:38.250197 django_modalds-0.1.2/django_modalds/templates/django_modalds/modalds.html
--rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.1.2/django_modalds/templates/django_modalds/type1.html
--rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.1.2/django_modalds/templates/django_modalds/type2.html
--rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.1.2/django_modalds/templates/django_modalds/type3.html
--rw-r--r--   0        0        0     2501 2024-03-18 03:18:17.561054 django_modalds-0.1.2/django_modalds/templates/django_modalds/type4.html
--rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.1.2/django_modalds/templates/django_modalds/type5.html
--rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.1.2/django_modalds/templatetags/__init__.py
--rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.1.2/django_modalds/templatetags/django_modalds_tags.py
--rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.1.2/django_modalds/tests.py
--rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.1.2/django_modalds/views.py
--rw-r--r--   0        0        0      685 2024-04-24 01:49:10.694190 django_modalds-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 django_modalds-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-05-18 02:13:53.917950 django_modalds-0.2.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.2.0/.gitattributes
+-rw-r--r--   0        0        0       29 2024-05-18 20:38:23.089873 django_modalds-0.2.0/.gitignore
+-rw-r--r--   0        0        0      561 2024-03-20 06:42:46.246240 django_modalds-0.2.0/.idea/django-modalds.iml
+-rw-r--r--   0        0        0      174 2024-03-20 06:42:46.266987 django_modalds-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      419 2024-03-20 06:42:46.257139 django_modalds-0.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2024-03-20 06:42:46.249379 django_modalds-0.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-20 06:42:46.269904 django_modalds-0.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     3472 2024-05-27 13:24:26.547979 django_modalds-0.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.2.0/LICENSE
+-rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.2.0/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.2.0/django_modalds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.2.0/django_modalds/__init__.py
+-rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.2.0/django_modalds/admin.py
+-rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.2.0/django_modalds/apps.py
+-rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.2.0/django_modalds/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3508 2024-05-28 02:31:29.978493 django_modalds-0.2.0/django_modalds/migrations/0002_alter_type1_h2_alter_type1_link_text_and_more.py
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.2.0/django_modalds/migrations/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-28 02:31:22.088340 django_modalds-0.2.0/django_modalds/models.py
+-rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.2.0/django_modalds/static/popupds/.DS_Store
+-rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.2.0/django_modalds/static/popupds/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.2.0/django_modalds/static/popupds/js/jquery.cookie.js
+-rw-r--r--   0        0        0     2515 2024-04-12 05:18:38.250197 django_modalds-0.2.0/django_modalds/templates/django_modalds/modalds.html
+-rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.2.0/django_modalds/templates/django_modalds/type1.html
+-rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.2.0/django_modalds/templates/django_modalds/type2.html
+-rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.2.0/django_modalds/templates/django_modalds/type3.html
+-rw-r--r--   0        0        0     2511 2024-05-28 02:27:26.477888 django_modalds-0.2.0/django_modalds/templates/django_modalds/type4.html
+-rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.2.0/django_modalds/templates/django_modalds/type5.html
+-rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.2.0/django_modalds/templatetags/__init__.py
+-rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.2.0/django_modalds/templatetags/django_modalds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.2.0/django_modalds/tests.py
+-rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.2.0/django_modalds/views.py
+-rw-r--r--   0        0        0      685 2024-05-28 02:32:28.895803 django_modalds-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 django_modalds-0.2.0/PKG-INFO
```

### Comparing `django_modalds-0.1.2/.DS_Store` & `django_modalds-0.2.0/django_modalds/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
-00000050: 0000 0001 0000 1000 0067 006f 005f 006d  .........g.o._.m
-00000060: 006f 0064 0000 0000 0000 0000 0000 0000  .o.d............
+00000050: 0000 0001 0000 1000 0070 0064 0073 6277  .........p.d.sbw
+00000060: 7370 626c 0000 0000 0000 0000 0000 0000  spbl............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0002 0000 000e  ................
-00000210: 0064 006a 0061 006e 0067 006f 005f 006d  .d.j.a.n.g.o._.m
-00000220: 006f 0064 0061 006c 0064 0073 6277 7370  .o.d.a.l.d.sbwsp
-00000230: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
-00000240: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-00000250: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00000260: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000270: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00000280: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00000290: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000002a0: 6261 7208 0908 095f 1019 7b7b 3133 3336  bar...._..{{1336
-000002b0: 2c20 3237 317d 2c20 7b39 3230 2c20 3433  , 271}, {920, 43
-000002c0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000002d0: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
-000002e0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 8c00 0000 0e00 6400 6a00 6100 6e00 6700  ......d.j.a.n.g.
-00000300: 6f00 5f00 6d00 6f00 6400 6100 6c00 6400  o._.m.o.d.a.l.d.
-00000310: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
+00000100: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00000110: 0070 006f 0070 0075 0070 0064 0073 6277  .p.o.p.u.p.d.sbw
+00000120: 7370 626c 6f62 0000 00b9 6270 6c69 7374  spblob....bplist
+00000130: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+00000140: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00000150: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+00000160: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00000170: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00000180: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00000190: 6465 6261 7208 0908 095f 1019 7b7b 3133  debar...._..{{13
+000001a0: 3336 2c20 3237 317d 2c20 7b39 3230 2c20  36, 271}, {920, 
+000001b0: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
+000001c0: 6e6f 8b00 0000 0000 0001 0100 0000 0000  no..............
+000001d0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 8c00 0000 0700 7000 6f00 7000 7500  ........p.o.p.u.
+000001f0: 7000 6400 7376 5372 6e6c 6f6e 6700 0000  p.d.svSrnlong...
+00000200: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `django_modalds-0.1.2/.idea/django-modalds.iml` & `django_modalds-0.2.0/.idea/django-modalds.iml`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/.idea/workspace.xml` & `django_modalds-0.2.0/.idea/workspace.xml`

 * *Files 19% similar despite different names*

#### Comparing `django_modalds-0.1.2/.idea/workspace.xml` & `django_modalds-0.2.0/.idea/workspace.xml`

```diff
@@ -1,20 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="e7de678e-305c-4307-87c6-2108e448b4bf" name="변경" comment="">
-      <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/media/images/popup/type1/스크린샷_2024-05-27_오후_10.18.12.png" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/media/images/popup/type1/스크린샷_2024-05-27_오후_10.20.36.png" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/db.sqlite3" beforeDir="false" afterPath="$PROJECT_DIR$/db.sqlite3" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/django_modalds-0.1.0-py2.py3-none-any.whl" beforeDir="false" afterPath="$PROJECT_DIR$/dist/django_modalds-0.1.0-py2.py3-none-any.whl" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/django_modalds-0.1.0.tar.gz" beforeDir="false" afterPath="$PROJECT_DIR$/dist/django_modalds-0.1.0.tar.gz" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/django_modalds/templates/django_modalds/modalds.html" beforeDir="false" afterPath="$PROJECT_DIR$/django_modalds/templates/django_modalds/modalds.html" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
```

### Comparing `django_modalds-0.1.2/LICENSE` & `django_modalds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/README.md` & `django_modalds-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/admin.py` & `django_modalds-0.2.0/django_modalds/admin.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/migrations/0001_initial.py` & `django_modalds-0.2.0/django_modalds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/models.py` & `django_modalds-0.2.0/django_modalds/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from django.db import models
 
 
 class Type5(models.Model):
-    modal_title = models.CharField('modal_title', default="NOTI", max_length=20, blank=True)
+    modal_title = models.CharField('modal_title', default="NOTI", max_length=50, blank=True)
     img = models.ImageField(upload_to=f'images/popup/type5')
     activate = models.BooleanField(default=False, help_text="활성창 1개만 가능")
 
     def __str__(self):
         return self.modal_title
 
 
 class Type4(models.Model):
     """
     <h3>Welcome to <strong>Tempo</strong></h3>
     <h1>We're Creative Agency</h1>
     <h2>We are team of talented designers making websites with Bootstrap</h2>
     <a href="#about" class="btn-get-started scrollto">Get Started</a>
     """
-    modal_title = models.CharField('modal_title', default="EVENT", max_length=20, blank=True)
-    h3 = models.CharField('h3', max_length=20, help_text="강조 : strong tag")
-    h1 = models.CharField('h1', max_length=40)
+    modal_title = models.CharField('modal_title', default="EVENT", max_length=50, blank=True)
+    h3 = models.CharField('h3', max_length=50, help_text="강조 : strong tag")
+    h1 = models.CharField('h1', max_length=100)
     h2 = models.TextField('h2', help_text="줄넘기기 : br tag, 강조 : strong tag")
     link_url = models.CharField('link_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_text = models.CharField('link_text', default="Get Started", max_length=20)
+    link_text = models.CharField('link_text', default="Get Started", max_length=50)
     bg = models.ImageField(upload_to=f'images/popup/type4')
     activate = models.BooleanField(default=False, help_text="활성창 1개만 가능")
 
     def __str__(self):
         return self.h1
 
 
@@ -35,21 +35,21 @@
     <h2 data-aos="fade-up">Enjoy Your Healthy<br>Delicious Food</h2>
     <p data-aos="fade-up" data-aos-delay="100">Sed autem laudantium dolores. Voluptatem itaque ea consequatur eveniet. Eum quas beatae cumque eum quaerat.</p>
     <div class="d-flex" data-aos="fade-up" data-aos-delay="200">
       <a href="#book-a-table" class="btn-book-a-table">Book a Table</a>
       <a href="https://www.youtube.com/watch?v=LXb3EKWsInQ" class="glightbox btn-watch-video d-flex align-items-center"><i class="bi bi-play-circle"></i><span>Watch Video</span></a>
     </div>
     """
-    modal_title = models.CharField('modal_title', default="EVENT", max_length=20, blank=True)
-    h2 = models.CharField('h2', max_length=40, help_text="줄넘기기 : br tag")
+    modal_title = models.CharField('modal_title', default="EVENT", max_length=50, blank=True)
+    h2 = models.CharField('h2', max_length=100, help_text="줄넘기기 : br tag")
     p = models.TextField('p', help_text="줄넘기기 : br tag, 강조 : strong tag")
     link_url = models.CharField('link_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_text = models.CharField('link_text', default="Book a Table", max_length=20)
+    link_text = models.CharField('link_text', default="Book a Table", max_length=50)
     link_video_url = models.CharField('link_video_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_video_text = models.CharField('link_video_text', default="Watch Video", max_length=20)
+    link_video_text = models.CharField('link_video_text', default="Watch Video", max_length=50)
     img = models.ImageField(upload_to=f'images/popup/type3')
     activate = models.BooleanField(default=False, help_text="활성창 1개만 가능")
 
     def __str__(self):
         return self.h2
 
 
@@ -60,21 +60,21 @@
       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perspiciatis cum recusandae eum laboriosam voluptatem repudiandae odio, vel exercitationem officiis provident minima. </p>
     </blockquote>
     <div class="d-flex" data-aos="fade-up" data-aos-delay="200">
       <a href="#about" class="btn-get-started">Get Started</a>
       <a href="https://www.youtube.com/watch?v=LXb3EKWsInQ" class="glightbox btn-watch-video d-flex align-items-center"><i class="bi bi-play-circle"></i><span>Watch Video</span></a>
     </div>
     """
-    modal_title = models.CharField('modal_title', default="EVENT", max_length=20, blank=True)
-    h2 = models.CharField('h2', max_length=40)
+    modal_title = models.CharField('modal_title', default="EVENT", max_length=50, blank=True)
+    h2 = models.CharField('h2', max_length=100)
     p = models.TextField('p', help_text="줄넘기기 : br tag, 강조 : strong tag")
     link_url = models.CharField('link_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_text = models.CharField('link_text', default="Get Started", max_length=20)
+    link_text = models.CharField('link_text', default="Get Started", max_length=50)
     link_video_url = models.CharField('link_video_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_video_text = models.CharField('link_video_text', default="Watch Video", max_length=20)
+    link_video_text = models.CharField('link_video_text', default="Watch Video", max_length=50)
     bg = models.ImageField(upload_to=f'images/popup/type2')
     activate = models.BooleanField(default=False, help_text="활성창 1개만 가능")
 
     def __str__(self):
         return self.h2
 
 
@@ -82,19 +82,19 @@
     """
     <div class="col-lg-6 text-center">
       <h2 data-aos="fade-down">행사 <span>UpConstruction</span></h2>
       <p data-aos="fade-up">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
       <a data-aos="fade-up" data-aos-delay="200" href="#get-started" class="btn-get-started">Get Started</a>
     </div>
     """
-    modal_title = models.CharField('modal_title', default="EVENT", max_length=20, blank=True)
-    h2 = models.CharField('h2', max_length=40, help_text="줄넘기기 : br tag, 강조 : span tag")
+    modal_title = models.CharField('modal_title', default="EVENT", max_length=50, blank=True)
+    h2 = models.CharField('h2', max_length=100, help_text="줄넘기기 : br tag, 강조 : span tag")
     p = models.TextField('p', help_text="줄넘기기 : br tag")
     link_url = models.CharField('link_url', blank=True, help_text="공란 가능", max_length=1200)
-    link_text = models.CharField('link_text', default="Get Started", max_length=20)
+    link_text = models.CharField('link_text', default="Get Started", max_length=50)
     bg = models.ImageField(upload_to=f'images/popup/type1')
     bg2 = models.ImageField(blank=True, upload_to=f'images/popup/type1')
     bg3 = models.ImageField(blank=True, upload_to=f'images/popup/type1')
     activate = models.BooleanField(default=False, help_text="활성창 1개만 가능")
 
     def __str__(self):
         return self.h2
```

### Comparing `django_modalds-0.1.2/django_modalds/static/popupds/.DS_Store` & `django_modalds-0.2.0/django_modalds/static/popupds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/static/popupds/js/jquery-3.6.0.min.js` & `django_modalds-0.2.0/django_modalds/static/popupds/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/static/popupds/js/jquery.cookie.js` & `django_modalds-0.2.0/django_modalds/static/popupds/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/modalds.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/modalds.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/type1.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/type1.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/type2.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/type2.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/type3.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/type3.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/type4.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/type4.html`

 * *Files 7% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 
 <!-- ======= MyModal Section ======= -->
 <section id="mymodal">
   <div class="mymodal-container">
     {% autoescape off %}
     <h3>{{ popup.h3 }}</h3>
     <h1>{{ popup.h1 }}</h1>
+    <br>
     <h2>{{ popup.h2 }}</h2>
     {% if popup.link_url %}
     <a href="{{ popup.link_url }}" class="btn-get-started scrollto">{{ popup.link_text }}</a>
     {% endif %}
     {% endautoescape %}
   </div>
 </section><!-- End MyModal -->
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 {% load static %}
 {% autoescape off %}
 ******** {{{{ ppooppuupp..hh33 }}}} ********
 ************ {{{{ ppooppuupp..hh11 }}}} ************
+
 ********** {{{{ ppooppuupp..hh22 }}}} **********
 {% if popup.link_url %} _{_{_ _p_o_p_u_p_._l_i_n_k___t_e_x_t_ _}_} {% endif %} {% endautoescape %}
```

### Comparing `django_modalds-0.1.2/django_modalds/templates/django_modalds/type5.html` & `django_modalds-0.2.0/django_modalds/templates/django_modalds/type5.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/django_modalds/templatetags/django_modalds_tags.py` & `django_modalds-0.2.0/django_modalds/templatetags/django_modalds_tags.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.2/pyproject.toml` & `django_modalds-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-modalds"
-version = "0.1.2"
+version = "0.2.0"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_modalds-0.1.2/PKG-INFO` & `django_modalds-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modalds
-Version: 0.1.2
+Version: 0.2.0
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: pillow >= 10.2.0
 Project-URL: Home, https://www.demiansoft.com
```

